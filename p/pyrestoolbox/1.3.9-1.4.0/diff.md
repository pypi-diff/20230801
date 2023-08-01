# Comparing `tmp/pyrestoolbox-1.3.9.tar.gz` & `tmp/pyrestoolbox-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrestoolbox-1.3.9.tar", last modified: Tue Jun 20 05:19:10 2023, max compression
+gzip compressed data, was "pyrestoolbox-1.4.0.tar", last modified: Tue Aug  1 08:53:07 2023, max compression
```

## Comparing `pyrestoolbox-1.3.9.tar` & `pyrestoolbox-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 05:19:10.725211 pyrestoolbox-1.3.9/
--rw-rw-rw-   0        0        0    33092 2021-12-19 10:23:37.000000 pyrestoolbox-1.3.9/LICENSE
--rw-rw-rw-   0        0        0       37 2022-01-30 04:13:11.000000 pyrestoolbox-1.3.9/MANIFEST.in
--rw-rw-rw-   0        0        0     5313 2023-06-20 05:19:10.726212 pyrestoolbox-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0    19717 2023-06-20 05:17:25.000000 pyrestoolbox-1.3.9/README.rst
--rw-rw-rw-   0        0        0      121 2022-01-07 02:09:05.000000 pyrestoolbox-1.3.9/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-20 05:19:10.711213 pyrestoolbox-1.3.9/pyrestoolbox/
--rw-rw-rw-   0        0        0        0 2022-01-07 01:15:07.000000 pyrestoolbox-1.3.9/pyrestoolbox/__init__.py
--rw-rw-rw-   0        0        0    41658 2022-01-30 01:52:14.000000 pyrestoolbox-1.3.9/pyrestoolbox/component_library.xlsx
--rw-rw-rw-   0        0        0   122791 2023-06-20 01:59:12.000000 pyrestoolbox-1.3.9/pyrestoolbox/pyrestoolbox.py
-drwxrwxrwx   0        0        0        0 2023-06-20 05:19:10.723243 pyrestoolbox-1.3.9/pyrestoolbox/simtools/
--rw-rw-rw-   0        0        0        0 2022-01-07 01:15:07.000000 pyrestoolbox-1.3.9/pyrestoolbox/simtools/__init__.py
--rw-rw-rw-   0        0        0    37326 2022-04-19 07:29:27.000000 pyrestoolbox-1.3.9/pyrestoolbox/simtools/simtools.py
-drwxrwxrwx   0        0        0        0 2023-06-20 05:19:10.719210 pyrestoolbox-1.3.9/pyrestoolbox.egg-info/
--rw-rw-rw-   0        0        0     5313 2023-06-20 05:19:10.000000 pyrestoolbox-1.3.9/pyrestoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2023-06-20 05:19:10.000000 pyrestoolbox-1.3.9/pyrestoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 05:19:10.000000 pyrestoolbox-1.3.9/pyrestoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-20 05:19:10.000000 pyrestoolbox-1.3.9/pyrestoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-20 05:19:10.000000 pyrestoolbox-1.3.9/pyrestoolbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      635 2023-06-20 05:19:10.727213 pyrestoolbox-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1205 2023-06-20 05:18:54.000000 pyrestoolbox-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:53:07.344916 pyrestoolbox-1.4.0/
+-rw-rw-rw-   0        0        0    33092 2021-12-19 10:23:37.000000 pyrestoolbox-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0       37 2022-01-30 04:13:11.000000 pyrestoolbox-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5663 2023-08-01 08:53:07.344916 pyrestoolbox-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    20319 2023-08-01 08:10:22.000000 pyrestoolbox-1.4.0/README.rst
+-rw-rw-rw-   0        0        0      121 2022-01-07 02:09:05.000000 pyrestoolbox-1.4.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-01 08:53:07.331912 pyrestoolbox-1.4.0/pyrestoolbox/
+-rw-rw-rw-   0        0        0        0 2022-01-07 01:15:07.000000 pyrestoolbox-1.4.0/pyrestoolbox/__init__.py
+-rw-rw-rw-   0        0        0    41658 2022-01-30 01:52:14.000000 pyrestoolbox-1.4.0/pyrestoolbox/component_library.xlsx
+-rw-rw-rw-   0        0        0   165393 2023-08-01 08:40:42.000000 pyrestoolbox-1.4.0/pyrestoolbox/pyrestoolbox.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:53:07.342914 pyrestoolbox-1.4.0/pyrestoolbox/simtools/
+-rw-rw-rw-   0        0        0        0 2022-01-07 01:15:07.000000 pyrestoolbox-1.4.0/pyrestoolbox/simtools/__init__.py
+-rw-rw-rw-   0        0        0    37326 2022-04-19 07:29:27.000000 pyrestoolbox-1.4.0/pyrestoolbox/simtools/simtools.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:53:07.339912 pyrestoolbox-1.4.0/pyrestoolbox.egg-info/
+-rw-rw-rw-   0        0        0     5663 2023-08-01 08:53:07.000000 pyrestoolbox-1.4.0/pyrestoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2023-08-01 08:53:07.000000 pyrestoolbox-1.4.0/pyrestoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:53:07.000000 pyrestoolbox-1.4.0/pyrestoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-01 08:53:07.000000 pyrestoolbox-1.4.0/pyrestoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-01 08:53:07.000000 pyrestoolbox-1.4.0/pyrestoolbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      635 2023-08-01 08:53:07.345923 pyrestoolbox-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1205 2023-08-01 08:06:36.000000 pyrestoolbox-1.4.0/setup.py
```

### Comparing `pyrestoolbox-1.3.9/LICENSE` & `pyrestoolbox-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrestoolbox-1.3.9/PKG-INFO` & `pyrestoolbox-1.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pyrestoolbox
-Version: 1.3.9
+Version: 1.4.0
 Summary: pyResToolbox - A collection of Reservoir Engineering Utilities
 Home-page: https://github.com/mwburgoyne/pyResToolbox
 Author: Mark W. Burgoyne
 Author-email: mark.w.burgoyne@gmail.com
 Keywords: restoolbox,petroleum,reservoir
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 `pyrestoolbox`
 ==============
 
-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\--A collection of
-Reservoir Engineering Utilities
+\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\--
+A collection of Reservoir Engineering Utilities
 \-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\--
 
 This set of functions focuses on those that the author uses often while
 crafting programming solutions. These are the scripts that are often
 copy/pasted from previous work - sometimes slightly modified - resulting
 in a trail of slightly different versions over the years. Some attempt
 has been made here to make this implementation flexible enough such that
@@ -36,17 +36,22 @@
 -   Creation of layered permeability distribution consistent with a
     Lorenze heterogeneity factor
 -   Extract problem cells information from Intesect (IX) print files
 -   Generation of AQUTAB include file influence functions for use in
     ECLIPSE
 -   Creation of Corey and LET relative permeability tables in Eclipse
     format
+-   Calculation of Methane and CO2 saturated brine properties
 
 Apologies in advance that it is only in oilfield
-units with no current plans to add multi-unit support.
+units with no current plans to add universal multi-unit support.
+
+Changelist in 1.4.0:
+- Introduced CO2 saturated brine calculations using Spycher & Pruess modified SRK EOS method
+- Rectified an error introduced in Gas Z-Factor calculations due to errant indentation
 
 Changelist in 1.3.9:
 - Tweaks to speed DAK and Hall & Yarborough Z-Factor calculations
 
 Changelist in 1.3.8:
 - Fix bug in Hall & Yarborough Z-Factor calculation
 
@@ -118,15 +123,16 @@
 -   Generate Black Oil Table data              
 -   Estimate soln gas SG from oil                
 -   Estimate SG of gas post separator               
 -   Calculate weighted average surface gas SG  
 -   Oil API to SG              
 -   Oil SG to API
 ----------------------------
--   Calculate suite of brine properties        
+-   Calculate suite of methane saturated brine properties  
+-   Calculate suite of CO2 saturated brine properties   
 ----------------------------
 -   Lorenz coefficient from Beta value                   
 -   Lorenz coefficient from flow fraction                
 -   Lorenz coefficient to flow fraction                
 -   Lorenz coefficient to permeability array      
 ----------------------------
 -   Summarize IX convergence errors from PRT file
```

### Comparing `pyrestoolbox-1.3.9/README.rst` & `pyrestoolbox-1.4.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,21 @@
 - PVT calculation for gas
 - Return critical parameters for typical components
 - Creation of Black Oil Table information
 - Creation of layered permeability distribution consistent with a Lorenze heterogeneity factor
 - Extract problem cells information from Intesect (IX) print files
 - Generation of AQUTAB include file influence functions for use in ECLIPSE
 - Creation of Corey and LET relative permeability tables in Eclipse format
