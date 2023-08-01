# Comparing `tmp/gpcal-0.9.5.5.tar.gz` & `tmp/gpcal-0.9.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpcal-0.9.5.5.tar", last modified: Fri Jul 28 05:58:46 2023, max compression
+gzip compressed data, was "dist/gpcal-0.9.5.6.tar", last modified: Tue Aug  1 05:00:56 2023, max compression
```

## Comparing `gpcal-0.9.5.5.tar` & `gpcal-0.9.5.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-28 05:58:46.000000 gpcal-0.9.5.5/
--rw-rw-r--   0 jpark     (1000) jpark     (1000)      701 2023-07-28 05:58:46.000000 gpcal-0.9.5.5/PKG-INFO
--rw-r--r--   0 jpark     (1000) jpark     (1000)       62 2023-03-20 13:01:37.000000 gpcal-0.9.5.5/setup.cfg
--rw-r--r--   0 jpark     (1000) jpark     (1000)     1653 2023-07-28 05:58:42.000000 gpcal-0.9.5.5/setup.py
-drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-28 05:58:46.000000 gpcal-0.9.5.5/gpcal/
--rw-r--r--   0 jpark     (1000) jpark     (1000)      155 2023-07-26 07:11:13.000000 gpcal-0.9.5.5/gpcal/__init__.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    25243 2023-07-26 07:10:31.000000 gpcal-0.9.5.5/gpcal/synthetic.py
--rw-r--r--   0 jpark     (1000) jpark     (1000)     1256 2023-07-26 06:24:04.000000 gpcal-0.9.5.5/gpcal/cleanhelpers.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    36407 2023-07-26 07:10:24.000000 gpcal-0.9.5.5/gpcal/polsolver.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    67694 2023-07-26 07:10:43.000000 gpcal-0.9.5.5/gpcal/timecal.py
--rw-r--r--   0 jpark     (1000) jpark     (1000)    15099 2023-07-26 06:24:04.000000 gpcal-0.9.5.5/gpcal/aipsutil.py
--rw-r--r--   0 jpark     (1000) jpark     (1000)    27022 2023-07-26 07:10:07.000000 gpcal-0.9.5.5/gpcal/obshelpers.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    66424 2023-07-26 07:09:50.000000 gpcal-0.9.5.5/gpcal/channelcal.py
--rw-r--r--   0 jpark     (1000) jpark     (1000)   193500 2023-07-26 07:09:35.000000 gpcal-0.9.5.5/gpcal/gpcal.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    19944 2023-07-26 07:10:14.000000 gpcal-0.9.5.5/gpcal/plothelpers.py
+drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-08-01 05:00:56.000000 gpcal-0.9.5.6/
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)      701 2023-08-01 05:00:56.000000 gpcal-0.9.5.6/PKG-INFO
+-rw-r--r--   0 jpark     (1000) jpark     (1000)       62 2023-03-20 13:01:37.000000 gpcal-0.9.5.6/setup.cfg
+-rw-r--r--   0 jpark     (1000) jpark     (1000)     1653 2023-08-01 05:00:53.000000 gpcal-0.9.5.6/setup.py
+drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-08-01 05:00:56.000000 gpcal-0.9.5.6/gpcal/
+-rw-r--r--   0 jpark     (1000) jpark     (1000)      155 2023-08-01 05:00:05.000000 gpcal-0.9.5.6/gpcal/__init__.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    25216 2023-08-01 05:00:05.000000 gpcal-0.9.5.6/gpcal/synthetic.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)      916 2023-08-01 05:00:05.000000 gpcal-0.9.5.6/gpcal/cleanhelpers.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    33422 2023-08-01 05:00:05.000000 gpcal-0.9.5.6/gpcal/polsolver.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    67376 2023-08-01 05:00:05.000000 gpcal-0.9.5.6/gpcal/timecal.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)    14979 2023-08-01 05:00:05.000000 gpcal-0.9.5.6/gpcal/aipsutil.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)    22264 2023-08-01 05:00:05.000000 gpcal-0.9.5.6/gpcal/obshelpers.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    66047 2023-08-01 05:00:05.000000 gpcal-0.9.5.6/gpcal/channelcal.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)   193265 2023-08-01 05:00:05.000000 gpcal-0.9.5.6/gpcal/gpcal.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    19917 2023-08-01 05:00:05.000000 gpcal-0.9.5.6/gpcal/plothelpers.py
```

### Comparing `gpcal-0.9.5.5/PKG-INFO` & `gpcal-0.9.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gpcal
-Version: 0.9.5.5
+Version: 0.9.5.6
 Summary: A generalized instrumental polarization calibration pipeline for VLBI data
 Home-page: https://github.com/jhparkastro/gpcal
 Author: Jongho Park
 Author-email: jpark@asiaa.sinica.edu.tw
 License: gpl-2.0
 Download-URL: https://github.com/jhparkastro/gpcal/archive/v1.0.tar.gz
 Description: UNKNOWN
