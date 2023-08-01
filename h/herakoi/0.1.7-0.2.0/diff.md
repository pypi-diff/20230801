# Comparing `tmp/herakoi-0.1.7.tar.gz` & `tmp/herakoi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herakoi-0.1.7.tar", last modified: Tue May 16 17:16:20 2023, max compression
+gzip compressed data, was "herakoi-0.2.0.tar", last modified: Tue Aug  1 14:23:35 2023, max compression
```

## Comparing `herakoi-0.1.7.tar` & `herakoi-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lucadim    (501) staff       (20)        0 2023-05-16 17:16:20.207246 herakoi-0.1.7/
--rw-r--r--   0 lucadim    (501) staff       (20)     1072 2023-05-16 17:15:39.000000 herakoi-0.1.7/LICENSE.md
--rw-r--r--   0 lucadim    (501) staff       (20)     3048 2023-05-16 17:16:20.207098 herakoi-0.1.7/PKG-INFO
--rw-r--r--   0 lucadim    (501) staff       (20)     2431 2023-05-16 17:15:39.000000 herakoi-0.1.7/README.md
-drwxr-xr-x   0 lucadim    (501) staff       (20)        0 2023-05-16 17:16:20.205848 herakoi-0.1.7/herakoi/
--rw-r--r--   0 lucadim    (501) staff       (20)     1056 2023-05-16 17:15:39.000000 herakoi-0.1.7/herakoi/__init__.py
--rw-r--r--   0 lucadim    (501) staff       (20)       57 2023-05-16 17:15:39.000000 herakoi-0.1.7/herakoi/__main__.py
--rw-r--r--   0 lucadim    (501) staff       (20)    11662 2023-05-16 17:15:39.000000 herakoi-0.1.7/herakoi/core.py
-drwxr-xr-x   0 lucadim    (501) staff       (20)        0 2023-05-16 17:16:20.206870 herakoi-0.1.7/herakoi.egg-info/
--rw-r--r--   0 lucadim    (501) staff       (20)     3048 2023-05-16 17:16:20.000000 herakoi-0.1.7/herakoi.egg-info/PKG-INFO
--rw-r--r--   0 lucadim    (501) staff       (20)      279 2023-05-16 17:16:20.000000 herakoi-0.1.7/herakoi.egg-info/SOURCES.txt
--rw-r--r--   0 lucadim    (501) staff       (20)        1 2023-05-16 17:16:20.000000 herakoi-0.1.7/herakoi.egg-info/dependency_links.txt
--rw-r--r--   0 lucadim    (501) staff       (20)       42 2023-05-16 17:16:20.000000 herakoi-0.1.7/herakoi.egg-info/entry_points.txt
--rw-r--r--   0 lucadim    (501) staff       (20)       72 2023-05-16 17:16:20.000000 herakoi-0.1.7/herakoi.egg-info/requires.txt
--rw-r--r--   0 lucadim    (501) staff       (20)        8 2023-05-16 17:16:20.000000 herakoi-0.1.7/herakoi.egg-info/top_level.txt
--rw-r--r--   0 lucadim    (501) staff       (20)     1054 2023-05-16 17:15:39.000000 herakoi-0.1.7/pyproject.toml
--rw-r--r--   0 lucadim    (501) staff       (20)       38 2023-05-16 17:16:20.207292 herakoi-0.1.7/setup.cfg
+drwxr-xr-x   0 lucadim    (501) staff       (20)        0 2023-08-01 14:23:35.090607 herakoi-0.2.0/
+-rw-r--r--   0 lucadim    (501) staff       (20)     1072 2023-08-01 14:23:09.000000 herakoi-0.2.0/LICENSE.md
+-rw-r--r--   0 lucadim    (501) staff       (20)     2699 2023-08-01 14:23:35.090485 herakoi-0.2.0/PKG-INFO
+-rw-r--r--   0 lucadim    (501) staff       (20)     2082 2023-08-01 14:23:09.000000 herakoi-0.2.0/README.md
+drwxr-xr-x   0 lucadim    (501) staff       (20)        0 2023-08-01 14:23:35.089476 herakoi-0.2.0/herakoi/
+-rw-r--r--   0 lucadim    (501) staff       (20)     1267 2023-08-01 14:23:09.000000 herakoi-0.2.0/herakoi/__init__.py
+-rw-r--r--   0 lucadim    (501) staff       (20)       57 2023-08-01 14:23:09.000000 herakoi-0.2.0/herakoi/__main__.py
+-rw-r--r--   0 lucadim    (501) staff       (20)    11783 2023-08-01 14:23:09.000000 herakoi-0.2.0/herakoi/core.py
+drwxr-xr-x   0 lucadim    (501) staff       (20)        0 2023-08-01 14:23:35.090283 herakoi-0.2.0/herakoi.egg-info/
+-rw-r--r--   0 lucadim    (501) staff       (20)     2699 2023-08-01 14:23:35.000000 herakoi-0.2.0/herakoi.egg-info/PKG-INFO
+-rw-r--r--   0 lucadim    (501) staff       (20)      279 2023-08-01 14:23:35.000000 herakoi-0.2.0/herakoi.egg-info/SOURCES.txt
+-rw-r--r--   0 lucadim    (501) staff       (20)        1 2023-08-01 14:23:35.000000 herakoi-0.2.0/herakoi.egg-info/dependency_links.txt
+-rw-r--r--   0 lucadim    (501) staff       (20)       42 2023-08-01 14:23:35.000000 herakoi-0.2.0/herakoi.egg-info/entry_points.txt
+-rw-r--r--   0 lucadim    (501) staff       (20)      229 2023-08-01 14:23:35.000000 herakoi-0.2.0/herakoi.egg-info/requires.txt
+-rw-r--r--   0 lucadim    (501) staff       (20)        8 2023-08-01 14:23:35.000000 herakoi-0.2.0/herakoi.egg-info/top_level.txt
+-rw-r--r--   0 lucadim    (501) staff       (20)     1236 2023-08-01 14:23:09.000000 herakoi-0.2.0/pyproject.toml
+-rw-r--r--   0 lucadim    (501) staff       (20)       38 2023-08-01 14:23:35.090650 herakoi-0.2.0/setup.cfg
```

### Comparing `herakoi-0.1.7/LICENSE.md` & `herakoi-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `herakoi-0.1.7/PKG-INFO` & `herakoi-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herakoi
-Version: 0.1.7
+Version: 0.2.0
 Summary: A sonification tool
 Author-email: Michele Ginolfi <micheleginolfi@gmail.com>, Luca Di Mascolo <lucadimascolo@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/lucadimascolo/herakoi
 Project-URL: Bug Tracker, https://github.com/lucadimascolo/herakoi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,41 +12,26 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # herakoi 
 
+
+[![DOI](https://zenodo.org/badge/515594944.svg)](https://zenodo.org/badge/latestdoi/515594944)
+![PyPI version](https://img.shields.io/pypi/v/herakoi) [![Documentation Status](https://readthedocs.org/projects/herakoi/badge/?version=latest)](https://herakoi.readthedocs.io/en/latest/?badge=latest)
+
 `herakoi` is a motion-sensing sonification experiment. 
 
 It uses a Machine Learning (ML)-based algorithm for hand recognition to track in real-time the position of your hands in the scene observed by a webcam connected to your computer. The model landmarks coordinates of your hands are then re-projected onto the pixel coordinates of your favorite image. The visual properties of the "touched" pixels (at the moment, color and saturation) are then converted into sound properties of your favorite instrument, which you can choose from your favorite virtual MIDI keyboard.
 
 In this way, you can hear the sound of any images, for educational, artistic, or just-fun purposes!
 
 Fully written in python, `herakoi` requires relatively little computational power and can be run on different on the most popular operating systems (macOS, Microsoft Windows, Linux). 
 
-
-## Installation
-
-`herakoi` runs on python 3, so make sure to have it installed on your computer. The most stable release of `herakoi` can then be installed through [pip](https://pip.pypa.io/en/stable/) simply as
-
-```bash
-pip install herakoi
-```
-This will install `herakoi` as well as all the necessary dependencies. Before firing up `herakoi`, you however have to install an additional package, [`mediapipe`](https://google.github.io/mediapipe/). In general, you should be able to do so via
-
-```bash
-pip install mediapipe
-```
-If your computer is instead equipped with an Apple Silicon chip, you should use
-
-```
-pip install mediapipe-silicon
-```
-
 ## Usage
 
 1. run `herakoi path_to_your_favorite_image`
 2. open your favorite MIDI player (e.g., if you run `herakoi` on an Apple computer, GarageBang is a good option) 
 3. have fun!
 
 You can customize your `herakoi` by using the following flags:
```