+- Calculation of Methane and CO2 saturated brine properties
+
+
+Changelist in 1.4.0:
+
+- Introduced CO2 saturated brine calculations using Spycher & Pruess modified SRK EOS method
+- Rectified an error introduced in Gas Z-Factor calculations due to errant indentation
 
 Changelist in 1.3.9:
 
 - Tweaks to speed DAK and Hall & Yarborough Z-Factor calculations
 
 Changelist in 1.3.8:
 
@@ -109,15 +116,17 @@
 |                                                                                                    | - Generate Black Oil Table data                                 |
 |                                                                                                    | - Estimate soln gas SG from oil                                 |
 |                                                                                                    | - Estimate SG of gas post separator                             |
 |                                                                                                    | - Calculate weighted average surface gas SG                     |
 |                                                                                                    | - Oil API to SG                                                 |
 |                                                                                                    | - Oil SG to API                                                 |
 +----------------------------------------------------------------------------------------------------+-----------------------------------------------------------------+
-| `Brine PVT <https://github.com/mwburgoyne/pyResToolbox/blob/main/docs/water.rst>`_                 | - Calculate suite of brine properties                           |
+| `CH4 Saturated Brine PVT <https://github.com/mwburgoyne/pyResToolbox/blob/main/docs/water.rst>`_   | - Calculate suite of methane saturated brine properties         |
++----------------------------------------------------------------------------------------------------+-----------------------------------------------------------------+
+| `CO2 Saturated Brine PVT <https://github.com/mwburgoyne/pyResToolbox/blob/main/docs/brineco2.rst>`_| - Calculate suite of CO2 saturated brine properties             |
 +----------------------------------------------------------------------------------------------------+-----------------------------------------------------------------+
 | `Permeability Layering <https://github.com/mwburgoyne/pyResToolbox/blob/main/docs/layer.rst>`_     | - Lorenz coefficient from Beta value                            |
 |                                                                                                    | - Lorenz coefficient from flow fraction                         |
 |                                                                                                    | - Lorenz coefficient to flow fraction                           |
 |                                                                                                    | - Lorenz coefficient to permeability array                      |
 +----------------------------------------------------------------------------------------------------+-----------------------------------------------------------------+
 | `Simulation Helpers <https://github.com/mwburgoyne/pyResToolbox/blob/main/docs/sim.rst>`_          | - Summarize IX convergence errors from PRT file                 |
```

### Comparing `pyrestoolbox-1.3.9/pyrestoolbox/component_library.xlsx` & `pyrestoolbox-1.4.0/pyrestoolbox/component_library.xlsx`

 * *Files identical despite different names*

### Comparing `pyrestoolbox-1.3.9/pyrestoolbox/pyrestoolbox.py` & `pyrestoolbox-1.4.0/pyrestoolbox/pyrestoolbox.py`

 * *Files 18% similar despite different names*

```diff
@@ -596,35 +596,76 @@
         
         tr2, tr3 = tr**2, tr**3
         a = np.array([0,0.3265,-1.07,-0.5339,0.01569,-0.05165,0.5475,-0.7361,0.1844,0.1056,0.6134,0.7210])
         c1 = a[1]+(a[2]/tr) + (a[3]/tr3) + (a[4]/tr**4) + (a[5]/tr**5)
         c2 = a[6] + (a[7]/tr) + (a[8]/tr2)
         c3 = a[9] * ((a[7]/tr) + (a[8]/tr2))
     
+        # Unpublished empirical fit of reduced pressure at minimum DAK-Z as a function of 
+        # reduced Temperature over Tpr range 1.03 - 4.0
+        # By Mark Burgoyne, July 2023
+        def min_ppr(tpr): #  N. 127:   Y = A/X+B*EXP(C*X)+D <-- Hyp + exp + c
+            if tpr > 3.43:
+                return 0.0
+            if tpr < 1.03:
+                return 1.2625075898234461
+            A, B, C, D = 0.2283E+02, -.1359E+03, -.2188E+01, -.6614E+01
+            minppr = A/tpr+B*np.exp(C*tpr)+D
+            return minppr
+            
+        # Unpublished empirical fit of minimum DAK-Z values as a function of 
+        # reduced Temperature over Tpr range 1.03 - 4.0
+        # By Mark Burgoyne, July 2023
+        def fit_minz(tpr): # N. 149:   Y = (A+X)/(B+C*X**2)+D <--- Straight line / parabola + c
+            if tpr > 3.43:
+                return 1.0
+            A, B, C, D = -.1556E+01, 0.8930E-01, 0.8043E+00, 0.8019E+00
+            minzs = (A+tpr)/(B+C*tpr**2)+D 
+            return minzs
+    
         def new_dak_z(z, pr, tr):
             rhor = 0.27 * pr / (tr * z)  # 2.8
             c4 = a[10] * (1 + a[11] * rhor**2) * (rhor**2/tr3) * np.exp(-a[11] * rhor**2)
             err = fz(z, rhor, c4)
             return z - err/fz_prime(z, rhor, c4), err # Returns updated guess for Z, as well as the error
         
         def fz(z, rhor, c4):                          # The DAK Error function
             return z - (1 + c1*rhor + c2*rhor**2 - c3 * rhor**5 + c4)
     
         def fz_prime(z, rhor, c4):                    # Derivative of the DAK Error function
             return 1 + c1*rhor/z + (2*c2*rhor**2/z) - (5*c3*rhor**5/z) + 2*a[10]*rhor**2/(z*tr3)*(1+a[11]*rhor**2 - (a[11]*rhor**2)**2)*np.exp(-a[11]*rhor**2)
-    
+        
+        def z_err(z, *args):
+            pr = args[0]
+            rhor = 0.27 * pr / (tr * z)  # 2.8
+            c4 = a[10] * (1 + a[11] * rhor**2) * (rhor**2/tr3) * np.exp(-a[11] * rhor**2)
+            z2 = (1 + c1*rhor + c2*rhor**2 - c3 * rhor**5 + c4)
+            return z2 - z        
+            
         def z_dak_calc(pr, tr, tol = 1e-6):
             niter = 0
-            midz = min(max(0.1, z_wyw(pr, tr)),3) # First guess using explict calculation method
-            mid_err = 1
-            while abs(mid_err) > tol and niter < 100:
-                midz, mid_err = new_dak_z(midz, pr, tr)
-                niter += 1
+            minppr = min_ppr(tr)
+            
+            if abs(pr - minppr) > 0.05: # If Ppr is further from calculated minimum Ppr than 0.05, use Netwon solver
+                newton_solve = True
+            else:
+                newton_solve = False    # Else, use bisection solver, and setup Z bounds to search within
+                minz = fit_minz(tr)
+                bounds = (minz - 0.02, minz + 0.02)
+    
+            if newton_solve:
+                midz = min(max(0.1, z_wyw(pr, tr)),3) # First guess using explict calculation method
+                mid_err = 1
+                while abs(mid_err) > tol and niter < 100:
+                    midz, mid_err = new_dak_z(midz, pr, tr)
+                    niter += 1
+            else:
+                midz = brentq(z_err, bounds[0], bounds[1], args=(pr))  
             return midz
-
+        
         zout = [z_dak_calc(pr, tr) for pr in pprs]
             
         if single_p:
             return zout[0]
         else:
             return np.array(zout)
 
@@ -671,15 +712,14 @@
         zs = numerators/denominators
 
         if single_p:
             return float(zs)
         else:
             return zs
 
