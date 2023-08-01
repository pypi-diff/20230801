# Comparing `tmp/tissue-tag-0.1.6.tar.gz` & `tmp/tissue-tag-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tissue-tag-0.1.6.tar", last modified: Tue Jul  4 16:07:16 2023, max compression
+gzip compressed data, was "tissue-tag-0.1.7.tar", last modified: Tue Aug  1 20:54:09 2023, max compression
```

## Comparing `tissue-tag-0.1.6.tar` & `tissue-tag-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 16:07:16.500917 tissue-tag-0.1.6/
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1497 2023-06-30 14:25:56.000000 tissue-tag-0.1.6/LICENSE
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     2148 2023-07-04 16:07:16.500917 tissue-tag-0.1.6/PKG-INFO
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1764 2023-07-04 15:55:26.000000 tissue-tag-0.1.6/README.md
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       38 2023-07-04 16:07:16.500917 tissue-tag-0.1.6/setup.cfg
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      813 2023-07-04 16:07:03.000000 tissue-tag-0.1.6/setup.py
-drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 16:07:16.500917 tissue-tag-0.1.6/tissue_tag/
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:55:26.000000 tissue-tag-0.1.6/tissue_tag/__init__.py
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)    45249 2023-07-04 15:55:26.000000 tissue-tag-0.1.6/tissue_tag/tissue_tag.py
-drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 16:07:16.500917 tissue-tag-0.1.6/tissue_tag.egg-info/
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     2148 2023-07-04 16:07:16.000000 tissue-tag-0.1.6/tissue_tag.egg-info/PKG-INFO
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      243 2023-07-04 16:07:16.000000 tissue-tag-0.1.6/tissue_tag.egg-info/SOURCES.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        1 2023-07-04 16:07:16.000000 tissue-tag-0.1.6/tissue_tag.egg-info/dependency_links.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       84 2023-07-04 16:07:16.000000 tissue-tag-0.1.6/tissue_tag.egg-info/requires.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       11 2023-07-04 16:07:16.000000 tissue-tag-0.1.6/tissue_tag.egg-info/top_level.txt
+drwxr-xr-x   0 oamsalem  (1001) users      (100)        0 2023-08-01 20:54:09.221175 tissue-tag-0.1.7/
+-rw-r--r--   0 oamsalem  (1001) users      (100)     1497 2023-08-01 20:50:30.000000 tissue-tag-0.1.7/LICENSE
+-rw-r--r--   0 oamsalem  (1001) users      (100)     2629 2023-08-01 20:54:09.221175 tissue-tag-0.1.7/PKG-INFO
+-rw-r--r--   0 oamsalem  (1001) users      (100)     2245 2023-08-01 20:50:30.000000 tissue-tag-0.1.7/README.md
+-rw-r--r--   0 oamsalem  (1001) users      (100)       38 2023-08-01 20:54:09.221175 tissue-tag-0.1.7/setup.cfg
+-rw-r--r--   0 oamsalem  (1001) users      (100)      813 2023-08-01 20:53:40.000000 tissue-tag-0.1.7/setup.py
+drwxr-xr-x   0 oamsalem  (1001) users      (100)        0 2023-08-01 20:54:09.221175 tissue-tag-0.1.7/tissue_tag/
+-rw-r--r--   0 oamsalem  (1001) users      (100)       26 2023-08-01 20:50:30.000000 tissue-tag-0.1.7/tissue_tag/__init__.py
+-rw-r--r--   0 oamsalem  (1001) users      (100)    56779 2023-08-01 20:50:30.000000 tissue-tag-0.1.7/tissue_tag/tissue_tag.py
+drwxr-xr-x   0 oamsalem  (1001) users      (100)        0 2023-08-01 20:54:09.221175 tissue-tag-0.1.7/tissue_tag.egg-info/
+-rw-r--r--   0 oamsalem  (1001) users      (100)     2629 2023-08-01 20:54:09.000000 tissue-tag-0.1.7/tissue_tag.egg-info/PKG-INFO
+-rw-r--r--   0 oamsalem  (1001) users      (100)      243 2023-08-01 20:54:09.000000 tissue-tag-0.1.7/tissue_tag.egg-info/SOURCES.txt
+-rw-r--r--   0 oamsalem  (1001) users      (100)        1 2023-08-01 20:54:09.000000 tissue-tag-0.1.7/tissue_tag.egg-info/dependency_links.txt
+-rw-r--r--   0 oamsalem  (1001) users      (100)       84 2023-08-01 20:54:09.000000 tissue-tag-0.1.7/tissue_tag.egg-info/requires.txt
+-rw-r--r--   0 oamsalem  (1001) users      (100)       11 2023-08-01 20:54:09.000000 tissue-tag-0.1.7/tissue_tag.egg-info/top_level.txt
```

### Comparing `tissue-tag-0.1.6/LICENSE` & `tissue-tag-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tissue-tag-0.1.6/PKG-INFO` & `tissue-tag-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tissue-tag
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tissue Tag: jupyter image annotator
 Home-page: https://github.com/nadavyayon/TissueTag
 Author: Oren Amsalem, Nadav Yayon
 Author-email: nadav.yayon@mail.huji.ac.il
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -41,11 +41,16 @@
 
 ### importing in a notebook 
 `import tissue_tag as tt`
 
 ## How to cite:
 preprint coming! stay tuned
 