```

### Comparing `gpcal-0.9.5.5/setup.py` & `gpcal-0.9.5.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'gpcal',         # How you named your package folder (MyLib)
   packages = ['gpcal'],   # Chose the same as "name"
-  version = '0.9.5.5',      # Start with a small number and increase it with every change you make
+  version = '0.9.5.6',      # Start with a small number and increase it with every change you make
   license='gpl-2.0',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A generalized instrumental polarization calibration pipeline for VLBI data',   # Give a short description about your library
   author = 'Jongho Park',                   # Type in your name
   author_email = 'jpark@asiaa.sinica.edu.tw',      # Type in your E-Mail
   url = 'https://github.com/jhparkastro/gpcal',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/jhparkastro/gpcal/archive/v1.0.tar.gz',    # I explain this later on
   keywords = ['VLBI', 'polarimetry', 'astronomy', 'calibration'],   # Keywords that define your package best
```

### Comparing `gpcal-0.9.5.5/gpcal/synthetic.py` & `gpcal-0.9.5.6/gpcal/synthetic.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 from Wizardry.AIPSData import AIPSUVData as WAIPSUVData
 
 import aipsutil as au
 import obshelpers as oh
 
 import os
 
-from IPython import embed
-
 
 def synthetic_deq(nant, pang1, pang2, ant1, ant2, llamp, llphas, rramp, rrphas, model_ireal, model_iimag, model_rlreal, model_rlimag, model_lrreal, model_lrimag, stokes, *p):
     
     RiRj_Real = np.zeros(len(pang1))
     RiRj_Imag = np.zeros(len(pang1))
     LiLj_Real = np.zeros(len(pang1))
     LiLj_Imag = np.zeros(len(pang1))
```

### Comparing `gpcal-0.9.5.5/gpcal/polsolver.py` & `gpcal-0.9.5.6/gpcal/polsolver.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,115 +2,20 @@
 # -*- coding: utf-8 -*-
 """
 Created on Mon Nov 29 13:59:06 2021
 
 @author: jpark
 """
 
-
 import numpy as np
-import pandas as pd
 
 from scipy.optimize import curve_fit
 
-from astropy.coordinates import EarthLocation
-import astropy.time as at
-
-from AIPS import AIPS
-from AIPSTask import AIPSTask
-from AIPSData import AIPSUVData, AIPSImage
-from Wizardry.AIPSData import AIPSUVData as WAIPSUVData
-
-import aipsutil as au
-import obshelpers as oh
 import plothelpers as ph
 
