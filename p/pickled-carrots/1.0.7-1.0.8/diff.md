# Comparing `tmp/pickled_carrots-1.0.7.tar.gz` & `tmp/pickled_carrots-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pickled_carrots-1.0.7.tar", max compression
+gzip compressed data, was "pickled_carrots-1.0.8.tar", max compression
```

## Comparing `pickled_carrots-1.0.7.tar` & `pickled_carrots-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1309 2023-05-19 17:43:26.854143 pickled_carrots-1.0.7/README.md
--rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-1.0.7/pickled_carrots/DPData.py
--rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-1.0.7/pickled_carrots/DPPlot.py
--rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-1.0.7/pickled_carrots/DPUtil.py
--rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-1.0.7/pickled_carrots/__init__.py
--rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-1.0.7/pickled_carrots/database.py
--rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-1.0.7/pickled_carrots/dataclass.py
--rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-1.0.7/pickled_carrots/mathutil.py
--rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-1.0.7/pickled_carrots/plot.py
--rwxr-xr-x   0        0        0     1034 2023-05-24 14:49:39.883632 pickled_carrots-1.0.7/pickled_carrots/resources/event_type_lookup.pickle
--rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-1.0.7/pickled_carrots/vinegar/__init__.py
--rw-r--r--   0        0        0    13845 2023-05-26 13:00:40.817419 pickled_carrots-1.0.7/pickled_carrots/vinegar/core.py
--rw-r--r--   0        0        0     9312 2023-05-29 12:55:11.279181 pickled_carrots-1.0.7/pickled_carrots/vinegar/event.py
--rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-1.0.7/pickled_carrots/vinegar/inventory.py
--rw-r--r--   0        0        0     1069 2023-05-25 14:36:27.387680 pickled_carrots-1.0.7/pickled_carrots/vinegar/tests/test_read_hsf.py
--rw-r--r--   0        0        0   138987 2023-05-24 17:57:38.942953 pickled_carrots-1.0.7/pickled_carrots/waveforms.py
--rw-r--r--   0        0        0      678 2023-07-18 13:53:59.343042 pickled_carrots-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 pickled_carrots-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-01 18:37:10.807525 pickled_carrots-1.0.8/README.md
+-rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-1.0.8/pickled_carrots/DPData.py
+-rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-1.0.8/pickled_carrots/DPPlot.py
+-rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-1.0.8/pickled_carrots/DPUtil.py
+-rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-1.0.8/pickled_carrots/__init__.py
+-rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-1.0.8/pickled_carrots/database.py
+-rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-1.0.8/pickled_carrots/dataclass.py
+-rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-1.0.8/pickled_carrots/mathutil.py
+-rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-1.0.8/pickled_carrots/plot.py
+-rwxr-xr-x   0        0        0     1034 2023-05-24 14:49:39.883632 pickled_carrots-1.0.8/pickled_carrots/resources/event_type_lookup.pickle
+-rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-1.0.8/pickled_carrots/vinegar/__init__.py
+-rw-r--r--   0        0        0    13845 2023-05-26 13:00:40.817419 pickled_carrots-1.0.8/pickled_carrots/vinegar/core.py
+-rw-r--r--   0        0        0     9312 2023-05-29 12:55:11.279181 pickled_carrots-1.0.8/pickled_carrots/vinegar/event.py
+-rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-1.0.8/pickled_carrots/vinegar/inventory.py
+-rw-r--r--   0        0        0     1069 2023-05-25 14:36:27.387680 pickled_carrots-1.0.8/pickled_carrots/vinegar/tests/test_read_hsf.py
+-rw-r--r--   0        0        0   141094 2023-08-01 18:37:10.807525 pickled_carrots-1.0.8/pickled_carrots/waveforms.py
+-rw-r--r--   0        0        0      678 2023-08-01 18:37:20.295963 pickled_carrots-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 pickled_carrots-1.0.8/PKG-INFO
```

### Comparing `pickled_carrots-1.0.7/pickled_carrots/DPData.py` & `pickled_carrots-1.0.8/pickled_carrots/DPData.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.7/pickled_carrots/DPPlot.py` & `pickled_carrots-1.0.8/pickled_carrots/DPPlot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.7/pickled_carrots/DPUtil.py` & `pickled_carrots-1.0.8/pickled_carrots/DPUtil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.7/pickled_carrots/database.py` & `pickled_carrots-1.0.8/pickled_carrots/database.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.7/pickled_carrots/dataclass.py` & `pickled_carrots-1.0.8/pickled_carrots/dataclass.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.7/pickled_carrots/mathutil.py` & `pickled_carrots-1.0.8/pickled_carrots/mathutil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.7/pickled_carrots/plot.py` & `pickled_carrots-1.0.8/pickled_carrots/plot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.7/pickled_carrots/resources/event_type_lookup.pickle` & `pickled_carrots-1.0.8/pickled_carrots/resources/event_type_lookup.pickle`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.7/pickled_carrots/vinegar/core.py` & `pickled_carrots-1.0.8/pickled_carrots/vinegar/core.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.7/pickled_carrots/vinegar/event.py` & `pickled_carrots-1.0.8/pickled_carrots/vinegar/event.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.7/pickled_carrots/vinegar/inventory.py` & `pickled_carrots-1.0.8/pickled_carrots/vinegar/inventory.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.7/pickled_carrots/vinegar/tests/test_read_hsf.py` & `pickled_carrots-1.0.8/pickled_carrots/vinegar/tests/test_read_hsf.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.7/pickled_carrots/waveforms.py` & `pickled_carrots-1.0.8/pickled_carrots/waveforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,20 +89,19 @@
     # reading in the traces
     st = read(file_path, format='MSEED')
 
     # returning obspy stream to the user
     return st
 
 
-# function to convert hsf data into obspy structure
 def hsf_to_obspy(file=None, head=None, data=None, rotate=True, correct_g_to_mss=True,
                  print_out=True,
                  groundmotion=True, rotate_to_zrt=False, force_positive_down=False,
                  experimental=False,
-                 force_python_decompress=False, rotate_to_lqt=False, return_head=True):
+                 force_python_decompress=False, rotate_to_lqt=False):
     """
     Function to convert the information read from the hsf file by read_hsf into an obspy trace object
     There is some additional information saved to the header of each trace:
     stats.t0 - The P arrival time in seconds - 0 if there is no P arrival
     stats.t1 - The S arrival time in seconds - 0 if there is no S arrival
     stats.t2 - The origin time in seconds
     stats.t3 - The Sh arrival time in seconds - 0 if there is no Sh
@@ -118,100 +117,95 @@
     :param file: the name of the file to be used to read the hsf data from
     :param rotate: if True, rotates the data into a ZNE coordinate system
     :param correct_g_to_mss: if True, corrects accelerometer data from g to m/s/s
     :param print_out: if True, prints to screen when traces don't have P or S values
     :param groundmotion: if True, returns output in SI units rather than volts
     :param rotate_to_zrt: if True, rotates the data to radial and transverse - transverse contains mostly SH energy, and
         radial contains mostly P and Sv energy. Vertical component remains. For reference, H component in WaveVis is
-        the same as the T component here, and the V component is the Radial. R component in WaveVis is the polarity 
-        flipped down component, which is the same as the vertical component here. WaveVis uses down as positive 
+        the same as the T component here, and the V component is the Radial. R component in WaveVis is the polarity
+        flipped down component, which is the same as the vertical component here. WaveVis uses down as positive
         sometimes - might need futher work to build this in here.
         Also, we just obtain the azimuth from the earthquake location and station location saved in the file, we don't
         do anything fancy with detecting the ray path direction.
     :param force_positive_down: if True, then if the data has the use_elevation flag set to true, as in vertical motion
         is positive upwards, the code will flip this so the data has vertical motion positive downwards
     :param experimental: if True, uses the experimental version of read hsf rather than the normal version
     :param force_python_decompress: if True, forces code to use the Python decompression method
     :param rotate_to_lqt: if True, rotate to lqt instead of zrt (rotating to ray path)
-    :param return_head: if True returns the header
     :return: An obspy stream of traces of the data in the hsf file
     """
     import obspy
     import math
-    
+
     # making sure that rotate is turned on if rotate_to_zrt is turned on
     if rotate_to_zrt or rotate_to_lqt:
         rotate = True
 
     # setting experimental to True when on posix
+    if os.name == 'posix':
+        experimental = True
 
-    # if os.name == 'posix':
-    #     experimental = True
-    
     # whether to run the read_hsf function
     if head is None:
         if experimental is False:
-            tm, data, head = read_hsf(file=file, groundmotion=groundmotion, print_out=print_out,
+            tm, data, head = read_hsf(file=file, groundmotion=groundmotion,
+                                      print_out=print_out,
                                       from_hsf_to_obspy=True)
         else:
-            tm, data, head = read_hsf_exp(file=file, groundmotion=groundmotion, print_out=print_out,
+            tm, data, head = read_hsf_exp(file=file, groundmotion=groundmotion,
+                                          print_out=print_out,
                                           from_hsf_to_obspy=True, s3data=data,
                                           force_python_decompress=force_python_decompress)
 
-    # letting the user know that we follow the esg standard and report the vertical as positive up
+    # letting the user know that we follow the ESG standard and report the vertical as positive up
     if head['use_elevation'] == 1 and print_out:
         print('\n**************')
-        print('NOTE: we follow the hsf settings here and vertical is positive upwards rather than down.')
-        print('Changing to vertical positive down will change the amplitudes of the rotated traces due to\n'
-              'the change in the dip')
+        print(
+            'NOTE: we follow the hsf settings here and vertical is positive upwards rather than down.')
+        print(
+            'Changing to vertical positive down will change the amplitudes of the rotated traces due to\n'
+            'the change in the dip')
         print('**************\n')
         if force_positive_down is True:
             # TODO the vertical amplitudes don't appear to be forced to be positive?
             print('You have chosen to force vertical amplitudes to be positive down.')
 
     # checking whether the data is None
-    # this is for cases where I was having issues with files that did not have the correct amount of buffer for the 
+    # this is for cases where I was having issues with files that did not have the correct amount of buffer for the
     # given data size - not sure on the cause of this error but for now including this workaround
-    # IF YOU FIND an example file that is triggering this issue, then please drop me an email at 
+    # IF YOU FIND an example file that is triggering this issue, then please drop me an email at
     # joshua.williams@esgsolutions.com or drop me a line on teams.
     if data is None:
         return None
-    
+
     # setting up some header information
     stats = obspy.core.Stats()
-    stats.network = 'esg'
+    stats.network = 'ESG'
     stats.sampling_rate = head['fs']  # in Hz
     stats.npts = head['npts']
     stats.starttime = obspy.UTCDateTime(head['dt'])
 
     # pulling out the event type
     # according to the header file for hsf files
-    possible_types = ['Event', 'Blast', 'RockBurst', 'CasingFailure', 'Background', 'Noise', 'Custom1',
-                      'Custom2', 'Custom3', 'UnknownEvt', 'SgmEvent', 'Duplicate', 'none', 'none', 'none', 'none',
+    possible_types = ['Event', 'Blast', 'RockBurst', 'CasingFailure', 'Background',
+                      'Noise', 'Custom1',
+                      'Custom2', 'Custom3', 'UnknownEvt', 'SgmEvent', 'Duplicate',
+                      'none', 'none', 'none', 'none',
                       'none', 'none', 'none', 'none', 'none', 'none']
     stats.evtype = possible_types[head['evtype']]
 
     # reading in the data to traces in obspy streams
     stream = obspy.Stream()
     for i in range(0, len(data)):
         tr = obspy.Trace(data[i, :], header=stats)
         stream.append(tr)
 
     # detecting the instrument type of the data using the stype part of the header
-    possible_types = ['GEOPHONE', 'ACCELEROMETER', 'SGM_GEOPHONE', 'FBA_ACCELEROMETER', 'BVM_MICROPHONE']
-
-    # figuring out which traces have incomplete data
-    new_descr = []
-    for ij in range(len(head['ch_descr'])):
-        if head['ch_descr'][ij] not in new_descr:
-            new_descr.append(head['ch_descr'][ij])
-    new_descr = np.array(new_descr)
-    incomplete_stations = new_descr[head['incomplete_data']]
-    bad_time_sync_stations = new_descr[head['bad_sync']]
-    enabled_stations = new_descr[head['enabled']]
+    possible_types = ['GEOPHONE', 'ACCELEROMETER', 'SGM_GEOPHONE', 'FBA_ACCELEROMETER',
+                      'BVM_MICROPHONE']
 
     # assigning the channel names
     if head['ntr'] > 0 and len(head['ch_descr']) > 0:
         count = 0
         stcount = 0
 
         # saving the name of the first trace of the station to fix problems with inconsistent station
@@ -224,39 +218,39 @@
             # these counters are needed to select the collect part of the sensor rotation
             # 'count' goes through the stations, I had to introduce this because otherwise the code
             # won't work for uniaxial and triaxial sensors mixed in the file
             # 'stcount' counts through the trace location for the particular station, so goes through each channel
             if k != 0:
                 # so if we're onto a new station name and the number of sensors has gone past the number of channels
                 # then we must be onto the next station
-                if head['ch_descr'][k] != head['ch_descr'][k - 1] and stcount+1 > head['nch_sen'][count]:
+                if stcount + 1 > head['nch_sen'][count]:
                     count += 1
                     stcount = 0
                     ch_descr_temp = head['ch_descr'][k].rstrip('\x00')
 
             # saving the station name
             # old way of getting the station name
             # stream[k].stats.station = head['ch_descr'][k].split('_')[0].split('\'')[1]
             # new way of getting the station name
             stream[k].stats.station = ch_descr_temp
 
             # saving the incomplete status to the stream
-            if ch_descr_temp in incomplete_stations:
+            if head['incomplete_data'][count]:
                 stream[k].stats.kt2 = 'incomplete'
             else:
                 stream[k].stats.kt2 = 'complete'
 
             # saving the time sync status
-            if ch_descr_temp in bad_time_sync_stations:
+            if head['bad_sync'][count]:
                 stream[k].stats.kt3 = 'bad_time_sync'
             else:
                 stream[k].stats.kt3 = 'good_time_sync'
 
             # saving the enabled status
-            if ch_descr_temp in enabled_stations and not head['valid_flag_channelbad'][k]:
+            if head['enabled'][count] and not head['valid_flag_channelbad'][k]:
                 stream[k].stats.kt4 = 'enabled'
             else:
                 stream[k].stats.kt4 = 'disabled'
 
             # attempting to save the snr
             klist = list(head.keys())
             if 'p_snr' in klist:
@@ -267,23 +261,14 @@
                 stream[k].stats.p_pol = head['p_pol'][count]
             if 's_pol' in klist:
                 stream[k].stats.s_pol = head['s_pol'][count]
             if 'sv_pol' in klist:
                 stream[k].stats.sv_pol = head['sv_pol'][count]
             if 'sh_pol' in klist:
                 stream[k].stats.sh_pol = head['sh_pol'][count]
-            if 'senpos' in klist:
-                stream[k].stats.easting = head['senpos'][count][0]
-                stream[k].stats.northing = head['senpos'][count][1]
-                stream[k].stats.depth = head['senpos'][count][2]
-            # if 'sen_rot' in klist:
-            #     stream[k].stats.c0_rot = head['sen_rot'][count][0]
-            #     stream[k].stats.c1_rot = head['sen_rot'][count][0]
-            #     stream[k].stats.c2_rot = head['sen_rot'][count][0]
-            # if
 
             # saving the distance between the event and station to the header of the obspy trace
             stream[k].stats.distance = head['Distance'][count]
 
             # figuring out the instrument type
             actual_type = possible_types[head['stype'][count]]
 
@@ -299,21 +284,21 @@
                 # follow IRIS SEED naming conventions
                 chan_str_2 = 'N'
             else:
                 stream[k].stats.instrument_type = 'VEL'
 
                 # if the station is a geophone, then setting the second letter as H to try and
                 # follow IRIS SEED naming conventions
-                chan_str_2 = 'P'
+                chan_str_2 = 'H'
 
             # pulling out the channel name
             # got rid of the location based channel naming because the rotation should take care of that
             # plus if you base it off the orientation then some stations you will end up with the same name
             # for multiple channels
-            stream[k].stats.channel = 'G'+chan_str_2+str(stcount+1)
+            stream[k].stats.channel = 'H' + chan_str_2 + str(stcount + 1)
 
             # estimating the angle of the station from North
             azimuth = None
             if head['sen_rot'][count][stcount][0] != 0:
                 az_change = math.degrees(math.atan(head['sen_rot'][count][stcount][1] /
                                                    head['sen_rot'][count][stcount][0]))
 
@@ -352,15 +337,16 @@
                     # we are exactly north
                     azimuth = 0
                 elif head['sen_rot'][count][stcount][0] < 0:
                     # we are exactly south
                     azimuth = 180
 
             # for the case where both north and east are zero then its a perfect vertical component
-            if head['sen_rot'][count][stcount][0] == 0. and head['sen_rot'][count][stcount][1] == 0.:
+            if head['sen_rot'][count][stcount][0] == 0. and \
+                    head['sen_rot'][count][stcount][1] == 0.:
                 azimuth = 0
 
             # then calculating the back azimuth
             if azimuth < 180:
                 back_azimuth = azimuth + 180
             else:
                 back_azimuth = azimuth - 180
@@ -371,15 +357,16 @@
             # accounting for cases where the user has selected to force positive down motions
             if head['use_elevation'] == 1 and force_positive_down is True:
                 sen_rot_value = head['sen_rot'][count][stcount][2] * -1.
             else:
                 sen_rot_value = head['sen_rot'][count][stcount][2]
 
             # computing the dip and inclination
-            dip = math.degrees(math.acos(sen_rot_value)) - 90  # removed minus just before head
+            dip = math.degrees(
+                math.acos(sen_rot_value)) - 90  # removed minus just before head
             inclination = 90 - math.degrees(math.acos(sen_rot_value))
             stream[k].stats.inclination = inclination
             stream[k].stats.dip = dip
 
             # and setting the P wave and S wave arrival times
             stream[k].stats.kt0 = 'P'
             stream[k].stats.kt1 = 'S'
@@ -400,16 +387,17 @@
             # correction of instrument data from g to m/s/s
             # mult factor is determined above, so data will not be changed if the instrument units are m/s rather than
             # m/s/s
             stream[k].data = stream[k].data * mult_factor
 
             # warning user if there do not appear to be any P or S wave arrival picks
             if stream[k].stats.t0 == 0 and stream[k].stats.t1 == 0 and print_out is True:
-                print('Warning: There do not appear to be P and S picks for the trace ' + stream[k].stats.network +
-                      '.'+stream[k].stats.station + '.' + stream[k].stats.channel)
+                print('Warning: There do not appear to be P and S picks for the trace ' +
+                      stream[k].stats.network +
+                      '.' + stream[k].stats.station + '.' + stream[k].stats.channel)
 
             # iterating the stcount value
             stcount += 1
 
     if rotate is False and print_out is True:
         print('rotation is off')
     if rotate is True:
@@ -426,15 +414,16 @@
         for jk in range(len(stat_names)):
             # pulling out the station location
             sen_loc = head['pos'][jk]
 
             # estimating the azimuth clockwise from north of the earthquake relative to the station and thus
             # the back azimuth of the station relative to the source
             # 90 - is to make sure the negative angles get flipped, % 360
-            stat_azimuth = (360 + math.degrees(math.atan2(eq_loc[1] - sen_loc[1], eq_loc[0] - sen_loc[0]))) % 360
+            stat_azimuth = (360 + math.degrees(
+                math.atan2(eq_loc[1] - sen_loc[1], eq_loc[0] - sen_loc[0]))) % 360
             if stat_azimuth < 180:
                 stat_back_azimuth = stat_azimuth + 180
             else:
                 stat_back_azimuth = stat_azimuth - 180
 
             # testing Dougs approach for calculating inclination
             xvalue = sen_loc[1] - eq_loc[1]
@@ -451,25 +440,28 @@
 
         # making the inventory object using the stream
         inventory = create_obspy_inv(stream)
         if print_out is True:
             print('This code rotates traces into a ZNE coordinate system')
         for jk in range(len(stat_names)):
             stream_new = stream.select(station=stat_names[jk])
-            good_station = check_rotation(stream_new)
+            good_station = check_rotation(stream_new, print_out=print_out)
 
             # checking if the stream can be rotated
             if good_station is True:
                 try:
                     # noinspection PyProtectedMember
-                    stream.select(station=stat_names[jk])._rotate_to_zne(inventory=inventory)
+                    stream.select(station=stat_names[jk])._rotate_to_zne(
+                        inventory=inventory)
                 except ValueError:
-                    print('station ' + stat_names[jk] + ' could not be rotated to zne due to azimuth/dip problem')
+                    print('station ' + stat_names[
+                        jk] + ' could not be rotated to zne due to azimuth/dip problem')
                 except NotImplementedError:
-                    print('station ' + stat_names[jk] + ' could not be rotated due to hsf error.')
+                    print('station ' + stat_names[
+                        jk] + ' could not be rotated due to hsf error.')
                     temp_st = stream.select(station=stat_names[jk])
                     for tr in temp_st:
                         stream.remove(tr)
         # stream._rotate_to_zne(inventory=inventory)
 
         # option for rotating to zrt format
         # error if both are true
@@ -480,16 +472,16 @@
             rot_method = 'NE->RT'
             if rotate_to_lqt:
                 rot_method = 'ZNE->LQT'
 
             # looping through each of the stations
             for jk in range(len(stat_names)):
                 # extracting the azimuth and back azimuth from the dictionary
-                stat_azimuth = az_dict[stat_names[jk]+' az']
-                stat_inclination = az_dict[stat_names[jk]+' inc']
+                stat_azimuth = az_dict[stat_names[jk] + ' az']
+                stat_inclination = az_dict[stat_names[jk] + ' inc']
 
                 # now performing the rotation
                 if print_out is True:
                     print('Be wary of the ZRT or LQT rotation, '
                           'there may be some issues with the obspy function so compare '
                           'the waveforms with WaveVis')
                 stream.select(station=stat_names[jk]).rotate(rot_method,
@@ -498,18 +490,15 @@
 
                 # flipping the amplitude of the Q component to agree with the output that we see in WaveVis
                 if head['use_elevation']:
                     sttemp = stream.select(station=stat_names[jk], channel='**Q')
                     for tr in sttemp:
                         tr.data = tr.data * -1
 
-    if return_head:
-        return stream, head
-    else:
-        return stream
+    return stream
 
 
 def create_obspy_inv(stream):
     """
     Function for creating an obspy inventory object from the stream without using a station xml
     Based on the obspy tutorials for creating xml files from scratch
     This inventory does not include the response data, just the data needed for rotation
@@ -517,15 +506,16 @@
     :param stream: stream of data used
     :type stream: obspy stream
     :return: obspy inventory containing the station information
     :rtype: obspy inventory
     """
     # some handy imports
     from obspy import UTCDateTime
-    from obspy.core.inventory import Inventory, Network, Station, Channel, Site, Latitude, Longitude
+    from obspy.core.inventory import Inventory, Network, Station, Channel, Site, \
+        Latitude, Longitude
 
     # creating the overall inventory file
     inv = Inventory(
         # We'll add networks later.
         networks=[],
         # The source should be the id whoever create the file.
         source="esg")
@@ -562,15 +552,16 @@
         for tr in st_new:
             cha = Channel(
                 # This is the channel code according to the SEED standard.
                 code=tr.stats.channel,
                 # This is the location code according to the SEED standard.
                 location_code=tr.stats.location,
                 # Note that these coordinates can differ from the station coordinates.
-                latitude=Latitude(10.),  # these other parameters don't matter for rotation
+                latitude=Latitude(10.),
+                # these other parameters don't matter for rotation
                 longitude=Longitude(120.),
                 elevation=0.,
                 depth=1.,
                 azimuth=tr.stats.azimuth,
                 dip=tr.stats.dip,
                 sample_rate=tr.stats.sampling_rate)
 
@@ -614,19 +605,21 @@
                       base_vector_2,
                       base_vector_3])
         det = np.linalg.det(m)
 
         # if determinant is less than 0.99 then don't rotate the trace
         if abs(det) < 0.99:
             if log is False:
-                print('Station: ' + st[0].stats.station + ' cannot be rotated due to cosines \n '
-                      'not combining to unit vector')
+                print('Station: ' + st[
+                    0].stats.station + ' cannot be rotated due to cosines \n '
+                                       'not combining to unit vector')
             else:
-                logging.info('Station: ' + st[0].stats.station + ' cannot be rotated due to cosines \n '
-                             'not combining to unit vector')
+                logging.info('Station: ' + st[
+                    0].stats.station + ' cannot be rotated due to cosines \n '
+                                       'not combining to unit vector')
             # returning False if the station cannot be rotated
             return False
         else:
             return True
     else:
         # for uniaxial stations let obspy figure itself out
         return True
@@ -636,15 +629,16 @@
     """
     Pass through function
     """
     print('Function readhsf has been renamed to read_hsf.')
     read_hsf(**kwargs)
 
 
-def read_hsf(file, head_only=False, footer=0, groundmotion=False, print_out=True, stdout=True, from_hsf_to_obspy=False):
+def read_hsf(file, head_only=False, footer=0, groundmotion=False, print_out=True,
+             stdout=True, from_hsf_to_obspy=False):
     """
     Function to read hsf files into a python format, kind of magic, based on old code from
     Mike Preiksaitis and Lindsay Smith
     Author: Joshua Williams (joshua.williams@esgsolutions.com)
     :param file: name of the file to read the data from
     :param head_only: whether to only output the header info, defaults to 0 which is False
     :param footer: whether to include the footer info, as in the editing information for the program
@@ -746,22 +740,24 @@
     for isen in range(nsens):
         stp.append(int(struct.unpack('i', hrem[senh:senh + 4])[0]))
         nch_sen.append(int(struct.unpack('i', hrem[senh + 4:senh + 8])[0]))
         pos.append(np.array(struct.unpack('3f', hrem[senh + 12:senh + 24])))
         snstvt.append(np.array(struct.unpack('f', hrem[senh + 24:senh + 28]))[0])
         ttt.append(np.array(struct.unpack('2f', hrem[senh + 32:senh + 40])))
         rot_win.append(np.array(struct.unpack('2i', hrem[senh + 40:senh + 48])))
-        eig_rot.append(np.array(struct.unpack('9f', hrem[senh + 48:senh + 84])).reshape(3, 3))
+        eig_rot.append(
+            np.array(struct.unpack('9f', hrem[senh + 48:senh + 84])).reshape(3, 3))
         eig_val.append(np.array(struct.unpack('3f', hrem[senh + 84:senh + 96])))
         # print('sensor')
         # print(pos[isen])
         # print('event')
         # print(head['source'])
-        dis.append(np.math.sqrt((pos[isen][0] - head['source'][0]) ** 2 + (pos[isen][1] - head['source'][1]) ** 2 + (
-                pos[isen][2] - head['source'][2]) ** 2))
+        dis.append(np.math.sqrt((pos[isen][0] - head['source'][0]) ** 2 + (
+                    pos[isen][1] - head['source'][1]) ** 2 + (
+                                        pos[isen][2] - head['source'][2]) ** 2))
 
         dir_error.append(np.array(struct.unpack('3f', hrem[senh + 96:senh + 108])))
         sensor_id.append(struct.unpack('h', hrem[senh + 108:senh + 110])[0])
         station_ind.append(int(struct.unpack('i', hrem[senh + 110:senh + 114])[0]))
         pre_amp.append(np.array(struct.unpack('f', hrem[senh + 114:senh + 118]))[0])
         enabled.append(bool(struct.unpack('i', hrem[senh + 118:senh + 122])[0]))
         sensor_name.append(str(hrem[senh + 122:senh + 134]).split('\\x00')[0])
@@ -818,33 +814,36 @@
     head['senmodel'] = senmodel
     head['p_snr'] = p_snr
     head['s_snr'] = s_snr
     head['vp_sensor'], head['vs_sensor'] = vp, vs
     head['volt_range'] = volt_range
 
     # performing a quick check to see if any of the sensors are accelerometers and printing a warning if they are
-    possible_types = ['GEOPHONE', 'ACCELEROMETER', 'SGM_GEOPHONE', 'FBA_ACCELEROMETER', 'BVM_MICROPHONE']
+    possible_types = ['GEOPHONE', 'ACCELEROMETER', 'SGM_GEOPHONE', 'FBA_ACCELEROMETER',
+                      'BVM_MICROPHONE']
     for count in range(len(head['stype'])):
         actual_type = possible_types[head['stype'][count]]
-        if (actual_type == 'ACCELEROMETER' or actual_type == 'FBA_ACCELEROMETER') and print_out is True and \
+        if (
+                actual_type == 'ACCELEROMETER' or actual_type == 'FBA_ACCELEROMETER') and print_out is True and \
                 from_hsf_to_obspy is True:
-            print('BEWARE you will need to adjust the data for accelerometers by multiplying by 9.81\n'
-                  'Using hsf_to_obspy will automatically do this for you though.')
+            print(
+                'BEWARE you will need to adjust the data for accelerometers by multiplying by 9.81\n'
+                'Using hsf_to_obspy will automatically do this for you though.')
             break
 
     gain, ch_snstvt, descr = [], [], []
     ch_enabled = []
     low_f, high_f = [], []
     rms_amp, peak_amp = [], []
     sen_rot, parr, sarr, harr, varr = [], [], [], [], []
     p_pol, sv_pol, sh_pol = [], [], []
     p_pol_old, sv_pol_old, sh_pol_old = [], [], []
     omega_p, omega_s, corner_p, corner_s, energy_p, energy_s = [], [], [], [], [], []
     omega_sv, omega_sh, corner_sv, corner_sh, energy_sv, energy_sh = [], [], [], [], [], []
-    acq_chan_ind,  ppick_used, spick_used = [], [], []
+    acq_chan_ind, ppick_used, spick_used = [], [], []
     valid_flag_pickused, valid_flag_newpolarity, valid_flag_sensorhealthknown = [], [], []
     valid_flag_sensorhealth, valid_flag_sensorhealthcheck, valid_flag_sensorusedintriggering = [], [], []
     valid_flag_channelbad = []
     raw_descr = []
 
     for isen in range(nsens):
         ori = []
@@ -852,16 +851,18 @@
         p_pol.append(float(struct.unpack('h', hrem[senh + 94:senh + 96])[0]) / 32767.)
         p_pol_old.append(struct.unpack('h', hrem[senh + 52:senh + 54])[0])
 
         if nch_sen[isen] == 3:
             sarr.append(np.array(struct.unpack('f', hrem[senh + 62:senh + 66])))
             varr.append(np.array(struct.unpack('f', hrem[senh + 220:senh + 224])))
             harr.append(np.array(struct.unpack('f', hrem[senh + 378:senh + 382])))
-            sv_pol.append(float(struct.unpack('h', hrem[senh + 254:senh + 256])[0]) / 32767.)
-            sh_pol.append(float(struct.unpack('h', hrem[senh + 412:senh + 414])[0]) / 32767.)
+            sv_pol.append(
+                float(struct.unpack('h', hrem[senh + 254:senh + 256])[0]) / 32767.)
+            sh_pol.append(
+                float(struct.unpack('h', hrem[senh + 412:senh + 414])[0]) / 32767.)
             sv_pol_old.append(struct.unpack('h', hrem[senh + 212:senh + 214])[0])
             sh_pol_old.append(struct.unpack('h', hrem[senh + 370:senh + 372])[0])
             omega_p.append(np.array(struct.unpack('f', hrem[senh + 98:senh + 102])))
             omega_s.append(np.array(struct.unpack('f', hrem[senh + 102:senh + 106])))
             corner_p.append(np.array(struct.unpack('f', hrem[senh + 106:senh + 110])))
             corner_s.append(np.array(struct.unpack('f', hrem[senh + 110:senh + 114])))
             energy_p.append(np.array(struct.unpack('f', hrem[senh + 114:senh + 118])))
@@ -871,38 +872,46 @@
                 gain.append(struct.unpack('f', hrem[senh + 8:senh + 12])[0])
                 ori.append(np.array(struct.unpack('3f', hrem[senh + 12:senh + 24])))
                 low_f.append(struct.unpack('f', hrem[senh + 24:senh + 28])[0])
                 high_f.append(struct.unpack('f', hrem[senh + 28:senh + 32])[0])
                 rms_amp.append(struct.unpack('f', hrem[senh + 44:senh + 48])[0])
                 peak_amp.append(struct.unpack('f', hrem[senh + 48:senh + 52])[0])
                 ch_snstvt.append(struct.unpack('f', hrem[senh + 66:senh + 70])[0])
-                descr.append(hrem[senh + 70:senh + 87].decode('ISO-8859-1').rstrip("\x00"))  # 17 char
+                descr.append(hrem[senh + 70:senh + 87].decode('ISO-8859-1').rstrip(
+                    "\x00"))  # 17 char
                 acq_chan_ind.append(struct.unpack('h', hrem[senh + 87:senh + 89])[0])
                 ppick_used.append(struct.unpack('h', hrem[senh + 89:senh + 91])[0])
                 spick_used.append(struct.unpack('h', hrem[senh + 91:senh + 93])[0])
 
                 # pulling out the valid flags
                 temp = hrem[senh + 93:senh + 94]
-                vf_pickused, vf_polarity, vf_shk, vf_sh, vf_shc, vf_strig, vf_bad = extract_valid_flags(temp)
+                vf_pickused, vf_polarity, vf_shk, vf_sh, vf_shc, vf_strig, vf_bad = extract_valid_flags(
+                    temp)
                 valid_flag_pickused.append(vf_pickused)
                 valid_flag_newpolarity.append(vf_polarity)
                 valid_flag_sensorhealthknown.append(vf_shk)
                 valid_flag_sensorhealth.append(vf_sh)
                 valid_flag_sensorhealthcheck.append(vf_shc)
                 valid_flag_sensorusedintriggering.append(vf_strig)
                 valid_flag_channelbad.append(vf_bad)
 
                 if ich == 1:
-                    omega_sv.append(np.array(struct.unpack('f', hrem[senh + 102:senh + 106])))
-                    corner_sv.append(np.array(struct.unpack('f', hrem[senh + 110:senh + 114])))
-                    energy_sv.append(np.array(struct.unpack('f', hrem[senh + 118:senh + 122])))
+                    omega_sv.append(
+                        np.array(struct.unpack('f', hrem[senh + 102:senh + 106])))
+                    corner_sv.append(
+                        np.array(struct.unpack('f', hrem[senh + 110:senh + 114])))
+                    energy_sv.append(
+                        np.array(struct.unpack('f', hrem[senh + 118:senh + 122])))
                 elif ich == 2:
-                    omega_sh.append(np.array(struct.unpack('f', hrem[senh + 102:senh + 106])))
-                    corner_sh.append(np.array(struct.unpack('f', hrem[senh + 110:senh + 114])))
-                    energy_sh.append(np.array(struct.unpack('f', hrem[senh + 118:senh + 122])))
+                    omega_sh.append(
+                        np.array(struct.unpack('f', hrem[senh + 102:senh + 106])))
+                    corner_sh.append(
+                        np.array(struct.unpack('f', hrem[senh + 110:senh + 114])))
+                    energy_sh.append(
+                        np.array(struct.unpack('f', hrem[senh + 118:senh + 122])))
 
                 senh = senh + 158
         elif nch_sen[isen] == 1:
             sarr.append(np.array(struct.unpack('f', hrem[senh + 62:senh + 66])))
             harr.append(np.array([np.nan]))
             varr.append(np.array([np.nan]))
             # sv_pol.append(float(struct.unpack('h',hrem[senh+254:senh+256])[0])/32767.)
@@ -911,15 +920,16 @@
             sh_pol_old.append(struct.unpack('h', hrem[senh + 54: senh + 56])[0])
             acq_chan_ind.append(struct.unpack('h', hrem[senh + 87:senh + 89])[0])
             ppick_used.append(struct.unpack('h', hrem[senh + 89:senh + 91])[0])
             spick_used.append(struct.unpack('h', hrem[senh + 91:senh + 93])[0])
 
             # pulling out the valid flags
             temp = hrem[senh + 93:senh + 94]
-            vf_pickused, vf_polarity, vf_shk, vf_sh, vf_shc, vf_strig, vf_bad = extract_valid_flags(temp)
+            vf_pickused, vf_polarity, vf_shk, vf_sh, vf_shc, vf_strig, vf_bad = extract_valid_flags(
+                temp)
             valid_flag_pickused.append(vf_pickused)
             valid_flag_newpolarity.append(vf_polarity)
             valid_flag_sensorhealthknown.append(vf_shk)
             valid_flag_sensorhealth.append(vf_sh)
             valid_flag_sensorhealthcheck.append(vf_shc)
             valid_flag_sensorusedintriggering.append(vf_strig)
             valid_flag_channelbad.append(vf_bad)
@@ -1030,16 +1040,18 @@
         directories = str(footerblobdirectory).split('\\n')[1:]
 
         for d in directories:
             if '=' in d:
                 report, index = d.split('=')
                 index = np.int(index)
                 length = struct.unpack('I', n[index - offset + len(report) +
-                                              2 + 1:index - offset + len(report) + 2 + 4 + 1])[0]
-                data = n[index - offset + len(report) + 2 + 4 + 1:index - offset + len(report) + 2 + 4 + 1 + length]
+                                              2 + 1:index - offset + len(
+                    report) + 2 + 4 + 1])[0]
+                data = n[index - offset + len(report) + 2 + 4 + 1:index - offset + len(
+                    report) + 2 + 4 + 1 + length]
                 # parse report into dictionary
                 try:
                     buf = StringIO(data.decode())
                     cfg = configparser.ConfigParser()
                     cfg.read_file(buf)
                     # noinspection PyProtectedMember
                     data_dict = dict(cfg._sections)
@@ -1051,15 +1063,16 @@
 
         # find event history
         historystart = allfooter_str.find('<<SEVHistory:') + 15
         historyend = allfooter_str.find('>>', historystart)
 
         evthistory = allfooter_str[historystart:historyend]
         evthistory_header = ['ModTime', 'UserName', 'Program', 'Type', 'Action']
-        evthistory = pd.read_csv(StringIO(evthistory.replace('####', '\n').replace('##', ',').replace('|', ',')),
+        evthistory = pd.read_csv(StringIO(
+            evthistory.replace('####', '\n').replace('##', ',').replace('|', ',')),
                                  header=None, names=evthistory_header)
 
         # getting the valid start and end times
         try:
             validstart = allfooter_str.find('<<ValidStart:') + len('<<ValidStart:')
             validend = allfooter_str.find('>>', validstart)
             lastvalidstart = allfooter_str.find('<<LastValid:') + len('<<LastValid:')
@@ -1078,40 +1091,45 @@
     else:  # If we want to also read the waveform data then continue
 
         hsfcompressor = r"C:\esg\hsfcompressor.exe"  # location of the hsf compressor program
 
         # if compressed check the platform
         if head['compress'] != 0:
             if not glob.os.path.exists(hsfcompressor) and os.name == 'nt':
-                raise Exception("HSF file is compressed or resampled and HSFCompressor is missing. "
-                                "Install Hsfcompress.exe to c:\\esg_utils")
-            elif os.name != 'nt' and not glob.os.path.exists('/home/share/wine/HSFCompressor.exe'):
-                raise Exception("HSF file is compressed or resampled and HSFCompressor is missing on linux. "
-                                "Install Hsfcompress.exe to /home/share/wine")
+                raise Exception(
+                    "HSF file is compressed or resampled and HSFCompressor is missing. "
+                    "Install Hsfcompress.exe to c:\\esg_utils")
+            elif os.name != 'nt' and not glob.os.path.exists(
+                    '/home/share/wine/HSFCompressor.exe'):
+                raise Exception(
+                    "HSF file is compressed or resampled and HSFCompressor is missing on linux. "
+                    "Install Hsfcompress.exe to /home/share/wine")
 
         if os.name != "nt":
             # if we are on the jupyter server
             # adjusting the path of the hsf compressor call
             hsfcompressor = '/usr/bin/wine /home/share/wine/HSFCompressor.exe'
 
         if stdout:
             # Stdout option exists to directly pass waveform data to python
             logging.info('decompressing the HSFfile')
-            p = Popen(hsfcompressor + ' -none -stdout ' + file, stdout=PIPE, stderr=PIPE, shell=True)
+            p = Popen(hsfcompressor + ' -none -stdout ' + file, stdout=PIPE, stderr=PIPE,
+                      shell=True)
             hbin = ''
             err = ''
             try:
                 hbin, err = p.communicate()
             except IOError:
                 print('IOError: ' + str(IOError))
             if hbin == '':
                 print('Output returned is blank.' + err)
             hbin = hbin[wfst:]  # Remove header
         else:  # old method: uncompress, read in, and then recompress
-            if head['compress'] != 0 or head['resample'] != 0:  # if the header says the file is compressed or resampled
+            if head['compress'] != 0 or head[
+                'resample'] != 0:  # if the header says the file is compressed or resampled
                 f.close()  # close the file so that we can uncompress it
                 _ = call(hsfcompressor + ' -none ' + file, shell=True)  # uncompress file
 
             try:
                 f = open(file, 'rb')  # reopen the uncompressed file
             except FileNotFoundError:
                 time.sleep(30)
@@ -1121,20 +1139,24 @@
                     print('File not found!')
                     return None, None, None
 
             f.seek(wfst)  # jump past the header
             hbin = f.read()  # read in the rest of the data
             f.close()
 
-            if head['compress'] != 0 or head['resample']:  # if the file was compressed lets recompress it
+            if head['compress'] != 0 or head[
+                'resample']:  # if the file was compressed lets recompress it
                 resamp_args = ''
                 if head['resample'] != 0:
-                    downsample = head['resample'] & 0x0F  # last 4 bits store downsampling
-                    upsample = (head['resample'] & 0xF0) >> 4  # first 4 bits store upsampling
-                    resamp_args = '-decimate ' + str(downsample) + ' -upsample ' + str(upsample) + ' '
+                    downsample = head[
+                                     'resample'] & 0x0F  # last 4 bits store downsampling
+                    upsample = (head[
+                                    'resample'] & 0xF0) >> 4  # first 4 bits store upsampling
+                    resamp_args = '-decimate ' + str(downsample) + ' -upsample ' + str(
+                        upsample) + ' '
                 p = call(hsfcompressor + ' -rice ' + resamp_args + file, shell=True)
 
         num_elements = nch * npt
         frmt = str(num_elements) + 'i'
 
         # this is for cases where I was having issues with files that did not have the correct amount of buffer for the 
         # given data size - not sure on the cause of this error but for now including this workaround
@@ -1189,15 +1211,16 @@
         #
         #     # iterating the variable to count through the number of traces in the station
         #     stcount += 1
 
         return tm, data_array, head
 
 
-def read_hsf_exp(file, head_only=0, footer=0, groundmotion=False, print_out=True, from_hsf_to_obspy=False, s3data=None,
+def read_hsf_exp(file, head_only=0, footer=0, groundmotion=False, print_out=True,
+                 from_hsf_to_obspy=False, s3data=None,
                  force_python_decompress=False):
     """
     Function to read hsf files into a python format, kind of magic, based on old code from
     Mike Preiksaitis and Lindsay Smith
     Author: Joshua Williams (joshua.williams@esgsolutions.com)
     Experimental version using numpy to extract values from buffer
     :param file: name of the file to read the data from
@@ -1305,82 +1328,112 @@
     else:
         hrem = s3data[309: wfst]
 
     dis, sensor_name = [], []
 
     senh = 26 * npal
     srd = 222
-    head['stype'] = np.ndarray((nsens,), buffer=hrem, offset=senh, dtype='i', strides=(srd,))
-    head['nch_sen'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 4, dtype='i', strides=(srd,))
-    head['pos'] = np.ndarray((nsens, 3), buffer=hrem, offset=senh + 12, dtype='f', strides=(srd, 4))
-    head['snstvt'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 24, dtype='f', strides=(srd,))
-    head['ttt'] = np.ndarray((nsens, 2), buffer=hrem, offset=senh + 32, dtype='f', strides=(srd, 4))
-    head['rot_win'] = np.ndarray((nsens, 2), buffer=hrem, offset=senh + 40, dtype='i', strides=(srd, 4))
-    eig_rot = np.ndarray((nsens, 9), buffer=hrem, offset=senh + 48, dtype='f', strides=(srd, 4))
+    head['stype'] = np.ndarray((nsens,), buffer=hrem, offset=senh, dtype='i',
+                               strides=(srd,))
+    head['nch_sen'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 4, dtype='i',
+                                 strides=(srd,))
+    head['pos'] = np.ndarray((nsens, 3), buffer=hrem, offset=senh + 12, dtype='f',
+                             strides=(srd, 4))
+    head['snstvt'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 24, dtype='f',
+                                strides=(srd,))
+    head['ttt'] = np.ndarray((nsens, 2), buffer=hrem, offset=senh + 32, dtype='f',
+                             strides=(srd, 4))
+    head['rot_win'] = np.ndarray((nsens, 2), buffer=hrem, offset=senh + 40, dtype='i',
+                                 strides=(srd, 4))
+    eig_rot = np.ndarray((nsens, 9), buffer=hrem, offset=senh + 48, dtype='f',
+                         strides=(srd, 4))
     # making the copy to allow the array to be reshaped
     eig_rot = eig_rot.copy()
     head['eig_rot'] = eig_rot.reshape(nsens, 3, 3)
-    head['eig_val'] = np.ndarray((nsens, 3), buffer=hrem, offset=senh + 84, dtype='f', strides=(srd, 4))
-    head['dir_error'] = np.ndarray((nsens, 3), buffer=hrem, offset=senh + 96, dtype='f', strides=(srd, 4))
-    head['sensor_id'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 108, dtype='h', strides=(srd,))
-    head['station_ind'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 110, dtype='i', strides=(srd,))
-    head['pre_amp'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 114, dtype='f', strides=(srd,))
-    head['enabled'] = np.array(np.ndarray((nsens,), buffer=hrem, offset=senh + 118, dtype='i', strides=(srd,)),
-                               dtype=bool)
+    head['eig_val'] = np.ndarray((nsens, 3), buffer=hrem, offset=senh + 84, dtype='f',
+                                 strides=(srd, 4))
+    head['dir_error'] = np.ndarray((nsens, 3), buffer=hrem, offset=senh + 96, dtype='f',
+                                   strides=(srd, 4))
+    head['sensor_id'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 108, dtype='h',
+                                   strides=(srd,))
+    head['station_ind'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 110, dtype='i',
+                                     strides=(srd,))
+    head['pre_amp'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 114, dtype='f',
+                                 strides=(srd,))
+    head['enabled'] = np.array(
+        np.ndarray((nsens,), buffer=hrem, offset=senh + 118, dtype='i', strides=(srd,)),
+        dtype=bool)
     # TODO incomplete data is accurate, not sure about bad sync and enabled though
-    head['bad_sync'] = np.array(np.ndarray((nsens,), buffer=hrem, offset=senh + 134, dtype='i', strides=(srd,)),
-                                dtype=bool)
-    head['incomplete_data'] = np.array(np.ndarray((nsens,), buffer=hrem, offset=senh + 144, dtype='i', strides=(srd,)),
-                                       dtype=bool)
-    head['raydir'] = np.ndarray((nsens, 3), buffer=hrem, offset=senh + 154, dtype='f', strides=(srd, 4))
-    head['sv_ttt'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 166, dtype='f', strides=(srd,))
+    head['bad_sync'] = np.array(
+        np.ndarray((nsens,), buffer=hrem, offset=senh + 134, dtype='i', strides=(srd,)),
+        dtype=bool)
+    head['incomplete_data'] = np.array(
+        np.ndarray((nsens,), buffer=hrem, offset=senh + 144, dtype='i', strides=(srd,)),
+        dtype=bool)
+    head['raydir'] = np.ndarray((nsens, 3), buffer=hrem, offset=senh + 154, dtype='f',
+                                strides=(srd, 4))
+    head['sv_ttt'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 166, dtype='f',
+                                strides=(srd,))
     # load sensor model
-    head['senmodel'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 170, dtype='h', strides=(srd,))
+    head['senmodel'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 170, dtype='h',
+                                  strides=(srd,))
     # saving what might be the snr values from hsf
-    head['p_snr'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 172, dtype='f', strides=(srd,))
-    head['s_snr'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 176, dtype='f', strides=(srd,))
+    head['p_snr'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 172, dtype='f',
+                               strides=(srd,))
+    head['s_snr'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 176, dtype='f',
+                               strides=(srd,))
     # saving the Q value (attenuation?) and velocity at site
-    head['qp'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 186, dtype='f', strides=(srd,))
-    head['qs'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 190, dtype='f', strides=(srd,))
+    head['qp'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 186, dtype='f',
+                            strides=(srd,))
+    head['qs'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 190, dtype='f',
+                            strides=(srd,))
     # qs and qsv are same byte locations. if qsh does not exist then it is before the two were saved separately
-    head['qsv'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 190, dtype='f', strides=(srd,))
-    head['qsh'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 194, dtype='f', strides=(srd,))
-    head['vp'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 199, dtype='f', strides=(srd,))
-    head['vs'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 203, dtype='f', strides=(srd,))
+    head['qsv'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 190, dtype='f',
+                             strides=(srd,))
+    head['qsh'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 194, dtype='f',
+                             strides=(srd,))
+    head['vp'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 199, dtype='f',
+                            strides=(srd,))
+    head['vs'] = np.ndarray((nsens,), buffer=hrem, offset=senh + 203, dtype='f',
+                            strides=(srd,))
 
     # pulling out the volt range
-    volt_range = np.ndarray((nsens,), buffer=hrem, offset=senh + 207, dtype='f', strides=(srd,))
+    volt_range = np.ndarray((nsens,), buffer=hrem, offset=senh + 207, dtype='f',
+                            strides=(srd,))
     # have to copy it to allow it to be writeable
     volt_range = volt_range.copy()
     # correcting for old files which may have anomalous values above 6 volts
     ix = np.where(np.logical_or(volt_range == 0, volt_range > 6))[0]
     volt_range[ix] = 4.096
 
     # pulling out parameters that are a little trickier
     for isen in range(nsens):
         dis.append(np.math.sqrt((head['pos'][isen][0] - head['source'][0]) ** 2 +
                                 (head['pos'][isen][1] - head['source'][1]) ** 2 + (
-                head['pos'][isen][2] - head['source'][2]) ** 2))
+                                        head['pos'][isen][2] - head['source'][2]) ** 2))
 
         sensor_name.append(str(hrem[senh + 122:senh + 134]).split('\\x00')[0])
         # 10 bits left in dummy as buffer at the end
         senh = senh + srd
 
     head['Distance'] = dis
     head['sensor_name'] = sensor_name
     head['volt_range'] = volt_range
 
     # performing a quick check to see if any of the sensors are accelerometers and printing a warning if they are
-    possible_types = ['GEOPHONE', 'ACCELEROMETER', 'SGM_GEOPHONE', 'FBA_ACCELEROMETER', 'BVM_MICROPHONE']
+    possible_types = ['GEOPHONE', 'ACCELEROMETER', 'SGM_GEOPHONE', 'FBA_ACCELEROMETER',
+                      'BVM_MICROPHONE']
     for count in range(len(head['stype'])):
         actual_type = possible_types[head['stype'][count]]
-        if (actual_type == 'ACCELEROMETER' or actual_type == 'FBA_ACCELEROMETER') and print_out is True and \
+        if (
+                actual_type == 'ACCELEROMETER' or actual_type == 'FBA_ACCELEROMETER') and print_out is True and \
                 from_hsf_to_obspy is True:
-            print('BEWARE you will need to adjust the data for accelerometers by multiplying by 9.81\n'
-                  'Using hsf_to_obspy will automatically do this for you though.')
+            print(
+                'BEWARE you will need to adjust the data for accelerometers by multiplying by 9.81\n'
+                'Using hsf_to_obspy will automatically do this for you though.')
             break
 
     """
     Reading in the channel config from the header
     """
 
     descr, sen_rot = [], []
@@ -1388,103 +1441,141 @@
     valid_flag_sensorhealth, valid_flag_sensorhealthcheck, valid_flag_sensorusedintriggering = [], [], []
     valid_flag_channelbad = []
 
     # replacing what I can with the new approach
     nch_sen = head['nch_sen']
     srd = 158
     nchans = np.sum(nch_sen)
-    head['ch_enabled'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 4, dtype='i', strides=(srd,))
-    head['gain'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 8, dtype='f', strides=(srd,))
-    head['low_f'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 24, dtype='f', strides=(srd,))
-    head['high_f'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 28, dtype='f', strides=(srd,))
-    head['rms_amp'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 44, dtype='f', strides=(srd,))
-    head['peak_amp'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 48, dtype='f', strides=(srd,))
-    head['p_pol_old'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 52, dtype='h', strides=(srd,)),
-                                     nch_sen)
-    head['sv_pol_old'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 54, dtype='h', strides=(srd,)),
-                                      nch_sen, keep_ind=1)
-    head['sh_pol_old'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 54, dtype='h', strides=(srd,)),
-                                      nch_sen, keep_ind=-1)
-    head['parr'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 58, dtype='f', strides=(srd,)),
-                                nch_sen)
-    head['sarr'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 62, dtype='f', strides=(srd,)),
-                                nch_sen)
-    head['varr'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 62, dtype='f', strides=(srd,)),
-                                nch_sen, keep_ind=1)
-    head['harr'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 62, dtype='f', strides=(srd,)),
-                                nch_sen, keep_ind=-1)
-    head['ch_snstvt'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 66, dtype='f', strides=(srd,))
+    head['ch_enabled'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 4, dtype='i',
+                                    strides=(srd,))
+    head['gain'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 8, dtype='f',
+                              strides=(srd,))
+    head['low_f'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 24, dtype='f',
+                               strides=(srd,))
+    head['high_f'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 28, dtype='f',
+                                strides=(srd,))
+    head['rms_amp'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 44, dtype='f',
+                                 strides=(srd,))
+    head['peak_amp'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 48, dtype='f',
+                                  strides=(srd,))
+    head['p_pol_old'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 52, dtype='h', strides=(srd,)),
+        nch_sen)
+    head['sv_pol_old'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 54, dtype='h', strides=(srd,)),
+        nch_sen, keep_ind=1)
+    head['sh_pol_old'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 54, dtype='h', strides=(srd,)),
+        nch_sen, keep_ind=-1)
+    head['parr'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 58, dtype='f', strides=(srd,)),
+        nch_sen)
+    head['sarr'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 62, dtype='f', strides=(srd,)),
+        nch_sen)
+    head['varr'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 62, dtype='f', strides=(srd,)),
+        nch_sen, keep_ind=1)
+    head['harr'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 62, dtype='f', strides=(srd,)),
+        nch_sen, keep_ind=-1)
+    head['ch_snstvt'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 66, dtype='f',
+                                   strides=(srd,))
     # descr is pulled from here
-    head['acq_chan_ind'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 87, dtype='h', strides=(srd,))
-    head['ppick_used'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 89, dtype='h', strides=(srd,))
-    head['spick_used'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 91, dtype='h', strides=(srd,))
-    p_pol = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 94, dtype='h', strides=(srd,)), nch_sen)
+    head['acq_chan_ind'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 87,
+                                      dtype='h', strides=(srd,))
+    head['ppick_used'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 89, dtype='h',
+                                    strides=(srd,))
+    head['spick_used'] = np.ndarray((nchans,), buffer=hrem, offset=senh + 91, dtype='h',
+                                    strides=(srd,))
+    p_pol = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 94, dtype='h', strides=(srd,)),
+        nch_sen)
     p_pol = p_pol.copy()
     head['p_pol'] = np.divide(p_pol, 32767)
-    sv_pol = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 96, dtype='h', strides=(srd,)), nch_sen,
-                          keep_ind=1)
+    sv_pol = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 96, dtype='h', strides=(srd,)),
+        nch_sen,
+        keep_ind=1)
     sv_pol = sv_pol.copy()
     head['sv_pol'] = np.divide(sv_pol, 32767)
-    sh_pol = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 96, dtype='h', strides=(srd,)), nch_sen,
-                          keep_ind=-1)
+    sh_pol = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 96, dtype='h', strides=(srd,)),
+        nch_sen,
+        keep_ind=-1)
     sh_pol = sh_pol.copy()
     head['sh_pol'] = np.divide(sh_pol, 32767)
-    head['omega_p'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 98, dtype='f', strides=(srd,)),
-                                   nch_sen)
-    head['omega_s'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 102, dtype='f', strides=(srd,)),
-                                   nch_sen)
-    head['corner_p'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 106, dtype='f', strides=(srd,)),
-                                    nch_sen)
-    head['corner_s'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 110, dtype='f', strides=(srd,)),
-                                    nch_sen)
-    head['energy_p'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 114, dtype='f', strides=(srd,)),
-                                    nch_sen)
-    head['energy_s'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 118, dtype='f', strides=(srd,)),
-                                    nch_sen)
-    head['omega_sv'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 102, dtype='f', strides=(srd,)),
-                                    nch_sen, keep_ind=1)
-    head['corner_sv'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 110, dtype='f', strides=(srd,)),
-                                     nch_sen, keep_ind=1)
-    head['energy_sv'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 118, dtype='f', strides=(srd,)),
-                                     nch_sen, keep_ind=1)
-    head['omega_sh'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 102, dtype='f', strides=(srd,)),
-                                    nch_sen, keep_ind=-1)
-    head['corner_sh'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 110, dtype='f', strides=(srd,)),
-                                     nch_sen, keep_ind=-1)
-    head['energy_sh'] = simp_to_chan(np.ndarray((nchans,), buffer=hrem, offset=senh + 118, dtype='f', strides=(srd,)),
-                                     nch_sen, keep_ind=-1)
+    head['omega_p'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 98, dtype='f', strides=(srd,)),
+        nch_sen)
+    head['omega_s'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 102, dtype='f', strides=(srd,)),
+        nch_sen)
+    head['corner_p'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 106, dtype='f', strides=(srd,)),
+        nch_sen)
+    head['corner_s'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 110, dtype='f', strides=(srd,)),
+        nch_sen)
+    head['energy_p'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 114, dtype='f', strides=(srd,)),
+        nch_sen)
+    head['energy_s'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 118, dtype='f', strides=(srd,)),
+        nch_sen)
+    head['omega_sv'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 102, dtype='f', strides=(srd,)),
+        nch_sen, keep_ind=1)
+    head['corner_sv'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 110, dtype='f', strides=(srd,)),
+        nch_sen, keep_ind=1)
+    head['energy_sv'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 118, dtype='f', strides=(srd,)),
+        nch_sen, keep_ind=1)
+    head['omega_sh'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 102, dtype='f', strides=(srd,)),
+        nch_sen, keep_ind=-1)
+    head['corner_sh'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 110, dtype='f', strides=(srd,)),
+        nch_sen, keep_ind=-1)
+    head['energy_sh'] = simp_to_chan(
+        np.ndarray((nchans,), buffer=hrem, offset=senh + 118, dtype='f', strides=(srd,)),
+        nch_sen, keep_ind=-1)
 
     # the loop originally in the function
     for isen in range(nsens):
         ori = []
 
         if nch_sen[isen] == 3:
             for ich in range(3):
                 # pulling out the valid flags
                 temp = hrem[senh + 93:senh + 94]
-                vf_pickused, vf_polarity, vf_shk, vf_sh, vf_shc, vf_strig, vf_bad = extract_valid_flags(temp)
+                vf_pickused, vf_polarity, vf_shk, vf_sh, vf_shc, vf_strig, vf_bad = extract_valid_flags(
+                    temp)
                 valid_flag_pickused.append(vf_pickused)
                 valid_flag_newpolarity.append(vf_polarity)
                 valid_flag_sensorhealthknown.append(vf_shk)
                 valid_flag_sensorhealth.append(vf_sh)
                 valid_flag_sensorhealthcheck.append(vf_shc)
                 valid_flag_sensorusedintriggering.append(vf_strig)
                 valid_flag_channelbad.append(vf_bad)
 
                 # and the other values
                 ori.append(np.array(struct.unpack('3f', hrem[senh + 12:senh + 24])))
-                descr.append(hrem[senh + 70:senh + 87].decode('ISO-8859-1').rstrip("\x00"))  # 17 char
+                descr.append(hrem[senh + 70:senh + 87].decode('ISO-8859-1').rstrip(
+                    "\x00"))  # 17 char
                 senh = senh + srd
         elif nch_sen[isen] == 1:
             ori.append(np.array(struct.unpack('3f', hrem[senh + 12:senh + 24])))
             descr.append(hrem[senh + 70:senh + 87].decode('ISO-8859-1').rstrip("\x00"))
 
             # pulling out the valid flags
             temp = hrem[senh + 93:senh + 94]
-            vf_pickused, vf_polarity, vf_shk, vf_sh, vf_shc, vf_strig, vf_bad = extract_valid_flags(temp)
+            vf_pickused, vf_polarity, vf_shk, vf_sh, vf_shc, vf_strig, vf_bad = extract_valid_flags(
+                temp)
             valid_flag_pickused.append(vf_pickused)
             valid_flag_newpolarity.append(vf_polarity)
             valid_flag_sensorhealthknown.append(vf_shk)
             valid_flag_sensorhealth.append(vf_sh)
             valid_flag_sensorhealthcheck.append(vf_shc)
             valid_flag_sensorusedintriggering.append(vf_strig)
             valid_flag_channelbad.append(vf_bad)
@@ -1493,15 +1584,16 @@
         sen_rot.append(np.array(ori))
 
     head['valid_flag_pickused'] = np.array(valid_flag_pickused)
     head['valid_flag_newpolarity'] = np.array(valid_flag_newpolarity)
     head['valid_flag_sensorhealth'] = np.array(valid_flag_sensorhealth)
     head['valid_flag_sensorhealthknown'] = np.array(valid_flag_sensorhealthknown)
     head['valid_flag_sensorhealthcheck'] = np.array(valid_flag_sensorhealthcheck)
-    head['valid_flag_sensorusedintriggering'] = np.array(valid_flag_sensorusedintriggering)
+    head['valid_flag_sensorusedintriggering'] = np.array(
+        valid_flag_sensorusedintriggering)
     head['valid_flag_channelbad'] = np.array(valid_flag_channelbad)
     head['sen_rot'] = sen_rot
     head['ch_descr'] = descr
 
     """
     If we want the footer
     """
@@ -1549,16 +1641,18 @@
         directories = str(footerblobdirectory).split('\\n')[1:]
 
         for d in directories:
             if '=' in d:
                 report, index = d.split('=')
                 index = np.int(index)
                 length = struct.unpack('I', n[index - offset + len(report) +
-                                              2 + 1:index - offset + len(report) + 2 + 4 + 1])[0]
-                data = n[index - offset + len(report) + 2 + 4 + 1:index - offset + len(report) + 2 + 4 + 1 + length]
+                                              2 + 1:index - offset + len(
+                    report) + 2 + 4 + 1])[0]
+                data = n[index - offset + len(report) + 2 + 4 + 1:index - offset + len(
+                    report) + 2 + 4 + 1 + length]
                 # parse report into dictionary
                 try:
                     buf = StringIO(data.decode())
                     cfg = configparser.ConfigParser()
                     cfg.read_file(buf)
                     # noinspection PyProtectedMember
                     data_dict = dict(cfg._sections)
@@ -1572,15 +1666,16 @@
 
         # find event history
         historystart = allfooter_str.find('<<SEVHistory:') + 15
         historyend = allfooter_str.find('>>', historystart)
 
         evthistory = allfooter_str[historystart:historyend]
         evthistory_header = ['ModTime', 'UserName', 'Program', 'Type', 'Action']
-        evthistory = pd.read_csv(StringIO(evthistory.replace('####', '\n').replace('##', ',').replace('|', ',')),
+        evthistory = pd.read_csv(StringIO(
+            evthistory.replace('####', '\n').replace('##', ',').replace('|', ',')),
                                  header=None, names=evthistory_header)
 
         # getting the valid start and end times
         try:
             validstart = allfooter_str.find('<<ValidStart:') + len('<<ValidStart:')
             validend = allfooter_str.find('>>', validstart)
             lastvalidstart = allfooter_str.find('<<LastValid:') + len('<<LastValid:')
@@ -1620,29 +1715,35 @@
         data_array = None
         # if compressed check the platform and extract the data using hsf compressor
         if head['compress'] != 0:
             # make sure the hsf compressor exists
             if not glob.os.path.exists(hsfcompressor) and os.name == 'nt':
                 hsf_compress_exists = False
                 if print_out:
-                    print("HSF file is compressed or resampled and HSFCompressor is missing. "
-                          "Install Hsfcompress.exe to c:\\esg_utils")
-                    print('Instead using the in-Python approach, which is significantly slower')
-            elif os.name != 'nt' and not glob.os.path.exists('/home/share/wine/HSFCompressor.exe'):
+                    print(
+                        "HSF file is compressed or resampled and HSFCompressor is missing. "
+                        "Install Hsfcompress.exe to c:\\esg_utils")
+                    print(
+                        'Instead using the in-Python approach, which is significantly slower')
+            elif os.name != 'nt' and not glob.os.path.exists(
+                    '/home/share/wine/HSFCompressor.exe'):
                 hsf_compress_exists = False
                 if print_out:
-                    print("HSF file is compressed or resampled and HSFCompressor is missing on linux. "
-                          "Install Hsfcompress.exe to /home/share/wine")
-                    print('Instead using the in-Python approach, which is significantly slower')
+                    print(
+                        "HSF file is compressed or resampled and HSFCompressor is missing on linux. "
+                        "Install Hsfcompress.exe to /home/share/wine")
+                    print(
+                        'Instead using the in-Python approach, which is significantly slower')
 
             # running hsf compressor if it is present
             if hsf_compress_exists:
                 # running the hsf compressor to extract the data
                 # data is directly piped into Python
-                p = Popen(hsfcompressor + ' -none -stdout ' + file, stdout=PIPE, stderr=PIPE, shell=True)
+                p = Popen(hsfcompressor + ' -none -stdout ' + file, stdout=PIPE,
+                          stderr=PIPE, shell=True)
                 hbin = ''
                 err = ''
                 try:
                     hbin, err = p.communicate()
                 except IOError:
                     print('IOError: ' + str(IOError))
                 if hbin == '':
@@ -1670,22 +1771,25 @@
                     # if it is waveless, then we will need to read the data from the other file
                     # getting the file name
                     thbin = hbin.decode('cp437')
                     tfname = makeLinuxPath(thbin.split('.hsf')[0] + '.hsf')
 
                     # reading the data
                     # TODO risk of recursion here?
-                    ttm, data_array, thead = read_hsf_exp(tfname, head_only=head_only, footer=footer,
+                    ttm, data_array, thead = read_hsf_exp(tfname, head_only=head_only,
+                                                          footer=footer,
                                                           groundmotion=groundmotion,
-                                                          print_out=print_out, from_hsf_to_obspy=from_hsf_to_obspy,
+                                                          print_out=print_out,
+                                                          from_hsf_to_obspy=from_hsf_to_obspy,
                                                           s3data=s3data,
                                                           force_python_decompress=force_python_decompress)
                 else:
                     # extracting the decompressed data
-                    data_array = decompress_hsf_python(hbin, head['compresssize'], nch, npt, invalid_value=16843009)
+                    data_array = decompress_hsf_python(hbin, head['compresssize'], nch,
+                                                       npt, invalid_value=16843009)
 
         # else if the hsf file is not compressed, we can read the data directly
         else:
             if s3data is None:
                 # opening and reading the file
                 f = open(file, 'rb')
 
@@ -1703,15 +1807,16 @@
 
         # this is for cases where I was having issues with files that did not have the correct amount of buffer for the
         # given data size - not sure on the cause of this error but for now including this workaround
         # IF YOU FIND an example file that is triggering this issue, then please drop me an email at
         # joshua.williams@esgsolutions.com or drop me a line on teams.
         if data_array is None:
             try:
-                data_array = np.ndarray((num_elements,), buffer=hbin, offset=0, dtype='i').copy()
+                data_array = np.ndarray((num_elements,), buffer=hbin, offset=0,
+                                        dtype='i').copy()
             except:
                 print('Something went wrong with the data structure')
                 return None, None, None
 
         # setting bad data values to 0
         ibd = np.where(data_array == 16843009)  # find bad data values
         if len(data_array.shape) == 1:
@@ -1740,15 +1845,16 @@
         for i in range(0, len(data_array)):
             # need to pick the sensitivity
             # iterating through count variable to make sure the snstvt and volt_range is correct
 
             # skip the first iteration because i-1 will cause an error
             # if the station description has changed and we have gone over the number of channels on the
             # sensor, then we must be onto a new station
-            if i != 0 and head['ch_descr'][i] != head['ch_descr'][i - 1] and stcount > head['nch_sen'][count]:
+            if i != 0 and head['ch_descr'][i] != head['ch_descr'][i - 1] and stcount > \
+                    head['nch_sen'][count]:
                 count += 1
                 stcount = 1
 
             # correcting for gain and sensitivity is ground motion is True
             # otherwise just outputting the raw data
             if groundmotion is True:
                 div_value = head['gain'][i] * head['snstvt'][count]
@@ -1884,35 +1990,44 @@
 
     paraminfo, paramunits = [], []
     instdesc, typesen, units, ned, orient, group_ind, group_off = [], [], [], [], [], [], []
 
     # loop over stats_param
     for i in range(head['num_param']):
         # Parameter description
-        paraminfo.append(head_stats_param[i * 128:i * 128 + 64].decode('windows-1252').rstrip("\x00"))
+        paraminfo.append(
+            head_stats_param[i * 128:i * 128 + 64].decode('windows-1252').rstrip("\x00"))
         # Parameter units
-        paramunits.append(head_stats_param[i * 128 + 64:i * 128 + 80].decode('windows-1252').rstrip("\x00"))
+        paramunits.append(
+            head_stats_param[i * 128 + 64:i * 128 + 80].decode('windows-1252').rstrip(
+                "\x00"))
         # windows-1252 decoding seems to be required for accelerometers that have units of m/s2
 
     # Loop over stats_chan
     for i in range(head['num_chan']):
         # instrument description
-        instdesc.append(head_stats_chan[i * 128:128 + i * 128 + 64].decode(errors="replace").split('\x00')[0])
+        instdesc.append(
+            head_stats_chan[i * 128:128 + i * 128 + 64].decode(errors="replace").split(
+                '\x00')[0])
         # type of instrument
-        typesen.append(head_stats_chan[i * 128 + 64:128 + i * 128 + 80].decode(errors="replace").split('\x00')[0])
+        typesen.append(head_stats_chan[i * 128 + 64:128 + i * 128 + 80].decode(
+            errors="replace").split('\x00')[0])
         # units
-        units.append(str(head_stats_chan[i * 128 + 80:128 + i * 128 + 96]).split('\\x00')[0])
+        units.append(
+            str(head_stats_chan[i * 128 + 80:128 + i * 128 + 96]).split('\\x00')[0])
         # NED
         ned.append(struct.unpack('3f', head_stats_chan[i * 128 + 96:i * 128 + 108]))
         # Orient
         orient.append(struct.unpack('3f', head_stats_chan[i * 128 + 108:i * 128 + 120]))
         # group_ind
-        group_ind.append(struct.unpack('i', head_stats_chan[i * 128 + 120:i * 128 + 124])[0])
+        group_ind.append(
+            struct.unpack('i', head_stats_chan[i * 128 + 120:i * 128 + 124])[0])
         # group_offs
-        group_off.append(struct.unpack('i', head_stats_chan[i * 128 + 124:i * 128 + 128])[0])
+        group_off.append(
+            struct.unpack('i', head_stats_chan[i * 128 + 124:i * 128 + 128])[0])
 
     # Add stats_chan info to the header
     head['instdesc'] = instdesc
     head['typesen'] = typesen
     head['units'] = units
     head['ned'] = ned
     head['orient'] = orient
@@ -1926,29 +2041,31 @@
     npts = head['num_param'] * head['num_chan'] * 86400 / head['frame_length']
     npts = int(npts)
     data = struct.unpack(str(npts) + 'f', restofdata[0:npts * 4])
     data = pd.Series(data)
 
     # build list of datetimes to make an index
     t0 = datetime(head['year'], head['month'], head['day'])
-    daterange = pd.date_range(t0, t0.replace(hour=23, minute=59, second=55), freq=str(head['frame_length']) + 's')
+    daterange = pd.date_range(t0, t0.replace(hour=23, minute=59, second=55),
+                              freq=str(head['frame_length']) + 's')
 
     pts_in_a_day = int(86400 / head['frame_length'])
     pts_range = np.arange(0, pts_in_a_day)
     chan_range = np.arange(0, head['num_chan'])
     param_range = np.arange(0, head['num_param'])
 
     dataframes = {}
     for param in param_range:
         # start with a blank zeros dataframe
         df = np.zeros((pts_in_a_day, head['num_chan'], head['num_param']))
         # index = []
         # load in each channel
         for ch in chan_range:
-            index = pts_range * head['num_chan'] * head['num_param'] + ch * head['num_param'] + param
+            index = pts_range * head['num_chan'] * head['num_param'] + ch * head[
+                'num_param'] + param
             df[:, ch, param] = data[index]
 
         dataframes[paraminfo[param]] = pd.DataFrame(df[:, :, param], index=daterange)
         # Check for invalid values and set them to nan
         dataframes[paraminfo[param]].replace(badstatsval, np.nan, inplace=True)
 
     return head, dataframes
@@ -2068,15 +2185,15 @@
 
     if start is None:
         mindate = pd.datetime(1979, 1, 1)
     else:
         mindate = start
 
     if end is None:
-        maxdate = pd.datetime.now()+pd.Timedelta("1 day")
+        maxdate = pd.datetime.now() + pd.Timedelta("1 day")
     else:
         maxdate = end
 
     # filename appendix
     if dsftype == "Stats":
         suffix = ""
     elif dsftype == "Diagnostics":
@@ -2098,28 +2215,31 @@
         rootpath = rootpath[0:-1]
     # extract dsn from rootpath
     dsn = rootpath.split(slash)[-1]
 
     dsffile_list = []
 
     # get all folders in rootpath
-    year_list = [name for name in os.listdir(rootpath) if np.logical_and(os.path.isdir(os.path.join(rootpath, name)),
-                                                                         name.isdigit())]
+    year_list = [name for name in os.listdir(rootpath) if
+                 np.logical_and(os.path.isdir(os.path.join(rootpath, name)),
+                                name.isdigit())]
 
     for year in year_list:
         year_path = rootpath + slash + year
-        month_list = [name for name in os.listdir(year_path) if np.logical_and(os.path.isdir(os.path.join(year_path,
-                                                                                                          name)),
-                                                                               name.isdigit())]
+        month_list = [name for name in os.listdir(year_path) if
+                      np.logical_and(os.path.isdir(os.path.join(year_path,
+                                                                name)),
+                                     name.isdigit())]
 
         for month in month_list:
             month_path = year_path + slash + month
-            day_list = [name for name in os.listdir(month_path) if np.logical_and(os.path.isdir(os.path.join(month_path,
-                                                                                                             name)),
-                                                                                  name.isdigit())]
+            day_list = [name for name in os.listdir(month_path) if
+                        np.logical_and(os.path.isdir(os.path.join(month_path,
+                                                                  name)),
+                                       name.isdigit())]
 
             for day in day_list:
                 # ymd_path = rootpath + slash + year + slash + month + slash + day
                 folder_dt = datetime(int(year), int(month), int(day))
 
                 if np.logical_and(folder_dt >= mindate, folder_dt <= maxdate):
                     # get all dsf files within day folder
@@ -2154,38 +2274,49 @@
     f.close()
 
     import numpy.lib.recfunctions
 
     sensorfile = None
     if ver <= 2.0:
         headers = (
-                   'Description', 'Northing', 'Easting', 'Depth', 'S', 'Type', 'Cmp', 'ID', 'Gain', 'Sensitivity',
-                   'Vmax', 'LowFreq', 'HighFreq', 'CosineN', 'CosineE', 'CosineD', 'Se', 'Zone')
-        formats = ('a10', 'f8', 'f8', 'f2', 'i', 'a2', 'i', 'i', 'f2', 'f2', 'f2', 'f2', 'f2', 'f2', 'f2', 'f2',
-                   'i', 'i')
-        sensorfile = numpy.loadtxt(file_path, skiprows=9, dtype={'names': headers, 'formats': formats})
+            'Description', 'Northing', 'Easting', 'Depth', 'S', 'Type', 'Cmp', 'ID',
+            'Gain', 'Sensitivity',
+            'Vmax', 'LowFreq', 'HighFreq', 'CosineN', 'CosineE', 'CosineD', 'Se', 'Zone')
+        formats = (
+        'a10', 'f8', 'f8', 'f2', 'i', 'a2', 'i', 'i', 'f2', 'f2', 'f2', 'f2', 'f2', 'f2',
+        'f2', 'f2',
+        'i', 'i')
+        sensorfile = numpy.loadtxt(file_path, skiprows=9,
+                                   dtype={'names': headers, 'formats': formats})
 
     if ver == 2.1:
         headers = (
-                   'Description', 'Northing', 'Easting', 'Depth', 'S', 'Type', 'Mod', 'Cmp', 'ID', 'Gain',
-                   'Sensitivity', 'AmpCor', 'Vmax', 'LowFreq', 'HighFreq', 'CosineN', 'CosineE', 'CosineD', 'Se',
-                   'Zone')
+            'Description', 'Northing', 'Easting', 'Depth', 'S', 'Type', 'Mod', 'Cmp',
+            'ID', 'Gain',
+            'Sensitivity', 'AmpCor', 'Vmax', 'LowFreq', 'HighFreq', 'CosineN', 'CosineE',
+            'CosineD', 'Se',
+            'Zone')
         formats = (
-                   'a17', 'f8', 'f8', 'f2', 'i', 'a2', 'i', 'i', 'i', 'f2', 'f2', 'f2', 'f2', 'f2', 'f2', 'f2',
-                   'f2', 'f2', 'i', 'i')
+            'a17', 'f8', 'f8', 'f2', 'i', 'a2', 'i', 'i', 'i', 'f2', 'f2', 'f2', 'f2',
+            'f2', 'f2', 'f2',
+            'f2', 'f2', 'i', 'i')
 
-        sensorfile = numpy.loadtxt(file_path, skiprows=9, dtype={'names': headers, 'formats': formats})
+        sensorfile = numpy.loadtxt(file_path, skiprows=9,
+                                   dtype={'names': headers, 'formats': formats})
     if ver == 3.0:
         headers = (
-                   'Description', 'Northing', 'Easting', 'Depth', 'S', 'Type', 'Mod', 'Cmp', 'ID', 'Gain',
-                   'Sensitivity', 'AmpCor', 'Vmax', 'LowFreq', 'HighFreq', 'CosineN', 'CosineE', 'CosineD', 'Se',
-                   'Zone', 'MDepth', 'LegacyNames')
+            'Description', 'Northing', 'Easting', 'Depth', 'S', 'Type', 'Mod', 'Cmp',
+            'ID', 'Gain',
+            'Sensitivity', 'AmpCor', 'Vmax', 'LowFreq', 'HighFreq', 'CosineN', 'CosineE',
+            'CosineD', 'Se',
+            'Zone', 'MDepth', 'LegacyNames')
         formats = (
-                   'a17', 'f8', 'f8', 'f2', 'i', 'a2', 'i', 'i', 'i', 'f2', 'f2', 'f2', 'f2', 'f2', 'f2', 'f2', 'f2',
-                   'f2', 'i', 'i', 'f2', 'a12')
+            'a17', 'f8', 'f8', 'f2', 'i', 'a2', 'i', 'i', 'i', 'f2', 'f2', 'f2', 'f2',
+            'f2', 'f2', 'f2', 'f2',
+            'f2', 'i', 'i', 'f2', 'a12')
 
         i = 0
         skip = None
         colsrow = None
         datarow = None
         nbits_row = None
         for line in open(file_path, 'r'):
@@ -2207,20 +2338,22 @@
         if datarow is None:
             raise ValueError('Could not identify row before table headers.')
 
         # getting the NBITS out of the initial header
         nbits = int(nbits_row.split('=')[-1])
 
         # reading in the data
-        col_df = pd.read_csv(file_path, sep=':', skiprows=colsrow, nrows=datarow - colsrow - 1,
+        col_df = pd.read_csv(file_path, sep=':', skiprows=colsrow,
+                             nrows=datarow - colsrow - 1,
                              names=('Name', 'Description'))
         col_df['Name'] = col_df['Name'].map(str.strip)
 
         # read in sensor file table section
-        sensorfile = pd.read_csv(file_path, header=None, sep=r'\s+', quotechar='"', skiprows=skip)
+        sensorfile = pd.read_csv(file_path, header=None, sep=r'\s+', quotechar='"',
+                                 skiprows=skip)
 
         if len(sensorfile.columns) == len(col_df.Name):
             sensorfile.columns = col_df.Name
         else:
             Exception("Wrong number of columns somehow")
 
         # keep some old column names for legacy reasons...
@@ -2228,41 +2361,47 @@
         sensorfile['CosineE'] = sensorfile.V
         sensorfile['CosineD'] = sensorfile.W
 
         # Calculate azimuth and dip
         azim = np.arctan2(sensorfile['CosineE'].astype('float64'),
                           sensorfile['CosineN'].astype('float64')) * 180 / np.pi
         dip = np.arcsin(sensorfile['CosineD'].astype('float64') / np.sqrt(
-            sensorfile['CosineN'].astype('float64') ** 2 + sensorfile['CosineE'].astype('float64') ** 2 + sensorfile[
+            sensorfile['CosineN'].astype('float64') ** 2 + sensorfile['CosineE'].astype(
+                'float64') ** 2 + sensorfile[
                 'CosineD'].astype('float64') ** 2)) * 180.0 / np.pi
 
         for i in range(0, len(azim)):
             if azim[i] < 0:
                 azim[i] = azim[i] + 360
             if azim[i] >= 360:
                 azim[i] = azim[i] - 360
 
         if ver != 3.0:
-            sensorfile = numpy.lib.recfunctions.append_fields(sensorfile, ('Azimuth', 'Dip'), (azim, dip),
+            sensorfile = numpy.lib.recfunctions.append_fields(sensorfile,
+                                                              ('Azimuth', 'Dip'),
+                                                              (azim, dip),
                                                               usemask=False)
         else:
             sensorfile['Azimuth'], sensorfile['Dip'] = azim, dip
 
         # computing the correction to ground motion
         # WE ARE ASSUMING HERE THAT NBIT == 2
-        sensorfile['DIV_TO_GET_GM'] = (sensorfile['GAIN'] * sensorfile['SENSITIVITY']) / (
-                2 ** (nbits - 1) / sensorfile['VOLTAGE_RANGE'])
+        sensorfile['DIV_TO_GET_GM'] = (sensorfile['GAIN'] * sensorfile[
+            'SENSITIVITY']) / (
+                                              2 ** (nbits - 1) / sensorfile[
+                                          'VOLTAGE_RANGE'])
 
     if sensorfile is None:
         raise ValueError('Something went wrong when trying to read the sensor file.')
 
     return sensorfile
 
 
-def waveform_vel_shift(vel, sens, data_to_shift, norm_method, sensornames_by_ch, head, plot=True, downgoing=True):
+def waveform_vel_shift(vel, sens, data_to_shift, norm_method, sensornames_by_ch, head,
+                       plot=True, downgoing=True):
     """
         Function to shift sensors by an apparent velocity
 
         vel - velocity to shift
         sens - enabled sensors
         data_to_plot - STA/LTA data set
         norm_method - how to normalize data
@@ -2277,15 +2416,16 @@
     # Calculate shift of STALTA data
     data_shift = data_to_shift.copy()
     stack = []
 
     tracelen = len(data_shift[0, :])
 
     # Sensor spacing by channel
-    spacing_by_ch = np.hstack([np.ones(3) * i * 100 for i in range(0, int(len(data_to_shift) / 3.0))])
+    spacing_by_ch = np.hstack(
+        [np.ones(3) * i * 100 for i in range(0, int(len(data_to_shift) / 3.0))])
 
     # Loop over every channel
     for i in range(0, len(data_shift)):
         # s to ms, 4 data points per millisecond, sensor times spacing divided by velocity
         nstart = int(1000 * 4 * (spacing_by_ch[i] / vel))
 
         # if enabled sensor
@@ -2323,37 +2463,39 @@
     elif norm_method == 'None - amplitude stack':
         norm_stack = np.sum(stack, axis=0)
     elif norm_method == "Norm by number of channels enabled":
         norm_stack = np.sum(stack, axis=0) / (len(sens) * 3)
 
     # error catching
     if norm_stack is None:
-        raise ValueError('Something went wrong with the normalisation - possibly the norm method wasnt recognised')
+        raise ValueError(
+            'Something went wrong with the normalisation - possibly the norm method wasnt recognised')
 
     if plot:
         fig, ax = plt.subplots(figsize=(16, 2))
         ax.plot(norm_stack, 'black')
         ax.set_title(norm_method)
 
     return np.max(norm_stack, axis=0)
 
 
-def tubeWaveDetector(head, data, sta, lta, sens, norm_method="Norm by number of channels enabled",
+def tubeWaveDetector(head, data, sta, lta, sens,
+                     norm_method="Norm by number of channels enabled",
                      downgoing=True, metric=False):
     """
     Classify if an event is a tube-wave based on the velocity shift required to produce a maximal stack
 
     sta - short term average in milliseconds
     lta - long term average in milliseconds
 
     :return:
     """
 
     # Sampling to convert milliseconds to data points
-    sampling = int(1/(1000/head['fs']))
+    sampling = int(1 / (1000 / head['fs']))
 
     # List of sensornames
     sensornames = pd.Series(head['ch_descr'][::3])
     sensornames = sensornames.str.split("\x00").str[0]
     sensornames = sensornames.to_list()
     sensornames_by_ch = pd.Series(head['ch_descr'])
     sensornames_by_ch = sensornames_by_ch.str.split("\x00").str[0]
@@ -2361,47 +2503,49 @@
     # Detrend
     for i in range(0, len(data)):
         data[i, :] = signal.detrend(data[i, :])
 
     data_stalta = data.copy()
 
     for i in range(0, len(data)):
-        data_stalta[i, :] = sta_lta_mask(data_stalta[i, :], sta_w=sta * sampling, lta_w=lta * sampling)
+        data_stalta[i, :] = sta_lta_mask(data_stalta[i, :], sta_w=sta * sampling,
+                                         lta_w=lta * sampling)
 
     max_val = 0
     best_v = None
 
     for v in np.arange(300.0, 10000.0, 10):
         # velocity (convert m/s to ft/s)
         if metric is False:
             v *= 3.28084
 
-        val = waveform_vel_shift(v, sens, data_stalta, norm_method, sensornames_by_ch, head, False, downgoing)
+        val = waveform_vel_shift(v, sens, data_stalta, norm_method, sensornames_by_ch,
+                                 head, False, downgoing)
 
         if val > max_val:
             # Best so far
             max_val = val
             best_v = v
 
-    print("Best velocity: "+str(best_v))
-    print("Max Stack Score: "+str(max_val))
+    print("Best velocity: " + str(best_v))
+    print("Max Stack Score: " + str(max_val))
 
     tube_max = 1500
     tube_min = 1350
 
     if metric is False:
         tube_max *= 3.28084
         tube_min *= 3.28084
 
     if (best_v > tube_min) & (best_v < tube_max) & (max_val > 1.5):
         tubewave = True
     else:
         tubewave = False
 
-    print("Tube Wave: "+str(tubewave))
+    print("Tube Wave: " + str(tubewave))
 
     return tubewave, best_v, max_val
 
 
 def generateHSFFilePathFile(trgids, DSN, basepath, HSFListFile):
     """
     For a dataframe of database entries, create the file path and alternate file
@@ -2446,16 +2590,18 @@
     if debug:
         print(args)
     _ = subprocess.call(args)
 
     print("Batch complete")
 
 
-def get_cc_values(tr1, tr2, arriv1_loc, arriv2_loc, window=0.5, allowed_shift=0.5, plot_result=False,
-                  sampling_frequency=100, debug=False, orig_diff=0, return_shift_val=False):
+def get_cc_values(tr1, tr2, arriv1_loc, arriv2_loc, window=0.5, allowed_shift=0.5,
+                  plot_result=False,
+                  sampling_frequency=100, debug=False, orig_diff=0,
+                  return_shift_val=False):
     """
     Estimating the cross correlation differential times between two events for a particular phase
     :param tr1: the data for the first event (just a numpy array of values)
     :param tr2: the data for the second event (numpy array of values)
     :param arriv1_loc: the arrival time of the first event in samples (must be correct relative to the start of the data
         provided in tr1)
     :param arriv2_loc: the arrival time of the second event in samples (must be correct relative to the start of the
@@ -2496,19 +2642,21 @@
         print(tr2)
         print(tr2[arriv2_loc - window: arriv2_loc + window])
 
     # making the array of tr2 values
     tr2_arr = np.repeat(tr2[:, np.newaxis], len(shifts), axis=1).T
 
     # now shifting all the copies in that array by different amounts
-    arr_roll = tr2_arr[:, [*range(tr2_arr.shape[1]), *range(tr2_arr.shape[1] - 1)]].copy()  # need `copy`
+    arr_roll = tr2_arr[:, [*range(tr2_arr.shape[1]),
+                           *range(tr2_arr.shape[1] - 1)]].copy()  # need `copy`
     strd_0, strd_1 = arr_roll.strides
     n = tr2_arr.shape[1]
     # need to be careful that this function doesn't result in errors due to memory allocation (see docs)
-    result = np.lib.stride_tricks.as_strided(arr_roll, (*tr2_arr.shape, n), (strd_0, strd_1, strd_1))
+    result = np.lib.stride_tricks.as_strided(arr_roll, (*tr2_arr.shape, n),
+                                             (strd_0, strd_1, strd_1))
     # had to change n-shifts to n+shifts because behaviour was not as I expected
     shifted = result[np.arange(tr2_arr.shape[0]), (n + shifts) % n]
 
     # now indexing the shifted arrays
     # have to flip the order because they come out in the wrong order
     arr_var = np.flip(shifted[:, arriv2_loc - window:arriv2_loc + window], axis=0)
     if debug:
@@ -2550,33 +2698,36 @@
     # now compute the differential time in seconds
     # REMEMBER, this has to be in event 1 minus event2
     arriv_diff = arriv1_loc_shift - arriv2_loc_shift - orig_diff
 
     # option to plot out the result
     if plot_result is True:
         plt.figure()
-        plt.plot(win_1/np.max(win_1), 'b-')
-        plt.plot(arr_var[tloc]/np.max(arr_var[tloc]), 'g-', alpha=0.2)
-        plt.plot(tr2[arriv2_loc - window:arriv2_loc + window]/np.max(arr_var[tloc]), 'r-', alpha=0.2)
+        plt.plot(win_1 / np.max(win_1), 'b-')
+        plt.plot(arr_var[tloc] / np.max(arr_var[tloc]), 'g-', alpha=0.2)
+        plt.plot(tr2[arriv2_loc - window:arriv2_loc + window] / np.max(arr_var[tloc]),
+                 'r-', alpha=0.2)
         print('arrivs')
         print(arriv1_loc)
         print(arriv2_loc)
         print(shift_val)
         print(arriv_diff)
         plt.show()
 
     # returning the differential time and its cross correlation coefficient estimate
     if return_shift_val is False:
         return arriv_diff, ccc_max
     else:
         return arriv_diff, ccc_max, shift_val
 
 
-def get_mcc_values(tr1, tr2, arriv1_loc, arriv2_loc, window=0.5, allowed_shift=0.5, plot_result=False,
-                   sampling_frequency=100, debug=False, orig_diff=0, return_shift_val=False):
+def get_mcc_values(tr1, tr2, arriv1_loc, arriv2_loc, window=0.5, allowed_shift=0.5,
+                   plot_result=False,
+                   sampling_frequency=100, debug=False, orig_diff=0,
+                   return_shift_val=False):
     """
     Estimating the cross correlation differential times between two events for a particular phase. Essentially the same
     code as get_cc_values but with added capability of using "anti-correlated" signals to compensate for signal
     sign variability depending on source radiation pattern.
     Author: Doug Angus (adapted from get_cc_values by Joshua Williams)
     :param tr1: the data for the first event (just a numpy array of values)
     :param tr2: the data for the second event (numpy array of values)
@@ -2620,19 +2771,21 @@
         print(tr2)
         print(tr2[arriv2_loc - window: arriv2_loc + window])
 
     # making the array of tr2 values
     tr2_arr = np.repeat(tr2[:, np.newaxis], len(shifts), axis=1).T
 
     # now shifting all the copies in that array by different amounts
-    arr_roll = tr2_arr[:, [*range(tr2_arr.shape[1]), *range(tr2_arr.shape[1] - 1)]].copy()  # need `copy`
+    arr_roll = tr2_arr[:, [*range(tr2_arr.shape[1]),
+                           *range(tr2_arr.shape[1] - 1)]].copy()  # need `copy`
     strd_0, strd_1 = arr_roll.strides
     n = tr2_arr.shape[1]
     # need to be careful that this function doesn't result in errors due to memory allocation (see docs)
-    result = np.lib.stride_tricks.as_strided(arr_roll, (*tr2_arr.shape, n), (strd_0, strd_1, strd_1))
+    result = np.lib.stride_tricks.as_strided(arr_roll, (*tr2_arr.shape, n),
+                                             (strd_0, strd_1, strd_1))
     # had to change n-shifts to n+shifts because behaviour was not as I expected
     shifted = result[np.arange(tr2_arr.shape[0]), (n + shifts) % n]
 
     # now indexing the shifted arrays
     # have to flip the order because they come out in the wrong order
     arr_var = np.flip(shifted[:, arriv2_loc - window:arriv2_loc + window], axis=0)
     if debug:
@@ -2686,19 +2839,22 @@
     if plot_result is True:
         # plt.figure()
         # plt.plot(win_1/np.max(win_1), 'b-')
         # plt.plot(arr_var[tloc]/np.max(arr_var[tloc]), 'g-', alpha=0.2)
         # plt.plot(tr2[arriv2_loc - window:arriv2_loc + window]/np.max(arr_var[tloc]), 'r-', alpha=0.2)
         fig, axs = plt.subplots(5)
         fig.suptitle('MCC results')
-        axs[0].plot(win_1/np.max(win_1), 'b-')
-        axs[1].plot(arr_var[tloc]/np.max(arr_var[tloc]), 'g-', alpha=0.2)
-        axs[2].plot(tr2[arriv2_loc - window:arriv2_loc + window]/np.max(arr_var[tloc]), 'r-', alpha=0.2)
-        axs[3].plot(tr1[arriv1_loc - 2*window:arriv1_loc + 4*window], 'g-', alpha=0.2)
-        axs[4].plot(tr2[arriv2_loc - 2*window:arriv2_loc + 4*window], 'r-', alpha=0.2)
+        axs[0].plot(win_1 / np.max(win_1), 'b-')
+        axs[1].plot(arr_var[tloc] / np.max(arr_var[tloc]), 'g-', alpha=0.2)
+        axs[2].plot(tr2[arriv2_loc - window:arriv2_loc + window] / np.max(arr_var[tloc]),
+                    'r-', alpha=0.2)
+        axs[3].plot(tr1[arriv1_loc - 2 * window:arriv1_loc + 4 * window], 'g-',
+                    alpha=0.2)
+        axs[4].plot(tr2[arriv2_loc - 2 * window:arriv2_loc + 4 * window], 'r-',
+                    alpha=0.2)
         plt.show()
 
         print('cc values')
         print('cc_max:', ccc_max)
         print('cc_min:', ccc_min)
         print('Shift :', shift_val)
         print('dT    :', arriv_diff)
@@ -2762,15 +2918,16 @@
 
     # getting v2 as well
     v2 = np.array(bits[p1 + 1], dtype=np.int64)
 
     return p1, b, v, v2
 
 
-def numpy_get_int(bits, num_bits, debug=False, out_size=None, v=None, v2=None, b=None, adjust_v2=True):
+def numpy_get_int(bits, num_bits, debug=False, out_size=None, v=None, v2=None, b=None,
+                  adjust_v2=True):
     """
     Convert each integer in the array using the specific number of bits
     :param bits: the array of integers that we will extract values from
     :param num_bits: number of bits
     :param debug: optional debug parameter
     :param out_size: expected size of the output, defaults to the length of the bits
     :param v: option to include v if precalculating it
@@ -2880,15 +3037,15 @@
     :return:
     """
 
     # extracting the waveform data
     blob = hbin[:compresssize]
 
     # getting the individual bits in little endian
-    blob_arr = np.ndarray((int(len(blob)/4), ), buffer=blob, offset=0, dtype='<i')
+    blob_arr = np.ndarray((int(len(blob) / 4),), buffer=blob, offset=0, dtype='<i')
 
     # expect the first bit to be zero, non-zero value may be due to new compression format that this version
     # does not understand
     get_vals = numpy_get(blob_arr, out_size=1)
     loc = 0
     temp = get_vals[loc]
     if temp:
@@ -2915,15 +3072,16 @@
 
     # recreating the dictionaries now that we know how many values there will be
     v_vals = dict()
     call_vals = dict()
     for ij in range(0, 33):
         # start_time4 = time.time()
         if ij in [5, 16]:
-            v_vals[ij] = numpy_get_int(blob_arr, ij, out_size=true_out_size, v=v.copy(), b=b,
+            v_vals[ij] = numpy_get_int(blob_arr, ij, out_size=true_out_size, v=v.copy(),
+                                       b=b,
                                        v2=v2.copy(), adjust_v2=False)
         call_vals[ij] = []
         # print('Time taken for initial value calculations for ' + str(ij) + ':' + str(time.time() - start_time4))
 
     # getting the boolean values as well
     get_vals = numpy_get(blob_arr, out_size=true_out_size, p1=p1, b=b)
 
@@ -3007,15 +3165,16 @@
     # getting the values and setting up the locations counters for each different number of bits
     v_vals = dict()
     loc_vals = dict()
     for ij in range(0, 33):
         loc_vals[ij] = 0
         if len(call_vals[ij]) != 0:
             ix = np.array(call_vals[ij])
-            v_vals[ij] = numpy_get_int(blob_arr, ij, out_size=true_out_size, v=v[ix], b=b[ix],
+            v_vals[ij] = numpy_get_int(blob_arr, ij, out_size=true_out_size, v=v[ix],
+                                       b=b[ix],
                                        v2=v2[ix], adjust_v2=False)
 
     # iterating through to extract all the data points
     loc = orig_loc
     p = 0
     while p < n_out_size:
         # setting the size of the block
```

### Comparing `pickled_carrots-1.0.7/pyproject.toml` & `pickled_carrots-1.0.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pickled_carrots"
-version = "1.0.7"
+version = "1.0.8"
 description = ""
 authors = ["pickled cattots team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 plotly = "^5.14.1"
```