-
+## How to use 
+We supply 2 examples of usage for TissueTag annotations: 
+1) visium spatial transcriptomics 
+2) IBEX singel cell multiplex protein imaging
+   in this example we annotate a postnatal thymus image by calling the major anatomimcal reagios and training a random forst classifier for intial prediction follwed by manual corrections
+   [IBEX flourecent tutorial](https://github.com/nadavyayon/TissueTag/blob/main/Tutorials/image_annotation_tutorial_flourscent_final.ipynb)
```

### Comparing `tissue-tag-0.1.6/README.md` & `tissue-tag-0.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -29,11 +29,16 @@
 
 ### importing in a notebook 
 `import tissue_tag as tt`
 
 ## How to cite:
 preprint coming! stay tuned
 
-
+## How to use 
+We supply 2 examples of usage for TissueTag annotations: 
+1) visium spatial transcriptomics 
+2) IBEX singel cell multiplex protein imaging
+   in this example we annotate a postnatal thymus image by calling the major anatomimcal reagios and training a random forst classifier for intial prediction follwed by manual corrections
+   [IBEX flourecent tutorial](https://github.com/nadavyayon/TissueTag/blob/main/Tutorials/image_annotation_tutorial_flourscent_final.ipynb)
```

### Comparing `tissue-tag-0.1.6/setup.py` & `tissue-tag-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='tissue-tag',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),
     install_requires=[
         'opencv-python',
         'Pillow',
         'bokeh',
         'jupyter-bokeh',
         'matplotlib',
```

### Comparing `tissue-tag-0.1.6/tissue_tag/tissue_tag.py` & `tissue-tag-0.1.7/tissue_tag/tissue_tag.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,29 +8,31 @@
 import pandas as pd
 import pickle
 import random
 import scipy
 import seaborn as sns
 import skimage
 import warnings
+import os
 from bokeh.models import FreehandDrawTool, PolyDrawTool, PolyEditTool,TabPanel, Tabs
 from bokeh.plotting import figure, show
 from functools import partial
 from io import BytesIO
 from packaging import version
 from PIL import Image, ImageColor, ImageDraw, ImageEnhance, ImageFilter, ImageFont
 from scipy import interpolate
 from scipy.spatial import distance
 from skimage import data, feature, future, segmentation
 from skimage.draw import polygon, disk
 from sklearn.ensemble import RandomForestClassifier
 from tqdm import tqdm
 
+
 try:
-    import scanpy as sc
+    import scanpy as scread_visium
 except ImportError:
     print('scanpy is not available')
 
 Image.MAX_IMAGE_PIXELS = None
 
 font_path = fm.findfont('DejaVu Sans')
 
@@ -91,14 +93,15 @@
         If 'ppm_image' is not provided and cannot be extracted from the image metadata.
     """
     
     im = Image.open(path)
     if not(ppm_image):
         try:
             ppm_image = im.info['resolution'][0]
+            print('found ppm in image metadata!, its - '+str(ppm_image))
         except:
             print('could not find ppm in image metadata, please provide ppm value')
     width, height = im.size
     newsize = (int(width/ppm_image*ppm_out), int(height/ppm_image*ppm_out))
     # resize
     im = im.resize(newsize,Image.Resampling.LANCZOS)
     im = im.convert("RGBA")
@@ -768,15 +771,15 @@
     """
     print('generating grid with spot size - '+str(spot_diameter)+', with resolution of - '+str(ppm_in)+' ppm')
     positions = generate_hires_grid(im,spot_diameter,ppm_in)
     positions = positions.astype('float32')
     dim = [im.shape[0],im.shape[1]]
     # transform tissue annotation images to original size
 
-    radius = spot_diameter/8
+    radius = spot_diameter/4 # measure the annotation from the center of the spot 
     df = pd.DataFrame(
         np.vstack((np.array(range(len(positions.T[:,0]))),positions.T[:,0],
                    positions.T[:,1])).T,
         columns=['index','x','y'])
     for idx0,anno in enumerate(annotation_image_list):
         anno_orig = skimage.transform.resize(anno,dim,preserve_range=True).astype('uint8') 
         anno_dict = {}
@@ -803,16 +806,14 @@
 
     Parameters
     ----------
     df : pandas.DataFrame
         Dataframe containing spatial data.
     annotation : str
         The column in df that contains the structure annotation.
-    ppm : float
-        the coordinates of df in pixel scale
     KNN : int, optional
         Determines the number of closest points used to calculate the mean distance. Default is 4.
     calc_dist : bool, optional
         If true, calculates the distance. Default is True.
     logscale : bool, optional
         If true, applies a log10 transformation to the distance. Default is False.
     
@@ -844,14 +845,45 @@
                     df["L2_dist_log10_"+annotation+'_'+c] = np.log10(Dist2ClusterAll[c]/ppm)
                 else:
                     df["L2_dist_"+annotation+'_'+c] = Dist2ClusterAll[c]/ppm
             df[annotation] = categories[np.argmin(np.array(list(Dist2ClusterAll.values())), axis=0)]
     
     return Dist2ClusterAll
 
+def dist2cluster_fast(df, annotation, KNN=5, logscale=False):
+    from scipy.spatial import cKDTree
+
+    print('calculating distance matrix with cKDTree')
+
+    points = np.vstack([df['x'],df['y']]).T
+    categories = np.unique(df[annotation])
+
+    Dist2ClusterAll = {c: np.zeros(df.shape[0]) for c in categories}
+
+    for idx, c in enumerate(categories):
+        indextmp = df[annotation] == c
+        if np.sum(indextmp) > KNN:
+            print(c)
+            cluster_points = points[indextmp]
+            tree = cKDTree(cluster_points)
+            # Get KNN nearest neighbors for each point
+            distances, _ = tree.query(points, k=KNN)
+            # Store the mean distance for each point to the current category
+            if KNN == 1:
+                Dist2ClusterAll[c] = distances # No need to take mean if only one neighbor
+            else:
+                Dist2ClusterAll[c] = np.mean(distances, axis=1)
+
+    for c in categories:              
+        if logscale:
+            df["L2_dist_log10_"+annotation+'_'+c] = np.log10(Dist2ClusterAll[c])
+        else:
+            df["L2_dist_"+annotation+'_'+c] = Dist2ClusterAll[c]
+
+    return Dist2ClusterAll
 
     
 def anno_to_cells(df_cells, x_col, y_col, df_grid, annotation='annotations', plot=True):
     """
     Maps tissue annotations to segmented cells by nearest neighbors.
     
     Parameters
@@ -1256,79 +1288,358 @@
     out_img[:, :, 3] = 255
 
     if show:
         plt.imshow(out_img, origin='lower')
 
     return out_img
 
+
 def find_files(directory, query):
     for root, dirs, files in os.walk(directory):
         for file in files:
             if query in file:
                 return os.path.join(root, file)
 
 
-def migrate_annotations(df_source, df_target, ppm_source, ppm_target, plot=True, how='nearest', max_distance=10e10):
+
+def anno_transfer(df_spots, df_grid, ppm_spots, ppm_grid, plot=True, how='nearest', max_distance=10e10):
     """
-    Maps tissue annotations from the source DataFrame to the target DataFrame according to the nearest neighbors.
+    Maps tissue annotations to Visium spots according to the nearest neighbors.
     
     Parameters
     ----------
-    df_source : pandas.DataFrame
-        Source DataFrame with annotations.
-    df_target : pandas.DataFrame
-        Target DataFrame where annotations will be migrated.
-    ppm_source : float 
-        pixels per micron of the source DataFrame
-    ppm_target : float 
-        pixels per micron of the target DataFrame
+    df_spots : pandas.DataFrame
+        Dataframe with Visium spot data.
+    df_grid : pandas.DataFrame
+        Dataframe with grid data.
+    ppm_spots : float 
+        pixels per micron of spots
+    ppm_grid : float 
+        pixels per micron of grid
     plot : bool, optional
-        If true, plots the coordinates of the source and target spaces to make sure 
+        If true, plots the coordinates of the grid space and the spot space to make sure 
         they are aligned. Default is True.
-    how : string, optional
+    how : string, optinal
         This determines how the association between the 2 grids is made from the scipy.interpolate.griddata function. Default is 'nearest'
-    max_distance : int, optional
-        maximal distance where points are not migrated. Default is 10e10
+    max_distance : int
+        maximal distance where points are not migrated 
 
     Returns
     -------
-    df_target : pandas.DataFrame
-        Updated target DataFrame with annotations migrated from the source DataFrame.
+    df_spots : pandas.DataFrame
+        Updated dataframe with Visium spot data.
     """
     import numpy as np
     from scipy.interpolate import griddata
     from scipy.spatial import cKDTree
     import matplotlib.pyplot as plt
     
     print('Make sure the coordinate systems are aligned, e.g., axes are not flipped.') 
-    source_coords = np.vstack([df_source['x']*ppm_source, df_source['y']*ppm_source])
-    target_coords = np.vstack([df_target['x']*ppm_target, df_target['y']*ppm_target])
+    a = np.vstack([df_grid['x']/ppm_grid, df_grid['y']/ppm_grid])
+    b = np.vstack([df_spots['x']/ppm_spots, df_spots['y']/ppm_spots])
     
     if plot:
         plt.figure(dpi=100, figsize=[10, 10])
-        plt.title('Target space')
-        plt.plot(target_coords[0], target_coords[1], '.', markersize=1)
+        plt.title('Spot space')
+        plt.plot(b[0], b[1], '.', markersize=1)
         plt.show()
         
         plt.figure(dpi=100, figsize=[10, 10])
-        plt.plot(source_coords[0], source_coords[1], '.', markersize=1)
-        plt.title('Source space')
+        plt.plot(a[0], a[1], '.', markersize=1)
+        plt.title('Morpho space')
         plt.show()
+
+    # Create new DataFrame
+    new_df_spots = df_spots[['x', 'y']].copy()
+    
+    annotations = df_grid.columns[~df_grid.columns.isin(['x', 'y'])]
+    
+    for k in annotations:
+        print('Migrating morphology - ' + k + ' to target space.')
+        
+        # Interpolation
+        new_df_spots[k] = griddata(points=a.T, values=df_grid[k], xi=b.T, method=how)
+        
+        # Create KDTree
+        tree = cKDTree(a.T)
+        
+        # Query tree for nearest distance
+        distances, _ = tree.query(b.T, distance_upper_bound=max_distance)
+        
+        # Mask df_spots where the distance is too high
+        new_df_spots[k][distances==np.inf] = None
+  
+    return new_df_spots
+
+
+
+def anno_to_grid(folder, file_name, spot_diameter, load_colors=False,null_number=1):
+    """
+    Load annotations and transform them into a spot grid.
+    
+    Parameters
+    ----------
+    folder : str
+        Folder path for annotations.
+    file_name : str
+        Name for tif image and pickle without extensions.
+    spot_diameter : float
+        The diameter used for grid.
+    load_colors : bool, optional
+        If True, get original colors used for annotations. Default is False.
+    null_numer : int
+        value of the label image where no useful information is stored e.g. background or unassigned pixels (usually 0 or 1). Default is 1
+
+    Returns
+    -------
+    df : pandas.DataFrame
+        Dataframe with the grid annotations.
+    """
+    
+    im, anno_order, ppm, anno_color = load_annotation(folder, file_name, load_colors)
+
+    df = grid_anno(
+        im,
+        [im],
+        [file_name],
+        [anno_order],
+        spot_diameter,
+        ppm,
+        ppm,
+    )
+
+    return df,ppm
+
+
+def map_annotations_to_visium(vis_path, df_grid, ppm_grid, spot_diameter, plot=True, how='nearest', max_distance_factor=50, use_resolution='hires', res_in_ppm=1, count_file='raw_feature_bc_matrix.h5'):
+    """
+    Processes Visium data with high-resolution grid.
+
+    Parameters
+    ----------
+    vis_path : str
+        Path to the Visium data.
+    df_grid : pandas.DataFrame
+        Dataframe with grid data.
+    ppm_grid : float 
+        Pixels per micron of grid.
+    spot_diameter : float
+        Diameter of the spots.
+    plot : bool, optional
+        If true, plots the coordinates of the grid space and the spot space to make sure they are aligned. Default is True.
+    how : string, optinal
+        This determines how the association between the 2 grids is made from the scipy.interpolate.griddata function. Default is 'nearest'
+    max_distance_factor : int
+        Factor to calculate maximal distance where points are not migrated. The final max_distance used will be max_distance_factor * ppm_visium.
+    use_resolution : str, optional
+        Resolution to use. Default is 'hires'.
+    res_in_ppm : float, optional
+        Resolution in pixels per micron. Default is 1.
+    count_file : str, optional
+        Filename of the count file. Default is 'raw_feature_bc_matrix.h5'.
+
+    Returns
+    -------
+    adata_vis : anndata.AnnData
+        Annotated data matrix with Visium spot data and additional annotations.
+    """
+    import scanpy as sc
+    # calculate distance matrix between hires and visium spots
+    im, ppm_visium, visium_positions = read_visium(spaceranger_dir_path=vis_path+'/', use_resolution=use_resolution, res_in_ppm=res_in_ppm, plot=False)
+    
+    # rename columns for visium_positions DataFrame
+    visium_positions.rename(columns={'pxl_row_in_fullres': "y", 'pxl_col_in_fullres': "x"}, inplace=True) 
+
+    # Transfer annotations
+    spot_annotations = anno_transfer(df_spots=visium_positions, df_grid=df_grid, ppm_spots=ppm_visium, ppm_grid=ppm_grid, plot=plot, how=how, max_distance=max_distance_factor * ppm_visium)
+
+    # Read visium data
+    adata_vis = sc.read_visium(vis_path, count_file=count_file)
+
+    # Merge with adata_vis
+    adata_vis.obs = pd.concat([adata_vis.obs, spot_annotations], axis=1)
+
+    # Convert to int
+    adata_vis.obsm['spatial'] = adata_vis.obsm['spatial'].astype('int')
+
+    # Add to uns
+    adata_vis.uns['hires_grid'] = df_grid
+    adata_vis.uns['hires_grid_ppm'] = ppm_grid
+    adata_vis.uns['hires_grid_diam'] = spot_diameter
+    adata_vis.uns['visium_ppm'] = ppm_visium
+
+
+
+    return adata_vis
+
+
+def load_and_combine_annotations(folder, file_names, spot_diameter, load_colors=True):
+    """
+    Load tissue annotations from multiple files and combine them into a single DataFrame.
+
+    Parameters
+    ----------
+    folder : str
+        Folder path where the annotation files are stored.
+    file_names : list of str
+        List of names of the annotation files.
+    spot_diameter : int
+        Diameter of the spots.
+    load_colors : bool, optional
+        Whether to load colors. Default is True.
+
+    Returns
+    -------
+    df : pandas.DataFrame
+        DataFrame that combines all the loaded annotations.
+    ppm_grid : float
+        Pixels per micron for the grid of the last loaded annotation.
+    """
+    df_list = []
+    ppm_grid = None
+
+    for file_name in file_names:
+        df, ppm_grid = anno_to_grid(folder=folder, file_name=file_name, spot_diameter=spot_diameter, load_colors=load_colors)
+        df_list.append(df)
+
+    # Concatenate all dataframes
+    df = pd.concat(df_list, join='inner', axis=1)
+
+    # Remove duplicated columns
+    df = df.loc[:, ~df.columns.duplicated()].copy()
+
+    return df, ppm_grid
+
+def annotate_l2(df_target, df_grid, annotation='annotations_level_0', KNN=10, max_distance_factor=50, plot=False,calc_dist=True):
+    """
+    Process the given AnnData object to calculate distances and perform annotation transfer.
+    
+    Parameters
+    ----------
+    df_target : pandas.DataFrame
+        Dataframe with target data to be annotated.
+    df_grid : pandas.DataFrame
+        Dataframe with annotation data.
+    annotation : str, optional
+        Annotation column to be used for calculating distances, by default 'annotations_level_0'.
+    ppm_grid : float
+        should be the ppm resolution fot the grid data for visium would be stored here - adata_vis.uns['hires_grid_ppm']
+    ppm_spots : float
+        should be the ppm resolution fot the target data for visium would be stored here - adata_vis.uns['visium_ppm']
+    KNN : int, optional
+        Number of nearest neighbors to be considered for distance calculation, by default 10.
+    max_distance_factor : int, optional
+        Factor by which to calculate the maximum distance for annotation transfer, by default 50 in microns.
+    plot : bool, optional
+        Whether to plot during the annotation transfer, by default False.
+     calc_dist : bool, optional
+        If true, calculates the L2 distance. Default is True otherwise just migrates discrete annotations.
+    
+    Returns
+    -------
+    anndata.AnnData
+        Processed AnnData object with updated observations.
+    """
+    
+    df = df.obs[['x','y']].dropna()
+    dist2cluster_fast(df_grid, annotation=annotation, KNN=KNN,calc_dist=calc_dist) # calculate minimum mean distance of each spot to clusters 
+    df_grid_new = df_grid.filter(like=annotation)
+    df_grid_new['x'] = df_grid['x']
+    df_grid_new['y'] = df_grid['y']
+    spot_annotations = anno_transfer(df_spots=df_visium, df_grid=df_grid_new, ppm_spots=ppm_spots, ppm_grid=adata_vis.uns['hires_grid_ppm'], max_distance=max_distance_factor * adata_vis.uns['visium_ppm'], plot=plot)
+    for col in spot_annotations:
+        adata_vis.obs[col] = spot_annotations[col]
+        adata_vis.uns['hires_grid'][col] = df_grid_new[col]
+    # df1 = pd.concat([adata_vis.obs, spot_annotations], axis=1)
+    # df1 = df1.loc[:, ~df1.columns.duplicated()].copy()
+    # adata_vis.obs = df1
+
+    return adata_vis
+
+
+
+def map_annotations_to_target(df_source, df_target, ppm_source,ppm_target, plot=True, how='nearest', max_distance=50):
+    """
+    map annotations to any form of of csv where you have x y cooodinates spot df (cells or spots) data with high-resolution grid.
+    note! - xy coordinates must be named 'x' and 'y'
+
+    Parameters
+    ----------
+    df_source : pandas.DataFrame
+        Dataframe with grid data.
+    df_target : pandas.DataFrame
+        Dataframe with target data.
+    ppm_source : float 
+        Pixels per micron of source data.
+    ppm_target : float 
+        Pixels per micron of target data.
+    plot : bool, optional
+        If true, plots the coordinates of the grid space and the spot space to make sure they are aligned. Default is True.
+    how : string, optinal
+        This determines how the association between the 2 grids is made from the scipy.interpolate.griddata function. Default is 'nearest'
+        if the data is categorial then only the 'nearest' would work but if interpolation is needed one should supbset to only numeric data.
+    max_distance : int
+        Factor to calculate maximal distance where points are not migrated. The final max_distance used will be max_distance * ppm_target.
+   
+    Returns
+    -------
+    df_target : pandas.DataFrame
+        Annotated dataframe with additional annotations from the source data.
+    """
+    from scipy.interpolate import griddata
+    from scipy.spatial import cKDTree
+
     
-    annotations = df_source.columns[~df_source.columns.isin(['x', 'y'])]
+    # generate matched coordinate space 
+    a = np.vstack([df_source['x']/ppm_source, df_source['y']/ppm_source])
+    b = np.vstack([df_target['x']/ppm_target, df_target['y']/ppm_target])
+    
+    if plot:
+        print('Make sure the coordinate systems are aligned, e.g., axes are not flipped and the resolution is matched.') 
+        plt.figure(dpi=100, figsize=[10, 10])
+        plt.title('Target space')
+        plt.plot(b[0], b[1], '.', markersize=1)
+        plt.show()
+        
+        plt.figure(dpi=100, figsize=[10, 10])
+        plt.plot(a[0], a[1], '.', markersize=1)
+        plt.title('source space')
+        plt.show()
+
+    annotations = df_source.columns[~df_source.columns.isin(['x', 'y'])] # extract annotation categories
     
     for k in annotations:
-        print('Migrating - ' + k + ' to target DataFrame.')
+        print('Migrating source annotation - ' + k + ' to target space.')
         
         # Interpolation
-        df_target[k] = griddata(points=source_coords.T, values=df_source[k], xi=target_coords.T, method=how)
+        df_target[k] = griddata(points=a.T, values=df_source[k], xi=b.T, method=how)
         
         # Create KDTree
-        tree = cKDTree(source_coords.T)
+        tree = cKDTree(a.T)
         
         # Query tree for nearest distance
-        distances, _ = tree.query(target_coords.T, distance_upper_bound=max_distance)
+        distances, _ = tree.query(b.T, distance_upper_bound=max_distance)
         
-        # Mask df_target where the distance is too high
+        # Mask df_spots where the distance is too high
         df_target[k][distances==np.inf] = None
   
     return df_target
+
+
+def read_visium_table(vis_path):
+    """
+    This function reads a scale factor from a json file and a table from a csv file, 
+    then calculates the 'ppm' value and returns the table with the new column names.
+    
+    note that for CytAssist the header is changes so this funciton should be updated
+    """
+    with open(vis_path + '/spatial/scalefactors_json.json', 'r') as f:
+        scalef = json.load(f)
+
+    ppm = scalef['spot_diameter_fullres'] / 55 
+
+    df_visium_spot = pd.read_csv(vis_path + '/spatial/tissue_positions_list.csv', header=None)
+
+    df_visium_spot.rename(columns={4:'y',5:'x',1:'in_tissue',0:'barcode'}, inplace=True)
+    df_visium_spot.set_index('barcode', inplace=True)
+
+    return df_visium_spot, ppm
```

### Comparing `tissue-tag-0.1.6/tissue_tag.egg-info/PKG-INFO` & `tissue-tag-0.1.7/tissue_tag.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tissue-tag
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tissue Tag: jupyter image annotator
 Home-page: https://github.com/nadavyayon/TissueTag
 Author: Oren Amsalem, Nadav Yayon
 Author-email: nadav.yayon@mail.huji.ac.il
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -41,11 +41,16 @@
 
 ### importing in a notebook 
 `import tissue_tag as tt`
 
 ## How to cite:
 preprint coming! stay tuned
 
-
+## How to use 
+We supply 2 examples of usage for TissueTag annotations: 
+1) visium spatial transcriptomics 
+2) IBEX singel cell multiplex protein imaging
+   in this example we annotate a postnatal thymus image by calling the major anatomimcal reagios and training a random forst classifier for intial prediction follwed by manual corrections
+   [IBEX flourecent tutorial](https://github.com/nadavyayon/TissueTag/blob/main/Tutorials/image_annotation_tutorial_flourscent_final.ipynb)
```

