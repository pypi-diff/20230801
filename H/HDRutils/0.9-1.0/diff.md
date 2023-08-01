# Comparing `tmp/HDRutils-0.9.tar.gz` & `tmp/HDRutils-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HDRutils-0.9.tar", last modified: Thu Jan  6 14:35:43 2022, max compression
+gzip compressed data, was "HDRutils-1.0.tar", last modified: Tue Aug  1 11:56:02 2023, max compression
```

## Comparing `HDRutils-0.9.tar` & `HDRutils-1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 pmh64     (4240) pmh64     (4240)        0 2022-01-06 14:35:43.895869 HDRutils-0.9/
-drwxrwxr-x   0 pmh64     (4240) pmh64     (4240)        0 2022-01-06 14:35:43.702864 HDRutils-0.9/HDRutils/
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)      222 2021-08-24 15:15:35.000000 HDRutils-0.9/HDRutils/__init__.py
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     1018 2021-11-14 16:54:34.000000 HDRutils-0.9/HDRutils/graphs.py
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     3129 2021-06-11 13:55:56.000000 HDRutils-0.9/HDRutils/io.py
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     8754 2022-01-06 12:48:47.000000 HDRutils-0.9/HDRutils/merge.py
-drwxrwxr-x   0 pmh64     (4240) pmh64     (4240)        0 2022-01-06 14:35:43.879863 HDRutils-0.9/HDRutils/noise_modeling/
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)        0 2021-08-24 15:15:35.000000 HDRutils-0.9/HDRutils/noise_modeling/__init__.py
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)  1096085 2021-10-14 09:58:00.000000 HDRutils-0.9/HDRutils/noise_modeling/darktable.json
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     5087 2022-01-06 14:03:13.000000 HDRutils-0.9/HDRutils/noise_modeling/simulate.py
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)    15584 2022-01-06 12:59:13.000000 HDRutils-0.9/HDRutils/utils.py
-drwxrwxr-x   0 pmh64     (4240) pmh64     (4240)        0 2022-01-06 14:35:43.796869 HDRutils-0.9/HDRutils.egg-info/
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     4995 2022-01-06 14:35:43.000000 HDRutils-0.9/HDRutils.egg-info/PKG-INFO
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)      409 2022-01-06 14:35:43.000000 HDRutils-0.9/HDRutils.egg-info/SOURCES.txt
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)        1 2022-01-06 14:35:43.000000 HDRutils-0.9/HDRutils.egg-info/dependency_links.txt
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)       97 2022-01-06 14:35:43.000000 HDRutils-0.9/HDRutils.egg-info/requires.txt
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)        9 2022-01-06 14:35:43.000000 HDRutils-0.9/HDRutils.egg-info/top_level.txt
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     1068 2021-04-20 12:09:45.000000 HDRutils-0.9/LICENSE
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)       46 2021-08-24 15:15:35.000000 HDRutils-0.9/MANIFEST.in
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     4995 2022-01-06 14:35:43.897866 HDRutils-0.9/PKG-INFO
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     4081 2022-01-06 14:22:23.000000 HDRutils-0.9/README.md
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)      131 2022-01-06 14:35:43.910865 HDRutils-0.9/setup.cfg
--rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     1424 2022-01-06 14:24:11.000000 HDRutils-0.9/setup.py
+drwxrwxr-x   0 pmh64     (4240) pmh64     (4240)        0 2023-08-01 11:56:02.575546 HDRutils-1.0/
+drwxrwxr-x   0 pmh64     (4240) pmh64     (4240)        0 2023-08-01 11:56:01.999541 HDRutils-1.0/HDRutils/
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)      272 2022-09-05 22:09:54.000000 HDRutils-1.0/HDRutils/__init__.py
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     6605 2022-09-06 16:10:36.000000 HDRutils-1.0/HDRutils/capture.py
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     8970 2023-08-01 11:15:35.000000 HDRutils-1.0/HDRutils/exposures.py
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     1018 2021-11-14 16:54:34.000000 HDRutils-1.0/HDRutils/graphs.py
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     3755 2023-01-04 22:28:02.000000 HDRutils-1.0/HDRutils/io.py
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)    11021 2023-08-01 11:09:48.000000 HDRutils-1.0/HDRutils/merge.py
+drwxrwxr-x   0 pmh64     (4240) pmh64     (4240)        0 2023-08-01 11:56:02.552540 HDRutils-1.0/HDRutils/noise_modeling/
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)        0 2021-08-24 15:15:35.000000 HDRutils-1.0/HDRutils/noise_modeling/__init__.py
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)  1096085 2021-10-14 09:58:00.000000 HDRutils-1.0/HDRutils/noise_modeling/darktable.json
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     5145 2022-07-14 12:10:47.000000 HDRutils-1.0/HDRutils/noise_modeling/simulate.py
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)    10028 2023-01-04 22:28:02.000000 HDRutils-1.0/HDRutils/utils.py
+drwxrwxr-x   0 pmh64     (4240) pmh64     (4240)        0 2023-08-01 11:56:02.096540 HDRutils-1.0/HDRutils.egg-info/
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     7170 2023-08-01 11:56:01.000000 HDRutils-1.0/HDRutils.egg-info/PKG-INFO
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)      429 2023-08-01 11:56:01.000000 HDRutils-1.0/HDRutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)        1 2023-08-01 11:56:01.000000 HDRutils-1.0/HDRutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)      112 2023-08-01 11:56:01.000000 HDRutils-1.0/HDRutils.egg-info/requires.txt
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)        9 2023-08-01 11:56:01.000000 HDRutils-1.0/HDRutils.egg-info/top_level.txt
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     1068 2021-04-20 12:09:45.000000 HDRutils-1.0/LICENSE
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     7170 2023-08-01 11:56:02.572546 HDRutils-1.0/PKG-INFO
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     6444 2023-08-01 11:43:42.000000 HDRutils-1.0/README.md
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)       38 2023-08-01 11:56:02.576561 HDRutils-1.0/setup.cfg
+-rw-rw-r--   0 pmh64     (4240) pmh64     (4240)     1442 2023-08-01 11:50:41.000000 HDRutils-1.0/setup.py
```

### Comparing `HDRutils-0.9/HDRutils/graphs.py` & `HDRutils-1.0/HDRutils/graphs.py`

 * *Files identical despite different names*

### Comparing `HDRutils-0.9/HDRutils/io.py` & `HDRutils-1.0/HDRutils/io.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import numpy as np
-import imageio as io, rawpy
+import imageio.v3 as io, rawpy, pyexr
 
 logger = logging.getLogger(__name__)
 
 def imread_libraw(raw, color_space='srgb'):
 	wb = None
 	color_space = color_space.lower()
 	if color_space == 'srgb':
