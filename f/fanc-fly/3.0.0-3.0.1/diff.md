# Comparing `tmp/fanc-fly-3.0.0.tar.gz` & `tmp/fanc-fly-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fanc-fly-3.0.0.tar", last modified: Mon Jul 31 20:28:48 2023, max compression
+gzip compressed data, was "dist/fanc-fly-3.0.1.tar", last modified: Tue Aug  1 10:06:36 2023, max compression
```

## Comparing `fanc-fly-3.0.0.tar` & `fanc-fly-3.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/
--rw-rw-r--   0 jasper     (501) staff       (20)    35149 2022-12-10 21:47:19.000000 fanc-fly-3.0.0/LICENSE
--rw-rw-r--   0 jasper     (501) staff       (20)       75 2023-07-30 17:19:39.000000 fanc-fly-3.0.0/MANIFEST.in
--rw-rw-r--   0 jasper     (501) staff       (20)     7147 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/PKG-INFO
--rw-rw-r--   0 jasper     (501) staff       (20)     5827 2023-07-30 18:01:17.000000 fanc-fly-3.0.0/README.md
-drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc/
--rw-rw-r--   0 jasper     (501) staff       (20)      342 2023-07-08 11:24:01.000000 fanc-fly-3.0.0/fanc/__init__.py
--rw-rw-r--   0 jasper     (501) staff       (20)    10190 2023-07-08 11:24:01.000000 fanc-fly-3.0.0/fanc/annotations.py
--rw-rw-r--   0 jasper     (501) staff       (20)     2110 2023-01-24 17:02:26.000000 fanc-fly-3.0.0/fanc/auth.py
--rw-rw-r--   0 jasper     (501) staff       (20)     4197 2023-01-28 13:24:19.000000 fanc-fly-3.0.0/fanc/catmaid.py
--rw-rw-r--   0 jasper     (501) staff       (20)     4410 2023-07-22 19:29:57.000000 fanc-fly-3.0.0/fanc/connectivity.py
--rw-rw-r--   0 jasper     (501) staff       (20)    40101 2023-07-30 19:26:42.000000 fanc-fly-3.0.0/fanc/lookup.py
--rw-rw-r--   0 jasper     (501) staff       (20)     3027 2023-07-08 11:24:01.000000 fanc-fly-3.0.0/fanc/ngl_info.py
--rw-rw-r--   0 jasper     (501) staff       (20)    10702 2023-07-08 11:24:01.000000 fanc-fly-3.0.0/fanc/publish.py
--rw-rw-r--   0 jasper     (501) staff       (20)     3258 2023-05-20 17:30:54.000000 fanc-fly-3.0.0/fanc/render_neurons.py
--rw-rw-r--   0 jasper     (501) staff       (20)     7912 2023-07-31 20:23:30.000000 fanc-fly-3.0.0/fanc/skeletonize.py
--rw-rw-r--   0 jasper     (501) staff       (20)    17737 2023-07-30 18:56:59.000000 fanc-fly-3.0.0/fanc/statebuilder.py
--rw-rw-r--   0 jasper     (501) staff       (20)     1554 2022-12-10 21:47:20.000000 fanc-fly-3.0.0/fanc/statemanager.py
--rw-rw-r--   0 jasper     (501) staff       (20)     9728 2023-02-11 13:16:57.000000 fanc-fly-3.0.0/fanc/synaptic_links.py
--rw-rw-r--   0 jasper     (501) staff       (20)     3287 2023-01-30 21:05:39.000000 fanc-fly-3.0.0/fanc/template_spaces.py
-drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc/transforms/
--rw-rw-r--   0 jasper     (501) staff       (20)       83 2022-12-21 21:40:32.000000 fanc-fly-3.0.0/fanc/transforms/__init__.py
--rw-rw-r--   0 jasper     (501) staff       (20)    10074 2022-12-10 21:47:20.000000 fanc-fly-3.0.0/fanc/transforms/realignment.py
--rw-rw-r--   0 jasper     (501) staff       (20)    15072 2023-01-30 21:00:53.000000 fanc-fly-3.0.0/fanc/transforms/template_alignment.py
-drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc/transforms/transform_parameters/
--rw-rw-r--   0 jasper     (501) staff       (20)  5544904 2022-12-10 21:47:20.000000 fanc-fly-3.0.0/fanc/transforms/transform_parameters/TransformParameters.FixedFANC.txt
--rw-rw-r--   0 jasper     (501) staff       (20)  3338492 2022-12-10 21:47:20.000000 fanc-fly-3.0.0/fanc/transforms/transform_parameters/TransformParameters.FixedTemplate.Bspline.txt
--rw-rw-r--   0 jasper     (501) staff       (20)     1166 2022-12-10 21:47:20.000000 fanc-fly-3.0.0/fanc/transforms/transform_parameters/TransformParameters.FixedTemplate.affine.txt
--rw-rw-r--   0 jasper     (501) staff       (20)    26078 2023-07-30 18:57:12.000000 fanc-fly-3.0.0/fanc/upload.py
--rw-rw-r--   0 jasper     (501) staff       (20)    12528 2023-07-22 19:31:44.000000 fanc-fly-3.0.0/fanc/visualize.py
-drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc_fly.egg-info/
--rw-rw-r--   0 jasper     (501) staff       (20)     7147 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc_fly.egg-info/PKG-INFO
--rw-rw-r--   0 jasper     (501) staff       (20)      868 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc_fly.egg-info/SOURCES.txt
--rw-rw-r--   0 jasper     (501) staff       (20)        1 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc_fly.egg-info/dependency_links.txt
--rw-rw-r--   0 jasper     (501) staff       (20)      219 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc_fly.egg-info/requires.txt
--rw-rw-r--   0 jasper     (501) staff       (20)        5 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc_fly.egg-info/top_level.txt
--rw-rw-r--   0 jasper     (501) staff       (20)      219 2023-07-08 11:24:01.000000 fanc-fly-3.0.0/requirements.txt
--rw-rw-r--   0 jasper     (501) staff       (20)       38 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/setup.cfg
--rw-rw-r--   0 jasper     (501) staff       (20)      975 2023-07-31 20:26:19.000000 fanc-fly-3.0.0/setup.py
-drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/tests/
--rwxrwxr-x   0 jasper     (501) staff       (20)     2595 2023-07-31 20:23:30.000000 fanc-fly-3.0.0/tests/test_lookup.py
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-08-01 10:06:36.000000 fanc-fly-3.0.1/
+-rw-rw-r--   0 jasper     (501) staff       (20)    35149 2022-12-10 21:47:19.000000 fanc-fly-3.0.1/LICENSE
+-rw-rw-r--   0 jasper     (501) staff       (20)       75 2023-07-30 17:19:39.000000 fanc-fly-3.0.1/MANIFEST.in
+-rw-rw-r--   0 jasper     (501) staff       (20)     7147 2023-08-01 10:06:36.000000 fanc-fly-3.0.1/PKG-INFO
+-rw-rw-r--   0 jasper     (501) staff       (20)     5827 2023-07-30 18:01:17.000000 fanc-fly-3.0.1/README.md
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-08-01 10:06:36.000000 fanc-fly-3.0.1/fanc/
+-rw-rw-r--   0 jasper     (501) staff       (20)      342 2023-07-08 11:24:01.000000 fanc-fly-3.0.1/fanc/__init__.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    10178 2023-07-31 21:10:44.000000 fanc-fly-3.0.1/fanc/annotations.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     2137 2023-08-01 09:10:13.000000 fanc-fly-3.0.1/fanc/auth.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     4197 2023-01-28 13:24:19.000000 fanc-fly-3.0.1/fanc/catmaid.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     4410 2023-07-22 19:29:57.000000 fanc-fly-3.0.1/fanc/connectivity.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    40325 2023-08-01 10:05:15.000000 fanc-fly-3.0.1/fanc/lookup.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     3027 2023-07-08 11:24:01.000000 fanc-fly-3.0.1/fanc/ngl_info.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    10697 2023-07-31 21:10:17.000000 fanc-fly-3.0.1/fanc/publish.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     3258 2023-05-20 17:30:54.000000 fanc-fly-3.0.1/fanc/render_neurons.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     8001 2023-08-01 08:34:16.000000 fanc-fly-3.0.1/fanc/skeletonize.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    17733 2023-07-31 21:12:24.000000 fanc-fly-3.0.1/fanc/statebuilder.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     1554 2022-12-10 21:47:20.000000 fanc-fly-3.0.1/fanc/statemanager.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     9716 2023-07-31 21:11:04.000000 fanc-fly-3.0.1/fanc/synaptic_links.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     3287 2023-01-30 21:05:39.000000 fanc-fly-3.0.1/fanc/template_spaces.py
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-08-01 10:06:36.000000 fanc-fly-3.0.1/fanc/transforms/
+-rw-rw-r--   0 jasper     (501) staff       (20)       83 2022-12-21 21:40:32.000000 fanc-fly-3.0.1/fanc/transforms/__init__.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    10074 2022-12-10 21:47:20.000000 fanc-fly-3.0.1/fanc/transforms/realignment.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    15072 2023-01-30 21:00:53.000000 fanc-fly-3.0.1/fanc/transforms/template_alignment.py
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-08-01 10:06:36.000000 fanc-fly-3.0.1/fanc/transforms/transform_parameters/
+-rw-rw-r--   0 jasper     (501) staff       (20)  5544904 2022-12-10 21:47:20.000000 fanc-fly-3.0.1/fanc/transforms/transform_parameters/TransformParameters.FixedFANC.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)  3338492 2022-12-10 21:47:20.000000 fanc-fly-3.0.1/fanc/transforms/transform_parameters/TransformParameters.FixedTemplate.Bspline.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)     1166 2022-12-10 21:47:20.000000 fanc-fly-3.0.1/fanc/transforms/transform_parameters/TransformParameters.FixedTemplate.affine.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)    26022 2023-07-31 21:11:44.000000 fanc-fly-3.0.1/fanc/upload.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    12518 2023-07-31 21:12:06.000000 fanc-fly-3.0.1/fanc/visualize.py
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-08-01 10:06:36.000000 fanc-fly-3.0.1/fanc_fly.egg-info/
+-rw-rw-r--   0 jasper     (501) staff       (20)     7147 2023-08-01 10:06:36.000000 fanc-fly-3.0.1/fanc_fly.egg-info/PKG-INFO
+-rw-rw-r--   0 jasper     (501) staff       (20)      868 2023-08-01 10:06:36.000000 fanc-fly-3.0.1/fanc_fly.egg-info/SOURCES.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)        1 2023-08-01 10:06:36.000000 fanc-fly-3.0.1/fanc_fly.egg-info/dependency_links.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)      219 2023-08-01 10:06:36.000000 fanc-fly-3.0.1/fanc_fly.egg-info/requires.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)        5 2023-08-01 10:06:36.000000 fanc-fly-3.0.1/fanc_fly.egg-info/top_level.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)      219 2023-07-08 11:24:01.000000 fanc-fly-3.0.1/requirements.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)       38 2023-08-01 10:06:36.000000 fanc-fly-3.0.1/setup.cfg
+-rw-rw-r--   0 jasper     (501) staff       (20)      975 2023-08-01 10:06:07.000000 fanc-fly-3.0.1/setup.py
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-08-01 10:06:36.000000 fanc-fly-3.0.1/tests/
+-rwxrwxr-x   0 jasper     (501) staff       (20)     2595 2023-07-31 20:23:30.000000 fanc-fly-3.0.1/tests/test_lookup.py
```

### Comparing `fanc-fly-3.0.0/LICENSE` & `fanc-fly-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fanc-fly-3.0.0/PKG-INFO` & `fanc-fly-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fanc-fly
-Version: 3.0.0
+Version: 3.0.1
 Summary: Tools for the Female Adult Nerve Cord Drosophila EM dataset
 Home-page: https://github.com/htem/FANC_auto_recon
 Author: Jasper Phelps
 Author-email: jasper.s.phelps@gmail.com
 License: UNKNOWN
 Description: # FANC_auto_recon