-import os
-from os import path
-
-from IPython import embed
-
-
-from multiprocessing import cpu_count, Pool
-
-
-max_count = cpu_count()
-nproc = max_count - 1
-
-
-def cleanqu(direc, data, mask, save, bif, eif, ms, ps, uvbin, uvpower, dynam, shift_x, shift_y, stokes, log = None): # Version 1.1
-    """
-    Perform imaging of Stokes Q and U in Difmap.
-    
-    Args:
-        data (str): the name of the UVFITS file to be CLEANed.
-        mask (str): the name of the CLEAN windows to be used.
-        save (str): the name of the output Difmap save file.
-        log (str): the name of the Difmap log file.
-    """
-    
-    # logname = ''
-    
-    
-    # Write a simple Difmap script for CLEAN in the working directory.
-#        if not path.exists(self.direc+'GPCAL_Difmap_v1'):
-    f = open(direc+'GPCAL_Difmap_v1','w')
-    
-    f.write('observe %1\nmapcolor rainbow, 1, 0.5\nselect %13, %2, %3\nmapsize %4, %5\nuvweight %6, %7\nrwin %8\nshift %9,%10\ndo i=1,100\nclean 100, 0.02, imstat(rms)*%11\nend do\nselect i\nsave %12.%13\nexit')
-        
-    f.close()
-        
-    
-    curdirec = os.getcwd()
-    
-    logname = 'gpcal_difmap.log'
-
-    os.chdir(direc)
-    if log != None:
-        command = "echo @GPCAL_Difmap_v1 %s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s | difmap > %s" %(data,bif,eif,ms,ps,uvbin,uvpower,mask,shift_x,shift_y,dynam,save,stokes,logname) # Version 1.1!
-    else:
-        command = "echo @GPCAL_Difmap_v1 %s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s | difmap > /dev/null 2>&1" %(data,bif,eif,ms,ps,uvbin,uvpower,mask,shift_x,shift_y,dynam,save,stokes) # Version 1.1!
-    
-    # log.info('\nMaking CLEAN models for Stokes Q & U maps for {:s}...'.format(data))
-    
-    os.system(command)
-                
-    if log != None:
-        os.system('cat ' + logname + ' > ' + log)
-    
-    os.chdir(curdirec)
-    
-
-
-def cleanqu2(args): # Version 1.1
-    cleanqu3(*args)
-
-def cleanqu3(direc, data, mask, save, bif, eif, ms, ps, uvbin, uvpower, dynam, shift_x, shift_y, stokes, log): # Version 1.1
-    cleanqu(direc, data, mask, save, bif, eif, ms, ps, uvbin, uvpower, dynam, shift_x, shift_y, stokes, log = None)
-    
-
-def cleanqu_run(args): # Version 1.1
-    """
-    Perform imaging of Stokes Q and U in Difmap.
-    
-    Args:
-        data (str): the name of the UVFITS file to be CLEANed.
-        mask (str): the name of the CLEAN windows to be used.
-        save (str): the name of the output Difmap save file.
-        log (str): the name of the Difmap log file.
-    """
-
-    pool = Pool(processes = nproc)
-    pool.map(cleanqu2, args)
-    pool.close()
-    pool.join()
-    
-    # cleanqu(direc, data, mask, save, bif, eif, ms, ps, uvbin, uvpower, dynam, shift_x, shift_y, stokes, log = log)
-    
-
 
 def deq(x, *p):
     """
     The D-term models for the initial D-term estimation using the similarity assumption.
     
     Args:
         x: dummy parameters (not to be used).
```

### Comparing `gpcal-0.9.5.5/gpcal/timecal.py` & `gpcal-0.9.5.6/gpcal/timecal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,50 +1,33 @@
 
 
-import sys, os
+import os
 from os import path
 
 import pandas as pd
 import numpy as np
 from numpy.linalg import inv
 
-import timeit
 import logging
 import copy
-import glob
 
 from AIPS import AIPS
 from AIPSTask import AIPSTask
-from AIPSData import AIPSUVData, AIPSImage
+from AIPSData import AIPSUVData
 from Wizardry.AIPSData import AIPSUVData as WAIPSUVData
 
-from astropy.coordinates import EarthLocation
-import astropy.time as at
-
-from scipy.optimize import curve_fit
-
-import matplotlib
-matplotlib.use('Agg')
 import matplotlib.pyplot as plt
 
 import aipsutil as au
 import obshelpers as oh
 import cleanhelpers as ch
-import plothelpers as ph
 import polsolver as ps
 
-import gc
-import psutil
-
-from astropy.io import fits
-
-from multiprocessing import cpu_count, Pool
+from multiprocessing import Pool
 
-from IPython import embed
-        
 
 class timecal(object):
     """
     This is a class to calibrate instrumental polarization in VLBI data and produce D-term corrected UVFITS files.
     
     Attributes:
         aips_userno (int): AIPS user ID for ParselTongue
```

### Comparing `gpcal-0.9.5.5/gpcal/aipsutil.py` & `gpcal-0.9.5.6/gpcal/aipsutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,16 @@
 
 
 import numpy as np
 import pandas as pd
 import os, sys
 from os import path
 
-import timeit
-import logging
-import copy
-
-from AIPS import AIPS
 from AIPSTask import AIPSTask
 from AIPSData import AIPSUVData, AIPSImage
-from Wizardry.AIPSData import AIPSUVData as WAIPSUVData
 
 
 # Suppress AIPS printing on terminal
 def blockPrint():
     sys.stdout = open(os.devnull, 'w')
 
 # Enable AIPS printing on terminal