-
     zfuncs = {"DAK": zdak, "HY": z_hy, "WYW": z_wyw}
 
     return zfuncs[zmethod.name](pprs, tr)
 
 
 def gas_ug(
     p: npt.ArrayLike,
@@ -2974,19 +3014,19 @@
     b_coefic = [0, -0.03602, 0.18917, 0.97242, 0, 0]
     c_coefic = [0, 0.6855, -3.1992, -3.7968, 0.07711, 0.2229]
 
     A_t = Eq41(degc, a_coefic)
     B_t = Eq41(degc, b_coefic)
     C_t = Eq41(degc, c_coefic)
 
-    mch4w = np.exp(
-        A_t * np.power(np.log(Mpa - vap_pressure), 2)
-        + B_t * np.log(Mpa - vap_pressure)
-        + C_t
-    )  # Eq 4.15
+    try:
+        mch4w = np.exp(A_t * np.power(np.log(Mpa - vap_pressure), 2) + B_t * np.log(Mpa - vap_pressure) + C_t)  # Eq 4.15
+    except:
+        mch4w = 0
+    
     u_arr = [
         0,
         8.3143711,
         -7.2772168e-4,
         2.1489858e3,
         -1.4019672e-5,
         -6.6743449e5,
@@ -3073,14 +3113,21 @@
     vb0_sc = (
         1 / Rhob_scm
     )  # vb0 at standard conditions - (Calculated by evaluating vbo at 0.1013 MPa and 15 degC)
     Bw = (((1000 + m * 58.4428) * vb0) + (mch4 * Vmch4b)) / (
         (1000 + m * 58.4428) * vb0_sc
     )
 
+    # m =  Molar concentration of NaCl from wt % in gram mol/kg water
+    # mch4b = Methane solubility in brine (g-mol/kg H2O)
+    # mch4 = Fraction of saturated methane solubility
+    # Vmch4b = 
+
+
+
     zee_sc = gas_z(p=psc, sg=0.5537, degf=tscf)
     vmch4g_sc = zee_sc * 8.314467 * (273 + 15) / 0.1013  # Eq 4.34
     rsw_new = mch4 * vmch4g_sc / ((1000 + m * 58.4428) * vb0_sc)
     rsw_new_oilfield = rsw_new / 0.1781076  # Convert to scf/stb
 
     d = [
         0,
@@ -3415,9 +3462,819 @@
             return 'Property not in Library'
         if prop in [x.upper() for x in self.all_cols]:
             return self.all_dics[prop][comp]
         if prop in [x.upper() for x in self.model_cols]:
             return dic[prop][comp]
         return 'Component or Property not in library'
 
-
 comp_library = component_library()
+
+# CO2:Brine Library coded by Mark Burgoyne, July 2023
+# Leveraging some translated SRK code snippets from VBA supplied by Steve Furnival
+
+#import warnings
+#warnings.filterwarnings("error")
+
+EPS = 0.000001
+
+#--Unit Conversion Constants--------------------------------------------
+BAR2PSI = 14.5037738
+RGASCON = 83.1447      #--Units of bar.cm3/(mol.K)
+CEL2KEL = 273.15
+CONMOLA = 55.508       #--1000/Mw-Water [Molality Conversion Factor]
+PPM2MFR = 0.000001
+
+PSTND = 1.01325        #--Standard Pressure (bar)
+TSTND = 288.706        #--Standard Temperature (Kelvin)
+  
+#--Mole Weights & Densities at Standard Conditions----------------------
+MWSAL = 58.44          #--Mole Weight of Salt (NaCl)
+MWWAT = 18.02          #--Mole Weight of Pure Water
+MWCO2 = 44.01          #--Mole Weight of CO2
+  
+VMCO2S = 23690.5       #--Molar Volume of CO2 at STP [cm3/gmol]
+RHOCO2S = 0.00185771   #--Density CO2 at STP [gm/cm3]
+
+#============================================================================
+#    ***  Mutual solubilities between CO2 and Brine - Calculated with  ***
+#  A Phase-Partitioning Model for CO2–Brine Mixtures at Elevated Temperatures 
+#  and Pressures: Application to CO2-Enhanced Geothermal Systems
+#  Nicolas Spycher & Karsten Pruess, Transp Porous Med (2010) 82:173–196
+#  DOI 10.1007/s11242-009-9425-y
+#============================================================================
+
+#===================================================================================================================
+#  ***  Base Brine properties calculated using Spycher calculated xCO2. Additional calculations via the following ***
+#Property                       Source
+#-----------------------------  --------------------------------------------------------------------------------------------
+#Pure Brine Density             Spivey et al. (modified),
+#                               per "Petroleum Reservoir Fluid Property Correlations", (McCain, Spivey & Lenn: Chapter 4)
+#CO2 Corrected Brine Density    Molar volume of dissolved CO2 estimated with Garcia (2001) equation, used with xCO2 calculated 
+#                               from Spycher & Pruess, and CO2-free brine density from Spivey et al to calculate insitu density
+#Pure Brine viscosity           Mao-Duan (2009) approach for pure brine viscosity
+#CO2 Corrected Brine Viscosity  Used approach from "Viscosity Models and Effects of Dissolved CO2", Islam-Carlson (2012)
+#                               to adjust the pure brine viscosity for xCO2 calculated from Spycher & Pruess
+#===================================================================================================================
+
+class CO2_Brine_Mixture():
+    """ Calculates CO2 saturated Brine mutual solubilities and brine properties
+    
+            Inputs:
+                pres: Pressure (Bar / psia)
+                temp: Temperature (deg C / deg F)
+                ppm: NaCL equivalent weight concentration in brine in parts per million (10,000ppm = 1% by weight) (default zero)
+                metric: Boolean operator that determines units assumed for input, and return calculated (default True)
+    
+            Returns object with following calculated properties:
+                .x       : Mole fractions of CO2 and H2O in aqueous phase [xCO2, xH2O]
+                .y       : Mole fractions of CO2 and H2O in vapor phase [yCO2, yH2O]
+                .xSalt   : Mole fraction of NaCl in brine
+                .rhoGas  : CO2 rich gas density (gm/cm3)
+                .bDen    : Brine density (gm/cm3) [CO2 Saturated, Pure Brine]
+                .bVis    : Brine viscosity (cP)   [CO2 Saturated, Pure Brine]
+                .bVisblty: CO2 Saturated brine viscosibility (1/Bar or 1/psi)
+                .bw      : Brine formation volume factor (rm3/smr / rb/stb) [CO2 Saturated, Pure Brine]
+                .Rs      : CO2 Saturated Brine solution gas ratio (sm3/sm3 or scf/stb)
+                .Cf_usat : Brine undersaturated compressibility (1/Bar or 1/psi)
+                
+            Usage example for 5000 psia x 275 deg F and 3% NaCl brine:
+                mix = rtb.CO2_Brine_Mixture(pres = 5000, temp = 275, ppm = 30000, metric = False)
+                mix.bw  # Returns [CO2 Saturated Brine Bw, Pure Brine Bw]
+                >> [1.1085535365828796, 1.0543051557116332]
+                
+            Usage example for 175 Bara x 85 degC and 0% NaCl brine:
+                mix = rtb.CO2_Brine_Mixture(pres = 175, temp = 85)
+                mix.Rs  # Returns sm3 dissolved CO2 / sm3 Brine
+                >> 24.502168045494223
+                
+    """
+    
+    def __init__(self, pres, temp, ppm = 0, metric = True):
+        self.metric = metric              # Units. FIELD or METRIC
+        self.ppm = ppm                    # Parts per million (wt fraction) NaCl in brine
+        self.tKel = None                  # Deg K
+        self.P0 = None                    # Standard pressure (Bar)
+        self.fugPi = [None, None]         # Fugacity * Pressure for species i
+        self.K = [None, None]             # yi/xi at reservoir pressure
+        self.gamma_prime = None
+        self.gamma = ([1, 1])
+        self.pRT = None                   # P/RT
+        self.pRT0 = None                  # (P - P0)/RT
+        self.y = np.array([1.0, 0.0])     # Mole fraction split CO2 and H2O in vapor phase
+        self.x = np.array([0.0, 1.0])     # Mole fraction split CO2 and H2O in aqueous phase
+        self.A = None
+        self.Bprime = None
+        self.xSalt = None                 # Mole fraction salt in aqueous mixture
+        self.molaL = None                 #--Brine Molality (gmol/kg)
+        self.MolarVol = np.array([0.0, 0.0])  #--Molar Volumes from RK-EOS (cm3/gmol)
+        self.GASZ = None                  # Vapor phase Z-Factor
+        self.MwGas = None                 #--Mole weight  [gm/gmol]
+        self.MwBrine = None               #--Mole weight of CO2 free brine (gm/gmol)
+        self.rhoGas = None                #--Density of Gas Mixture (gm/cm3)
+        self.Amix = None                  # RK-EOS A_mix parameter
+        self.aij = None                   # RK-EOS aij
+        self.kij = None                   # RK-EOS kij
+        self.bMix = None                  # RK-EOS B_mix parameter
+        self.b = None                     # RK-EOS bij
+        self.vBar = [0, 0]                # Avg partial molar volume of pure condensed phase over the pressure interval P0 to pBar
+        self.bDen = None                  # CO2 laden Brine density (gm/cm3) [CO2 Saturated, CO2 Free]
+        self.bVis = None                  # Brine viscosity (cP)  [CO2 Saturated, CO2 Free]
+        self.bVisblty = None              # CO2 laden viscosibility (1/Bar or 1/psi) (at pressures above Psat)
+        self.bw = None                    # Brine formation volume factor (res vol/std vol) [CO2 Saturated, CO2 Free]
+        self.Rs = None                    # Solution gwr CO2 (sm3/sm3 or scf/stb brine)
+        self.Cf_usat = None               # Undersaturated brine compressibility (1/Bar or 1/psi)
+        self.CO2_sat = False              # Flag to determine if in P-T range for saturated liquid CO2 K values
+        
+        if self.metric:
+            self.pBar = pres              # Pressure (Bar)
+            self.degC = temp              # Deg C
+        else:
+            self.pBar = pres/14.5038      # Pressure (psia -> Bar)
+            self.degC = (temp - 32)/1.8   # Temperature (degF -> deg C)
+        self.tKel = self.degC + CEL2KEL
+        
+        if self.degC <= 31:
+            # Below saturated CO2 pressure equation emprically fit to data at https://www.ohio.edu/mechanical/thermo/property_tables/CO2/CO2_TempSat1.html
+            #if self.pBar >= 10**-15.90106469 * self.tKel**7.157992919: # Above CO2 Psat 
+            if self.pBar >= 26.481*self.degC**0.2827: # Alternate fit to discontinuity peak seen in calculated xCO2 at low temperatures
+                self.CO2_sat = True
+
+
+        self.co2BrineSolubility()         # Calculate mutual solubilities
+        self.brine()                      # Calculate Brine properties            
+        
+    def calc_type(self):
+        # == Figure out which calculation method to employ ==========================
+        # deg C <= 99: Non-iterative solution employed assuming negligible xCO2 for mixing rules
+        # deg C > 109: An iterative solution is employed with more robust mixing rules application
+        # 99 < deg C < 109: An iterative solution is employed. Partitioning factors and fugacity coefficients are blended between low temp and high temp relationships.
+        self.low_temp = True      # Use the simple approach for temp < 99 deg C
+        self.scaled = False       # No blending
+        if self.degC > 99 and self.degC <= 109:
+            self.low_temp = False # Use the iteretaive robust approach
+            self.scaled = True    # Also use the simpler < 99 degC approach for equilibrium factors and fugacities and scale the result
+        elif self.degC > 109:
+            self.low_temp = False # Only perform the more robust > 99 degC approach
+            self.scaled = False
+
+    # Vapor pressure of water with Buck equation
+    # https://en.wikipedia.org/wiki/Arden_Buck_equation
+    def water_vap_p(self):
+        kpa = 0.61121 * np.exp((18.678 - (self.degC/234.5))*(self.degC/(257.14+self.degC)))
+        return 0.145038 * kpa # Convert to psia
+        
+    def FT(self, t, x):                                       # Spycher Equation 6
+        return sum([x[i]*t**i for i in range(len(x))])
+    
+    # Initial estimate for yH2O in saturated Brine / CO2 system
+    # Unpublished empirical fit by Mark Burgoyne (Jul 2023) against data generated with modified Whitson PR-EOS method
+    def est_yH2O(self):
+        # Slope and intercept of ppH20/PPatm - 1 = slope * psia + intercept
+        # Slope as function of deg F
+        # Y = (A+B*X)**C+D <--- Bleasdale (Shifted power) + c
+        A, B, C, D = 0.1939E+01, 0.8913E-02, -.4844E+01, 0.2551E-03
+        degf = self.degC * 1.8 + 32
+        p = self.pBar * 14.5038
+        slope = (A+B*degf)**C+D
+        
+        # Intercept as a function of degF
+        # Y = -1/(A+B*X**2)**C <--- Inv pow
+        A, B, C = 0.3097E+00, 0.9136E-05, 0.1719E+01
+        intcpt = -1/(A+B*degf**2)**C
+        
+        pp_ratio = slope*p + intcpt + 1.0
+        atm_pvap = self.water_vap_p()
+        pp = pp_ratio * atm_pvap          # Partial pressure of water (yH2O * Pressure)
+        if pp < atm_pvap:
+            pp = atm_pvap
+        return max(min(pp/p, 1-EPS),0)
+        
+    def ppm2Molality(self):
+    #=======================================================================
+    #  Whitson & Brule, SPE Phase Behaviour Monograph, Equation (9.2c)
+    #=======================================================================
+        ppm = max(EPS, self.ppm) #--Ensure no divide by Zero 
+        return 17.1 / (1000000 / ppm - 1.0)
+    
+    def blended_val(self, low_val, high_val): # Blends results between 99 - 109 deg C
+        return ((self.degC - 99) * low_val + (109 - self.degC) * high_val)/(109-99)
+        
+    def aCO2_RK(self):
+    #=======================================================================
+    #  a-Coefficient of CO2 for RK-EoS is Temperature Dependent
+    #  Delineating with low_temp flag to permit calculating low_temp relationship 
+    #  values between 99 - 109 deg C
+    #=======================================================================
+        if self.low_temp:
+            return self.FT(self.tKel, [7.54e7, -4.13e4])   # Low temperature relationship
+        return self.FT(self.tKel, [8.008e7, -4.984e4])     # High temperature relationship
+    
+    def aH2O_RK(self):
+    #=======================================================================
+    # a-Coefficient of H2O for RK-EoS is Temperature Dependent
+    # Only used for high temperature method
+    #=======================================================================
+        return self.FT(self.tKel, [1.337e8, -1.4e4])
+    
+    def gammaCO2(self):
+        # Equation 18 from Spycher 2010 paper (Gamma dash)
+    #=======================================================================
+    #  CO2 Activity Coefficients
+    #  Spycher, N., and Pruess, K.,
+    #  "A Phase-Partitioning Model for CO2-Brine Mixtures ..."
+    #  Transp Porous Med (2010), 82, pp. 173-196
+    #=======================================================================
+    
+        cL = [0.0002217, 1.074, 2648.0]
+        cZ = [0.000013, -20.12, 5259.0]
+      
+        #--(lamB,zetA) from Spycher & Pruess Equation (19) and Table 1---------------
+        lamB = cL[0] * self.tKel + cL[1] / self.tKel + cL[2] / self.tKel ** 2
+        zetA = cZ[0] * self.tKel + cZ[1] / self.tKel + cZ[2] / self.tKel ** 2
+      
+        #==Hassanzadeh Equation (12)============================================
+        self.gamma_prime = (1.0 + self.molaL / CONMOLA) * np.exp(self.molaL * (2.0 * lamB + self.molaL * zetA))
+    
+    
+    def aMix_RK(self):
+    #=======================================================================
+    #  a-Coefficient of CO2-H2O Mixture for RK-EoS
+    #=======================================================================
+        
+        # Setup Kij array    
+        K = np.zeros((2,2))
+        if not self.low_temp:  # Use high temp method
+            K[0][1] = self.FT(self.tKel, [0.4228, -7.422e-4])   # KCO2-H2O
+            K[1][0] = self.FT(self.tKel, [1.427e-2, -4.037e-4]) # KH2O-CO2
+        else:
+            K[0][1] = 7.89e7
+            K[1][0] = 7.89e7
+        
+        # Calculate kij array
+        k = np.zeros((2,2))
+        k[0][1] = (K[0][1] * self.y[0]) + (K[1][0] * self.y[1])  # Eq. A-6
+        k[1][0] = k[0][1]
+        
+        # Setup aij array
+        a = np.zeros((2,2))
+        a[0][0] = self.aCO2_RK()
+        a[1][1] = self.aH2O_RK()
+        if self.low_temp:
+            a[0][1] = 7.89e7
+            a[1][0] = a[0][1]
+        else:
+            for i in range(2):
+                j = 1 - i
+                a[i][j] = (a[i][i] * a[j][j])**0.5 *(1-k[i][j])  # Eq. A-5
+        amix = 0
+        for i in range(2):
+            for j in range(2):
+                amix += self.y[i]*self.y[j]*a[i][j]
+            
+        self.aMix = amix
+        self.aij = a
+        self.kij = k
+        
+    
+    def bMix_RK(self):
+    #=======================================================================
+    #  b-Coefficient of CO2-H2O Mixture for RK-EoS
+    #=======================================================================
+        if self.low_temp:
+            b = np.array([27.80, 18.18])
+        else:
+            b = np.array([28.25, 15.70])
+        self.bMix = np.dot(self.y, b)
+        self.b = b
+        
+    
+    def sgn(self, x):
+        # Duplicates the VBA sgn function
+        if x > 0:
+            return 1
+        elif x == 0:
+            return 0
+        else:
+            return -1
+    
+    def cubicSolver(self, e2, e1, e0):
+    #=======================================================================
+    #  Cubic Polynomial Solver: f(Z) = Z**3 + E2*Z**2 + E1*Z + E1 = 0
+    #=======================================================================
+        Z = [0,0,0]
+        Half = 0.5
+        Third = (1.0 / 3.0)
+      
+        #-- iType = -1 => Three Real Roots
+        #--       =  0 => Three Real Roots
+        #--          1 => One   Real Root
+      
+        #-- Some useful varaiables----------------------------------------------
+        B13 = e2 * Third
+        B23 = e1 * Third
+      
+        Q = B13 * B13 - B23
+        r = B13 * (Q - Half * B23) + e0 * Half
+      
+        R2Q3 = r * r - Q * Q * Q
+      
+        #== Sort Roots depending on value of R2Q3 ==============================
+    
+        if R2Q3 > 0:
+            iType = 1
+            QRT = (R2Q3**0.5 + abs(r)) ** Third
+            Z[0] = -self.sgn(r) * abs(QRT + Q / QRT) - B13
+            Z[2] = Z[0]
+        elif R2Q3 < 0:
+            iType = -1
+            QRT = Q**0.5
+            cosT = math.cos(Third * math.acos(r / (QRT * Q)))
+            Z[0] = -2.0 * QRT * cosT - B13
+            Z[2] = QRT * ((3.0 * (1.0 - cosT * cosT))**0.5 + cosT) - B13
+        else:
+            iType = 0
+            QRT = Q**0.5
+            if r >= 0:
+                Z[0] = -2.0 * QRT - B13
+                Z[2] = QRT - B13
+            else:
+                Z[0] = -QRT - B13
+                Z[2] = 2.0 * QRT - B13
+      
+        #== Ensure the smaller root is positive ================================
+        if Z[0] < 0:
+            Z[0] = Z[2]
+      
+        return iType, Z
+        
+    def MolarVolume(self):
+    #=======================================================================
+    #  Forms Coefficients of RK-EoS and Solves Cubic for Mixture Molar Volume
+    #=======================================================================
+    
+        RTp = RGASCON * self.tKel / self.pBar
+        aT12p = self.aMix / (self.pBar * self.tKel**0.5)
+    
+        #--Coefficients of the (RK) Cubic Eqn. A-2---------------------------------
+        e2 = -RTp                                   # Coeffic of V**2
+        e1 = aT12p - self.bMix * (RTp + self.bMix)  # Coeffic of V
+        e0 = -aT12p * self.bMix                     # Constant
+        
+        #--Solve the Cubic------------------------------------------------------
+        iType, cubV = self.cubicSolver(e2, e1, e0)
+      
+        if iType == 1:
+            gasMolarVol = cubV[0]    #--Only 1-Root
+        else:
+            if cubV[0] >= cubV[2]:   #--3-Real Roots: As Gas, Take Largest
+                gasMolarVol = cubV[0]
+            else:
+                gasMolarVol = cubV[2]
+        self.MolarVol = np.array([gasMolarVol, min(cubV)])
+
+        
+    def fugP(self):
+    #=======================================================================
+    #  Pressure * Fugacity Coefficient of CO2 or H2O in CO2-Water Mixture
+    #  k = 0 => CO2
+    #  k = 1 => H2O
+    #=======================================================================
+        x, y, kij, aMix, aij = self.x, self.y, self.kij, self.aMix, self.aij
+        bMix, b = self.bMix, self.b
+        vMol = self.MolarVol[0] # Always vapor molar volume
+        yCO2 = max(min(1,y[0]), 0)
+        xCO2 = max(min(1,x[0]), 0)
+        self.y = np.array([yCO2, 1.0-yCO2])
+        self.x = np.array([xCO2, 1.0-xCO2])
+        
+        for k in range(2):
+            
+            t1 = b[k] / bMix * (self.pRT * vMol - 1) 
+            t2 = -np.log(self.pRT * (vMol - bMix))
+            t3 = sum([y[i] * (aij[i][k] + aij[k][i]) for i in range(2)])
+            for i in range(2):
+                for j in range(2):
+                    t3 -= y[i]**2 * y[j] * (kij[i][j] - kij[j][i]) * (aij[i][i] * aij[j][j])**0.5
+            t3 += sum([x[k] * x[i] * (kij[k][i] - kij[i][k]) * (aij[i][i] * aij[k][k])**0.5 for i in range(2)])
+            t3 /= aMix
+            t3 -= b[k] / bMix
+            t4 = (aMix / (bMix * RGASCON * self.tKel ** 1.5)) * np.log(vMol / (vMol + bMix))
+         
+            #==CO2 Fugacity Coefficient=============================================
+            logPhi = t1 + t2 + t3 * t4  # Eq. A-8
+      
+            #==Pressure * Fugacity Coefficient=============================================
+            self.fugPi[k] = self.pBar * np.exp(logPhi)
+    
+    def Ktp(self, K0, Vbar):              # Equation 5
+        return K0 * np.exp(self.pRT0 * Vbar)
+    
+    def K_CO2(self): # Units: bar
+    #=======================================================================
+    #  CO2 K-value at reservoir Pressure
+    #=======================================================================
+        if self.low_temp:
+            x = [1.189, 1.304e-2, -5.446e-5]
+            if self.CO2_sat:
+                x = [1.169, 1.368e-2, -5.380e-5] # Liquid CO2 below 31 deg C and above CO2 Psat 
+        else:
+            x = [1.668, 3.992e-3, -1.156e-5, 1.593e-9]
+
+        K0 = 10**self.FT(self.degC, x)
+        
+        if self.scaled:
+            K0_lt = 10**self.FT(self.degC, [1.189, 1.304e-2, -5.446e-5])
+            K0 = self.blended_val(K0_lt, K0)
+            
+        self.K[0] =  self.Ktp(K0, self.vBar[0])
+    
+    def K_H2O(self): # Units: bar.mol-1
+    #=======================================================================
+    #  H2O K-value at reservoir pressure
+    #=======================================================================
+        if self.low_temp:
+            x = [-2.209, 3.097e-2, -1.098e-4, 2.048e-7]
+        else:
+            x = [-2.1077, 2.8127e-2, -8.4298e-5, 1.4969e-7, -1.1812e-10]
+        
+        K0 = 10**self.FT(self.degC, x)
+        
+        if self.scaled:
+            K0_lt = 10**self.FT(self.degC, [-2.209, 3.097e-2, -1.098e-4, 2.048e-7])
+            K0 = self.blended_val(K0_lt, K0)
+            
+        self.K[1] =  self.Ktp(K0, self.vBar[1])
+    
+    def mixMolar(self, x, P1, P2):
+    #=======================================================================
+    #  Calculate Mixture Property of two Molar Species
+    #=======================================================================
+        return x * P1 + (1 - x) * P2
+    
+    def calc_gammas(self):
+        if self.low_temp:
+            return [1,1]
+        Am = -3.084e-2*(self.tKel - 373.15) + 1.927e-5*(self.tKel - 373.15)**2                                 # Eq 15
+        self.gamma = [np.exp(2*Am*self.x[0]*(1-self.x[0])**2), np.exp((Am - 2*Am*(1-self.x[0]))*self.x[0]**2)] # Eq 12, 13
+        
+    def A_B(self):
+        A = self.K[1] * self.gamma[1] / self.fugPi[1]                                 # Eq 10.
+        B = self.fugPi[0] /(CONMOLA * self.gamma[0] * self.gamma_prime * self.K[0])   # Eq 17.
+        B = max(EPS,min(1-EPS, B))
+        self.A = A
+        self.Bprime = B
+    
+    #============================================================================
+    #  A Phase-Partitioning Model for CO2–Brine Mixtures at Elevated Temperatures 
+    #  and Pressures: Application to CO2-Enhanced Geothermal Systems
+    #  Nicolas Spycher & Karsten Pruess, Transp Porous Med (2010) 82:173–196
+    #  DOI 10.1007/s11242-009-9425-y
+    #============================================================================
+    
+    def co2BrineSolubility(self):
+        # Calculates CO2 saturated Brine mutual solubilities
+
+        pBar = self.pBar
+        degC = self.degC
+        ppm = self.ppm
+        
+        #  Initialisation       
+        if pBar <= 1.0:
+            pBar = 1+EPS
+        
+        self.tKel = degC + CEL2KEL
+        self.pRT = pBar / (RGASCON * self.tKel)
+
+        
+        if ppm == None:
+            if self.ppm == None:      # If salt concentration not defined, set to zero
+                self.ppm = 0          # If previously defined, but not redefined here, then leave as it was
+        else:
+            self.ppm = ppm            # Else if explcitly defined as function parameters, overwrite
+        
+        if self.degC <= 100:          # Reference pressures delineated by 100 deg C cutoff. 
+            self.P0 = 1.0             # Reference Pressure (1 bar at < 100 degC)
+        else:                         # Ref Pressure (Water saturation pressure Bar at >= 100 degC)
+            self.P0 = self.FT(self.degC, [-1.9906e-1, 2.0471e-3, 1.0152e-4, -1.4234e-6, 1.4168e-8]) 
+    
+        self.pRT0 = (self.pBar - self.P0) / (RGASCON * self.tKel)
+        self.pRT = self.pBar / (RGASCON * self.tKel)
+        
+        fppM = PPM2MFR * ppm                                              #--Weight Fraction from PPM
+        self.molaL = self.ppm2Molality()                                  #--Molality [gmol/kg]
+        self.xSalt = fppM * MWWAT / (fppM * MWWAT + (1.0 - fppM) * MWSAL)
+        self.gammaCO2()  # ----- Calculate Gamma Prime
+        
+        self.calc_type() # ----- Update the calculation type
+        
+        #== Component molar volumes
+        if self.low_temp:
+            VCO2 = 32.6                                 #--CO2 Molar Volume [cm3/gmol]
+            VH2O = 18.1                                 #--H2O Molar Volume [cm3/gmol]
+        else:
+            VCO2 = self.FT(self.tKel - 373.15, [32.6, 3.413e-2])  #--CO2 Molar Volume [cm3/gmol]
+            VH2O = self.FT(self.tKel - 373.15, [18.1, 3.137e-2])  #--H2O Molar Volume [cm3/gmol]
+        self.vBar = [VCO2, VH2O]
+        
+        #==k-Parameters (y/x partitioning factors) Equations 5 and 6 ==========================
+        self.K_CO2()
+        self.K_H2O()
+            
+        #== First estimates of yCO2 and xCO2 ================================================
+        if not self.low_temp:
+            yCO2 = 1 - self.est_yH2O() # Paper suggests using Psat/P, but this empirical fit appears more accurate
+            xCO2 = yCO2 / self.K[0]
+        else:
+            yCO2 = 1.0
+            xCO2 = 0.0
+            
+        self.y = np.array([yCO2, 1.0-yCO2])
+        self.x = np.array([xCO2, 1.0-xCO2])
+        
+        # Trigger mixing rules
+        self.aMix_RK()
+        self.bMix_RK()
+        
+        #--Solve the Cubic Equation A-2 --------------------------------------------
+        self.MolarVolume()
+        
+        #--Calculate Fugacity Coefficients*Pressure---------------------------------------
+        self.fugP()
+        
+        if self.scaled: # Recalculate mixing rules and fugacity pressure products with low temp relationships
+            phiP_ht = self.fugPi
+            self.low_temp = True  # Set flag for low temp coefficiencts
+            self.aMix_RK()
+            self.bMix_RK()
+            
+            self.fugP()
+            self.fugPi[0] = self.blended_val(self.fugPi[0], phiP_ht[0])
+            self.fugPi[1] = self.blended_val(self.fugPi[1], phiP_ht[1])
+            self.low_temp = False # Reset low temp flag
+
+        self.calc_gammas()
+        self.A_B()
+        
+        # Calculate results. 
+        self.y[1] = (1 - self.Bprime) * CONMOLA / ((1/self.A - self.Bprime) * (2.0 * self.molaL + CONMOLA) + 2 * self.molaL * self.Bprime) # Eq B-7
+        self.x[0] = self.Bprime * (1.0 - self.y[1])
+        self.y[0] = 1.0 - self.y[1]
+
+        mCO2 = min(max((1.0 - self.x[0]), EPS),1) * (CONMOLA + 2.0 * self.molaL) / min(max((1.0 - self.x[0]), EPS),1)
+        self.xSalt = 2.0 * self.molaL / (2.0 * self.molaL + CONMOLA + mCO2)  # Eq B-3. The 2.0x is stoichiometric ions for NaCl
+        self.x[1] = 1.0 - self.x[0] - self.xSalt
+        self.x[1] = min(max(self.x[1], 0), 1)
+
+        if not self.low_temp:  # Iterate to solution
+            err = 1
+            iternum = 0
+            while err > 1e-8 and iternum < 100:
+                yH2O_last = max(self.y[1], EPS)
+                
+                # Trigger mixing rules for changed compositions
+                self.aMix_RK()
+                self.bMix_RK()
+        
+                #--Fugacity Coefficients*Pressure---------------------------------------
+                self.fugP()
+                
+                if self.scaled:
+                    phiP_ht = self.fugPi
+                    self.low_temp = True  # Set flag for low temp coefficient calculations
+                    self.aMix_RK()
+                    self.bMix_RK()
+            
+                    self.fugP()
+                    self.fugPi[0] = self.blended_val(self.fugPi[0], phiP_ht[0])
+                    self.fugPi[1] = self.blended_val(self.fugPi[1], phiP_ht[1])
+                    self.low_temp = False # Reset low temp flag
+                
+                self.calc_gammas()
+                self.A_B()
+                
+                self.y[1] = (1 - self.Bprime) * CONMOLA / ((1/self.A - self.Bprime) * (2.0 * self.molaL + CONMOLA) + 2 * self.molaL * self.Bprime) # Eq B-7
+                self.y[1] = max(EPS, min(1-EPS, self.y[1]))
+                self.x[0] = self.Bprime * (1.0 - self.y[1])
+                self.x[0] = max(EPS, min(1-EPS, self.x[0]))
+                self.y[0] = 1.0 - self.y[1]
+                
+                mCO2 = min(max((1.0 - self.x[0]), EPS),1) * (CONMOLA + 2.0 * self.molaL) / min(max((1.0 - self.x[0]), EPS),1)
+                self.xSalt = 2.0 * self.molaL / (2.0 * self.molaL + CONMOLA + mCO2)  # Eq B-3. The 2.0x is stoichiometric ions for NaCl
+                self.x[1] = 1.0 - self.x[0] - self.xSalt
+                
+                err = abs(self.y[1]/yH2O_last-1)
+                
+                iternum += 1
+        
+        #=======================================================================
+        #  Re-Compute the CO2/H2O Gas Phase Density
+        #=======================================================================
+        self.y[1] = min(max(self.y[1], EPS), 1.0)
+        self.x[0] = self.Bprime * (1.0 - self.y[1])
+        self.y[0] = 1.0 - self.y[1]
+        
+        mCO2 = min(max((1.0 - self.x[0]), EPS),1) * (CONMOLA + 2.0 * self.molaL) / min(max((1.0 - self.x[0]), EPS),1)
+        self.xSalt = 2.0 * self.molaL / (2.0 * self.molaL + CONMOLA + mCO2)  # Eq B-3. The 2.0x is stoichiometric ions for NaCl
+        self.x[1] = 1.0 - self.x[0] - self.xSalt
+        self.x[1] = min(max(self.x[1], 0), 1)
+        
+        mole_frac_salt_in_brine = self.xSalt / (self.xSalt + self.x[1])
+        self.MwBrine = mole_frac_salt_in_brine * MWSAL + ((1-mole_frac_salt_in_brine) * MWWAT)
+
+        self.aMix_RK()
+        self.bMix_RK()
+        
+        #--Solve the Cubic------------------------------------------------------
+        self.MolarVolume()                                   #--Molar Volume [cm3/gmol]
+        self.MwGas = self.mixMolar(self.y[0], MWCO2, MWWAT)  #--Mole weight  [gm/gmol]
+        self.rhoGas = self.MwGas / self.MolarVol[0]          #--Density of Gas Mixture [gm/cm3]
+        self.GASZ = self.MolarVol[0] * self.pRT
+
+        
+    def brine(self):
+        results = co2_brine_props(self.pBar, self.degC, self.ppm, self.x[0], self.MwBrine)
+        self.bDen, self.bVis, self.bVisblty, self.bw, self.Rs, self.Cf_usat = results
+        
+        if not self.metric:
+            self.bVisblty = self.bVisblty / 14.5038   # CO2 laden viscosibility (1/psi) (at pressures above Psat)
+            self.Rs = self.Rs * 35.3147 / 6.28981     # Solution gwr CO2 (scf/stb brine)
+            self.Cf_usat = self.Cf_usat / 14.5038     # Undersaturated brine compressibility (1/psi)
+
+        
+def co2_brine_props(pBar, degc, ppm, xCO2, MwB):
+    """ Calculates CO2 saturated Brine properties
+        1. Pure Brine Density:            Spivey et al. (modified)
+        2. Pure Brine viscosity:          Mao-Duan (2009)
+        3. CO2 Corrected Brine Density:   Garcia (2001)
+        4. CO2 Corrected Brine Viscosity: Islam-Carlson (2012)
+        
+        pBar: Pressure (Bar)
+        degc: Temperature (deg C)
+        molaL: Salt molar concentration (gram mol/kg water)
+        xCO2: Mole fraction CO2 in brine at pBar
+        MwB: MW CO2 free Brine
+        
+        Returns tuple of CO2 Saturated;
+         - Brine Density (gm/cm3)
+         - viscosity (cP)
+         - viscosibility (1/psi))
+         - Formation volume factor (res vol/ std vol)
+         - Brine compressibility as pressure increases with no change to CO2 saturation (1/Bar)
+         - Brine compressibility as pressure decreases with reducing CO2 saturation (1/Bar)
+         - Brine solution gas ratio (sm3 CO2 / sm3 brine)
+    """
+    MwG = MWCO2
+    wt = ppm / 10000 # Wt % (0 - 100)
+    m = (1000 * (wt / 100) / (58.4428 * (1 - (wt / 100))))  # Molar concentration of NaCl from wt % in gram mol/kg 
+    
+    Mpa = pBar * 0.1                    # Pressure in mPa
+    tKel = degc + CEL2KEL               # Temperature in deg K
+    
+    def Eq41(t, input_array):           # From McCain Petroleum Reservoir Fluid Properties
+        t2 = t / 100
+        return (input_array[1] * t2 ** 2 + input_array[2] * t2 + input_array[3]) / (input_array[4] * t2 ** 2 + input_array[5] * t2 + 1)
+
+    # Table 4-6 Coefficients
+    rhow_t70_arr = [0, -0.127213, 0.645486, 1.03265, -0.070291, 0.639589]
+    Ewt_arr = [0, 4.221, -3.478, 6.221, 0.5182, -0.4405]
+    Fwt_arr = [0, -11.403, 29.932, 27.952, 0.20684, 0.3768]
+    
+    # Table 4-7 Coefficients
+    Dm2t_arr = [0, -0.00011149, 0.000175105, -0.00043766, 0, 0]
+    Dm32t_arr = [0, -0.0008878, -0.0001388, -0.00296318, 0, 0.51103]
+    Dm1t_arr = [0, 0.0021466, 0.012427, 0.042648, -0.081009, 0.525417]
+    Dm12t_arr = [0, 0.0002356, -0.0003636, -0.0002278, 0, 0]
+    
+    # Table 4-8 Coefficients
+    Emt_arr = [0, 0, 0, 0.1249, 0, 0]
+    Fm32t_arr = [0, -0.617, -0.747, -0.4339, 0, 10.26]
+    Fm1t_arr = [0, 0, 9.917, 5.1128, 0, 3.892]
+    Fm12t_arr = [0, 0.0365, -0.0369, 0, 0, 0]
+    
+    # Table 4-14 Mao-Duan Coefficients
+    d = [0, 2885310, -11072.577, -9.0834095, 0.030925651, -0.0000274071, -1928385.1, 5621.6046, 13.82725, -0.047609523, 0.000035545041]
+    
+    # Table 4-14 Mao-Duan Coefficients
+    a = [-0.21319213, 0.0013651589, -0.0000012191756]
+    b = [0.069161945, -0.00027292263, 0.0000002085244]
+    c = [-0.0025988855, 0.0000077989227]
+            
+    def calc_props(degc):
+        arrays = [rhow_t70_arr, Ewt_arr, Fwt_arr, Dm2t_arr, Dm32t_arr, Dm1t_arr, Dm12t_arr, Emt_arr, Fm32t_arr, Fm1t_arr, Fm12t_arr]
+        return [Eq41(degc, x) for x in arrays]
+    
+    # Calculate properties from steps 1, 2 and  4
+    rhow_t70, Ewt, Fwt, Dm2t, Dm32t, Dm1t, Dm12t, Emt, Fm32t, Fm1t, Fm12t = calc_props(degc)
+    
+    # -- CO2-Free Brine Density (gm/cm3)
+    def brine_denw(Mpa):
+        # cw(T, p), in MPa–1, of pure water at temperature T and pressure p,
+        cwtp = (1 / 70) * (1 / (Ewt * (Mpa / 70) + Fwt))        # Eq 4.2
+
+        #Density of pure water at temperature T and pressure p.
+        Iwt70 = (1 / Ewt) * np.log(abs(Ewt + Fwt))              # Eq 4.3
+        Iwtp = (1 / Ewt) * np.log(abs(Ewt * (Mpa / 70) + Fwt))  # Eq 4.4
+        rhowtp = rhow_t70 * np.exp(Iwtp - Iwt70)                # Eq 4.5
+        
+        # Density of brine at temperature T and the reference pressure of 70 MPa
+        rhobt70 = (rhow_t70 + Dm2t * m **2 + Dm32t * m ** 1.5 + Dm1t * m + Dm12t * m ** 0.5)  # Eq 4.6
+        
+        # Brine compressibility coefficients Eb(T,m) and Fb(T,m) from equations (4.7) and (4.8).
+        Ebtm = Ewt + Emt * m                                                                  # Eq 4.7
+        Fbtm = Fwt + Fm32t * m ** 1.5 + Fm1t * m + Fm12t * m ** 0.5                           # Eq 4.8
+        
+        # Return methane-free brine density Rhob(T,p,m), in g/cm3
+        cbtpm = (1 / 70) * (1 / (Ebtm * (Mpa / 70) + Fbtm))                                   # Eq 4.9 (Step 6)
+        Ibt70 = (1 / Ebtm) * np.log(abs(Ebtm + Fbtm))                                         # Eq 4.10 (Step 7)
+        Ibtpm = (1 / Ebtm) * np.log(abs(Ebtm * (Mpa / 70) + Fbtm))                            # Eq 4.11
+        return rhobt70 * np.exp(Ibtpm - Ibt70), rhowtp                                        # Eq 4.12
+    
+    # -- CO2 free brine viscosity Mao-Duan (2009)
+    def vis_brine(Mpa, rhowtp):
+        
+        #-- Viscosity of pure water - Eq 4.41 - 4.42
+        lnuw_tp = sum([d[i] * np.power(tKel, (i - 3)) for i in range(1, 6)])
+        
+        lnuw_tp += sum([rhowtp * (d[i] * np.power(tKel, (i - 8))) for i in range(6, 11)])
+        uw_tp = np.exp(lnuw_tp)
+
+        #-- Calculate relative viscosity of brine.    Eq 4.43 - 4.47
+        AA = a[0] + a[1] * tKel + a[2] * tKel * tKel 
+        BB = b[0] + b[1] * tKel + b[2] * tKel * tKel
+        CC = c[0] + c[1] * tKel
+        lnur_tm = AA * m + BB * m ** 2 + CC * m ** 3
+        ur_tm = np.exp(lnur_tm)
+        
+        # And then brine viscosity in Pa.s, converted to cP
+        return ur_tm * uw_tp * 1000  # cP - Eq 4.48
+    
+    def partMolVol(degK):
+        #  Partial Molar Volume of dissolved CO2: Garcia Eq (3)
+        tC = degK - 273.15
+        tC2 = tC * tC
+        tC3 = tC * tC2
+        return 37.51 + tC * (-0.09585 + tC * (0.000874 - tC * 0.0000005044))
+    
+    # -- Correcting brine density for dissolved CO2, JE Garcia, LBNL Report# 49023, Oct 2011, "Density of Aqueous Solutions of CO2"
+    def garciaDensity(rhoBRnoCO2, tKel, pBar, ppm, xCO2, MwB, MwG):
+        fppM = PPM2MFR * ppm                         #--Weight Fraction from PPM
+        xNotCO2 = 1.0 - xCO2                         #--Brine (H20+Salt) Mole Fraction
+        xRat = xCO2 / xNotCO2                        #--Mole Fraction Ratio, Gas/Brine
+        mRat = MwG / MwB                             #--Mole Weight Ratio  , Gas/Brine
+        vPhi = partMolVol(tKel)                      #--Apparent Molar Volume of Dissolved CO2
+        return (1.0 + mRat * xRat) / (vPhi * xRat / MwB + 1.0 / rhoBRnoCO2)
+    
+    # Correct CO2 free brine viscosity for dissolved CO2
+    # Using approach from "Viscosity Models and Effects of Dissolved CO2", Akand W. Islam and Eric S. Carlson (Jul 2012), Energy Fuels 2012, 26, 8, 5330–5336, https://doi.org/10.1021/ef3006228
+    def co2_vis_brine(cP_brine, xCO2):
+        # Uses CO2 free brine viscosity (cP) and mole fraction CO2 in brine (xCO2), and returns cP
+        return cP_brine * (1 + 4.65 * xCO2**1.0134)
+
+    # Density and viscosity at specified pressure & temperature (No CO2)
+    sg_brine, rhowtp = brine_denw(Mpa)                        # rhowtp is density of pure water
+    cP_brine = co2_vis_brine(vis_brine(Mpa, rhowtp), xCO2)
+    
+    # Correct for CO2 content
+    sg_CO2_Brine = garciaDensity(sg_brine, tKel, pBar, ppm, xCO2, MwB, MwG)
+    cP_CO2_brine = co2_vis_brine(cP_brine, xCO2)
+    
+    # Revaluate at +1 bar for viscosibility calculations
+    # Use unchanged xCO2, as viscosibility typically used to characterized UNDERsaturated viscosity behaviour
+    sg_brine_, rhowtp_ = brine_denw(Mpa + 0.1)
+    cP_brine_ = co2_vis_brine(vis_brine(Mpa + 0.1, rhowtp_), xCO2)
+    sg_CO2_Brine_ = garciaDensity(sg_brine_, tKel, pBar, ppm, xCO2, MwB, MwG)
+    cP_CO2_brine_ = co2_vis_brine(cP_brine_, xCO2)
+    
+    # -- Numerically calculate viscosibility from Mao-Duan (2009) base viscosity with Garcia correction for CO2
+    dvdpsi = (cP_CO2_brine_ - cP_CO2_brine)  #-- d[Viscosity/dp [cP/bar]
+    viscosblty = dvdpsi * 2 / (cP_CO2_brine + cP_CO2_brine_)  # (1/bar)
+    
+    # Re-evaluate at reservoir temperature and 1 atmosphere (Rhob_atm)
+    Rhob_atm, rhowtp_atm_ = brine_denw(0.101325)
+
+    # Re-evaluate at standard conditions
+    # CO2-Free Brine Density at standard conditions (gm/cm3)
+    degc = (60 - 32)/1.8 # 60 deg F
+    rhow_t70, Ewt, Fwt, Dm2t, Dm32t, Dm1t, Dm12t, Emt, Fm32t, Fm1t, Fm12t = calc_props(degc)
+    sg_SC_Brine, rhowSC = brine_denw(0.101325)
+
+    # Calculate mass, moles and reservoir volume of 1 sm3 of brine without CO2
+    brine_mass = sg_SC_Brine * 1000              # kg brine / sm3 (No CO2)
+    brine_moles = brine_mass / MwB               # Moles of brine per sm3
+    brine_res_vol = brine_mass / (sg_brine*1000) # reservoir volume of brine (res m3 No CO2)
+    
+    # Calculate moles and mass of CO2 using xCO2 and moles of brine
+    co2_moles = xCO2 / (1 - xCO2) * brine_moles  # Moles of dissolved CO2 per sm3
+    co2_mass = co2_moles * MWCO2                 # kg co2 / sm3 brine
+    
+    # Calculate CO2 volume associated with moles of CO2 in each sm3 of brine
+    rs = 22.413962 * co2_moles                   # sm3 CO2 per sm3 Brine
+    
+    # Mass balance to work out reservoir volume of dissolved CO2
+    # sg_CO2_Brine = (mass_co2 + mass_brine)/(brine_res_vol + co2_res_vol). Rearranging yields following equation
+    co2_res_vol = ((co2_mass + brine_mass) - (sg_CO2_Brine * 1000 * brine_res_vol)) / (sg_CO2_Brine * 1000)
+    bw = co2_res_vol + brine_res_vol # rm3 / sm3
+    
+    # Undersaturated compressibility = 1/V dV/dP
+    c_usat = 1 - sg_CO2_Brine / sg_CO2_Brine_ # 1/Bar    
+    
+    return ([sg_CO2_Brine, sg_brine], [cP_CO2_brine, cP_brine], viscosblty, [bw, brine_res_vol], rs, c_usat)
```

### Comparing `pyrestoolbox-1.3.9/pyrestoolbox/simtools/simtools.py` & `pyrestoolbox-1.4.0/pyrestoolbox/simtools/simtools.py`

 * *Files identical despite different names*

### Comparing `pyrestoolbox-1.3.9/pyrestoolbox.egg-info/PKG-INFO` & `pyrestoolbox-1.4.0/pyrestoolbox.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pyrestoolbox
-Version: 1.3.9
+Version: 1.4.0
 Summary: pyResToolbox - A collection of Reservoir Engineering Utilities
 Home-page: https://github.com/mwburgoyne/pyResToolbox
 Author: Mark W. Burgoyne
 Author-email: mark.w.burgoyne@gmail.com
 Keywords: restoolbox,petroleum,reservoir
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 `pyrestoolbox`
 ==============
 
-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\--A collection of
-Reservoir Engineering Utilities
+\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\--
+A collection of Reservoir Engineering Utilities
 \-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\--
 
 This set of functions focuses on those that the author uses often while
 crafting programming solutions. These are the scripts that are often
 copy/pasted from previous work - sometimes slightly modified - resulting
 in a trail of slightly different versions over the years. Some attempt
 has been made here to make this implementation flexible enough such that
@@ -36,17 +36,22 @@
 -   Creation of layered permeability distribution consistent with a
     Lorenze heterogeneity factor
 -   Extract problem cells information from Intesect (IX) print files
 -   Generation of AQUTAB include file influence functions for use in
     ECLIPSE
 -   Creation of Corey and LET relative permeability tables in Eclipse
     format
+-   Calculation of Methane and CO2 saturated brine properties
 
 Apologies in advance that it is only in oilfield
-units with no current plans to add multi-unit support.
+units with no current plans to add universal multi-unit support.
+
+Changelist in 1.4.0:
+- Introduced CO2 saturated brine calculations using Spycher & Pruess modified SRK EOS method
+- Rectified an error introduced in Gas Z-Factor calculations due to errant indentation
 
 Changelist in 1.3.9:
 - Tweaks to speed DAK and Hall & Yarborough Z-Factor calculations
 
 Changelist in 1.3.8:
 - Fix bug in Hall & Yarborough Z-Factor calculation
 
@@ -118,15 +123,16 @@
 -   Generate Black Oil Table data              
 -   Estimate soln gas SG from oil                
 -   Estimate SG of gas post separator               
 -   Calculate weighted average surface gas SG  
 -   Oil API to SG              
 -   Oil SG to API
 ----------------------------
--   Calculate suite of brine properties        
+-   Calculate suite of methane saturated brine properties  
+-   Calculate suite of CO2 saturated brine properties   
 ----------------------------
 -   Lorenz coefficient from Beta value                   
 -   Lorenz coefficient from flow fraction                
 -   Lorenz coefficient to flow fraction                
 -   Lorenz coefficient to permeability array      
 ----------------------------
 -   Summarize IX convergence errors from PRT file
```

### Comparing `pyrestoolbox-1.3.9/setup.cfg` & `pyrestoolbox-1.4.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6465 7363  [metadata]..desc
 00000010: 7269 7074 696f 6e5f 6669 6c65 203d 2052  ription_file = R
 00000020: 4541 444d 452e 6d64 0d0a 6e61 6d65 203d  EADME.md..name =
 00000030: 2070 7972 6573 746f 6f6c 626f 780d 0a76   pyrestoolbox..v
-00000040: 6572 7369 6f6e 203d 2031 2e33 2e39 0d0a  ersion = 1.3.9..
+00000040: 6572 7369 6f6e 203d 2031 2e34 2e30 0d0a  ersion = 1.4.0..
 00000050: 6175 7468 6f72 203d 204d 6172 6b20 572e  author = Mark W.
 00000060: 2042 7572 676f 796e 650d 0a61 7574 686f   Burgoyne..autho
 00000070: 725f 656d 6169 6c20 3d20 6d61 726b 2e77  r_email = mark.w
 00000080: 2e62 7572 676f 796e 6540 676d 6169 6c2e  .burgoyne@gmail.
 00000090: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 000000a0: 203d 2070 7952 6573 546f 6f6c 626f 7820   = pyResToolbox 
 000000b0: 2d20 4120 636f 6c6c 6563 7469 6f6e 206f  - A collection o
```

### Comparing `pyrestoolbox-1.3.9/setup.py` & `pyrestoolbox-1.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 f = open('C:\\Users\\vinom\OneDrive - Santos\\Work in progress\\Python\\0-ResEng\\pyResToolbox\\source_dir\\README.md', 'r').read()
 long_description= f #markdown.markdown( f.read() )
 
 setup(
     name = 'pyrestoolbox',
     packages = find_packages(),
     include_package_data=True,
-    version = '1.3.9',  # Ideally should be same as your GitHub release tag varsion
+    version = '1.4.0',  # Ideally should be same as your GitHub release tag varsion
     description = 'pyResToolbox - A collection of Reservoir Engineering Utilities',
     long_description= long_description,
     long_description_content_type = 'text/markdown',
     author = 'Mark W. Burgoyne',
     author_email = 'mark.w.burgoyne@gmail.com',
     url = 'https://github.com/mwburgoyne/pyResToolbox',
     keywords = ['restoolbox', 'petroleum', 'reservoir'],
```