```

### Comparing `fanc-fly-3.0.0/README.md` & `fanc-fly-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fanc-fly-3.0.0/fanc/annotations.py` & `fanc-fly-3.0.1/fanc/annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     """
     def _build_tree(annotations: dict, parent: dict = None, nodes: dict = {}):
         for annotation in annotations.keys():
             node = anytree.Node(annotation, parent=parent)
             nodes[annotation] = nodes.get(annotation, []) + [node]
             _build_tree(annotations[annotation], parent=node, nodes=nodes)
         return nodes
-    
+
     return _build_tree(dict)
 
 annotation_tree = _dict_to_anytree(annotation_hierarchy)
 
 
 def print_annotation_tree():
     """
@@ -122,15 +122,15 @@
     if annotation_class == 'neuron identity':
         if annotation in annotation_tree:
             if raise_errors:
                 raise ValueError(f'The term "{annotation}" is a class,'
                                  f' not an identity. {help_msg}')
             return False
         return True
-    
+
     try:
         class_nodes = annotation_tree[annotation_class]
     except:
         if raise_errors:
             raise ValueError(f'Annotation class "{annotation_class}" not'
                              f' recognized. {help_msg}')
         else:
@@ -160,15 +160,15 @@
         else:
             raise ValueError(f'Annotation "{annotation}" belongs to classes'
                              f' {parent_names} but you specified class'
                              f' "{annotation_class}". {help_msg}')
 
     else:
         return False