```

### Comparing `gpcal-0.9.5.5/gpcal/obshelpers.py` & `gpcal-0.9.5.6/gpcal/obshelpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,26 +9,21 @@
 
 import numpy as np
 
 from astropy.coordinates import EarthLocation
 import astropy.time as at
 import datetime as dt
 
-
-from AIPS import AIPS
-from AIPSTask import AIPSTask
 from AIPSData import AIPSUVData, AIPSImage
 from Wizardry.AIPSData import AIPSUVData as WAIPSUVData
 
 import aipsutil as au
 
 from os import path
 
-from IPython import embed
-
 
 def uvprt(data, select):
     """
     Extract UV data from ParselTongue UVData.
     
     Args:
         data (ParselTongue UVData): an input ParselTongue UVData.
@@ -155,82 +150,14 @@
     altitude = np.arcsin(np.sin(decarr) * np.sin(latarr) + np.cos(decarr) * np.cos(latarr) * np.cos(hangle))
     pang = f_el_arr * altitude + f_par_arr * parang + phi_off_arr
     
     
     return pang
     
 
-# #    def get_parang(self, time, ant, sourcearr, source, obsra, obsdec):
-# def get_parang(time, ant, sourcearr, year, month, day, source, obsra, obsdec, longarr, latiarr, f_el, f_par, phi_off): # Version 1.1!
-#     """
-#     Calculate antenna field-rotation angles.
-    
-#     Args:
-#         time (numpy.array): a numpy array of time in UTC of the visibilities.
-#         ant (numpy.array): a numpy array of antenna number of the visibilities.
-#         sourcearr (numpy.array): a numpy array of source of the visibilities.
-#         source (list): a list of calibrators.
-#         obsra (list): a list of calibrators' right ascension in units of degrees.
-#         obsdec (list): a list of calibrators' declination in units of degrees.
-    
-#     Returns:
-#         a numpy of the field-rotation angles.
-#     """        
-    
-#     nant = np.max(ant) + 1
-#     num = len(time)
-    
-#     lonarr, latarr, raarr, decarr, elarr, pararr, phiarr, yeararr, montharr, dayarr = \
-#         np.zeros(num), np.zeros(num), np.zeros(num), np.zeros(num), np.zeros(num), np.zeros(num), np.zeros(num), np.zeros(num), np.zeros(num), np.zeros(num) # Version 1.1!
-        
-#     # Produce numpy arrays for antenna longitudes, latitudes, and the coefficients of the field-rotation angle equations.
-#     for m in range(nant):
-#         lonarr[(ant == m)] = longarr[m]
-#         latarr[(ant == m)] = latiarr[m]
-#         elarr[(ant == m)] = f_el[m]
-#         pararr[(ant == m)] = f_par[m]
-#         phiarr[(ant == m)] = phi_off[m]
-    
-#     # Produce numpy arrays for sources RA and Dec.
-#     for l in range(len(source)):
-#         raarr[sourcearr == source[l]] = obsra[l]
-#         decarr[sourcearr == source[l]] = obsdec[l]
-#         yeararr[sourcearr == source[l]] = year[l]
-#         montharr[sourcearr == source[l]] = month[l]
-#         dayarr[sourcearr == source[l]] = day[l]
-        
-#     latarr, decarr = np.radians(latarr), np.radians(decarr)
-
-    
-#     hour = np.floor(time)
-#     minute = np.floor((time - hour) * 60.)
-#     second = (time - hour - minute / 60.) * 3600.
-    
-#     for i in range(100):
-#         dayarr[hour>=24.] += 1. # Version 1.1!
-#         hour[hour>=24.] -= 24. # Version 1.1!
-        
-#     # Convert UTC to GST using astropy Time.
-# #        dumt = at.Time(["{:04d}-{:02d}-{:02d}T{:02d}:{:02d}:{:f}".format(self.year, self.month, self.day+int(dt), int(hr), int(mn), sec) for dt, hr, mn, sec in zip(date, hour, minute, second)])
-    
-#     dumt = at.Time(["{:04d}-{:02d}-{:02d}T{:02d}:{:02d}:{:f}".format(int(yr), int(mo), int(dt), int(hr), int(mn), sec) for yr, mo, dt, hr, mn, sec in zip(yeararr, montharr, dayarr, hour, minute, second)]) # Version 1.1!
-#     gst = dumt.sidereal_time('mean','greenwich').hour
-    
-    
-#     # Obtain field-rotation angles using the known equations.
-#     hangle = np.radians(gst * 15. + lonarr - raarr)        
-#     parang = np.arctan2((np.sin(hangle) * np.cos(latarr)), (np.sin(latarr) * np.cos(decarr) - np.cos(latarr) * np.sin(decarr) * np.cos(hangle)))        
-#     altitude = np.arcsin(np.sin(decarr) * np.sin(latarr) + np.cos(decarr) * np.cos(latarr) * np.cos(hangle))
-#     pang = elarr * altitude + pararr * parang + phiarr
-        
-    
-#     return pang
-    
-
-
 def coord(antname, antx, anty, antz):
     """
     Convert antenna positions from Cartesian to spherical coordinates using astropy.
     
     Returns:
         lists of antenna longitudes, latitudes, and heights.
     """      
