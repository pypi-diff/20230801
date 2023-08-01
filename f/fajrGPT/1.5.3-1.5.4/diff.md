# Comparing `tmp/fajrGPT-1.5.3.tar.gz` & `tmp/fajrGPT-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.5.3.tar", last modified: Tue Aug  1 02:31:47 2023, max compression
+gzip compressed data, was "fajrGPT-1.5.4.tar", last modified: Tue Aug  1 11:10:09 2023, max compression
```

## Comparing `fajrGPT-1.5.3.tar` & `fajrGPT-1.5.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-08-01 02:31:47.211844 fajrGPT-1.5.3/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.5.3/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-08-01 02:31:47.211647 fajrGPT-1.5.3/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.5.3/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-08-01 02:31:47.207912 fajrGPT-1.5.3/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.5.3/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     4095 2023-07-31 02:16:34.000000 fajrGPT-1.5.3/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)    22056 2023-07-31 11:25:34.000000 fajrGPT-1.5.3/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-08-01 02:31:47.211414 fajrGPT-1.5.3/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-08-01 02:31:47.000000 fajrGPT-1.5.3/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-08-01 02:31:47.000000 fajrGPT-1.5.3/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-08-01 02:31:47.000000 fajrGPT-1.5.3/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-08-01 02:31:47.000000 fajrGPT-1.5.3/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       68 2023-08-01 02:31:47.000000 fajrGPT-1.5.3/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-08-01 02:31:47.000000 fajrGPT-1.5.3/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-08-01 02:31:47.211884 fajrGPT-1.5.3/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1165 2023-08-01 02:31:08.000000 fajrGPT-1.5.3/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-08-01 11:10:09.794444 fajrGPT-1.5.4/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.5.4/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-08-01 11:10:09.794285 fajrGPT-1.5.4/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.5.4/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-08-01 11:10:09.791799 fajrGPT-1.5.4/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.5.4/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     4095 2023-07-31 02:16:34.000000 fajrGPT-1.5.4/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)    22151 2023-08-01 11:08:56.000000 fajrGPT-1.5.4/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-08-01 11:10:09.794091 fajrGPT-1.5.4/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-08-01 11:10:09.000000 fajrGPT-1.5.4/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-08-01 11:10:09.000000 fajrGPT-1.5.4/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-08-01 11:10:09.000000 fajrGPT-1.5.4/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-08-01 11:10:09.000000 fajrGPT-1.5.4/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       68 2023-08-01 11:10:09.000000 fajrGPT-1.5.4/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-08-01 11:10:09.000000 fajrGPT-1.5.4/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-08-01 11:10:09.794480 fajrGPT-1.5.4/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1165 2023-08-01 11:09:06.000000 fajrGPT-1.5.4/setup.py
```

### Comparing `fajrGPT-1.5.3/LICENSE` & `fajrGPT-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.5.3/PKG-INFO` & `fajrGPT-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.5.3
+Version: 1.5.4
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.5.3/README.md` & `fajrGPT-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.5.3/fajrGPT/quran_metadata.py` & `fajrGPT-1.5.4/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.5.3/fajrGPT/wake.py` & `fajrGPT-1.5.4/fajrGPT/wake.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 @click.option('--url', required=True, help='YouTube URL containing desired audio data.')
 @click.option('--time', required=True, help='Countdown time in format [number][h/m/s], i.e. 1h would create a 1 hour timer.')
 @click.option('--output', required=True, help='Name of the output file.')
 @click.option('--names-flag', required=False, help='Whether or not to include a randomly selected name of Allah in the preamble.', default=True)
 @click.option('--transition-time', required=False, help='Time in seconds for the transition between the output audio and the Quran verses.', default=600)
 @click.option('--surah', required=False, help='Specific Surah from the Quran. Should be given as integer.')
 @click.option('--english', required=False, help='Whether or not to play audio with the english translation of the Quran verses. Note this option only applies if the --surah option is not None.', default=False)
-@click.option('--low-pass', required=False, help='Whether or not to apply a low pass filter to the audio.', default=True)
+@click.option('--low-pass', required=False, help='Amount of low-pass to apply to the audio (float (KHz) or None). Default is 10 (KHz).', default=10)
 
-def main(url, time, output, names_flag, transition_time=600, surah=None, english=False, low_pass=True):
+def main(url, time, output, names_flag, transition_time=600, surah=None, english=False, low_pass=10):
     # Check surah option
     if surah:
         # make the output file name the same as the surah
         output = 'quran-' + '{:03d}'.format(int(surah))
         if not english:
             flag = download_surah(surah, output)
         else:
@@ -46,15 +46,16 @@
         flag = download_video(url, output)
 
     # test audio
     test_audio(f'{output}.mp3',output,flag)
 
     # apply low pass filter to the audio
     if low_pass:
-        apply_low_pass_filter(f'{output}.mp3')
+        cutoff_filter = float(low_pass) * 1000
+        apply_low_pass_filter(f'{output}.mp3', cutoff_filter)
 
     # convert time to seconds
     countdown_seconds = convert_to_seconds(time)
 
     # Start countdown
     countdown(countdown_seconds)
 
@@ -523,26 +524,26 @@
     return y
 
 def array_to_audio_segment(np_array, audio):
     # Scale numpy array and convert to a list of integers
     int_array = np.int16(np_array * 2**15)
     return audio._spawn(int_array.tobytes())
 
-def apply_low_pass_filter(mp3_filename, cutoff=10000, order=5, fs=44100):
+def apply_low_pass_filter(mp3_filename, cutoff_filter, order=5, fs=44100):
     # Read the mp3 file
     audio = AudioSegment.from_mp3(mp3_filename)
 
     # Convert to numpy array
     np_array = audio.get_array_of_samples()
 
     # divide by max value to normalize the data
     np_array = np_array / np.max(np.abs(np_array))
 
     # Apply the low pass filter
-    filtered = butter_lowpass_filter(np_array, cutoff, fs, order)
+    filtered = butter_lowpass_filter(np_array, cutoff_filter, fs, order)
 
     # Convert the numpy array back to an audio segment
     filtered_audio = array_to_audio_segment(filtered, audio)
 
     # Export the audio segment as an mp3 file
     filtered_audio.export(mp3_filename, format="mp3")
```

### Comparing `fajrGPT-1.5.3/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.5.4/fajrGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.5.3
+Version: 1.5.4
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.5.3/setup.py` & `fajrGPT-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.5.3",
+    version="1.5.4",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