-    
+
     return True
 
 def is_allowed_to_post(segid, annotation_class, annotation,
                        table_name='neuron_information',
                        raise_errors=True) -> bool:
     """
     Determine whether a particular segment is allowed to be annotated
```

### Comparing `fanc-fly-3.0.0/fanc/auth.py` & `fanc-fly-3.0.1/fanc/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     # If a nickname was used, get the proper datastack name
     dataset = DATASTACK_NICKNAMES.get(dataset, dataset)
 
     if dataset not in _cloudvolumes:
         client = get_caveclient(dataset=dataset)
 
         _cloudvolumes[dataset] = CloudVolume(
-            client.info.get_datastack_info()['segmentation_source'],
+            client.info.get_datastack_info()['segmentation_source'].replace('middleauth+', ''),
             use_https=True,
             secrets=client.auth.token
         )
 
     return _cloudvolumes[dataset]
```

### Comparing `fanc-fly-3.0.0/fanc/catmaid.py` & `fanc-fly-3.0.1/fanc/catmaid.py`

 * *Files identical despite different names*

### Comparing `fanc-fly-3.0.0/fanc/connectivity.py` & `fanc-fly-3.0.1/fanc/connectivity.py`

 * *Files identical despite different names*

### Comparing `fanc-fly-3.0.0/fanc/lookup.py` & `fanc-fly-3.0.1/fanc/lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -538,14 +538,17 @@
         table_name,
         timestamp=timestamp,
         filter_in_dict={table_name: {'pt_root_id': segids}})
     cell_ids.set_index('pt_root_id', inplace=True)
     if any([i not in cell_ids.index for i in segids]):
         raise ValueError("These segment IDs don't have a cell ID: {}".format(
             [i for i in segids if i not in cell_ids.index]))
+    if any(cell_ids.index.value_counts() > 1):
+        raise ValueError("These segment IDs have multiple cell IDs: {}".format(
+            [segid for segid, count in cell_ids.index.value_counts().iteritems() if count > 1]))
     return cell_ids.loc[segids, 'id'].to_list()
 # --- END SEGMENTATION/CHUNKEDGRAPH SECTION --- #
 
 
 # --- START KEY ATTRIBUTES SECTION --- #
 def anchor_point(segids: int or list[int],
                  source_tables=default_anchor_point_sources,
```

### Comparing `fanc-fly-3.0.0/fanc/ngl_info.py` & `fanc-fly-3.0.1/fanc/ngl_info.py`

 * *Files identical despite different names*

### Comparing `fanc-fly-3.0.0/fanc/publish.py` & `fanc-fly-3.0.1/fanc/publish.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,14 @@
         raise ValueError('{} not in {}'.format(template_space,
                                                VALID_TEMPLATE_SPACES))
 
     already_published_ids = list_public_segment_ids(template_space=template_space,
                                                     gcloud_path=gcloud_path)
     already_published_ids = set(already_published_ids)
 
-    
     fancneurons_cloudvolume = cloudvolume.CloudVolume(gcloud_path.format(template_space))
 
     mm = auth.get_meshmanager()
     for segid in segids:
         if segid in already_published_ids:
             print(f'Segment {segid} already published in {template_space}-space, skipping.')
             continue
```

### Comparing `fanc-fly-3.0.0/fanc/render_neurons.py` & `fanc-fly-3.0.1/fanc/render_neurons.py`

 * *Files identical despite different names*

### Comparing `fanc-fly-3.0.0/fanc/skeletonize.py` & `fanc-fly-3.0.1/fanc/skeletonize.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 diameter_smoothing_defaults = {'smooth_method': 'smooth',
                                'smooth_bandwidth': 1000}
 
 
 def skeletonize_neuron(seg_id,
                        soma_pt,
                        output='meshwork',
-                       cloudvolume=auth.get_cloudvolume(),
+                       cloudvolume=None,
                        voxel_resolution=skeletonization_defaults['voxel_resolution']):
     """
     Skeletonize a neuron from a FANC segmentation object (mesh).
 
     This function is more flexible than get_pcg_skeleton (there are a
     ton of parameters that you could tweak if you're really motivated to
     get a skeleton that's optimized for your purposes) and produces
@@ -76,20 +76,22 @@
 
     soma_pt: 3-element iterable (xyz)
       The coordinates of the soma, in voxels
 
     output: 'meshwork' or 'navis'
       A string specifying the type of object to return.
 
-    cv: cloudvolume.CloudVolume
-      The cloudvolume to use for fetching meshes. Defaults to the FANC
-      segmentation cloudvolume.
+    cv: None or cloudvolume.CloudVolume
+      The cloudvolume to use for fetching meshes. If None, will use the
+      one returned by auth.get_cloudvolume() by default.
     """
-    mesh = cloudvolume.mesh.get(seg_id, use_byte_offsets=True)[seg_id]
+    if cloudvolume is None:
+        cloudvolume = auth.get_cloudvolume()
 
+    mesh = cloudvolume.mesh.get(seg_id, use_byte_offsets=True)[seg_id]
     mp_mesh = trimesh_io.Mesh(mesh.vertices, mesh.faces)
 
     mp_mesh.merge_large_components(size_threshold=skeletonization_defaults['merge_size_threshold'],
                                    max_dist=skeletonization_defaults['merge_max_dist'],
                                    dist_step=skeletonization_defaults['merge_distance_step'])
     in_comp = mesh_filters.filter_largest_component(mp_mesh)
     mesh_anchor = mp_mesh.apply_mask(in_comp)
```

### Comparing `fanc-fly-3.0.0/fanc/statebuilder.py` & `fanc-fly-3.0.1/fanc/statebuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         Override the default url for the segmentation layer
     state_server: str
         Override the default url for the json state server
     bg_color: str
         Set the background color. Must be 'w'/'white' or a hex color code
     nuclei: int or list or DataFrame or np.array
         Nucleus IDs to visualize specific nuclei. Set nuclei_layer=True when using.
-    
+
     ---Returns---
     Neuroglancer state (as a json or a url depending on 'return_as')
     """
     # This import is delayed because it triggers creation of a CAVEclient,
     # which I don't want to do until this function is called
     from . import ngl_info
```

### Comparing `fanc-fly-3.0.0/fanc/statemanager.py` & `fanc-fly-3.0.1/fanc/statemanager.py`

 * *Files identical despite different names*

### Comparing `fanc-fly-3.0.0/fanc/synaptic_links.py` & `fanc-fly-3.0.1/fanc/synaptic_links.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     convention: 'xyz' (default) or 'zyx'
         Determines ordering of the 3 columns representing each point.
     units: 'voxels' (default) or 'nm'/'nanometers'
         Determines units of the returned points.
     voxel_size: None (default) or 3-tuple (e.g. (4, 4, 40))
         Determines voxel size to use for conversions. If left as None, the code
         knows what default voxel size to use for different file formats.
-    
+
     threshold: int, threshold to apply based on "sum"
     """
     assert convention in ['xyz', 'zyx']
     assert units in ['voxels', 'nm', 'nanometers']
 
     if fn.endswith('.npy'):
         if verbose: print('Mode 1: npy')
@@ -138,15 +138,15 @@
         # of voxels at (4, 4, 40)nm
 
     else:
         if verbose: print('Mode 3: binary')
         # For opening binary files saved by ../detection/worker.py
         # post coord(x,y,z), pre coord(x,y,z), mean, max, area, 4x4x4 moments
         data = np.fromfile(fn, dtype=np.dtype("6f8,3f8,(4,4,4)f8"))
-        
+
         # Apply threshold based on "sum" and return links that pass.
         try:
             links = np.stack([x[0].astype("int32") for x in data if x[2][0][0][0] > threshold])
         except:
             return np.array([])
 
         if True:  # The Feb 7 predictions were saved in post-pre order
```

### Comparing `fanc-fly-3.0.0/fanc/template_spaces.py` & `fanc-fly-3.0.1/fanc/template_spaces.py`

 * *Files identical despite different names*

### Comparing `fanc-fly-3.0.0/fanc/transforms/realignment.py` & `fanc-fly-3.0.1/fanc/transforms/realignment.py`

 * *Files identical despite different names*

### Comparing `fanc-fly-3.0.0/fanc/transforms/template_alignment.py` & `fanc-fly-3.0.1/fanc/transforms/template_alignment.py`

 * *Files identical despite different names*

### Comparing `fanc-fly-3.0.0/fanc/transforms/transform_parameters/TransformParameters.FixedFANC.txt` & `fanc-fly-3.0.1/fanc/transforms/transform_parameters/TransformParameters.FixedFANC.txt`

 * *Files identical despite different names*

### Comparing `fanc-fly-3.0.0/fanc/transforms/transform_parameters/TransformParameters.FixedTemplate.Bspline.txt` & `fanc-fly-3.0.1/fanc/transforms/transform_parameters/TransformParameters.FixedTemplate.Bspline.txt`

 * *Files identical despite different names*

### Comparing `fanc-fly-3.0.0/fanc/transforms/transform_parameters/TransformParameters.FixedTemplate.affine.txt` & `fanc-fly-3.0.1/fanc/transforms/transform_parameters/TransformParameters.FixedTemplate.affine.txt`

 * *Files identical despite different names*

### Comparing `fanc-fly-3.0.0/fanc/upload.py` & `fanc-fly-3.0.1/fanc/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,16 +172,16 @@
 
 
 class SomaTableOrganizer(object):
     def __init__(
         self,
         client=None
     ):
-        self._client = client      
-        
+        self._client = client
+
     def initialize(self,
                    soma_table_name="",
                    subset_table_name=""):
         """
         Set soma table and subset table you want to edit.
 
         ---Arguments---
@@ -239,28 +239,28 @@
         return self._soma_table
 
     @property
     def subset_table(self):
         return self._subset_table
 
     @property
-    def subset_table_dict(self):    
+    def subset_table_dict(self):
         return self._subset_table_dict
 
     @subset_table_dict.setter
     def subset_table_dict(self, value):
         self._subset_table_dict = value
 
     def _required_props(self):
         return self._client.schema.schema_definition('nucleus_detection')['definitions']['NucleusDetection']['required']
 
     def add_radius_column(self, soma_table):
         if ('bb_start_position' not in soma_table.columns) or ('bb_end_position' not in soma_table.columns):
             raise ValueError("Need 'bb_start_position' and 'bb_end_position' columns.")
-        
+
         soma_table['radius_nm'] = 0
         for i, r in soma_table.iterrows():
             if soma_table['bb_start_position'][i] is not np.nan and soma_table['bb_end_position'][i] is not np.nan:
                 dist = np.array(soma_table['bb_end_position'][i]) - np.array(soma_table['bb_start_position'][i])
                 soma_table.at[i,'radius_nm'] = np.linalg.norm(dist[:2])/2 # distance in nm in xy plane
             else:
                 soma_table.at[i,'radius_nm'] = 10 # np.nan
@@ -283,24 +283,24 @@
     def _get_man_id_column(self, length, initial_digit=1, digit=17):
         ExistingID = self.find_manual_ids(self._soma_table.id.values, initial_digit=1)
         if len(ExistingID) >0:
             MaxExistingID = np.max(ExistingID)
         else:
             MaxExistingID =initial_digit*10**(digit-1)
         return [MaxExistingID + i for i in range(1, 1+length)]
-    
+
     def _check_change(self, table_name, timestamp=datetime.utcnow()):
         try:
             return self._client.materialize.live_live_query(table_name, timestamp, allow_missing_lookups=False).reset_index(level=0)
         except HTTPError as e:
             raise UpdateUnsuccessful(red(e.response.text + "Please check after 1 hour. Only works between 10 AM - 12 AM PST."))
 
     def update_tables(self, timestamp=datetime.utcnow()):
         """
-        Update both soma table and subset table to the most recent version. Will give 
+        Update both soma table and subset table to the most recent version. Will give
         an error if newly added points are not ingested yet.
         """
         self._soma_table = self._check_change(self._soma_table_name, timestamp)
         self._subset_table = self._check_change(self._subset_table_name, timestamp)
 
     def _validate(self, df):
         stage = self._client.annotation.stage_annotations(self._soma_table_name, schema_name="nucleus_detection", id_field=True)
@@ -314,15 +314,15 @@
         if sum(overlap) == 0:
             pass
         else:
             raise UploadUnsuccessful("The information below has root ids that are already registed in soma table. \n {}".format(df.drop(columns=['id'])[overlap].to_string()))
 
     def join_table(self):
         return self._subset_table.join(self._soma_table.set_index('id'), on='target_id', lsuffix='_subset', rsuffix='_soma')
-    
+
     def preview(self, asPoint=True, asSphere=False):
         """
         Generate Neuroglancer link to inspect somata on the subset table.
 
         ---Arguments---
         asPoint: bool (default True)
             If True, produce an annotation layer that has all the subset somas as points
@@ -558,39 +558,39 @@
     points: pd.DataFrame
         Point coordinates (with or without IDs that you want to use) of somata to upload
 
     is_neuron: bool
         True, if it is neuron
 
     pt_position_column: str
-        If points has a column of point coordinates and use a non-standarized name (i.e., not 'pt_position'), 
+        If points has a column of point coordinates and use a non-standarized name (i.e., not 'pt_position'),
         you need to tell the name of the column to this code.
 
     id_column: str
-        If points has a column of IDs and use a non-standarized name (i.e., not 'id'),  you need to tell the 
-        name of the column to this code. If you don't have preference, you can use np.nan (by default). 
-        The code then will check the nucleus IDs by looking up the same coordinates on the nucleus segmentation, 
-        and use the nucleus IDs that it finds. If it cannot find anything, then the code will generate 
+        If points has a column of IDs and use a non-standarized name (i.e., not 'id'),  you need to tell the
+        name of the column to this code. If you don't have preference, you can use np.nan (by default).
+        The code then will check the nucleus IDs by looking up the same coordinates on the nucleus segmentation,
+        and use the nucleus IDs that it finds. If it cannot find anything, then the code will generate
         "meaningless" artificial annotation IDs for this soma.
     """
     sto = SomaTableOrganizer(client=auth.get_caveclient())
     if is_neuron:
         sto.initialize(subset_table_name='neuron')
     else:
         sto.initialize(subset_table_name='glia')
-    
+
     if len(points.columns)<2:
         points['id'] = np.nan
 
     points = points.rename(columns={pt_position_column: 'pt_position', id_column: 'id'})
     sto.add_dataframe(points)
     # transfer_segmentation()
 
 
 class UploadUnsuccessful(Exception):
-    def __init__(self, message):      
+    def __init__(self, message):
         super().__init__(red("Uploading failed. ") + message)
 
 
 class UpdateUnsuccessful(Exception):
-    def __init__(self, message):      
+    def __init__(self, message):
         super().__init__(red("Updating failed. ") + message)
```

### Comparing `fanc-fly-3.0.0/fanc/visualize.py` & `fanc-fly-3.0.1/fanc/visualize.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         CAVEclient to use instead of the default one
 
     Returns
     -------
     vtk.vtkRenderer
         renderer when code was finished
     png
-        output png image 
+        output png image
         (generate two images with/without scale bar if you specify to plot it)
     """
 
     if isinstance(segment_ids, (int, np.integer)):
         segment_ids = [segment_ids]
 
     colormap = cm.get_cmap(cmap, len(segment_ids))
@@ -217,33 +217,33 @@
             else:
                 scale_bar_ctr = np.array(scale_bar_origin_2D)*np.array(resolution) - np.array([0,scale_bar_length,0])
                 scale_bar_actor = scale_bar_actor_2D(scale_bar_ctr,view=view,camera=camera,length=scale_bar_length,linewidth=1)
         else:
             raise Exception('Need camera to set up scale bar')
 
     if (scale_bar_origin_3D is None) and (scale_bar_origin_2D is None):
-        trimesh_vtk.render_actors(all_actors, camera=camera, do_save=save, 
-                                  filename=save_path, 
+        trimesh_vtk.render_actors(all_actors, camera=camera, do_save=save,
+                                  filename=save_path,
                                   scale=4, video_width=width, video_height=height)
     elif save_path is None:
-        trimesh_vtk.render_actors((all_actors + [scale_bar_actor]), camera=camera, do_save=save, 
-                                  filename=save_path, 
+        trimesh_vtk.render_actors((all_actors + [scale_bar_actor]), camera=camera, do_save=save,
+                                  filename=save_path,
                                   scale=4, video_width=width, video_height=height)
     else:
-        trimesh_vtk.render_actors(all_actors, camera=camera, do_save=save, 
-                                  filename=save_path, 
+        trimesh_vtk.render_actors(all_actors, camera=camera, do_save=save,
+                                  filename=save_path,
                                   scale=1, video_width=width, video_height=height)
-        trimesh_vtk.render_actors((all_actors + [scale_bar_actor]), camera=camera, do_save=save, 
-                                    filename=(save_path.rsplit('.', 1)[0] + '_scalebar.' + save_path.rsplit('.', 1)[1]), 
+        trimesh_vtk.render_actors((all_actors + [scale_bar_actor]), camera=camera, do_save=save,
+                                    filename=(save_path.rsplit('.', 1)[0] + '_scalebar.' + save_path.rsplit('.', 1)[1]),
                                     scale=1, video_width=width, video_height=height)
 
 
 def scale_bar_actor_2D(center, camera, view='X', length=10000, color=(0, 0, 0), linewidth=5, font_size=20):
     """
-    Creates a scale bar actor very similar to trimesh_vtk.scale_bar_actor(), but on a specific plane with 
+    Creates a scale bar actor very similar to trimesh_vtk.scale_bar_actor(), but on a specific plane with
     a given size.
     """
     axes_actor = vtk.vtkCubeAxesActor2D()
     axes_actor.SetBounds(center[0], center[0]+length,
                          center[1], center[1]+length,
                          center[2], center[2]+length)
```

### Comparing `fanc-fly-3.0.0/fanc_fly.egg-info/PKG-INFO` & `fanc-fly-3.0.1/fanc_fly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fanc-fly
-Version: 3.0.0
+Version: 3.0.1
 Summary: Tools for the Female Adult Nerve Cord Drosophila EM dataset
 Home-page: https://github.com/htem/FANC_auto_recon
 Author: Jasper Phelps
 Author-email: jasper.s.phelps@gmail.com
 License: UNKNOWN
 Description: # FANC_auto_recon
```

### Comparing `fanc-fly-3.0.0/fanc_fly.egg-info/SOURCES.txt` & `fanc-fly-3.0.1/fanc_fly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fanc-fly-3.0.0/setup.py` & `fanc-fly-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open('requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
     requirements = [l for l in requirements if not l.startswith('#')]
 
 setuptools.setup(
     name='fanc-fly',
-    version='3.0.0',
+    version='3.0.1',
     author='Jasper Phelps',
     author_email='jasper.s.phelps@gmail.com',
     description='Tools for the Female Adult Nerve Cord Drosophila EM dataset',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/htem/FANC_auto_recon',
     packages=setuptools.find_packages(),
```

### Comparing `fanc-fly-3.0.0/tests/test_lookup.py` & `fanc-fly-3.0.1/tests/test_lookup.py`

 * *Files identical despite different names*