@@ -404,20 +331,15 @@
         data.loc[:,"rrsigma"], data.loc[:,"llsigma"], data.loc[:,"rlsigma"], data.loc[:,"lrsigma"]
     
     data.loc[:,"rrphas_sigma"], data.loc[:,"llphas_sigma"], data.loc[:,"rlphas_sigma"], data.loc[:,"lrphas_sigma"] = \
         data.loc[:,"rrsigma"] / np.abs(data.loc[:,"rrreal"] + 1j*data.loc[:,"rrimag"]), \
         data.loc[:,"llsigma"] / np.abs(data.loc[:,"llreal"] + 1j*data.loc[:,"llimag"]), \
         data.loc[:,"rlsigma"] / np.abs(data.loc[:,"rlreal"] + 1j*data.loc[:,"rlimag"]), \
         data.loc[:,"lrsigma"] / np.abs(data.loc[:,"lrreal"] + 1j*data.loc[:,"lrimag"])
-        
-        # phaserror(data.loc[:,"rrreal"] + 1j*data.loc[:,"rrimag"], data.loc[:,"rrsigma"] + 1j*data.loc[:,"rrsigma"]), \
-        # phaserror(data.loc[:,"llreal"] + 1j*data.loc[:,"llimag"], data.loc[:,"llsigma"] + 1j*data.loc[:,"llsigma"]), \
-        # phaserror(data.loc[:,"rlreal"] + 1j*data.loc[:,"rlimag"], data.loc[:,"rlsigma"] + 1j*data.loc[:,"rlsigma"]), \
-        # phaserror(data.loc[:,"lrreal"] + 1j*data.loc[:,"lrimag"], data.loc[:,"lrsigma"] + 1j*data.loc[:,"lrsigma"])
-        
+
     
     dumrl, dumlr = data.loc[:,"rlreal"] + 1j*data.loc[:,"rlimag"], data.loc[:,"lrreal"] + 1j*data.loc[:,"lrimag"]
     dumrlsigma, dumlrsigma = data.loc[:,"rlsigma"] + 1j*data.loc[:,"rlsigma"], data.loc[:,"lrsigma"] + 1j*data.loc[:,"lrsigma"]
     
     dumq, dumu = (dumrl + dumlr) / 2., -1j * (dumrl - dumlr) / 2.
     dumqsigma, dumusigma = np.sqrt(dumrlsigma**2 + dumlrsigma**2) / 2., np.sqrt(dumrlsigma**2 + dumlrsigma**2) / 2.
     
@@ -436,23 +358,14 @@
 
 def get_model(data, direc, dataname, calsour, polcal_unpol, ifnum, pol_IF_combine, outputname = None, selfcal = False):
     """
     Extract Stokes Q and U visibility models and append them to the pandas dataframe.
     
     """
     
-    # self.logger.info('\nGetting source polarization models for {:d} sources for {:d} IFs...'.format(len(self.polcalsour), self.ifnum))
-        
-    # AIPS.userno = self.aips_userno
-    
-    # if self.aipslog:
-    #     AIPS.log = open(self.logfile, 'a')
-    # AIPSTask.msgkill = -1
-            
-    
     mod_qrealarr, mod_qimagarr, mod_urealarr, mod_uimagarr = [], [], [], []
     
     
     for l in range(len(calsour)):
     
         inname = str(calsour[l])
     
@@ -488,26 +401,15 @@
                     qmap.zap()
 
                 if pol_IF_combine:
                     fitsname = direc+dataname+calsour[l]+'.allIF.q.fits'
                 else:
                     fitsname = direc+dataname+calsour[l]+'.IF'+str(k+1)+'.q.fits'
                 