@@ -41,50 +41,66 @@
 	ldr_ext = ('.jpg', '.jpeg', '.png', '.tif', '.tiff')
 	hdr_ext = ('.exr', '.hdr')
 
 	if file.lower().endswith(raw_ext):
 		# Raw formats may be optionally processed with libraw
 		raw = rawpy.imread(file)
 		if libraw:
-			return imread_libraw(raw, color_space)
+			img = imread_libraw(raw, color_space)
 		else:
-			return raw.raw_image_visible
+			img = raw.raw_image_visible
 	else:
 		# Imagio imread should handle most formats
 		if file.lower().endswith(ldr_ext):
 			logger.info('LDR image file format provided')
 			if file.lower().endswith('.png'):
 				# 16-bit pngs require an additional flag
-				return io.imread(file, format='PNG-FI')
+				img = io.imread(file, plugin='PNG-FI')
 		elif file.lower().endswith(hdr_ext):
 			logger.info('HDR image file format provided')
+			if file.lower().endswith('.exr'):
+				# Imagio's exr is inaccuarate
+				# See https://github.com/imageio/imageio/issues/517
+				precisions = pyexr.open(file).precisions
+				assert precisions.count(precisions[0]) == len(precisions), 'All channels must have same precision'
+				img = pyexr.read(file, precision=precisions[0])
+			elif file.lower().endswith('.hdr'):
+				img = io.imread(file)
 		else:
 			logger.warning('Unknown image file format. Reverting to imageio imread')
