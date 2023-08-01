# Comparing `tmp/lost_cat_images-0.0.1.tar.gz` & `tmp/lost_cat_images-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lost_cat_images-0.0.1.tar", last modified: Tue Jan 24 16:26:16 2023, max compression
+gzip compressed data, was "lost_cat_images-1.0.0.tar", last modified: Tue Aug  1 19:20:34 2023, max compression
```

## Comparing `lost_cat_images-0.0.1.tar` & `lost_cat_images-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-01-24 16:26:16.807753 lost_cat_images-0.0.1/
--rw-rw-rw-   0        0        0     1101 2022-11-04 21:36:19.000000 lost_cat_images-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2484 2023-01-24 16:26:16.804749 lost_cat_images-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      534 2023-01-17 20:23:47.000000 lost_cat_images-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-24 16:26:16.715221 lost_cat_images-0.0.1/lost_cat_images/
--rw-rw-rw-   0        0        0        0 2023-01-14 15:56:39.000000 lost_cat_images-0.0.1/lost_cat_images/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:26:16.739222 lost_cat_images-0.0.1/lost_cat_images/examples/
--rw-rw-rw-   0        0        0     5478 2023-01-24 16:14:25.000000 lost_cat_images-0.0.1/lost_cat_images/examples/run_engimg.py
--rw-rw-rw-   0        0        0     6274 2023-01-24 16:14:25.000000 lost_cat_images-0.0.1/lost_cat_images/examples/test_rules.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:26:16.754220 lost_cat_images-0.0.1/lost_cat_images/parsers/
--rw-rw-rw-   0        0        0        0 2023-01-14 15:56:39.000000 lost_cat_images-0.0.1/lost_cat_images/parsers/__init__.py
--rw-rw-rw-   0        0        0     5655 2023-01-22 20:18:45.000000 lost_cat_images-0.0.1/lost_cat_images/parsers/engimg_parser.py
--rw-rw-rw-   0        0        0     3156 2023-01-17 22:39:33.000000 lost_cat_images-0.0.1/lost_cat_images/parsers/image_parser.py
--rw-rw-rw-   0        0        0     4725 2023-01-16 18:29:44.000000 lost_cat_images-0.0.1/lost_cat_images/parsers/pdf_parser.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:26:16.761221 lost_cat_images-0.0.1/lost_cat_images/processors/
--rw-rw-rw-   0        0        0        0 2023-01-14 15:56:39.000000 lost_cat_images-0.0.1/lost_cat_images/processors/__init__.py
--rw-rw-rw-   0        0        0     6688 2023-01-14 15:56:39.000000 lost_cat_images-0.0.1/lost_cat_images/processors/image_processor.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:26:16.783228 lost_cat_images-0.0.1/lost_cat_images/utils/
--rw-rw-rw-   0        0        0        0 2023-01-14 15:56:39.000000 lost_cat_images-0.0.1/lost_cat_images/utils/__init__.py
--rw-rw-rw-   0        0        0     1787 2023-01-14 15:56:39.000000 lost_cat_images-0.0.1/lost_cat_images/utils/utils_image.py
--rw-rw-rw-   0        0        0    33710 2023-01-24 16:16:37.000000 lost_cat_images-0.0.1/lost_cat_images/utils/utils_ocr.py
--rw-rw-rw-   0        0        0     5005 2023-01-14 16:55:14.000000 lost_cat_images-0.0.1/lost_cat_images/utils/utils_pdf.py
--rw-rw-rw-   0        0        0     9885 2023-01-22 17:20:11.000000 lost_cat_images-0.0.1/lost_cat_images/utils/utils_shapes.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:26:16.732224 lost_cat_images-0.0.1/lost_cat_images.egg-info/
--rw-rw-rw-   0        0        0     2484 2023-01-24 16:26:16.000000 lost_cat_images-0.0.1/lost_cat_images.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      805 2023-01-24 16:26:16.000000 lost_cat_images-0.0.1/lost_cat_images.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-24 16:26:16.000000 lost_cat_images-0.0.1/lost_cat_images.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-01-24 16:26:16.000000 lost_cat_images-0.0.1/lost_cat_images.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-01-24 16:26:16.000000 lost_cat_images-0.0.1/lost_cat_images.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1038 2023-01-24 16:14:25.000000 lost_cat_images-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-24 16:26:16.807753 lost_cat_images-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-24 16:26:16.799749 lost_cat_images-0.0.1/test/
--rw-rw-rw-   0        0        0     2434 2023-01-16 23:00:38.000000 lost_cat_images-0.0.1/test/test_ocr.py
--rw-rw-rw-   0        0        0     2784 2023-01-14 15:56:39.000000 lost_cat_images-0.0.1/test/test_pdf.py
--rw-rw-rw-   0        0        0     2492 2023-01-18 23:20:08.000000 lost_cat_images-0.0.1/test/test_shapes.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:20:34.046105 lost_cat_images-1.0.0/
+-rw-rw-rw-   0        0        0     1101 2023-01-18 17:26:24.000000 lost_cat_images-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3388 2023-08-01 19:20:34.042090 lost_cat_images-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1438 2023-06-21 17:46:37.000000 lost_cat_images-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 19:20:33.762083 lost_cat_images-1.0.0/lost_cat_images/
+-rw-rw-rw-   0        0        0        0 2023-01-11 17:43:13.000000 lost_cat_images-1.0.0/lost_cat_images/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:20:33.807211 lost_cat_images-1.0.0/lost_cat_images/examples/
+-rw-rw-rw-   0        0        0     2648 2023-05-18 18:49:50.000000 lost_cat_images-1.0.0/lost_cat_images/examples/init_lostcat.py
+-rw-rw-rw-   0        0        0    12669 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/lost_cat_images/examples/run_engimg.py
+-rw-rw-rw-   0        0        0    24666 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/lost_cat_images/examples/run_v2.py
+-rw-rw-rw-   0        0        0    11162 2023-05-18 18:49:50.000000 lost_cat_images-1.0.0/lost_cat_images/examples/save_rules.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:20:33.822596 lost_cat_images-1.0.0/lost_cat_images/parsers/
+-rw-rw-rw-   0        0        0        0 2023-01-11 17:43:13.000000 lost_cat_images-1.0.0/lost_cat_images/parsers/__init__.py
+-rw-rw-rw-   0        0        0     6082 2023-01-25 16:08:59.000000 lost_cat_images-1.0.0/lost_cat_images/parsers/engimg_parser.py
+-rw-rw-rw-   0        0        0     3156 2023-01-20 17:28:13.000000 lost_cat_images-1.0.0/lost_cat_images/parsers/image_parser.py
+-rw-rw-rw-   0        0        0     4725 2023-01-18 17:26:24.000000 lost_cat_images-1.0.0/lost_cat_images/parsers/pdf_parser.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:20:33.830633 lost_cat_images-1.0.0/lost_cat_images/processors/
+-rw-rw-rw-   0        0        0        0 2023-01-11 17:43:13.000000 lost_cat_images-1.0.0/lost_cat_images/processors/__init__.py
+-rw-rw-rw-   0        0        0     6688 2023-01-13 18:33:50.000000 lost_cat_images-1.0.0/lost_cat_images/processors/image_processor.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:20:33.940370 lost_cat_images-1.0.0/lost_cat_images/utils/
+-rw-rw-rw-   0        0        0     2120 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/lost_cat_images/utils/__init__.py
+-rw-rw-rw-   0        0        0     8676 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/lost_cat_images/utils/clean.py
+-rw-rw-rw-   0        0        0    21091 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/lost_cat_images/utils/extract.py
+-rw-rw-rw-   0        0        0     5030 2023-06-19 16:35:47.000000 lost_cat_images-1.0.0/lost_cat_images/utils/image_templates.py
+-rw-rw-rw-   0        0        0     4752 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/lost_cat_images/utils/tools.py
+-rw-rw-rw-   0        0        0    25848 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/lost_cat_images/utils/utils_boxes.py
+-rw-rw-rw-   0        0        0    23352 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/lost_cat_images/utils/utils_graphics.py
+-rw-rw-rw-   0        0        0    28218 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/lost_cat_images/utils/utils_grids.py
+-rw-rw-rw-   0        0        0     1787 2023-01-13 21:33:26.000000 lost_cat_images-1.0.0/lost_cat_images/utils/utils_image.py
+-rw-rw-rw-   0        0        0     3927 2023-06-19 16:35:47.000000 lost_cat_images-1.0.0/lost_cat_images/utils/utils_nodepaths.py
+-rw-rw-rw-   0        0        0    39921 2023-06-19 16:35:47.000000 lost_cat_images-1.0.0/lost_cat_images/utils/utils_ocr.py
+-rw-rw-rw-   0        0        0    13460 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/lost_cat_images/utils/utils_ocr_engines.py
+-rw-rw-rw-   0        0        0     5005 2023-04-28 21:18:48.000000 lost_cat_images-1.0.0/lost_cat_images/utils/utils_pdf.py
+-rw-rw-rw-   0        0        0     7290 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/lost_cat_images/utils/utils_rules.py
+-rw-rw-rw-   0        0        0    11627 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/lost_cat_images/utils/utils_shapes.py
+-rw-rw-rw-   0        0        0     2068 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/lost_cat_images/utils/utils_text.py
+-rw-rw-rw-   0        0        0     4122 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/lost_cat_images/utils/utils_words.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:20:33.788342 lost_cat_images-1.0.0/lost_cat_images.egg-info/
+-rw-rw-rw-   0        0        0     3388 2023-08-01 19:20:33.000000 lost_cat_images-1.0.0/lost_cat_images.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1539 2023-08-01 19:20:33.000000 lost_cat_images-1.0.0/lost_cat_images.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 19:20:33.000000 lost_cat_images-1.0.0/lost_cat_images.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2023-08-01 19:20:33.000000 lost_cat_images-1.0.0/lost_cat_images.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-01 19:20:33.000000 lost_cat_images-1.0.0/lost_cat_images.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1136 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 19:20:34.046105 lost_cat_images-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 19:20:34.038478 lost_cat_images-1.0.0/test/
+-rw-rw-rw-   0        0        0     4830 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/test/test_clean.py
+-rw-rw-rw-   0        0        0     3027 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/test/test_extract.py
+-rw-rw-rw-   0        0        0     9317 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/test/test_grids.py
+-rw-rw-rw-   0        0        0     1612 2023-06-19 16:35:47.000000 lost_cat_images-1.0.0/test/test_image_templates.py
+-rw-rw-rw-   0        0        0     2423 2023-06-19 16:35:47.000000 lost_cat_images-1.0.0/test/test_ocr.py
+-rw-rw-rw-   0        0        0     2784 2023-01-13 22:09:57.000000 lost_cat_images-1.0.0/test/test_pdf.py
+-rw-rw-rw-   0        0        0     2602 2023-05-24 21:31:36.000000 lost_cat_images-1.0.0/test/test_shapes.py
+-rw-rw-rw-   0        0        0     1012 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/test/test_tools.py
+-rw-rw-rw-   0        0        0     1584 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/test/test_util_graphics.py
+-rw-rw-rw-   0        0        0     2935 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/test/test_util_ocr_engines.py
+-rw-rw-rw-   0        0        0     3606 2023-08-01 19:16:13.000000 lost_cat_images-1.0.0/test/test_utils_boxes.py
+-rw-rw-rw-   0        0        0     2435 2023-06-19 16:35:47.000000 lost_cat_images-1.0.0/test/test_utils_paths.py
```

### Comparing `lost_cat_images-0.0.1/LICENSE` & `lost_cat_images-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lost_cat_images-0.0.1/lost_cat_images/parsers/engimg_parser.py` & `lost_cat_images-1.0.0/lost_cat_images/parsers/engimg_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,14 +115,27 @@
                     "thresh": 75,
                     "maxval": 255,
                     "type": cv2.THRESH_BINARY | cv2.THRESH_OTSU,
                 },
                 "contours": {
                     "mode": cv2.RETR_TREE,
                     "method": cv2.CHAIN_APPROX_TC89_L1
+                },
+                "extract": {
+                    "ratio": 3,
+                    "bleed": 4,
+                    "mindim": 1000,
+                    "useblur": False,
+                    "kernel": 3,
+                    "shape": "",
+                    "dilate": 1,
+                    "erode": 3,
+                    "tesseract": {
+                        "i2d": "--psm 1"
+                    },
                 }
             }
         }
 
     def close(self, force: bool = False, block: bool = False, timeout: int = -1):
         """will close the """
         if self._file:
@@ -154,8 +167,7 @@
         for iidx, pil_img in enumerate(self.images):
             # convert and process each image
             img = np.array(pil_img)
             logger.info("IMG: [%s] => %s", iidx, img.shape)
             _data[iidx] = extract_artifacts(image= img, config=self._config.get("parser"))
 
         return _data
-
```

### Comparing `lost_cat_images-0.0.1/lost_cat_images/parsers/image_parser.py` & `lost_cat_images-1.0.0/lost_cat_images/parsers/image_parser.py`

 * *Files identical despite different names*

### Comparing `lost_cat_images-0.0.1/lost_cat_images/parsers/pdf_parser.py` & `lost_cat_images-1.0.0/lost_cat_images/parsers/pdf_parser.py`

 * *Files identical despite different names*

### Comparing `lost_cat_images-0.0.1/lost_cat_images/processors/image_processor.py` & `lost_cat_images-1.0.0/lost_cat_images/processors/image_processor.py`

 * *Files identical despite different names*

### Comparing `lost_cat_images-0.0.1/lost_cat_images/utils/utils_image.py` & `lost_cat_images-1.0.0/lost_cat_images/utils/utils_image.py`

 * *Files identical despite different names*

### Comparing `lost_cat_images-0.0.1/lost_cat_images/utils/utils_ocr.py` & `lost_cat_images-1.0.0/lost_cat_images/utils/utils_ocr.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 import cv2
 import math
 import numpy as np
 import pytesseract
 import statistics
 
 from collections import namedtuple