### Comparing `herakoi-0.1.7/README.md` & `herakoi-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,21 @@
 # herakoi 
 
+
+[![DOI](https://zenodo.org/badge/515594944.svg)](https://zenodo.org/badge/latestdoi/515594944)
+![PyPI version](https://img.shields.io/pypi/v/herakoi) [![Documentation Status](https://readthedocs.org/projects/herakoi/badge/?version=latest)](https://herakoi.readthedocs.io/en/latest/?badge=latest)
+
 `herakoi` is a motion-sensing sonification experiment. 
 
 It uses a Machine Learning (ML)-based algorithm for hand recognition to track in real-time the position of your hands in the scene observed by a webcam connected to your computer. The model landmarks coordinates of your hands are then re-projected onto the pixel coordinates of your favorite image. The visual properties of the "touched" pixels (at the moment, color and saturation) are then converted into sound properties of your favorite instrument, which you can choose from your favorite virtual MIDI keyboard.
 
 In this way, you can hear the sound of any images, for educational, artistic, or just-fun purposes!
 
 Fully written in python, `herakoi` requires relatively little computational power and can be run on different on the most popular operating systems (macOS, Microsoft Windows, Linux). 
 
-
-## Installation
-
-`herakoi` runs on python 3, so make sure to have it installed on your computer. The most stable release of `herakoi` can then be installed through [pip](https://pip.pypa.io/en/stable/) simply as
-
-```bash
-pip install herakoi
-```
-This will install `herakoi` as well as all the necessary dependencies. Before firing up `herakoi`, you however have to install an additional package, [`mediapipe`](https://google.github.io/mediapipe/). In general, you should be able to do so via
-
-```bash
-pip install mediapipe
-```
-If your computer is instead equipped with an Apple Silicon chip, you should use
-
-```
-pip install mediapipe-silicon
-```
-
 ## Usage
 
 1. run `herakoi path_to_your_favorite_image`
 2. open your favorite MIDI player (e.g., if you run `herakoi` on an Apple computer, GarageBang is a good option) 
 3. have fun!
 
 You can customize your `herakoi` by using the following flags:
```

### Comparing `herakoi-0.1.7/herakoi/__init__.py` & `herakoi-0.2.0/herakoi/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 def basic():
   pars = argparse.ArgumentParser()
   pars.add_argument('image',
                     help='Input image',
                     nargs='?')
   pars.add_argument('--notes',
                     help='Define the pitch range (as note+octave format; e.g., C4)',
-                    nargs=2,default=['C1','B8'],metavar=('low','high'))
+                    nargs=2,default=['C2','B6'],metavar=('low','high'))
   pars.add_argument('--volume',
                     help='Change the low volume threshold (in percentage)',
                     default=20,metavar=('volume'),type=float)
   pars.add_argument('--mode',
                     help='Select herakoi mode [single/adaptive/scan]',
                     default='single',metavar=('mode'))
   pars.add_argument('--box',
                     help='sonification box size in units of frame percentage',
                     default=2,metavar=('box'),type=float)
+  pars.add_argument('--video',
+                    help='Select video source',
+                    default=0,type=int)
   pars.add_argument('--switch',action='store_true')
+  pars.add_argument('--imgonly',action='store_false')
   args = pars.parse_args()
 
-  start(image=args.image,mode=args.mode,notes=(args.notes[0],args.notes[1]),volume=args.volume,box=args.box,switch=args.switch)
+  start(image=args.image,mode=args.mode,notes=(args.notes[0],args.notes[1]),volume=args.volume,box=args.box,switch=args.switch,imgonly=args.imgonly,video=args.video)
```

### Comparing `herakoi-0.1.7/herakoi/core.py` & `herakoi-0.2.0/herakoi/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,16 @@
         return image[hi:-hi,:]
     else:
       return image
 
 # Single-user mode
 # =====================================
   def run(self,mode='single',vlims=vlims_,flims=flims_,**kwargs):
+    imgonly = kwargs.get('imgonly',False)
+
     ophands = self.mphands.Hands(max_num_hands=2 if mode=='scan' else 1)
 
     onmusic = False
 
     pxshift = kwargs.get('shift',2)
     pxshift = (pxshift/100)*np.minimum(self.opmusic.w,self.opmusic.h)
 
@@ -257,16 +259,20 @@
             self.mpdraws.draw_landmarks(opframe,immarks,self.mphands.HAND_CONNECTIONS,None)
 
             px, py, _ = self.posndraw(immusic,immarks,imlabel,False)
 
             if imlabel=='Right': pxmusic[0] = px
             if imlabel=='Left':  pxmusic[1] = py
 
+            pxpatch = [self.oppatch,self.oppatch]
+
           cv2.circle(immusic,(pxmusic[0],pxmusic[1]),pxmusic[2],(255,255,255),-1)
 
+          bhmidif, bhmidiv = self.getmex(pxmusic,pxpatch,vlims,flims)
+
         else:
           for mi, immarks in enumerate(imhands.multi_hand_landmarks):
             imlabel = imhands.multi_handedness[mi].classification[0].label
 
             _       = self.posndraw(opframe,immarks,imlabel,True)
 
             if self.oppatch is None:
@@ -295,60 +301,59 @@
             
             if (mode in ['single','adaptive'] and imlabel=='Right'):
               rhmidif, rhmidiv = self.getmex(pxmusic,pxpatch,vlims,flims)
 
               bhmidif = rhmidif if bhmidif is None else int(0.50*(rhmidif+bhmidif))
               bhmidiv = rhmidiv if bhmidiv is None else int(0.50*(rhmidiv+bhmidiv))
 
-        if mode in ['single','adaptive']:
+        if mode in ['single','adaptive','scan']:
           if (bhmidif is not None) and (bhmidiv is not None):
             if time.time()-tictime>toctime and not onmusic:
               self.midiout.send(mido.Message('note_on',channel=8,note=bhmidif,velocity=bhmidiv))
               pxmusicold = pxmusic
               onmusic = True
 
             if time.time()-tictime>toctime+offtime and np.hypot(pxmusicold[0]-pxmusic[0],pxmusicold[1]-pxmusic[1])>pxshift:
               self.midiout.send(mido.Message('note_off',channel=8,note=bhmidif))
               self.panic(); onmusic = False
               
               tic = time.time()
           else: self.panic()
       else: self.panic()
 
-      if False:
-        cv2.imshow('imframe',opframe)
-        cv2.imshow('immusic',immusic)
+      if imgonly:
+        mixframe = immusic
       else:
         opframe = cv2.resize(opframe,None,fx=immusic.shape[0]/opframe.shape[0],fy=immusic.shape[0]/opframe.shape[0])
 
         mixframe = np.zeros((max(opframe.shape[0], immusic.shape[0]), opframe.shape[1] + immusic.shape[1], 3), dtype=np.uint8)
         mixframe[:opframe.shape[0],:opframe.shape[1],:] = opframe
         mixframe[:immusic.shape[0],opframe.shape[1]:,:] = immusic
 
-        # Show the combined image in a window
-        cv2.imshow('mixframe',mixframe)
+      # Show the combined image in a window
+      cv2.imshow('mixframe',mixframe)
 
-        hm, wm, _ = mixframe.shape
+      hm, wm, _ = mixframe.shape
 
-        if   (hm/wm)>(scrh/scrw):
-          hr = fill*scrh
-          wr = fill*scrh*wm/hm
-        elif (hm/wm)<=(scrh/scrw):
-          hr = fill*scrw*hm/wm
-          wr = fill*scrw
+      if   (hm/wm)>(scrh/scrw):
+        hr = fill*scrh
+        wr = fill*scrh*wm/hm
+      elif (hm/wm)<=(scrh/scrw):
+        hr = fill*scrw*hm/wm
+        wr = fill*scrw
 
-        wr, hr = int(wr), int(hr)
+      wr, hr = int(wr), int(hr)
 
-        cv2.resizeWindow('mixframe',wr,hr)
+      cv2.resizeWindow('mixframe',wr,hr)
 
       if (cv2.waitKey(1) & 0xFF == ord('q')) or (pressed is not None): break
 
     self.opvideo.release()
     cv2.destroyAllWindows()
-
+    cv2.waitKey(1)
 
 # Turn off all MIDI notes
 # =====================================
   def panic(self):
     for note in range(0,127):
       self.midiout.send(mido.Message('note_off',channel=8,note=note))
     self.midiout.reset()
```

### Comparing `herakoi-0.1.7/herakoi.egg-info/PKG-INFO` & `herakoi-0.2.0/herakoi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herakoi
-Version: 0.1.7
+Version: 0.2.0
 Summary: A sonification tool
 Author-email: Michele Ginolfi <micheleginolfi@gmail.com>, Luca Di Mascolo <lucadimascolo@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/lucadimascolo/herakoi
 Project-URL: Bug Tracker, https://github.com/lucadimascolo/herakoi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,41 +12,26 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # herakoi 
 
+
+[![DOI](https://zenodo.org/badge/515594944.svg)](https://zenodo.org/badge/latestdoi/515594944)
+![PyPI version](https://img.shields.io/pypi/v/herakoi) [![Documentation Status](https://readthedocs.org/projects/herakoi/badge/?version=latest)](https://herakoi.readthedocs.io/en/latest/?badge=latest)
+
 `herakoi` is a motion-sensing sonification experiment. 
 
 It uses a Machine Learning (ML)-based algorithm for hand recognition to track in real-time the position of your hands in the scene observed by a webcam connected to your computer. The model landmarks coordinates of your hands are then re-projected onto the pixel coordinates of your favorite image. The visual properties of the "touched" pixels (at the moment, color and saturation) are then converted into sound properties of your favorite instrument, which you can choose from your favorite virtual MIDI keyboard.
 
 In this way, you can hear the sound of any images, for educational, artistic, or just-fun purposes!
 
 Fully written in python, `herakoi` requires relatively little computational power and can be run on different on the most popular operating systems (macOS, Microsoft Windows, Linux). 
 
-
-## Installation
-
-`herakoi` runs on python 3, so make sure to have it installed on your computer. The most stable release of `herakoi` can then be installed through [pip](https://pip.pypa.io/en/stable/) simply as
-
-```bash
-pip install herakoi
-```
-This will install `herakoi` as well as all the necessary dependencies. Before firing up `herakoi`, you however have to install an additional package, [`mediapipe`](https://google.github.io/mediapipe/). In general, you should be able to do so via
-
-```bash
-pip install mediapipe
-```
-If your computer is instead equipped with an Apple Silicon chip, you should use
-
-```
-pip install mediapipe-silicon
-```
-
 ## Usage
 
 1. run `herakoi path_to_your_favorite_image`
 2. open your favorite MIDI player (e.g., if you run `herakoi` on an Apple computer, GarageBang is a good option) 
 3. have fun!
 
 You can customize your `herakoi` by using the following flags:
```