-		return io.imread(file)
+			img = io.imread(file)
+	return img
 
 
 def imwrite(file, img):
 	"""
 	Wrapper for io.imwrite with some inital sanity checks
 
 	:file: output filename with correct extension
 	:img: HDR image to write; datatype should ideally be floating point image
 	"""
 	written = False
 	if img.dtype in (np.uint8, np.uint16):
 		logger.info(f'LDR image provided, it is encoded using {img.dtype}')
 		if file.endswith('.png'):
 			# 16-bit pngs require an additional flag
-			io.imwrite(file, img, format='PNG-FI')
+			io.imwrite(file, img, plugin='PNG-FI')
 			written = True
-	elif img.dtype in (np.float32, np.float64, np.float128):
-		if file.endswith(('.exr', '.hdr')):
+	elif img.dtype in (np.float32, np.float64):
+		if file.endswith('.hdr'):
 			# Imegio needs an additional flag to prevent clipping to (2**16 - 1)
-			io.imwrite(file, img.astype(np.float32), flags=0x0001)
+			io.imwrite(file, img.astype(np.float32))
+			written = True
+		elif file.endswith('.exr'):
+			pyexr.write(file, img.astype(np.float32))
 			written = True
 	elif img.dtype == np.float16:
-		if file.endswith(('.exr', '.hdr')):
+		if file.endswith('.hdr'):
+			logger.warning('Cannot write float16 to .hdr, converting to float32')
 			io.imwrite(file, img.astype(np.float32))
 			written = True
+		elif file.endswith('.exr'):
+			pyexr.write(file, img, precision=pyexr.HALF)
+			written = True
 	if not written:
 		logger.warning('Unknown extension/datatype. Reverting to imageio imwrite')
 		io.imwrite(file, img)
```

### Comparing `HDRutils-0.9/HDRutils/merge.py` & `HDRutils-1.0/HDRutils/merge.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging, tqdm
 
 import numpy as np
-import rawpy
-import colour_demosaicing as cd
 
 import HDRutils.io as io
 from HDRutils.utils import *
+from HDRutils.exposures import estimate_exposures
 
 logger = logging.getLogger(__name__)
 
 
 def merge(files, do_align=False, demosaic_first=True, normalize=False, color_space='sRGB',
 		  wb=None, saturation_percent=0.98, black_level=0, bayer_pattern='RGGB',
-		  exp=None, gain=None, aperture=None, estimate_exp='gfxdisp', cam='default',
-		  perc=10, outlier='cerman'):
+		  exp=None, gain=None, aperture=None, estimate_exp=None, cam=None,
+		  outlier=None, demosaic='bilinear', clip_highlights=False, bits=None, solver='wls',
+		  return_exif_exp=False):
 	"""
 	Merge multiple SDR images into a single HDR image after demosacing. This is a wrapper
 	function that extracts metadata and calls the appropriate function.
 
 	:files: Filenames containing the inpt images
 	:do_align: Align by estimation homography
 	:demosaic_first: Order of operations
@@ -28,60 +28,85 @@
 	:black_level: Camera's black level
 	:bayer_patter: Color filter array pattern of the camera
 	:exp: Exposure time (in seconds) required when metadata is not present
 	:gain: Camera gain (ISO/100) required when metadata is not present
 	:aperture: Aperture required when metadata is not present
 	:estimate_exp: Estimate exposure times by solving a system. Pick 1 of ['gfxdisp','cerman']
 	:cam: Camera noise model for exposure estimation
-	:perc: Estimate exposures using min-variance rows
 	:outlier: Iterative outlier removal. Pick 1 of [None, 'cerman', 'ransac']
-	:return: Merged FP32 HDR image
+	:demosaic: Demosaicing algorithm if "demosaic_first" is False. Pick 1 of ['bilinear', 'malvar', 'menon']
+	:clip_highlights: Clip pixels that are saturated in the lowest exposure
+	:bits: Number of quantization bits for simulated data
+	:solver: How to solve the linear system for exposure estimation
+
+	:return: Merged FP32 HDR image, mask of unsaturated pixels
 	"""