-from lost_cat_images.utils.utils_shapes import Rectangle, intersect, merge, ShapeGrouper, printTree
+from lost_cat_images.utils.utils_shapes import Rectangle, rectangle_intersect, rectangle_merge, ShapeGrouper, printTree
 
 logger = logging.getLogger(__name__)
 
 Contour = namedtuple("Contour", ["x", "y", "w", "h", "p", "c", "a"])
 
 def extactImageContours(img: np.array, markup:np.ndarray=None, config: dict = None,
-        minheight: int = 30, minwidth: int = 30,
-        grid: int = -1, bleed: int = 4,
+        minheight: int = 25, minwidth: int = 25,
+        grid: int = 1, bleed: int = 2, min = 15,
         max_r: int = 120, fidx: int = None, save_steps: bool = False
     ) -> dict:
     """
     """
     if markup is not None:
         img_return = markup.copy()
     else:
@@ -39,36 +39,62 @@
     if grid == -1:
         iw = img.shape[1]
         grid = minwidth // 2
 
     # process the image...
     contours, _ = cv2.findContours(image=img, **config)
     cv2.drawContours(image=img_return, contours=contours, contourIdx=-1, color=(255, 0, 0), thickness=1)
-
+    review = {
+        "contours": len(contours)
+    }
     # now to extract rectangles from the image...
     font = cv2.FONT_HERSHEY_SIMPLEX
     found = []
     idx = -1
     cidx = 0
     bidx = 0
-    yc = 6629
-    xc = 8074 # 6629, 6753, 8074, 8154
     borders = []
+    modws = []
+    modhs = []
+
+    hlines = []
+    vlines = []
+    count_cut = 0
 
-    for c in contours: #.sort(key=lambda r: [int(minheight * round(float(r[1]) / minheight)), int(minwidth * round(float(r[0]) / minwidth))]):
+    shpgrp = ShapeGrouper()
+
+    for cidx, c in enumerate(contours): #.sort(key=lambda r: [int(minheight * round(float(r[1]) / minheight)), int(minwidth * round(float(r[0]) / minwidth))]):
         peri = cv2.arcLength(c, True)
-        approx = cv2.approxPolyDP(c, 0.04 * peri, True)
+        approx = cv2.approxPolyDP(c, 0.04 * peri, True)  # assume closed curve
 
         # look for any contours that contain the selected pixel
         (bbx,bby,bbw,bbh) = cv2.boundingRect(c)
-        (ibx,iby,ibw,ibh) = cv2.boundingRect(c)
 
-        if minwidth >= bbw or minheight >= bbh:
+        # cut out the small pixels
+        if bbw < min and bbh < min:
+            logger.debug("EIC: {%s:<%s>} EXCLUDE: SML BBW:%s BBH:%s", fidx, idx, bbw, bbh)
+            count_cut += 1
             continue
 
+        # get the approx points
+        #if len(approx) != 4:
+        #    logger.debug("EIC: {%s:<%s>} EXCLUDE Approx: L:%s A:%s", fidx, idx, len(approx), approx)
+        #    continue
+
+        # gather data for stats
+        modhs.append(bbh)
+        modws.append(bbw)
+        hlines.append(int(((2* bby) + bbh)/2 ))
+        vlines.append(int(((2* bbx) + bbw)/2 ))
+
+        # exlucde the check for small boxes
+        #if minwidth >= bbw or minheight >= bbh:
+        #    logger.debug("EIC: {%s:<%s>} EXCLUDE: BBW:%s BBH:%s", fidx, idx, bbw, bbh)
+        #    continue
+
         # detect border % black to white pixels...
         bbxt, bbyt, bbxb, bbyb = bbx-bleed, bby-bleed, bbx+bbw+bleed, bby+bbh+bleed
 
         crop = img[bby:bby+bbh, bbx:bbx+bbw]
         pixels1 = img[bbyt:bbyb, bbxt:bbxt+bleed]
         pixels2 = img[bbyt:bbyb, bbxb-bleed:bbxb]
         pixels3 = img[bbyt:bbyt+bleed, bbxt:bbxb]
@@ -80,65 +106,132 @@
 
         contents_ratio = crop.sum() / crop.size if crop.size > 0 else 0
 
         idx += 1
         #if save_steps:
         #    cv2.imwrite(f'data/eng/crops/F{fidx}.{idx}.IC.png', crop)
 
-        logger.debug("Crop: %s", idx)
-        logger.debug("Counts: C: %s => P1: %s P2: %s P3: %s P4: %s", crop.size, pixels1.size, pixels2.size, pixels3.size, pixels4.size)
-        logger.debug("Sums:   C: %s => P1: %s P2: %s P3: %s P4: %s", crop.sum(), pixels1.sum(), pixels2.sum(), pixels3.sum(), pixels4.sum())
-        logger.debug("Ratios:\t%s\t%s\t%s\t%s\t%s\t%s\t%s\t%s\t%s", fidx, idx, border_ratio / contents_ratio, border_ratio, contents_ratio, bbx, bby, bbw, bbh)
+        logger.debug("EIC: {%s:<%s>} Crop", fidx, idx)
+        logger.debug("EIC: {%s:<%s>} Counts: C: %s => P1: %s P2: %s P3: %s P4: %s", fidx, idx, crop.size, pixels1.size, pixels2.size, pixels3.size, pixels4.size)
+        logger.debug("EIC: {%s:<%s>} Sums:   C: %s => P1: %s P2: %s P3: %s P4: %s", fidx, idx, crop.sum(), pixels1.sum(), pixels2.sum(), pixels3.sum(), pixels4.sum())
+        #logger.debug("EIC: {%s:<%s>} Ratios:\t%s\t%s\t%s\t%s\t%s\t%s\t%s\t%s\t%s", fidx, idx, border_ratio / contents_ratio, border_ratio, contents_ratio, bbx, bby, bbw, bbh)
 
         if border_ratio < max_r:
+            rect = Rectangle(x=bbx, y=bby, w=bbw, h=bbh)
+            rect.add_tags(contour=c, fidx=fidx, approx=approx)
+            shpgrp.add_rectangle(rect=rect)
+
             cv2.rectangle(img_return, (bbx, bby), (bbx + bbw, bby + bbh), (0, 0, 255), 1)
             cv2.putText(img=img_return, text=str(bidx),
                 org=(bbx+10, bby+10), fontFace=font, fontScale=0.5, color=(0, 255, 0),
                 thickness=1)
 
             borders.append(c)
             # use bleed
             found.append((bbxt, bbyt, bbw+(2*bleed), bbh+(2*bleed)))
             # no bleed
             #found.append((bbxt, bbyt, bbw, bbh))
             logger.debug("Box: %s [%s] %s => %s", idx, bidx, (bby,bby+bbh,bbx,bbx+bbw), (bbxt, bbyt, bbw+(2*bleed), bbh+(2*bleed)))
             bidx += 1
 