-                
-                # if not path.exists(fitsname):
-                #     dum = 0
-                #     calib = WAIPSUVData(inname, 'EDIT', 1, 1)
-                #     for visibility in calib:
-                #         if((visibility.visibility[k,0,0,2] > 0) & (visibility.visibility[k,0,1,2] > 0) & (visibility.visibility[k,0,2,2] > 0) & (visibility.visibility[k,0,3,2] > 0)):
-                #             dum += 1 
-    
-                #     mod_qrealarr = mod_qrealarr + [0.] * dum
-                #     mod_qimagarr = mod_qimagarr + [0.] * dum
-                    
-                #     calib = AIPSUVData(inname, 'EDIT', 1, 1)
+
                 if not path.exists(fitsname):
                     raise Exception("The requested {:} file does not exist!".format(fitsname))
                     
                 else:
                     
                     au.runfitld(inname, 'QMAP', fitsname)
                     qmap = AIPSImage(inname, 'QMAP', 1, 1)
```

### Comparing `gpcal-0.9.5.5/gpcal/channelcal.py` & `gpcal-0.9.5.6/gpcal/channelcal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,31 @@
 
-
-import sys, os
+import os
 from os import path
 
 import pandas as pd
 import numpy as np
-from numpy.linalg import inv
 
-import timeit
 import logging
 import copy
 import glob
 
 from AIPS import AIPS
-from AIPSTask import AIPSTask
 from AIPSData import AIPSUVData, AIPSImage
 from Wizardry.AIPSData import AIPSUVData as WAIPSUVData
 
-from astropy.coordinates import EarthLocation
-import astropy.time as at
-
-from scipy.optimize import curve_fit
-
-import matplotlib
-matplotlib.use('Agg')
-import matplotlib.pyplot as plt
-
 import aipsutil as au
 import obshelpers as oh
 import cleanhelpers as ch
-import plothelpers as ph
 import polsolver as ps
 
 import gc
-import psutil
-
-from astropy.io import fits
 
-from multiprocessing import cpu_count, Pool
+from multiprocessing import Pool
 
-from IPython import embed
-        
     
 class channelcal(object):
     """
     This is a class to calibrate instrumental polarization in VLBI data and produce D-term corrected UVFITS files.
     
     Attributes:
         aips_userno (int): AIPS user ID for ParselTongue
```

### Comparing `gpcal-0.9.5.5/gpcal/gpcal.py` & `gpcal-0.9.5.6/gpcal/gpcal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,49 +1,37 @@
 
 import sys, os
 from os import path
 
 import pandas as pd
 import numpy as np
-from numpy.linalg import inv
 
 import timeit
 import logging
 import copy
-import glob
 
 from AIPS import AIPS
 from AIPSTask import AIPSTask
 from AIPSData import AIPSUVData, AIPSImage
 from Wizardry.AIPSData import AIPSUVData as WAIPSUVData
 
-from astropy.coordinates import EarthLocation
-import astropy.time as at
 
 from scipy.optimize import curve_fit
 
 import matplotlib
-matplotlib.use('Agg')
 import matplotlib.pyplot as plt
 
 import aipsutil as au
 import obshelpers as oh
 import cleanhelpers as ch
 import plothelpers as ph
 import polsolver as ps
 
-import gc
-import psutil
+from multiprocessing import Pool
 
-from astropy.io import fits
-
-from multiprocessing import cpu_count, Pool
-
-from IPython import embed
-        
 
 # Default matplotlib parameters
 plt.rc('font', size=21)
 matplotlib.rc('font', family='Dejavu Sans')
 matplotlib.rc('font', serif='Helvetica Neue')
 plt.rc('text', usetex=True)
 plt.rc('xtick', labelsize=18)
```

### Comparing `gpcal-0.9.5.5/gpcal/plothelpers.py` & `gpcal-0.9.5.6/gpcal/plothelpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 import matplotlib
 import matplotlib.pyplot as plt
 
 import obshelpers as oh
 
 from multiprocessing import Pool
 
-from IPython import embed
-
 
 # Default matplotlib parameters
 plt.rc('font', size=21)
 matplotlib.rc('font', family='Dejavu Sans')
 matplotlib.rc('font', serif='Helvetica Neue')
 plt.rc('text', usetex=True)
 plt.rc('xtick', labelsize=18)
```