-	data = get_metadata(files, color_space, saturation_percent, black_level, exp, gain, aperture)
+	data = get_metadata(files, exp, gain, aperture, color_space, saturation_percent, black_level, bits)
+	exif = data['exp'].copy()
 	if estimate_exp:
 		# TODO: Handle imamge stacks with varying gain and aperture
 		assert len(set(data['gain'])) == 1 and len(set(data['aperture'])) == 1
 		if do_align:
 			# TODO: Perform exposure alignment after homography (adds additional overhead since
 			# images need to be demosaiced)
 			logger.warning('Exposure alignment is done before homography, may cause it to fail')
 
 		Y = np.array([io.imread(f, libraw=False) for f in files], dtype=np.float32)
-		exif_exp = data['exp']
 		estimate = np.ones(data['N'], dtype=bool)
+		black_frame = np.tile(data['black_level'].reshape(2, 2), (data['h']//2, data['w']//2))
+		if Y.ndim == 4:
+			assert Y.shape[-1] == 3 or Y[...,3].all() == 0
+			Y = Y[...,:3]
+			black_frame = np.ones_like(Y[0]) * data['black_level'][:3][None,None]
 		for i in range(data['N']):
-			# Skip images where > 90% of the pixels are saturated
-			if (Y[i] >= data['saturation_point']).sum() > 0.9*Y[i].size:
+			# Skip images where > 95% of the pixels are overexposed or underexposed
+			noise_floor = max(data['saturation_point']/1000, np.abs((Y[0] - black_frame).min()))
+			if (Y[i] >= data['saturation_point']).sum() > 0.95*Y[i].size:
 				logger.warning(f'Skipping exposure estimation for file {files[i]} due to saturation')
 				estimate[i] = False
-		data['exp'][estimate] = estimate_exposures(Y[estimate], data['exp'][estimate], data,
-												   estimate_exp, cam=cam, outlier=outlier)
+			elif (Y[i] - black_frame <= noise_floor).sum() > 0.95*Y[i].size:
+				logger.warning(f'Skipping exposure estimation for file {files[i]} due to noise')
+				estimate[i] = False
+		if estimate.sum() > 2:
+			data['exp'][estimate] = estimate_exposures(Y[estimate], data['exp'][estimate], data,
+													   estimate_exp, cam=cam, outlier=outlier,
+													   noise_floor=noise_floor, solver=solver)
 
 	if demosaic_first:
 		HDR, num_sat = imread_demosaic_merge(files, data, do_align, saturation_percent)
 	else:
-		HDR, num_sat = imread_merge_demosaic(files, data, do_align, bayer_pattern)
+		HDR, num_sat = imread_merge_demosaic(files, data, do_align, bayer_pattern, demosaic)
 
 	if num_sat > 0:
 		logger.warning(f'{num_sat/(data["h"]*data["w"]):.3f}% of pixels (n={num_sat}) are ' \
 					   'saturated in the shortest exposure. The values for these pixels will ' \
-					   'be inaccurate.')
+					   'be inaccurate. If there color artifacts in the final HDR image, ' \
+					   'consider setting the option \'clip_highlights\'=True')
 
-	if wb == 'camera':
+	if isinstance(wb, str) and wb == 'camera':
 		wb = data['white_balance'][:3]
 	if wb is not None:
 		assert len(wb) == 3, 'Provide list [R G B] corresponding to white patch in the image'
 		HDR = HDR * np.array(wb)[None,None,:]
 	if HDR.min() < 0:
 		logger.info('Clipping negative pixels.')
-		HDR[HDR < 0] = 0
+		HDR = HDR.clip(min=0)
 
 	if normalize:
 		HDR = HDR / HDR.max()
-	return HDR.astype(np.float32)
+	shortest_exposure = np.argmin(data['exp'] * data['gain'] * data['aperture'])
+	unsaturated = get_unsaturated(io.imread(files[shortest_exposure], libraw=False), data['saturation_point'])
+	if clip_highlights:
+		logger.info(f'Clipping all saturated highlights to {HDR.max()}')
+		HDR[np.logical_not(unsaturated)] = HDR.max()
+
+	if return_exif_exp:
+		return HDR.astype(np.float32), exif, data['exp']
+	else:
+		return HDR.astype(np.float32), unsaturated
 
 
 def imread_demosaic_merge(files, metadata, do_align, sat_percent):
 	"""
 	First postprocess using libraw and then merge RGB images. This function merges in an online
 	way and can handle a large number of inputs with little memory.
 	"""
@@ -125,19 +150,26 @@
 		num[unsaturated] += X_times_t[unsaturated]
 
 	HDR = num / denom
 
 	return HDR, num_sat
 
 
-def imread_merge_demosaic(files, metadata, do_align, pattern):
+def imread_merge_demosaic(files, metadata, do_align, pattern, demosaic):
 	"""
 	Merge RAW images before demosaicing. This function merges in an online
 	way and can handle a large number of inputs with little memory.
 	"""
+	import rawpy
+	import colour_demosaicing as cd
+
+	supported_demosaic = ('bilinear', 'malvar', 'menon')
+	assert demosaic in supported_demosaic, f'Unknown demosaicing method {demosaic}. ' \
+		'Pick one of {supported_demosaic}. For more information, please see ' \
+		'https://colour-demosaicing.readthedocs.io/en/latest/colour_demosaicing.bayer.html'
 	if do_align:
 		ref_idx = np.argsort(metadata['exp'] * metadata['gain']
 							 * metadata['aperture'])[len(files)//2]
 		ref_img = io.imread(files[ref_idx]).astype(np.float32)
 		if metadata['raw_format']:
 			ref_img = cd.demosaicing_CFA_Bayer_bilinear(ref_img, pattern=pattern)
 		ref_img = ref_img / metadata['exp'][ref_idx] \
@@ -207,15 +239,23 @@
 		denom[unsaturated] += metadata['exp'][i]
 		num[unsaturated] += X_times_t[unsaturated]
 		
 	HDR_bayer = num / denom
 
 	# Libraw does not support 32-bit values. Use colour-demosaicing instead:
 	# https://colour-demosaicing.readthedocs.io/en/latest/manual.html
-	logger.info('Running bilinear demosaicing')
-	HDR = cd.demosaicing_CFA_Bayer_bilinear(HDR_bayer, pattern=pattern)
+	if demosaic == 'bilinear':
+		logger.info('Running bilinear demosaicing')
+		HDR = cd.demosaicing_CFA_Bayer_bilinear(HDR_bayer, pattern=pattern)
+	elif demosaic == 'malvar':
+		logger.info('Running Malvar (2004) demosaicing')
+		HDR = cd.demosaicing_CFA_Bayer_Malvar2004(HDR_bayer, pattern=pattern)
+	elif demosaic == 'menon':
+		logger.info('Running DDFPAD by Menon (2007)')
+		HDR = cd.demosaicing_CFA_Bayer_Menon2007(HDR_bayer, pattern=pattern)
 
 	# Convert to output color-space
 	logger.info(f'Using color matrix: {color_mat}')
 	HDR = HDR @ color_mat
+	HDR = metadata['libraw_scale'](HDR)
 
 	return HDR, num_sat
```

### Comparing `HDRutils-0.9/HDRutils/noise_modeling/darktable.json` & `HDRutils-1.0/HDRutils/noise_modeling/darktable.json`

 * *Files identical despite different names*

### Comparing `HDRutils-0.9/HDRutils/noise_modeling/simulate.py` & `HDRutils-1.0/HDRutils/noise_modeling/simulate.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,24 +120,24 @@
 			eps = np.abs(var).min()
 			logger.warning('Predicted variance is non-positive for some pixels. These will be clipped.')
 			var = np.maximum(var, eps)
 		logger.info(f'Variance statistics: {var.min()}, {var.mean()}, {var.max()}')
 		return var
 
 
-	def simulate(self, phi, exp, iso=None, make=None, model=None, disable_static_noise=False, bits=8, black_level=0):
-		assert bits <= 16
+	def simulate(self, phi, exp, iso=None, make=None, model=None, disable_static_noise=False, black_level=0):
 		t = float(exp)
 
 		img = phi * t * self.g
 		var = self.var(img, make, model, iso, disable_static_noise)
 		noise = np.random.normal(scale=np.sqrt(var))
 
-		dtype = np.uint8 if bits <= 8 else np.uint16
-		max_value = 2**bits - 1
+		dtype = np.uint8 if self.bits <= 8 else np.uint16
+		logger.info(f'Quantizing to type {dtype} since bit-depth is {self.bits}')
+		max_value = 2**self.bits - 1
 		quantized = ((img + noise + black_level/max_value).clip(0, 1)*max_value).astype(dtype)
 		return quantized
 
 
 	def set_bayer(self, size):
 		# Assume RGGB
 		assert len(size) == 2
```

### Comparing `HDRutils-0.9/HDRutils.egg-info/PKG-INFO` & `HDRutils-1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,46 @@
-Metadata-Version: 2.1
-Name: HDRutils
-Version: 0.9
-Summary: Utility functions for performing basic operations on HDR images, including merging and deghosting
-Home-page: https://github.com/gfxdisp/HDRutils
-Author: Param Hanji
-Author-email: param.hanji@gmail.com
-License: MIT
-Download-URL: https://github.com/gfxdisp/HDRutils/archive/v0.9.tar.gz
-Keywords: HDR,Merging,Deghosting,simulation
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # HDRutils
 
-Some utility functions to generate HDR images from a sequence of exposure time or gain modulated images. You can find a separate Readme describing some functinos for noise simulations [here](HDRutils/noise_modeling).
+Some utility functions to generate HDR images from a sequence of exposure time or gain modulated images. You can find a separate README describing some functinos for realistic noise simulations [here](HDRutils/noise_modeling).
+
+**Table of contents**
+- [Installation](#installation)
+    - [Additional dependencies](#additional-dependencies)
+- [HDR image I/O](#reading-and-writing)
+- [Capture](#multi-exposure-capture)
+- [HDR merge](#merge-input-images)
+    - [Demosaicing](#merge-and-demosaic-or-demosaic-and-merge)
+    - [RAW bayer input](#merge-raw-bayer-frames-from-non-raw-formats)
+    - [Alignment](#alignment)
+    - [Exposure estimation](#exposure-estimation)
+- [Noise simulation](#noise-simulation)
+- [Citation](#citation)
 
 ## Installation
 To download HDRUtils, use Pypi via pip:
 
     pip install HDRutils
 
 If you prefer cloning this repository, install the dependencies using pip:
     
     pip clone https://github.com/gfxdisp/HDRutils.git
     cd HDRutils
     pip install -e .
 
-### Additional dependency
-You will need the [FreeImage plugin](https://imageio.readthedocs.io/en/stable/format_exr-fi.html) for reading and writing OpenEXR images:
+### Additional dependencies
+You will need the [FreeImage plugin](https://imageio.readthedocs.io/en/stable/_autosummary/imageio.plugins.freeimage.html) for reading and writing OpenEXR images:
 
     imageio_download_bin freeimage
 
-## Usage
-Just import HDRutils and call the required functions
+If you wish to capture HDR stacks using a DSLR, you will need gphoto2:
+
+    sudo apt install gphoto2
+
 
-### Reading and writing
+## Reading and writing
 Simple wrapper functions for [imageio's](https://imageio.github.io/) `imread` and `imwrite` are provided to set appropriate flags for HDR data. You can even call `imread` on RAW file formats:
 
 ```python
 import HDRutils
 
 raw_file = 'example_raw.arw'
 img_RGB = HDRutils.imread(raw_file)
@@ -56,52 +48,83 @@
 hdr_file = 'example.exr'
 img = HDRutils.imread(raw_file)
 
 HDRutils.imwrite('rgb.png', img_RGB)
 HDRutils.imwrite('output_filename.exr', img)
 ```
 
-### Merge input images
-The [rawpy](https://github.com/letmaik/rawpy) wrapper is used to read RAW images. [Noise-aware merging](https://www.cl.cam.ac.uk/research/rainbow/projects/noise_aware_merging/) is performed using the Poisson-noise optimal estimator. The generated HDR image is linearly related to the scene radiance
+## Multi-exposure capture
+Make sure gphoto2 is installed. Additionally, set camera to **manual mode** and **disable autofocus** on the lens. Then, decide valid exposure times (by scrolling on the camera) and run:
+
+```python
+from HDRutils.capture import DSLR
+camera = DSLR(ext='.arw')
+exposures = ['10', '1', '1/10', '1/100']
+camera.capture_HDR_stack('image', exposures)
+```
+
+## Merge input images
+The [rawpy](https://github.com/letmaik/rawpy) wrapper is used to read RAW images. [Noise-aware merging](https://www.cl.cam.ac.uk/research/rainbow/projects/noise-aware-merging/) is performed using the Poisson-noise optimal estimator. The generated HDR image is linearly related to the scene radiance
 
 ```python
-files = ['file1.dng', 'file2.dng', 'file3.dng']		# RAW input files
-HDR_img = HDRutils.merge(files)
+files = ['`image_0.arw`', '`image_1.arw`', '`image_2.arw`']		# RAW input files
+HDR_img = HDRutils.merge(files)[0]
 HDRutils.imwrite('merged.exr', HDR_img)
 ```
 
-The default function processes each image individually using [libraw](https://www.libraw.org/) and then merges the RGB images. This behaviour can be overriden to merge RAW bayer image by setting the flag `demosaic_first=False`.
+Sometimes the shortest exposure may contain saturated pixels. These cause artifacts when manual white-balance/color calibration is performed. Thus, `HDRutils.merge()` returns an unsaturated mask in addition to the merged image. The saturated pixels can be clipped after manual white-balance/color calibration.
+
+### Merge and demosaic or demosaic and merge?
+The default function processes each image individually using [libraw](https://www.libraw.org/) and then merges the RGB images. This result relies on the robust camera pipeline (including black-level subtraction, demosaicing, white-balance) provided by libraw, and should be suitable for most projects.
+
+If you need finer control over the exact radiance values, this behaviour can be overriden to merge RAW bayer images by setting the flag `demosaic_first=False`. This mode is useful when the camera is custom-calibrated and you have an exact correspondance between camera pixels with the scene luminance and/or color. Moreover, saturated pixels can be precisely identified before demosaicing. In this mode, a basic camera pipeline is reproduced with the following steps:
+
+Subtract black level -> Merge image stack -> Color transformation -> White-balance
+
+Demosaicing algorithms that are currently supported can be found at [this page](https://colour-demosaicing.readthedocs.io/en/latest/colour_demosaicing.bayer.html). Change the algorithm using `HDRutils.merge(..., demosaic_first=False, demosaic=*algorithm*)`
+
 
 ### Merge RAW bayer frames from non-RAW formats
 If your camera provides RAW frames in a non-standard format, you can still merge them in the camera color-space without libraw processing
 
 ```python
 files = ['file1.png', 'file2.png', 'file3.png']     # PNG bayer input files
-HDR_img = HDRutils.merge(files, demosaic_first=False, color_space='raw')
+HDR_img = HDRutils.merge(files, demosaic_first=False, color_space='raw')[0]
 HDRutils.imwrite('merged.exr', HDR_img)
 ```
 
 ### Alignment
-While merging, some ghosting artifacts an be removed by setting `HDRutils.merge(..., align=True)`. This attempts homography alignment and corrects camera motion for still scenes.
+While merging, some ghosting artifacts can be removed by setting `HDRutils.merge(..., align=True)`. This attempts homography alignment and corrects camera motion for still scenes. Unfortunately non-rigid motion requiring dense optical flow is not yet implemented.
 
-### Estimate exposure times
-The exposure times reported in EXIF camera metadata may be inaccurate. The merge function solves a linear least squares problem to estimate most suitable exposure times. This setting can be disabled by `HDRutils.merge(..., estimate_exp=False)`. The default behaviour is to use the brightest 10% of the pixels for estimation.
 
 ### Exposure estimation
-Exposure metadata from EXIF may be inaccurate. The default behaviour is to estimate relative exposures directly from the image stack. If you are confident that metadata is correct, disable exposure estimation by specifying `HDRutils.merge(..., estimate_exp=None)`.
+Exposure metadata from EXIF may be inaccurate and it may be benificial to estimate relative exposures directly from the image stack. Please see [our paper](https://www.cl.cam.ac.uk/research/rainbow/projects/exposure-estimation/) for details.
+
+This feauture is currently disabled, and EXIF values are used by default. To enable exposure estimation, run `HDRutils.merge(..., estimate_exp='mst')`.
 
-For robustness, the estimation includes an iterative outlier removal procedure which may take a couple of minutes to converge especially for large images and deep stacks. You can override this by `HDRutils.merge(..., outlier=None)`. For best results, supply the exact camera (instance of `HDRutils.NormalNoise`). Otherwise a default camera that works reasonably well for tested images will be used.
+## Noise simulation
+Generating realistic camera noise using calibrated parameters of real-world cameras is described [here](HDRutils/noise_modeling/).
 
 ## Citation
-If you find this package useful, please cite
+If you find this package useful, we would be grateful if you cite
 
     @inproceedings{hanji2020noise,
         author    = {Hanji, Param and Zhong, Fangcheng and Mantiuk, Rafa{\l} K.},
         title     = {Noise-Aware Merging of High Dynamic Range Image Stacks without Camera Calibration},
         booktitle = {Advances in Image Manipulation (ECCV workshop)},
         year      = {2020},
         publisher = {Springer},
         pages     = {376--391},
         url       = {http://www.cl.cam.ac.uk/research/rainbow/projects/noise-aware-merging/},
     }
 
-
+    @ARTICLE{hanji2023exposures,
+        author    = {Hanji, Param and and Mantiuk, Rafa{\l} K.},
+        journal   = {IEEE Transactions on Computational Imaging}, 
+        title     = {Efficient Approximation of Jacobian Matrices Involving a Non-Uniform Fast Fourier Transform (NUFFT)}, 
+        year      = {2023},
+        volume    = {},
+        number    = {},
+        pages     = {},
+        doi       = {},
+        url       = {https://www.cl.cam.ac.uk/research/rainbow/projects/exposure-estimation/},
+    }
```

### Comparing `HDRutils-0.9/LICENSE` & `HDRutils-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `HDRutils-0.9/setup.py` & `HDRutils-1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 # Based on the following article:
 # https://medium.com/@joel.barmettler/how-to-upload-your-python-package-to-pypi-65edc5fe9c56
 
 from setuptools import setup, find_packages
+
+with open("README.md", "r", encoding="utf8") as fh:
+    long_description = fh.read()
+
 setup(
   name = 'HDRutils',
   packages = find_packages(),
+  package_data = {'HDRutils': ['noise_modeling/darktable.json']},
   include_package_data=True,
-  version = '0.9',
+  version = '1.0',
   license='MIT',
   description = 'Utility functions for performing basic operations on HDR images, including ' \
                 'merging and deghosting',
   author = 'Param Hanji',
   author_email = 'param.hanji@gmail.com',
   url = 'https://github.com/gfxdisp/HDRutils',
-  download_url = 'https://github.com/gfxdisp/HDRutils/archive/v0.9.tar.gz',
+  long_description=long_description,
+  long_description_content_type='text/markdown',
   keywords = ['HDR', 'Merging', 'Deghosting', 'simulation'],
   install_requires=[
           'numpy',
-          'imageio',
+          'imageio>=2.21.2',
           'rawpy',
           'exifread',
           'tqdm',
           'colour-demosaicing',
           'matplotlib',
-          'opencv_python',
-          'scipy',
-          'scikit-image'
-      ],
+          'scipy>=1.7.1',
+          'scikit-image>=0.18.3',
+          'pyexr'],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
-    'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
-    'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-  ],
+    'Programming Language :: Python :: 3.9'],
 )
```