+    # we need to get the modal bounding box h and w...
+    logger.info("EIC: {%s} CUT: %s TOTAL: %s", fidx, count_cut, len(contours))
+
+    review["cut"] = count_cut
+
+    maxh = max(modhs)
+    maxw = max(modws)
+    modh = statistics.mode(modhs)
+    modw = statistics.mode(modws)
+    logger.info("EIC: {%s} MOD: H %s W %s", fidx, modh, modw)
+
+    medh = statistics.median(modhs)
+    medw = statistics.median(modws)
+    logger.info("EIC: {%s} MED: H %s W %s", fidx, medh, medw)
+    logger.info("EIC: {%s} MAX: H %s W %s", fidx, maxh, maxw)
+
+    mmmodh = statistics.multimode(modhs)
+    mmmodw = statistics.multimode(modws)
+    logger.info("EIC: {%s} MMH: %s", fidx, mmmodh)
+    logger.info("EIC: {%s} MMW: %s", fidx, mmmodw)
+
+    mmhline = statistics.multimode(hlines)
+    mmvline = statistics.multimode(vlines)
+
+    logger.info("EIC: {%s} HLines: C %s L %s", fidx, len(hlines), set(hlines))
+    logger.info("EIC: {%s} Vlines: C %s L %s", fidx, len(vlines), set(vlines))
+    logger.info("EIC: {%s} MM HLines: C %s L %s", fidx, len(hlines), list(mmhline))
+    logger.info("EIC: {%s} MM Vlines: C %s L %s", fidx, len(vlines), list(mmvline))
+
     # now print these boxes if they are close to the borders in a table
     boxes = []
     vertices = set()
-    logger.debug("Found: %s", len(found))
+    logger.debug("EIC: {%s} Boxes: %s", fidx, len(found))
+
+    bbhlines = []
+    bbvlines = []
+    bbwidths = []
+    bbheights = []
 
     for (x,y,w,h) in found:
+        bbhlines.append(x)
+        bbvlines.append(y)
+        bbwidths.append(w)
+        bbheights.append(h)
+
         xtl, ytl = (x // grid) * grid, (y // grid) * grid
         xtr, ytr = ((x + w) // grid) * grid, (y // grid) * grid
         xbl, ybl = (x // grid) * grid, ((y + h) // grid) * grid
         xbr, ybr = ((x + w) // grid) * grid, ((y + h) // grid) * grid
-        logger.debug("Grid: [%s %s %s %s] => [%s %s %s %s]", x, y, w, h, xtl, ytl, xbr, ybr)
+
+        #logger.debug("Grid: [%s %s %s %s] => [%s %s %s %s]", x, y, w, h, xtl, ytl, xbr, ybr)
         vertices.add((xtl, ytl))
         vertices.add((xtr, ytr))
         vertices.add((xbl, ybl))
         vertices.add((xbr, ybr))
 
         boxes.append((x,y,w,h))
         cv2.rectangle(img_return, (x, y), (x + w, y + h), (255, 255, 0), 1)
-        #cv2.putText(img=img_return, text=('width = {}, height = {}'.format(w, h)),
-        #    org=(x+30, y+30), fontFace=font, fontScale=0.5, color=(255, 255, 0),
-        #    thickness=1)
 
-    # Hallsm!n!sCannonsAddr3ss
+    # Draw the verices
     logger.debug("Vertices: %s", len(vertices))
     for (x,y) in vertices:
         cv2.circle(img=img_return, center=(x, y), radius=(grid // 2), color=(255,0,255), thickness=1)
         cv2.circle(img=img_return, center=(x, y), radius=(grid), color=(255,0,255), thickness=2)
 
+    # log the stats
+    bbmmh = statistics.multimode(bbheights)
+    bbmmw = statistics.multimode(bbwidths)
+    logger.info("EIC: {%s} BB MMH: %s", fidx, bbmmh)
+    logger.info("EIC: {%s} BB MMW: %s", fidx, bbmmw)
+
+    logger.info("EIC: {%s} BB HLines: C %s L %s", fidx, len(bbhlines), set(bbhlines))
+    logger.info("EIC: {%s} BB Vlines: C %s L %s", fidx, len(bbvlines), set(bbvlines))
+
+    bbmmhline = statistics.multimode(bbhlines)
+    bbmmvline = statistics.multimode(bbvlines)
+    logger.info("EIC: {%s} BB MM HLines: C %s L %s", fidx, len(bbmmhline), list(bbmmhline))
+    logger.info("EIC: {%s} BB MM Vlines: C %s L %s", fidx, len(bbmmvline), list(bbmmvline))
+
     return {
         "image": img_return,
         "borders": borders,
-        "boxes": boxes
+        "boxes": boxes,
+        "review": review,
+        "shapes": shpgrp,
+        "alignments": {
+            "contours": {
+                "horizontal": hlines,
+                "vertical": vlines
+            },
+            "boxes": {
+                "horizontal": bbhlines,
+                "vertical": bbvlines
+            }
+        }
     }
 
 def box_connected(img:np.ndarray, markup:np.ndarray=None,
         boxes:list= None, contours:list = None,
         fidx:int = None, bleed:int = 3, save_steps:bool = False) -> list:
     """Will take the gioven boxes and selected the boxes of interest."""
     dims = img.shape
@@ -153,15 +246,15 @@
     trbox = Box(-1, 0, 0, 0, iy)
     brbox = Box(-1, 0, 0, 0, 0)
 
     # echeck for for heirachy and connected edges
     for idx, (tx,ty,bw,bh) in enumerate(boxes):
         bx = tx + bw
         by = ty + bh
-        logger.debug("Box: %s => %s", idx, (tx,ty,bw,bh))
+        logger.debug("BC: {%s:%s} Box: %s", fidx, idx, (tx,ty,bw,bh))
         label = f"{tx}:{ty}:{bw}:{bh}"
 
         if ((trbox.x + trbox.w) < (tx + bw) or
                 (trbox.y) > (ty)):
             trbox = Box(idx, tx,ty,bw,bh)
 
         if ((brbox.x + brbox.w) < (tx + bw) or
@@ -195,23 +288,23 @@
                 if conn_box[idx] is None:
                     conn_box[idx] = set()
                 conn_box[idx].add(jdx)
                 if conn_box[jdx] is None:
                     conn_box[jdx] = set()
                 conn_box[jdx].add(idx)
 
-                logger.debug("\t%s <=> %s: %s", idx, jdx, score)
+                logger.debug("BC: {%s:%s} <=> J: %s S: %s", fidx, idx, jdx, score)
 
     if logger.level == logging.DEBUG:
-        logger.info("Connected:")
+        logger.info("BC: {%s:--} Connected:", fidx)
         for idx, v in enumerate(conn_box):
-            logger.info("\t%s\t%s", idx, v)
+            logger.info("BC: {%s:%s} %s", fidx, idx, v)
 
-        logger.info("\tTR: %s", trbox)
-        logger.info("\tBR: %s", brbox)
+        logger.info("BC: {%s:--} TR: %s", fidx, trbox)
+        logger.info("BC: {%s:--} BR: %s", fidx, brbox)
 
     # start from BR Box
     selidx = set()
     selidx.add(trbox.idx)
     selidx.add(brbox.idx)
     q = list(selidx)
     while q and len(q) > 0:
@@ -224,20 +317,20 @@
                     q.append(idx)
 
     logger.debug("\tCB: %s", selidx)
 
     # return on the leaf boxes
     selected = []
     borders = []
-    logger.info("Selected:")
+    logger.info("BC: {%s:--} Selected:", fidx)
     for idx in selidx:
         if idx == -1:
             continue
 
-        logger.info("\t%s: %s", idx, boxes[idx])
+        logger.info("BC: {%s:--} %s: %s", fidx, idx, boxes[idx])
         selected.append(boxes[idx])
         borders.append(contours[idx])
 
     return {
         "boxes": selected,
         "borders": borders,
     }
@@ -279,26 +372,30 @@
     logger.info("SI: {%s:%s} SHP: %s CNTS: %s", fidx, idx, img.shape, len(contours))
     boxes = []
     selected = []
     found = []
     modws = []
     modhs = []
 
+    hlines = []
+    vlines = []
+
     # quick segementation, too small and to large :)
     for c in contours:
         # update the markup image
         (bbx,bby,bbw,bbh) = cv2.boundingRect(c)
+
         if (bbw == w) and (bbh == h):
             logger.debug("SI: {%s:%s} C: OUT %s", fidx, idx, (bbx,bby,bbw,bbh))
             continue
 
         # filter small contours...
-        #if (bbh <= closesize) and (bbw <= closesize):
-        #    logger.debug("SI: {%s:%s} C: SML %s", fidx, idx, (bbx,bby,bbw,bbh))
-        #    continue
+        if (bbh <= closesize) and (bbw <= closesize):
+            logger.debug("SI: {%s:%s} C: SML %s", fidx, idx, (bbx,bby,bbw,bbh))
+            continue
 
         if (bbh > (h * 0.9)) and (bbw > (w + 0.9)):
             logger.debug("SI: {%s:%s} C: LRG %s", fidx, idx, (bbx,bby,bbw,bbh))
             continue
 
         logger.debug("SI: {%s:%s} C: USE %s", fidx, idx, (bbx,bby,bbw,bbh))
         modhs.append(bbh)
@@ -322,14 +419,19 @@
     logger.info("SI: {%s:%s} MOD: H %s W %s", fidx, idx, modh, modw)
 
     medh = statistics.median(modhs)
     medw = statistics.median(modws)
     logger.info("SI: {%s:%s} MED: H %s W %s", fidx, idx, medh, medw)
     logger.info("SI: {%s:%s} MAX: H %s W %s", fidx, idx, maxh, maxw)
 
+    mmmodh = statistics.multimode(modhs)
+    mmmodw = statistics.multimode(modws)
+    logger.info("SI: {%s:%s} MMH: %s", fidx, idx, mmmodh)
+    logger.info("SI: {%s:%s} MMW: %s", fidx, idx, mmmodw)
+
     # process the found elements
     for cidx, (bbx,bby,bbw,bbh, c) in enumerate(found):
         peri = cv2.arcLength(c, True)
         approx = cv2.approxPolyDP(c, 0.04 * peri, True)
 
         # log and show the results
         logger.debug("SI: {%s:%s:%s} C: %s", fidx, idx, cidx, (bbx,bby,bbw,bbh))
@@ -339,31 +441,53 @@
         cv2.putText(img=img_blank, text=str(cidx),
             org=(bbx, bby), fontFace=font, fontScale=0.5, color=(255, 0, 0),
             thickness=1)
 
         # check the length of the contour...
         # remove large lines (2 points or less)
         # consider size, number of points in the approx
-        if bbh == maxh:
-            logger.info("SI: {%s:%s:%s} EXCLUDE %s", fidx, idx, cidx, (bbw, medw, bbh, medh))
-            cv2.drawContours(img_blank, [approx], -1, (0,255,0), 1)
+        #if bbh == maxh:
+        #    logger.info("SI: {%s:%s:%s} EXCLUDE %s", fidx, idx, cidx, (bbw, medw, bbh, medh))
+        #    cv2.drawContours(img_blank, [approx], -1, (0,255,0), 1)
+
+        #el
+        if (bbw < (medw * factor)) or (bbh < (medh * factor)):
+
+            hlines.append(int(((2* bby) + bbh)/2 ))
+            vlines.append(int(((2* bbx) + bbw)/2 ))
 
-        elif (bbw < (medw * factor)) or (bbh < (medh * factor)):
             logger.info("SI: {%s:%s:%s} INCLUDE %s", fidx, idx, cidx, (bbw, medw, bbh, medh))
             cv2.drawContours(img_blank, [approx], -1, (0,0,255), 1)
 
             # add the conotur to the mask...
             cv2.drawContours(img_mask, [c], -1, (255), -1)
             boxes.append((bbx, bby, bbw, bbh, approx))
             selected.append(approx)
         else:
             logger.info("SI: {%s:%s:%s} EXCLUDE %s", fidx, idx, cidx, (bbw, medw, bbh, medh))
             cv2.drawContours(img_blank, [approx], -1, (0,255,0), 1)
 
-    if save_steps:
+    # print the lines
+    mmhline = statistics.multimode(hlines)
+    mmvline = statistics.multimode(vlines)
+
+    logger.info("SI: {%s:%s} HLines: C %s L %s", fidx, idx, len(hlines), list(hlines))
+    logger.info("SI: {%s:%s} Vlines: C %s L %s", fidx, idx, len(vlines), list(vlines))
+    logger.info("SI: {%s:%s} MM HLines: C %s L %s", fidx, idx, len(hlines), list(mmhline))
+    logger.info("SI: {%s:%s} MM Vlines: C %s L %s", fidx, idx, len(vlines), list(mmvline))
+
+    if save_steps:
+        for hy in hlines:
+            cv2.line(img=img_blank, pt1=(0,hy), pt2=(10, hy), color=(128,128,255), thickness=1)
+        for vx in vlines:
+            cv2.line(img=img_blank, pt1=(vx,0), pt2=(vx, 10), color=(128,128,255), thickness=1)
+        for hy in mmhline:
+            cv2.line(img=img_blank, pt1=(0,hy), pt2=(10, hy), color=(75,0,255), thickness=1)
+        for vx in mmvline:
+            cv2.line(img=img_blank, pt1=(vx,0), pt2=(vx, 10), color=(75,0,255), thickness=1)
         cv2.imwrite(f'data/eng/crops/F{fidx}.{idx}.SIC.png', img_blank)
 
     img_blank = np.zeros(img.shape[:2], dtype="uint8")
     img_blank.fill(255)
 
     masked = np.where(img_mask, img, img_blank)
     if save_steps:
@@ -374,47 +498,69 @@
         "image": masked,
         "boxes": boxes,
         "contours": selected
     }
 
 def processTableBoxes(img:np.ndarray, markup:np.ndarray=None,
             boxes:list= None, contours:list = None,
-            fidx:int = None, use_blur: bool = True,
-            bleed: int = 4, mindim: int = 1000,
+            fidx:int = None,
             config: dict = None,
             save_steps: bool = False) -> dict:
     """will take the supplied images and the boxes, will order the boxes"""
     if markup is not None:
         img_return = markup.copy()
     else:
         img_return = img.copy()
 
     logger.info("PTB: {%s:--} B:%s C:%s S:%s", fidx, len(boxes), len(contours), img.shape)
 
+    # load config
+    defratio = config.get("ratio", 3) if config is not None else 3
+    use_blur = config.get("useblur", False) if config is not None else False
+    bleed = config.get("bleed", 4) if config is not None else 4
+    mindim = config.get("mindim", 1000) if config is not None else 1000
+    kernel = config.get("kernel", 3) if config is not None else 3
+    dilate = config.get("dilate", -1) if config is not None else -1
+    erode = config.get("erode", -1) if config is not None else -1
+    resize = config.get("resize", cv2.INTER_AREA) if config is not None else cv2.INTER_AREA
+    kerneldim = (kernel, kernel)
+
     img_edit = img.copy()
-    kernelX = cv2.getStructuringElement(cv2.MORPH_CROSS,(3,3))
-    kernelE = cv2.getStructuringElement(cv2.MORPH_ELLIPSE,(3,3))
+    if config and config.get("shape", "cross") == "ellipse":
+        kernelX = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, kerneldim)
+    else:
+        kernelX = cv2.getStructuringElement(cv2.MORPH_CROSS, kerneldim)
 
     font = cv2.FONT_HERSHEY_SIMPLEX
     idx = -1
     border = 10
 
     # a list of the boxes, and found text areas
     rows = []
     for (x,y,w,h) in boxes:
         idx += 1
+        logger.info("PTB: {%s:%s} BB:%s", fidx, idx, (x,y,w,h))
+
         # draw the contour as white...
         cv2.drawContours(image=img_edit, contours=contours[idx], contourIdx=-1, color=(255), thickness=bleed)
         #cv2.rectangle(img_edit, (x+bleed, y+bleed), (x + w - (2*bleed), y + h - (2*bleed)), (255), bleed)
 
         cv2.rectangle(img_return, (x, y), (x + w, y + h), (255, 0, 0), 1)
         cv2.rectangle(img_return, (x+bleed, y+bleed), (x + w - (2*bleed), y + h - (2*bleed)), (255, 255, 0), 1)
 
         # sele3ct the region to use for anlysis
-        crop_img = cv2.copyMakeBorder(src=img_edit[y+bleed:y+h-(2*bleed), x-bleed:x+w-(2*bleed)],
+        # bleed cutrs into the box shape
+        #       ╔ bleed
+        # x,y ┌───────┐
+        #     │ ┌───┐ │ ═ bleed
+        #     │ │   │ │
+        #     │ └───┘ │ ═ bleed
+        #     └───────┘ x+w,y+h
+        #
+        crop_img = cv2.copyMakeBorder(src=img_edit[y+bleed:y+h-(2*bleed), x+bleed:x+w-(2*bleed)],
             top=border+bleed,
             bottom=border+bleed,
             left=border+bleed,
             right=border+bleed,
             borderType=cv2.BORDER_CONSTANT,
             value=[255])
 
@@ -434,90 +580,92 @@
         text_data = segmentImage(img=crop_img, fidx=fidx, idx=idx, save_steps=save_steps)
         crop_img = text_data.get("image")
         if crop_img is None:
             continue
         if save_steps:
             cv2.imwrite(f'data/eng/crops/F{fidx}.{idx}.PTB.png', crop_img)
 
-        if use_blur:
-            crop_img = cv2.blur(src=crop_img, ksize=(3,3))
-            #crop_img = cv2.erode(crop_img, kernelX, iterations=3)
-            #crop_img = cv2.dilate(crop_img, kernelX, iterations=1)
+        #if use_blur:
+        #    crop_img = cv2.blur(src=crop_img, ksize=(3,3))
+        #    #crop_img = cv2.erode(crop_img, kernelX, iterations=3)
+        #    #crop_img = cv2.dilate(crop_img, kernelX, iterations=1)
 
         # create image to put text on...
         ch,cw = crop_img.shape[:2]
-        img_text = np.zeros((ch,cw,3), dtype="uint8")
-        img_text.fill(255)
 
         ratio = 1
-        if w < mindim or h < mindim:
-            mindim = min(w,h)
-            ratio = int(config.get("ratio",3))
+        if ch < mindim or cw < mindim:
+            ratio = defratio
 
-            rw = int(w * ratio)
-            rh = int(h * ratio)
+            rw = int(cw * ratio)
+            rh = int(ch * ratio)
             logger.info("Ratio: {%s:%s} %s %s => %s", fidx, idx, rw, rh, ratio)
+            logger.info("Ops: {%s:%s} E:%s D:%s B:%s I:%s", fidx, idx, erode, dilate, use_blur, resize)
 
             # rescale:
-            crop_img = cv2.resize(src=crop_img, dsize=(rw, rh), interpolation = cv2.INTER_AREA)
+            crop_img = cv2.resize(src=crop_img, dsize=(rw, rh), interpolation = resize)
+            if erode > 0:
+                crop_img = cv2.erode(crop_img, kernelX, iterations=erode)
+            if dilate > 0:
+                crop_img = cv2.dilate(crop_img, kernelX, iterations=dilate)
+            if use_blur:
+                crop_img = cv2.blur(src=crop_img, ksize=kerneldim)
 
             # detect text orientation...
             try:
-                results = pytesseract.image_to_osd(image=crop_img, output_type=pytesseract.Output.DICT, config='--psm 11 -c min_characters_to_try=5')
+                results = pytesseract.image_to_osd(image=crop_img, output_type=pytesseract.Output.DICT, config='--psm 1 -c min_characters_to_try=5')
                 logger.info("OSD: {%s:%s} => %s", fidx, idx, results)
             except Exception as ex:
                 logger.error("OSD: {%s:%s} => %s", fidx, idx, ex)
 
-        # hack to fix speckels etc....
-        # double size and then shrink
-        if ratio == 1:
-            crop_img = cv2.resize(src=crop_img, dsize=(w*2, h*2), interpolation = cv2.INTER_AREA)
+            img_text = np.zeros((rh,rw,3), dtype="uint8")
+            img_text.fill(255)
         else:
-            crop_img = cv2.resize(src=crop_img, dsize=(rw*2, rh*2), interpolation = cv2.INTER_AREA)
-            crop_img = cv2.erode(crop_img, kernelX, iterations=1)
-            crop_img = cv2.dilate(crop_img, kernelX, iterations=1)
+            img_text = np.zeros((ch,cw,3), dtype="uint8")
+            img_text.fill(255)
+
+        if save_steps:
+            cv2.imwrite(f'data/eng/crops/F{fidx}.{idx}.RAT.png', crop_img)
+
+        # add a border to the image
+
 
         # process the text in the image...
-        def_opt = "--psm 12"
+        def_opt = "--psm 1"
         tess_options = config.get("tesseract", {}).get("i2d", def_opt) if config else def_opt
+        logger.info("TESS: {%s:%s} => %s", fidx, idx, tess_options)
+
         d = pytesseract.image_to_data(image=crop_img, output_type=pytesseract.Output.DICT, config=tess_options)
         flds = d.keys()
         r = len(d['level'])
 
-        # now shrink the image by 50%
-        if ratio == 1:
-            crop_img = cv2.resize(src=crop_img, dsize=(w, h), interpolation = cv2.INTER_AREA)
-        else:
-            crop_img = cv2.resize(src=crop_img, dsize=(rw, rh), interpolation = cv2.INTER_AREA)
-
-        cv2.fillPoly(img=img_return, pts=contours[idx], color=(0,255,255))
-
+        cv2.fillPoly(img=img_return, pts=contours[idx], color=(0,255,0))
 
         for i in range(r):
             # get the the detected text values...
             if len(d.get("text",[])[i].strip()) == 0:
                 continue
 
             row = {
                 "file": fidx,
                 "idx": idx
             }
             for f in flds:
                 row[f] = d.get(f,[])[i]
 
-            # correct the ratio...
-            for f in ['left', 'top', 'width', 'height']:
-                row[f] = int(row[f] / ratio)
-
             # save the crop image for post analysis - debug
             (xt, yt, wt, ht) = (row['left'], row['top'], row['width'], row['height'])
             cv2.putText(img=img_text, text=(row['text']),
                     org=(xt, yt), fontFace=font, fontScale=1, color=(0, 0, 255),
                     thickness=1)
 
+            # correct the ratio...
+            for f in ['left', 'top', 'width', 'height']:
+                row[f] = int(row[f] / ratio)
+
             # apply the offset...
             row['left'] += (x - border)
             row['top'] += (y - border)
             rows.append(row)
 
             logger.info("Text: {%s:%s} %s", fidx, idx, row)
 
@@ -535,15 +683,15 @@
     will try to extract the following:
         grids: connected boxes
         text: text and it's position
     """
     data = {}
     img = image.copy()
     fidx = config.get("file",{}).get("id", -1)
-    logger.info("File IDX: %s", fidx)
+    logger.info("ETA: {%s} FIDX", fidx)
 
     save_steps = config.get("debug", {}).get("save")
     if save_steps:
         logger.debug("Saving Images...")
         data["images"] = {}
 
     # get some kernels to use...
@@ -563,26 +711,35 @@
     contour_data = extactImageContours(img=img_thresh, markup=img,
                 config=config.get("contours,{}"), fidx=fidx)
 
     if save_steps:
         logger.debug("Save Contour Image")
         data["images"]["contours"] = contour_data.get("image")
 
+    # review the findings...
+    cc = contour_data.get("review",{}).get("contours",0)
+    cut = contour_data.get("review",{}).get("cut",0)
+    cut_ratio = cut / cc if cc != 0 else 0
+    logger.info("ETA: {%s} Review %s \ %s = %s", fidx, cut, cc, cut_ratio)
+    # blur is too many cut contours
+    if cut_ratio >= 50.0:
+        cv2.blur(src=img_thresh, ksize=(kernel_size, kernel_size))
+
     if len(contour_data.get("borders",[])) > 0:
         box_data = box_connected(img=img_thresh, markup=img, boxes=contour_data.get("boxes",[]),
                 contours=contour_data.get("borders",[]), fidx=fidx, save_steps=save_steps)
 
         if save_steps:
             logger.debug("Save Box Image")
             data["images"]["boxes"] = box_data.get("image")
 
         if len(box_data.get("boxes",[])) > 0:
             text_data = processTableBoxes(img=img_thresh, markup=img,
                     boxes=box_data.get("boxes",[]), contours=box_data.get("borders",[]),
-                    fidx=fidx, save_steps=save_steps, use_blur=config.get("operations", {}).get("blur", False))
+                    fidx=fidx, save_steps=save_steps, config=config.get("extract",{}))
 
             if save_steps:
                 logger.debug("Save Text Image")
                 data["images"]["text"] = text_data.get("image")
             data["text"] = text_data.get("boxes", [])
 
     if save_steps:
@@ -797,14 +954,16 @@
     fidx = config.get("file",{}).get("id", -1)
     logger.info("File IDX: %s", fidx)
 
     save_steps = config.get("debug", {}).get("save")
     if save_steps:
         logger.debug("Saving Images...")
 
+    data = {}
+
     # pre process the image...
     image_data = process_image(image=image, config=config)
 
     # get the shapes (any contour)
     # get the boxes A contour whose approx length is 4
     img_gray = image_data.get("gray")
     img_thresh = image_data.get("thresh")
@@ -814,14 +973,15 @@
 
     # process for circles if required...
     if config.get("operations", {}).get("circles", False):
         cc_circles = classify_circles(image=img_gray, config=config)
 
     # now build the grid and tables...
 
+    return data
 
 def process_alignments(image: np.array, markup: np.array = None,
     config: dict = None, baselines:dict=None, data: dict=None):
     """this process will group the contorurs into blocks...
     find the horizontal related contours...
         baselines = {
             "x": {},
@@ -843,21 +1003,21 @@
                 #rects.append(r1)
                 contours.append(contour)
                 # check if the rectangle is close to an already seen one
 
 
                 rects = np.append(rects,np.array([[contour.x, contour.y, contour.w, contour.h]]), axis=0)
                 rects, _ = cv2.groupRectangles(rects, 0, 0.85)
-                #mrg_rects = [merge(r1=r1, r2=r2) for r2 in rects if intersect(r1=r1,r2=r2, border=border)]
-                #descrete_rects = [r2 for r2 in rects if not intersect(r1=r1, r2=r2, border=border)]
+                #mrg_rects = [rectangle_merge(r1=r1, r2=r2) for r2 in rects if rectangle_intersect(r1=r1,r2=r2, border=border)]
+                #descrete_rects = [r2 for r2 in rects if not rectangle_intersect(r1=r1, r2=r2, border=border)]
                 #rects = mrg_rects + descrete_rects
 
         # merge shapes together...
-        #mrg_rects = [merge(r1=r1, r2=r2) for r2 in rects if intersect(r1=r1,r2=r2, border=border)]
-        #descrete_rects = [r2 for r2 in rects if not intersect(r1=r1, r2=r2, border=border)]
+        #mrg_rects = [rectangle_merge(r1=r1, r2=r2) for r2 in rects if rectangle_intersect(r1=r1,r2=r2, border=border)]
+        #descrete_rects = [r2 for r2 in rects if not rectangle_intersect(r1=r1, r2=r2, border=border)]
         #rects = mrg_rects + descrete_rects
 
         #cv2.line(img=img_return, pt1=(minx,ly), pt2=(maxx,ly), color=(255, 255, 0), thickness=1)
         #for r1 in rects:
         for r in rects:
             cv2.putText(img=img_return, text=str(r), org=(5,ly), fontFace=cv2.FONT_HERSHEY_SIMPLEX, fontScale=0.5, color=(255, 255, 0), thickness=1)
             r1 = Rectangle(r[0], r[1], r[2], r[3])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lost_cat_images-0.0.1/lost_cat_images/utils/utils_pdf.py` & `lost_cat_images-1.0.0/lost_cat_images/utils/utils_pdf.py`

 * *Files identical despite different names*

### Comparing `lost_cat_images-0.0.1/pyproject.toml` & `lost_cat_images-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lost_cat_images"
-version = "0.0.1"
+version = "1.0.0"
 authors = [
   { name="Dreffed aka David Gloyn-Cox", email="dreffed@gmail.com" },
   { name="Thoughtswin Systems Inc", email="david.gloyn-cox@thoughtswinsystems.com" },
 ]
 description = "Lost Cat (images) is a package for image related uris and tools"
 readme = "README.md"
 license = { file="LICENSE" }
@@ -19,20 +19,25 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "lost_cat>=0.1.6",
+    "lost_cat_office",
     "numpy",
     "opencv-python",
+    "pandas",
     "pillow",
+    "psutil",
     "pymupdf",
     "pytesseract",
-    "scipy"
+    "python-dotenv",
+    "scipy",
+    "scikit-image",
 ]
 
 [tool.setuptools.packages.find]
 include = ["lost_cat_images*"]
 
 [project.urls]
 "Homepage" = "https://github.com/thoughtswinsystems/lost_cat_images"
```

### Comparing `lost_cat_images-0.0.1/test/test_ocr.py` & `lost_cat_images-1.0.0/test/test_ocr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """A test case for the path utils module"""
 import logging
 import glob
 import os
-import sys
 import unittest
 
 from lost_cat_images.parsers.engimg_parser import EngImgParser
 from lost_cat_images.utils.utils_pdf import make_pdf_images, cv2
-from lost_cat_images.utils.utils_ocr import classify_contours, Contour
+#from lost_cat_images.utils.utils_ocr import classify_contours, Contour
 
 logger = logging.getLogger(__name__)
 logger.level = logging.DEBUG
 file_handler = logging.FileHandler(f"logs/test_ocr.log")
 logger.addHandler(file_handler)
 
 class TestOCR(unittest.TestCase):
@@ -54,18 +53,18 @@
         """This will scan the provided pdf and image files and
         extract the text using original flow"""
         for fidx, f in enumerate(self.files):
             logger.info("File: [%s] => %s", fidx, f)
             _, ext = os.path.splitext(f)
             if ext.lower() in [".pdf"]:
                 # we have a PDF so now process.
-                pdf = EngImgParser(f)
-                conf = pdf.get_config()
+                obj = EngImgParser(f)
+                conf = obj.get_config()
                 if "file" not in conf:
                     conf["file"] = {}
                 conf["file"]["id"] = fidx
-                pdf.set_config(conf)
+                obj.set_config(conf)
 
-                funx = pdf.avail_functions().get("parser")
+                funx = obj.avail_functions().get("parser")
                 data = funx()
                 for key, value in data.items():
                     logger.info("\t%s => %s", key, type(value))
```

### Comparing `lost_cat_images-0.0.1/test/test_pdf.py` & `lost_cat_images-1.0.0/test/test_pdf.py`

 * *Files identical despite different names*

### Comparing `lost_cat_images-0.0.1/test/test_shapes.py` & `lost_cat_images-1.0.0/test/test_shapes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """A test case for the path utils module"""
 import logging
 import unittest
 
-from lost_cat_images.utils.utils_shapes import Rectangle, ShapeGrouper, intersect, merge, contains
+from lost_cat_images.utils.utils_shapes import Rectangle, ShapeGrouper, rectangle_intersect, rectangle_merge, rectangle_contains
 
 logger = logging.getLogger(__name__)
 logger.level = logging.DEBUG
 file_handler = logging.FileHandler("logs/test_shapes.log")
 logger.addHandler(file_handler)
 
 class TestShapes(unittest.TestCase):
@@ -14,16 +14,16 @@
 
     def test_rect_interset(self):
         """test the intersection"""
         rect1 = Rectangle(1,1,2,2)  # 3,3
         rect2 = Rectangle(2,2,2,2)  # 4,4
         rect3 = Rectangle(4,4,2,2)  # 6,6
 
-        self.assertTrue(intersect(rect1, rect2), msg="Rectangle do overlap!")
-        self.assertFalse(intersect(rect1,rect3), msg="Rectangle don't overlap!")
+        self.assertTrue(rectangle_intersect(rect1, rect2), msg="Rectangle do overlap!")
+        self.assertFalse(rectangle_intersect(rect1,rect3), msg="Rectangle don't overlap!")
 
     def test_vars(self):
         """test that the data call works"""
         rect1 = Rectangle(1,1,1,1)
         tags = {
             "id": 0,
             "contours": [[1,2],[3,4]]
@@ -35,35 +35,35 @@
             logger.info("\t%s: %s", key ,value)
 
     def test_rect_merge(self):
         """Test merging rectangles"""
         rect1 = Rectangle(1,1,2,2)  # 3,3
         rect2 = Rectangle(2,2,2,2)  # 4,4
 
-        rect3 = merge(rect1, rect2)
+        rect3 = rectangle_merge(rect1, rect2)
         self.assertTrue(rect3.x == 1 and rect3.y == 1 and \
                 rect3.w == 3 and rect3.h == 3, msg="Merge failed!")
 
     def test_rect_interset_border(self):
         """Test the intersect with a border set"""
         rect1 = Rectangle(1,1,2,2)  # 3,3
         rect2 = Rectangle(5,5,2,2)  # 6,6
 
-        self.assertFalse(intersect(rect1,rect2), msg="Rectangle don't overlap!")
-        self.assertFalse(intersect(rect1,rect2, 1), msg="Rectangle don't overlap!")
-        self.assertTrue(intersect(rect1, rect2, 2), msg="Rectangle do overlap!")
+        self.assertFalse(rectangle_intersect(rect1,rect2), msg="Rectangle don't overlap!")
+        self.assertFalse(rectangle_intersect(rect1,rect2, 1), msg="Rectangle don't overlap!")
+        self.assertTrue(rectangle_intersect(rect1, rect2, 2), msg="Rectangle do overlap!")
 
     def test_shapes(self):
         """Test the shape heirarchy, currently contains only"""
         rect1 = Rectangle(1,1,15,15)
         rect2 = Rectangle(2,2,4,4)
         rect3 = Rectangle(14,14,3,3)
 
-        self.assertTrue(contains(rect1, rect2), msg=f"{rect1} should contain {rect2}")
-        self.assertFalse(contains(rect1, rect3), msg=f"{rect1} should not contain {rect3}")
+        self.assertTrue(rectangle_contains(rect1, rect2), msg=f"{rect1} should contain {rect2}")
+        self.assertFalse(rectangle_contains(rect1, rect3), msg=f"{rect1} should not contain {rect3}")
 
         shpg = ShapeGrouper()
         shpg.add_rectangle(rect1)
         shpg.add_rectangle(rect2)
         shpg.add_rectangle(rect3)
 
         logger.info(shpg.shapes)
```

