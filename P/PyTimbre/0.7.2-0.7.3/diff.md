# Comparing `tmp/PyTimbre-0.7.2.tar.gz` & `tmp/PyTimbre-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTimbre-0.7.2.tar", last modified: Wed Jul 19 19:35:59 2023, max compression
+gzip compressed data, was "PyTimbre-0.7.3.tar", last modified: Tue Aug  1 19:17:10 2023, max compression
```

## Comparing `PyTimbre-0.7.2.tar` & `PyTimbre-0.7.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 19:35:59.307570 PyTimbre-0.7.2/
--rw-rw-rw-   0        0        0     1106 2023-04-27 18:41:59.000000 PyTimbre-0.7.2/LICENSE.txt
--rw-rw-rw-   0        0        0    14637 2023-07-19 19:35:59.303571 PyTimbre-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     5339 2023-04-27 18:41:59.000000 PyTimbre-0.7.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-19 19:35:59.308570 PyTimbre-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0     1071 2023-07-19 19:35:33.000000 PyTimbre-0.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 19:35:59.024810 PyTimbre-0.7.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-19 19:35:59.144569 PyTimbre-0.7.2/src/PyTimbre.egg-info/
--rw-rw-rw-   0        0        0    14637 2023-07-19 19:35:58.000000 PyTimbre-0.7.2/src/PyTimbre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      775 2023-07-19 19:35:58.000000 PyTimbre-0.7.2/src/PyTimbre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 19:35:58.000000 PyTimbre-0.7.2/src/PyTimbre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2023-07-19 19:35:58.000000 PyTimbre-0.7.2/src/PyTimbre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-19 19:35:58.000000 PyTimbre-0.7.2/src/PyTimbre.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-19 19:35:59.181947 PyTimbre-0.7.2/src/pytimbre/
--rw-rw-rw-   0        0        0       75 2023-04-27 18:41:59.000000 PyTimbre-0.7.2/src/pytimbre/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 19:35:59.222083 PyTimbre-0.7.2/src/pytimbre/audio_files/
--rw-rw-rw-   0        0        0      108 2023-04-27 18:41:59.000000 PyTimbre-0.7.2/src/pytimbre/audio_files/__init__.py
--rw-rw-rw-   0        0        0    24251 2023-06-27 12:09:48.000000 PyTimbre-0.7.2/src/pytimbre/audio_files/ansi_standard_formatted_files.py
--rw-rw-rw-   0        0        0    15392 2023-04-27 18:41:59.000000 PyTimbre-0.7.2/src/pytimbre/audio_files/calibrated_binary_files.py
--rw-rw-rw-   0        0        0    70823 2023-07-19 19:35:33.000000 PyTimbre-0.7.2/src/pytimbre/audio_files/wavefile.py
-drwxrwxrwx   0        0        0        0 2023-07-19 19:35:59.297602 PyTimbre-0.7.2/src/pytimbre/spectral/
--rw-rw-rw-   0        0        0      150 2023-04-27 18:41:59.000000 PyTimbre-0.7.2/src/pytimbre/spectral/__init__.py
--rw-rw-rw-   0        0        0    15326 2023-04-27 18:41:59.000000 PyTimbre-0.7.2/src/pytimbre/spectral/acoustic_weights.py
--rw-rw-rw-   0        0        0    15705 2023-04-27 18:41:59.000000 PyTimbre-0.7.2/src/pytimbre/spectral/fractional_octave_band.py
--rw-rw-rw-   0        0        0    16910 2023-04-27 18:41:59.000000 PyTimbre-0.7.2/src/pytimbre/spectral/fundamental_frequency.py
--rw-rw-rw-   0        0        0    59502 2023-07-19 19:35:33.000000 PyTimbre-0.7.2/src/pytimbre/spectral/spectra.py
--rw-rw-rw-   0        0        0     6656 2023-04-27 18:41:59.000000 PyTimbre-0.7.2/src/pytimbre/spectral/spectrogram.py
--rw-rw-rw-   0        0        0    14243 2023-04-27 18:41:59.000000 PyTimbre-0.7.2/src/pytimbre/spectral/swipe.py
--rw-rw-rw-   0        0        0    37011 2023-07-19 19:35:33.000000 PyTimbre-0.7.2/src/pytimbre/spectral/time_histories.py
--rw-rw-rw-   0        0        0   100362 2023-07-19 19:35:33.000000 PyTimbre-0.7.2/src/pytimbre/waveform.py
--rw-rw-rw-   0        0        0     7939 2023-04-27 18:41:59.000000 PyTimbre-0.7.2/src/pytimbre/yin.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:17:10.400559 PyTimbre-0.7.3/
+-rw-rw-rw-   0        0        0     1106 2023-02-28 16:15:07.000000 PyTimbre-0.7.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    14764 2023-08-01 19:17:10.400559 PyTimbre-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5339 2023-04-25 22:51:37.000000 PyTimbre-0.7.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 19:17:10.400559 PyTimbre-0.7.3/setup.cfg
+-rw-rw-rw-   0        0        0     1111 2023-08-01 19:16:09.000000 PyTimbre-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:17:10.338609 PyTimbre-0.7.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 19:17:10.356005 PyTimbre-0.7.3/src/PyTimbre.egg-info/
+-rw-rw-rw-   0        0        0    14764 2023-08-01 19:17:10.000000 PyTimbre-0.7.3/src/PyTimbre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2023-08-01 19:17:10.000000 PyTimbre-0.7.3/src/PyTimbre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 19:17:10.000000 PyTimbre-0.7.3/src/PyTimbre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2023-08-01 19:17:10.000000 PyTimbre-0.7.3/src/PyTimbre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-01 19:17:10.000000 PyTimbre-0.7.3/src/PyTimbre.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 19:17:10.364940 PyTimbre-0.7.3/src/pytimbre/
+-rw-rw-rw-   0        0        0       75 2023-04-13 00:23:16.000000 PyTimbre-0.7.3/src/pytimbre/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:17:10.371469 PyTimbre-0.7.3/src/pytimbre/audio_files/
+-rw-rw-rw-   0        0        0      108 2023-04-04 13:59:30.000000 PyTimbre-0.7.3/src/pytimbre/audio_files/__init__.py
+-rw-rw-rw-   0        0        0    24251 2023-06-26 00:38:01.000000 PyTimbre-0.7.3/src/pytimbre/audio_files/ansi_standard_formatted_files.py
+-rw-rw-rw-   0        0        0    15392 2023-04-14 23:28:06.000000 PyTimbre-0.7.3/src/pytimbre/audio_files/calibrated_binary_files.py
+-rw-rw-rw-   0        0        0    77426 2023-08-01 19:15:05.000000 PyTimbre-0.7.3/src/pytimbre/audio_files/wavefile.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:17:10.399073 PyTimbre-0.7.3/src/pytimbre/spectral/
+-rw-rw-rw-   0        0        0      150 2023-03-03 22:01:28.000000 PyTimbre-0.7.3/src/pytimbre/spectral/__init__.py
+-rw-rw-rw-   0        0        0    15326 2023-04-13 01:01:21.000000 PyTimbre-0.7.3/src/pytimbre/spectral/acoustic_weights.py
+-rw-rw-rw-   0        0        0    15705 2023-04-13 21:59:41.000000 PyTimbre-0.7.3/src/pytimbre/spectral/fractional_octave_band.py
+-rw-rw-rw-   0        0        0    16910 2023-04-15 02:25:52.000000 PyTimbre-0.7.3/src/pytimbre/spectral/fundamental_frequency.py
+-rw-rw-rw-   0        0        0    59615 2023-08-01 19:15:01.000000 PyTimbre-0.7.3/src/pytimbre/spectral/spectra.py
+-rw-rw-rw-   0        0        0     6656 2023-04-13 01:01:21.000000 PyTimbre-0.7.3/src/pytimbre/spectral/spectrogram.py
+-rw-rw-rw-   0        0        0    13865 2023-04-13 17:16:30.000000 PyTimbre-0.7.3/src/pytimbre/spectral/swipe.py
+-rw-rw-rw-   0        0        0    37011 2023-08-01 19:15:01.000000 PyTimbre-0.7.3/src/pytimbre/spectral/time_histories.py
+-rw-rw-rw-   0        0        0   100989 2023-08-01 19:15:01.000000 PyTimbre-0.7.3/src/pytimbre/waveform.py
+-rw-rw-rw-   0        0        0     7703 2023-04-13 01:31:15.000000 PyTimbre-0.7.3/src/pytimbre/yin.py
```

### Comparing `PyTimbre-0.7.2/LICENSE.txt` & `PyTimbre-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.7.2/PKG-INFO` & `PyTimbre-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTimbre
-Version: 0.7.2
+Version: 0.7.3
 Summary: Python conversion of Timbre Toolbox
 Home-page: https://gitlab.com/python-audio-feature-extraction/pytimbre
 Download-URL: 
 Author: Dr. Frank Mobley
 Author-email: frank.mobley.1@afrl.af.mil
 License: MIT
 Keywords: machine learning,feature extraction,MATLAB,audio
@@ -216,14 +216,18 @@
 - Added a property to set the method for the thresholding required in the attack determination
 - Updated the tests so that they will execute with python setup.py test
 - Incremented to 0.7.1 with the completion of all issues slated for the 0.7.1 increment.
 - Incremented to 0.7.2
 - Added spectrogram class that uses the spectrogram function in scipy.signal to create the matrix of sound pressure levels
 - Added a plotting function to the time history class.
 
+#### July
+- Added speech features from python_speech_features
+- Fixed errors in start_time function within WaveFile class
+
 
 MIT License
 
 Copyright (c) 2021 Frank Mobley, Gregory Bowers
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

### Comparing `PyTimbre-0.7.2/README.md` & `PyTimbre-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.7.2/setup.py` & `PyTimbre-0.7.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         HISTORY = history_file.read()
 
         with open('LICENSE.txt') as license_file:
             LICENSE = license_file.read()
 
 setup(
     name='PyTimbre',
-    version='0.7.2',
+    version='0.7.3',
     description='Python conversion of Timbre Toolbox',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY + '\n\n' + LICENSE,
     license='MIT',
     packages=find_packages('src'),
     author='Dr. Frank Mobley',
     author_email='frank.mobley.1@afrl.af.mil',
@@ -24,11 +24,12 @@
     download_url='',
     install_requires=[
         'numpy>=1.21.5',
         'pandas>=1.4.3',
         'scipy>=1.9.1',
         'statsmodels>=0.13.2',
         'mosqito>=1.0.8',
-        'colorednoise>=2.1.0'
+        'colorednoise>=2.1.0',
+        'python_speech_features~=0.6'
     ],
     package_dir={'': 'src'}
 )
```

### Comparing `PyTimbre-0.7.2/src/PyTimbre.egg-info/PKG-INFO` & `PyTimbre-0.7.3/src/PyTimbre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTimbre
-Version: 0.7.2
+Version: 0.7.3
 Summary: Python conversion of Timbre Toolbox
 Home-page: https://gitlab.com/python-audio-feature-extraction/pytimbre
 Download-URL: 
 Author: Dr. Frank Mobley
 Author-email: frank.mobley.1@afrl.af.mil
 License: MIT
 Keywords: machine learning,feature extraction,MATLAB,audio
@@ -216,14 +216,18 @@
 - Added a property to set the method for the thresholding required in the attack determination
 - Updated the tests so that they will execute with python setup.py test
 - Incremented to 0.7.1 with the completion of all issues slated for the 0.7.1 increment.
 - Incremented to 0.7.2
 - Added spectrogram class that uses the spectrogram function in scipy.signal to create the matrix of sound pressure levels
 - Added a plotting function to the time history class.
 
+#### July
+- Added speech features from python_speech_features
+- Fixed errors in start_time function within WaveFile class
+
 
 MIT License
 
 Copyright (c) 2021 Frank Mobley, Gregory Bowers
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

### Comparing `PyTimbre-0.7.2/src/PyTimbre.egg-info/SOURCES.txt` & `PyTimbre-0.7.3/src/PyTimbre.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.7.2/src/pytimbre/audio_files/ansi_standard_formatted_files.py` & `PyTimbre-0.7.3/src/pytimbre/audio_files/ansi_standard_formatted_files.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.7.2/src/pytimbre/audio_files/calibrated_binary_files.py` & `PyTimbre-0.7.3/src/pytimbre/audio_files/calibrated_binary_files.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.7.2/src/pytimbre/audio_files/wavefile.py` & `PyTimbre-0.7.3/src/pytimbre/audio_files/wavefile.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,18 @@
         #   of data chunks that can be parsed in a similar manner.
 
         #   The first chunk is required to be the RIFF chunk, with the file size minus 8.
 
         name = ChunkScanner.read_chunk_name(file)
 
         if name != "RIFF":
-            raise ValueError("A canonical file begins with the RIFF chunk.  This file does not, please provide a "
-                             "canonical file")
+            raise ValueError(
+                "A canonical file begins with the RIFF chunk.  This file does not, please provide a "
+                "canonical file"
+            )
 
         size = ChunkScanner.read_chunk_size(file)
 
         # if size + 8 != file_size:
         #     raise ValueError("The RIFF chunk size does not match the file size.  Please provide a canonical file")
 
         if ChunkScanner.read_chunk_name(file) != "WAVE":
@@ -213,15 +215,15 @@
 
     @property
     def chunk_offset(self):
         return self._offset
 
 
 class FactChunk(ChunkInformation):
-    def __init__(self, reader: FileIO=None, chunk_offset: int=None, chunk_size: int=None, chunk_name: str=None):
+    def __init__(self, reader: FileIO = None, chunk_offset: int = None, chunk_size: int = None, chunk_name: str = None):
         """
         The constructor for the format chunk.  This will contain the ability to read the 16 and 40 byte formatted
         header
         :param reader: File - The binary reader that will represent the data file that we are reading
         :param chunk_offset: int - offset from the beginning of the file where the format chunk data begins
         :param chunk_size: int - the number of bytes to read that contain the data
         """
@@ -243,15 +245,15 @@
 
 
 class FormatChunk(ChunkInformation):
     """
     The format chunk is a specialized data chunk found within the wav formatted files.
     """
 
-    def __init__(self, reader: FileIO=None, chunk_offset: int=None, chunk_size: int=None, chunk_name: str=None):
+    def __init__(self, reader: FileIO = None, chunk_offset: int = None, chunk_size: int = None, chunk_name: str = None):
         """
         The constructor for the format chunk.  This will contain the ability to read the 16 and 40 byte formatted
         header
         :param reader: File - The binary reader that will represent the data file that we are reading
         :param chunk_offset: int - offset from the beginning of the file where the format chunk data begins
         :param chunk_size: int - the number of bytes to read that contain the data
         """
@@ -303,15 +305,14 @@
                 self.fs = struct.unpack('<I', reader.read(4))[0]
                 self.byte_rate = struct.unpack('<I', reader.read(4))[0]
                 self.block_align = struct.unpack('<H', reader.read(2))[0]
                 self.bits_per_sample = struct.unpack('<H', reader.read(2))[0]
             except Exception as e:
                 raise e
 
-
     @property
     def waveform_format(self):
         if self.audio_format == 1:
             return "PCM - Uncompressed"
         elif self.audio_format == 3:
             return "IEEE Floating Point"
 
@@ -363,16 +364,18 @@
 
 
 class PeakChunk(ChunkInformation):
     """
     This class contains the information about the peaks within each channel of the wave file
     """
 
-    def __init__(self, reader: FileIO = None, offset: int = None, size: int = None, name: str = None,
-                 channel_count: int = 1):
+    def __init__(
+            self, reader: FileIO = None, offset: int = None, size: int = None, name: str = None,
+            channel_count: int = 1
+    ):
         """
         Constructor for the peak chunk.  This will read the peak from multiple channels
         :param reader: FileIO - the reader for the chunk data
         :param offset: int - the offset within the file of the actual data of the chunk
         :param size: int - the number of bytes within the chunk
         :param name: str - the name of the chunk
         :param channel_count: int - the number of channels within the wav file
@@ -473,16 +476,18 @@
 
 
 class DataChunk(ChunkInformation):
     """
     This class understand the various types of data formats that exist within wav files
     """
 
-    def __init__(self, reader: FileIO, offset: int, size: int, name: str, fmt: FormatChunk, peak: PeakChunk,
-                 s0: int = None, s1: int = None, normalized: bool = False):
+    def __init__(
+            self, reader: FileIO, offset: int, size: int, name: str, fmt: FormatChunk, peak: PeakChunk,
+            s0: int = None, s1: int = None, normalized: bool = False
+    ):
         """
         This constructor employs the Format_Chunk object to understand how to read the data from the wav file.
         :param reader: FileIO - The file object to read the data
         :param offset: int - the offset of the beginning of the data chunk's data
         :param size: int - the overall size of the data chunk's data
         :param name: str - the name of the chunk
         :param fmt: Format_Chunk - the object that understands how to format the waveform
@@ -557,38 +562,42 @@
         #   The order of the samples is channel 0 sample 0, channel 1 sample 0, ... channel N sample 0, channel 0
         #   sample 1...So we first loop through the samples, then the channels.  However, to keep track of where we are
         #   within the array that was read from the data there will be an index outside of the loops.
         #
         #   Start by moving through the samples
 
         idx = 0
-        sample_size = int(np.floor(fmt.bits_per_sample/8))
+        sample_size = int(np.floor(fmt.bits_per_sample / 8))
 
         if sample_size == 4 and fmt.audio_format == 3:
             #   This is the IEEE Float and 32-bit, which is required for the floating point value
 
-            samples = np.asarray(struct.unpack("<{}f".format(int(np.floor(sample_count * fmt.channel_count))),
-                                               byte_array),
-                                 dtype='float')
+            samples = np.asarray(
+                struct.unpack(
+                    "<{}f".format(int(np.floor(sample_count * fmt.channel_count))),
+                    byte_array
+                ),
+                dtype='float'
+            )
 
         elif sample_size == 3:
             tmp = list([0, 0, 0, 0])
 
-            samples = np.zeros((int(len(byte_array)/3),), dtype=float)
+            samples = np.zeros((int(len(byte_array) / 3),), dtype=float)
             n = 0
             for i in range(0, len(byte_array), 3):
                 tmp[1] = byte_array[i]
                 tmp[2] = byte_array[i + 1]
                 tmp[3] = byte_array[i + 2]
 
                 samples[n] = struct.unpack("<i", bytearray(tmp))[0]
                 n += 1
 
             samples = np.asarray(samples, dtype=float)
-            samples /= 2**31
+            samples /= 2 ** 31
 
         elif fmt.audio_format == 1:
             #   This is all the integer formatted data.
 
             if sample_size == 1:
                 data = struct.unpack("<{}b".format(int(np.floor(sample_count * fmt.channel_count))), byte_array)
                 samples = np.asarray(data, dtype='float') / (2 ** 8 - 1)
@@ -596,17 +605,21 @@
                 data = struct.unpack("<{}h".format(int(np.floor(sample_count * fmt.channel_count))), byte_array)
                 samples = np.asarray(data, dtype='float') / (2 ** 16 - 1)
             elif sample_size == 4:
                 data = struct.unpack("<{}i".format(int(np.floor(sample_count * fmt.channel_count))), byte_array)
                 samples = np.asarray(data, dtype='float') / (2 ** 32 - 1)
 
         elif fmt.audio_format > 500:
-            samples = np.asarray(struct.unpack("<{}i".format(int(np.floor(sample_count * fmt.channel_count))),
-                                               byte_array),
-                                 dtype='float') / 2**31
+            samples = np.asarray(
+                struct.unpack(
+                    "<{}i".format(int(np.floor(sample_count * fmt.channel_count))),
+                    byte_array
+                ),
+                dtype='float'
+            ) / 2 ** 31
 
         #   Scale the samples by the peak levels
 
         #   Assign the data to the class's sample object
 
         self.samples = samples.reshape((sample_count, fmt.channel_count))
 
@@ -620,26 +633,27 @@
     @property
     def waveform(self):
         return self.samples
 
 
 class ListChunk(ChunkInformation):
     """
-    This is an extra chunk that can provide meta data to the user through customizable fields.
+    This is an extra chunk that can provide metadata to the user through customizable fields.
     """
 
     def __init__(self, reader: FileIO = None, size: int = None, offset: int = None, name: str = None):
         """
         This will construct the information within the class and read the contents of the LIST chunk
         :param reader: FileIO - the binary reader that will be able to extract the information from the file
         :param size: int - the size of the data chunk
         :param offset: int - the offset of the chunk's data
         :param name: str - the name of the chunk
 
-        https://www.recordingblogs.com/wiki/list-chunk-of-a-wave-file#:~:text=List%20chunk%20%28of%20a%20RIFF%20file%29%20%20,%20Depends%20on%20the%20list%20type%20ID%20
+        https://www.recordingblogs.com/wiki/list-chunk-of-a-wave-file#:~:text=List%20chunk%20%28of%20a%20RIFF%20file
+        %29%20%20,%20Depends%20on%20the%20list%20type%20ID%20
         """
 
         if reader is None:
             #   Create the dictionaries that will be used for the creation of the data
 
             self.time0 = datetime.fromtimestamp(0)
             self.meta_data = {
@@ -649,45 +663,36 @@
             return
 
         super().__init__(name, size, offset)
 
         self.meta_data = dict()
         self.header = dict()
 
-        self.time0 = datetime.fromtimestamp(0)
-        self.meta_data['creation_date'] = self.time0
-
         #   Move to the offset within the file where the LIST chunk starts and read the data
-
         reader.seek(self.chunk_offset, 0)
         bytes = reader.read(self.chunk_size)
 
         #   The expected keyword should contain INFO for the description
-
         if bytes[:4] == b"INFO":
             #   Now we can begin parsing this information into elements that are important for the understanding
             #   of the audio file.
 
             offset = 4
 
             while offset < len(bytes):
                 #   Get the command
-
                 cmd = bytes[offset:offset + 4].decode()
 
                 #   Get the size of the string
-
                 size = int.from_bytes(bytes[offset + 4:offset + 8], 'little')
 
                 #   Read the string
-
                 data = bytes[offset + 8:offset + 8 + size].decode()
 
                 #   Remove the null characters that exist at the end of the data
-
                 if '\0' in data:
                     while data[-1] == '\0' and len(data) > 0:
                         data = data[:-1]
                         if len(data) <= 0:
                             break
 
                 offset += 8 + size
@@ -716,24 +721,14 @@
                                 data = header_element.split('=')[1]
 
                                 self.header[cmd] = data
                 elif cmd == "ICOP":
                     self.meta_data['copyright'] = data
                 elif cmd == "ICRD":
                     self.meta_data['creation_date'] = data
-
-                    #   Now use the information within the creation date to parse out the actual start time of
-                    #   the file
-                    try:
-                        self.time0 = datetime.strptime(data, "%Y-%m-%d %H:%M:%S.%f")
-                    except:
-                        try:
-                            self.time0 = datetime.strptime(data, "%Y-%m-%d %H:%M:%S")
-                        except:
-                            print('Creation_date {} could not be parsed as a datetime'.format(self.meta_data['creation_date']))
                 elif cmd == "ICRP":
                     self.meta_data['cropping_information'] = data
                 elif cmd == "IDIM":
                     self.meta_data['originating_object_dimensions'] = data
                 elif cmd == "IDPI":
                     self.meta_data['dots_per_inch'] = data
                 elif cmd == "IENG":
@@ -773,15 +768,15 @@
         return self.time0
 
     @property
     def archival_location(self):
         if "archival_location" in self.meta_data.keys():
             return self.meta_data["archival_location"]
         else:
-           return None
+            return None
 
     @property
     def artist(self):
         if "artist" in self.meta_data.keys():
             return self.meta_data["artist"]
         else:
             return None
@@ -936,158 +931,186 @@
     def write_chunk(self, writer: FileIO):
         """
         This function writes the contents of this LIST chunk to the file at the current cursor location
         :param writer: FileIO - The object controlling how the data is written to the file
         """
 
         #   Write the header command
-
         writer.write("LIST".encode('utf-8'))
 
         #   Get the position so that we know where to write the size of the chunk
-
         size_offset = writer.tell()
 
         #   At this point we do not know how big the chunk will be, so we will write a zero 4 byte value
-
         writer.write(struct.pack("<i", 0))
 
         #   Now store the location within the file so that we can calculate how big the chunk is
-
         start_byte = writer.tell()
         writer.write("INFO".encode('utf-8'))
 
-        self._write_list_chunk(writer, "IART", self.time0)
-
-        #   Work through each of the potential elements that may exist within the meta data and write it to the output
-        #   file if it exists within the dictionary
-
-        if "archival_location" in self.meta_data.keys():
-            self._write_list_chunk(writer, "IARL", self.meta_data["archival_location"])
-
-        if "artist" in self.meta_data.keys():
-            self._write_list_chunk(writer, "IART", self.meta_data["artist"])
-
-        if "commissioned_organization" in self.meta_data.keys():
-            self._write_list_chunk(writer, "ICMS", self.meta_data['commissioned_organization'])
-
-        if "general_comments" in self.meta_data.keys() or self.header is not None:
-            if self.header is not None:
-                if isinstance(self.header, dict):
-                    elements = list()
-                    for key in self.header.keys():
-                        elements.append("{}={}".format(key, self.header[key]))
+        #   Specify the names that we want to use in the creation of the contents of the list chunk. This dictionary
+        #   will contain the names of the objects in the metadata dictionary, and the data in the dictionary will be
+        #   the LIST chunk command. This is in effort to simplify the structure of this function.
+        list_commands = {"archival_location": "IARL",
+                         "artist": "IART",
+                         "commissioned_organization": "ICMS",
+                         "general_comments": "ICMT",
+                         "copyright": "ICOP",
+                         "creation_date": "ICRD",
+                         "cropping_information": "ICRP",
+                         "originating_object_dimensions": "IDIM",
+                         "dots_per_inch": "IDPI",
+                         "engineer_name": "IENG",
+                         "subject_genre": "IGNR",
+                         "key_words": "IKEY",
+                         "lightness_settings": "ILGT",
+                         "originating_object_medium": "IMED",
+                         "title": "INAM",
+                         "color_palette_count": "IPLT",
+                         "subject_name": "IPRD",
+                         "description": "ISBJ",
+                         "creation_software": "ISFT",
+                         "data_source": "ISRC",
+                         "original_form": "ISRF",
+                         "digitizing_engineer": "ITCH",
+                         "track_no": "ITRK"}
+
+        for key in list_commands.keys():
+            if key in self.meta_data.keys():
+                ListChunk._write_list_chunk(writer, list_commands[key], self.meta_data[key])
+
+        if self.header is not None:
+            if isinstance(self.header, dict):
+                elements = list()
+                for key in self.header.keys():
+                    elements.append("{}={}".format(key, self.header[key]))
 
-                self._write_list_chunk(writer, "ICMT", "|".join(elements))
+                ListChunk._write_list_chunk(writer, "ICMT", "|".join(elements))
             else:
-                self._write_list_chunk(writer, "ICMT", self.meta_data["general_comments"])
-
-        if "copyright" in self.meta_data.keys():
-            self._write_list_chunk(writer, "ICOP", self.meta_data['copyright'])
-
-        # if "creation_date" in self.meta_data.keys(): # There will always be a list chunk, there will always be a start time, there will always be a creation_date
-        self._write_list_chunk(writer, "ICRD", datetime.strftime(self.time0, "%Y-%m-%d %H:%M:%S.%f"))
-
-        if "cropping_information" in self.meta_data.keys():
-            self._write_list_chunk(writer, "ICRP", self.meta_data['cropping_information'])
-
-        if "originating_object_dimensions" in self.meta_data.keys():
-            self._write_list_chunk(writer, "IDIM", self.meta_data['originating_object_dimensions'])
-
-        if "dots_per_inch" in self.meta_data.keys():
-            self._write_list_chunk(writer, "IDPI", self.meta_data['dots_per_inch'])
-
-        if "engineer_name" in self.meta_data.keys():
-            self._write_list_chunk(writer, "IENG", self.meta_data['engineer_name'])
-
-        if "subject_genre" in self.meta_data.keys():
-            self._write_list_chunk(writer, "IGNR", self.meta_data['subject_genre'])
-
-        if "key_words" in self.meta_data.keys():
-            self._write_list_chunk(writer, "IKEY", self.meta_data['key_words'])
-
-        if "lightness_settings" in self.meta_data.keys():
-            self._write_list_chunk(writer, "ILGT", self.meta_data['lightness_settings'])
-
-        if "originating_object_medium" in self.meta_data.keys():
-            self._write_list_chunk(writer, "IMED", self.meta_data['originating_object_medium'])
-
-        if "title" in self.meta_data.keys():
-            self._write_list_chunk(writer, "INAM", self.meta_data['title'])
-
-        if "color_palette_count" in self.meta_data.keys():
-            self._write_list_chunk(writer, "IPLT", self.meta_data['color_palette_count'])
-
-        if "subject_name" in self.meta_data.keys():
-            self._write_list_chunk(writer, "IPRD", self.meta_data['subject_name'])
-
-        if "description" in self.meta_data.keys():
-            self._write_list_chunk(writer, "ISBJ", self.meta_data['description'])
-
-        if "creation_software" in self.meta_data.keys():
-            self._write_list_chunk(writer, "ISFT", self.meta_data['creation_software'])
-
-        if "data_source" in self.meta_data.keys():
-            self._write_list_chunk(writer, "ISRC", self.meta_data['data_source'])
-
-        if "original_form" in self.meta_data.keys():
-            self._write_list_chunk(writer, "ISRF", self.meta_data['original_form'])
+                ListChunk._write_list_chunk(writer, "ICMT", self.meta_data["general_comments"])
 
-        if "digitizing_engineer" in self.meta_data.keys():
-            self._write_list_chunk(writer, "ITCH", self.meta_data['digitizing_engineer'])
-
-        if "track_no" in self.meta_data.keys():
-            self._write_list_chunk(writer, "ITRK", self.meta_data['track_no'])
+        # #   Work through each of the potential elements that may exist within the metadata and write it to the output
+        # #   file if it exists within the dictionary
+        # if "archival_location" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "IARL", self.meta_data["archival_location"])
+        #
+        # if "artist" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "IART", self.meta_data["artist"])
+        #
+        # if "commissioned_organization" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "ICMS", self.meta_data['commissioned_organization'])
+        #
+        # if "general_comments" in self.meta_data.keys() or self.header is not None:
+        #     if self.header is not None:
+        #         if isinstance(self.header, dict):
+        #             elements = list()
+        #             for key in self.header.keys():
+        #                 elements.append("{}={}".format(key, self.header[key]))
+        #
+        #         self._write_list_chunk(writer, "ICMT", "|".join(elements))
+        #     else:
+        #         self._write_list_chunk(writer, "ICMT", self.meta_data["general_comments"])
+        #
+        # if "copyright" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "ICOP", self.meta_data['copyright'])
+        #
+        # #   To provide the start time inside the wave files we will ensure that the WaveFile class always creates a
+        # #   list chunk, and that the chunk will always contain a creation date object. Thus we do not check to see if
+        # #   it exists within the dictionary.
+        # self._write_list_chunk(writer, "ICRD", datetime.strftime(self.time0, "%Y-%m-%d %H:%M:%S.%f"))
+        #
+        # if "cropping_information" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "ICRP", self.meta_data['cropping_information'])
+        #
+        # if "originating_object_dimensions" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "IDIM", self.meta_data['originating_object_dimensions'])
+        #
+        # if "dots_per_inch" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "IDPI", self.meta_data['dots_per_inch'])
+        #
+        # if "engineer_name" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "IENG", self.meta_data['engineer_name'])
+        #
+        # if "subject_genre" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "IGNR", self.meta_data['subject_genre'])
+        #
+        # if "key_words" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "IKEY", self.meta_data['key_words'])
+        #
+        # if "lightness_settings" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "ILGT", self.meta_data['lightness_settings'])
+        #
+        # if "originating_object_medium" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "IMED", self.meta_data['originating_object_medium'])
+        #
+        # if "title" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "INAM", self.meta_data['title'])
+        #
+        # if "color_palette_count" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "IPLT", self.meta_data['color_palette_count'])
+        #
+        # if "subject_name" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "IPRD", self.meta_data['subject_name'])
+        #
+        # if "description" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "ISBJ", self.meta_data['description'])
+        #
+        # if "creation_software" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "ISFT", self.meta_data['creation_software'])
+        #
+        # if "data_source" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "ISRC", self.meta_data['data_source'])
+        #
+        # if "original_form" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "ISRF", self.meta_data['original_form'])
+        #
+        # if "digitizing_engineer" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "ITCH", self.meta_data['digitizing_engineer'])
+        #
+        # if "track_no" in self.meta_data.keys():
+        #     self._write_list_chunk(writer, "ITRK", self.meta_data['track_no'])
 
         #   Now that we have walked through each of the potential elements of the LIST chunk, we need to determine the
         #   size of the chunk
-
         chunk_size = writer.tell() - start_byte
 
         #   Update the size
-
         writer.seek(size_offset, 0)
         writer.write(struct.pack("<i", chunk_size))
 
         #   Now move back to the end of the file
-
         writer.seek(0, 2)
 
-    def _write_list_chunk(self, writer: FileIO, id: str, contents):
+    @staticmethod
+    def _write_list_chunk(writer: FileIO, id: str, contents):
         """
         This is a private helper function that assists in writing the data to the LIST chunk.
         :param writer: FileIO - the writer object
         :param id: str - the string identifier for the chunk that is within the accepted LIST commands
         :param contents: str - the data to write to the file
         """
 
         if not isinstance(contents, str):
             contents = "{}".format(contents)
 
         byte_count = 0
 
         #   write the command
-
         writer.write(id.encode('utf-8'))
 
         #   post-pend the null character
-
         contents += '\0'
 
         #   Ensure that there is an even number of bytes
-
         if len(contents) % 2 != 0:
             contents += '\0'
 
         #   Write the length of the string in bytes
-
         writer.write(struct.pack("<i", len(contents)))
-
         byte_count += 8
-
         writer.write(contents.encode('utf-8'))
         byte_count += len(contents)
 
         return byte_count
 
 
 class XMLChunk(ChunkInformation):
@@ -1184,14 +1207,18 @@
 
 class WaveFile(Waveform):
     """
     This class mimics information within the NAudio interface and will read a wave file, however it will only process
     the canonical chunks: RIFF, WAVE, fmt, and data.
 
     http://www-mmsp.ece.mcgill.ca/Documents/AudioFormats/WAVE/WAVE.html
+
+    In favor of using the LIST chunk within the WaveFile rather than using the Waveform.start_time, properties were
+    created within this class to expose the creation date property within the list chunk to hold and expose the start
+    time of the waveform.
     """
 
     @staticmethod
     def audio_info(path: str):
         """
         Sometimes it is important to obtain information about the audio within the wave file without actually reading
         the audio data.  This will scan the chunks and extract the information about the audio from that info.
@@ -1206,30 +1233,36 @@
         """
 
         scanner = ChunkScanner(path)
 
         with open(path, 'rb') as file:
 
             #   The format chunk is required by all wav files
-            format_chunk = FormatChunk(file, scanner.format_chunk.chunk_offset, scanner.format_chunk.chunk_size,
-                                       scanner.format_chunk.chunk_name)
+            format_chunk = FormatChunk(
+                file, scanner.format_chunk.chunk_offset, scanner.format_chunk.chunk_size,
+                scanner.format_chunk.chunk_name
+            )
 
             #   If there is a peak chunk, read it
 
             if scanner.peak_chunk is not None:
-                peak_chunk = PeakChunk(file, scanner.peak_chunk.chunk_offset, scanner.peak_chunk.chunk_size,
-                                       scanner.peak_chunk.chunk_name, format_chunk.channel_count)
+                peak_chunk = PeakChunk(
+                    file, scanner.peak_chunk.chunk_offset, scanner.peak_chunk.chunk_size,
+                    scanner.peak_chunk.chunk_name, format_chunk.channel_count
+                )
             else:
                 peak_chunk = None
 
             #   If there is a list chunk, read it
 
             if scanner.list_chunk is not None:
-                list_chunk = ListChunk(file, scanner.list_chunk.chunk_size, scanner.list_chunk.chunk_offset,
-                                       scanner.list_chunk.chunk_name)
+                list_chunk = ListChunk(
+                    file, scanner.list_chunk.chunk_size, scanner.list_chunk.chunk_offset,
+                    scanner.list_chunk.chunk_name
+                )
                 time0 = list_chunk.time0
                 if list_chunk.cropping_information is not None:
                     if list_chunk.cropping_information == "normalized":
                         normalized = True
                     else:
                         normlized = False
                 else:
@@ -1251,158 +1284,257 @@
                            'duration': duration,
                            'has_peak_chunk': scanner.peak_chunk is not None,
                            'has_list_chunk': scanner.list_chunk is not None,
                            'has_xml_chunk': scanner.xml_chunk is not None}
 
         return information
 
-    def __init__(self, path=None, s0: int = None, s1: int = None, fs: int = None, samples=None, time=None, get_peak:bool = True):
+    def _read_format_chunk(self, file):
         """
-        This constructor reads the chunks from the wave file and then processes those that are canonical.
+        To further reduce the cognitive complexity of the functions, this will read the format chunk from the file
 
-        :param path: str - the full path to the file that we want to read
-        :param s0: int - the starting sample for the reading of the audio file
-        :param s1: int - the ending sample for the reading of the audio file
-        :param fs: int - the number of samples per second.  This facilitates calling the based class with the required
-            data
-        :param samples: ndarray - the actual samples to define the waveform
-        :param time: float or datetime - the time of the first sample
-        :param get_peak: bool - whether or not the constructor should get the peak value (and create the peak chunk). Getting this value doubles memory usage.
+        :param file:
+            The file reader that provides access to the file's contents
         """
+        self.format_chunk = FormatChunk(
+            file,
+            self.scanner.format_chunk.chunk_offset,
+            self.scanner.format_chunk.chunk_size,
+            self.scanner.format_chunk.chunk_name
+        )
+        self.sample_rate = self.format_chunk.sample_rate
 
-        # warnings.warn('Test for Insert Start Time using wfm.start_time=...is failing.')
-        # TODO - Correct the wfm.start_time setting feature.
+    def _read_peak_chunk(self, file):
+        """
+        To further reduce the cognitive complexity of the functions, this will read the format chunk from the file
 
-        if path is None:
-            if(fs is None) and (samples is None) and (time is None):
-                self.samples = None
-                self.start_time = None
-                self.sample_rate = None
-                self.list_chunk = ListChunk()
-                self.format_chunk = FormatChunk()
-                self.peak_chunk = None
-                self.normalized = False
-            elif (fs is not None) and (samples is not None):
-                if time is None:
-                    t0 = 0
+        :param file:
+            The file reader that provides access to the file's contents
+        """
+        if self.scanner.peak_chunk is not None:
+            self.peak_chunk = PeakChunk(
+                file,
+                self.scanner.peak_chunk.chunk_offset,
+                self.scanner.peak_chunk.chunk_size,
+                self.scanner.peak_chunk.chunk_name,
+                self.format_chunk.channel_count
+            )
+        else:
+            self.peak_chunk = None
+
+    def _read_list_chunk(self, file):
+        """
+        To further reduce the cognitive complexity of the functions, this will read the format chunk from the file
+
+        :param file:
+            The file reader that provides access to the file's contents
+        """
+
+        if self.scanner.list_chunk is not None:
+            self.list_chunk = ListChunk(
+                file,
+                self.scanner.list_chunk.chunk_size,
+                self.scanner.list_chunk.chunk_offset,
+                self.scanner.list_chunk.chunk_name
+            )
+            if self.list_chunk.cropping_information is not None:
+                if self.list_chunk.cropping_information == "normalized":
+                    self.normalized = True
                 else:
-                    t0 = time
+                    self.normalized = False
+            else:
+                self.normalized = False
+        else:
+            #   If there is no list chunk in the file, create one so that we can hold the start_time data for the
+            #   waveform
+            self.list_chunk = ListChunk()
+            self.normalized = False
 
-                super().__init__(samples, sample_rate=fs, start_time=t0)
+    def _read_xml_chunk(self, file):
+        """
+        To further reduce the cognitive complexity of the functions, this will read the format chunk from the file
 
-                #   Now build the format chunk from this information
+        :param file:
+            The file reader that provides access to the file's contents
+        """
+        if self.scanner.xml_chunk is not None:
+            self.xml_chunk = XMLChunk(
+                file,
+                self.scanner.xml_chunk.chunk_size,
+                self.scanner.xml_chunk.chunk_offset,
+                self.scanner.xml_chunk.chunk_name
+            )
 
-                self.format_chunk = FormatChunk()
+            #   You can store the start time in the XML chunk if using Broadcast Wave Format. So this should be
+            #   called after the _read_list_chunk so that we can guarantee that there is a list chunk within the
+            #   class and that the time is overwritten based on what was contained in the XML chunk
+            self.start_time = self.xml_chunk.start_time
+        else:
+            self.xml_chunk = None
 
-                if len(self.samples.shape) == 1:
-                    self.format_chunk.channel_count = 1
-                else:
-                    self.format_chunk.channel_count = self.samples.shape[1]
+    def _read_fact_chunk(self, file):
+        """
+        To further reduce the cognitive complexity of the functions, this will read the format chunk from the file
 
-                self.peak_chunk = None
-                self.list_chunk = ListChunk()
+        :param file:
+            The file reader that provides access to the file's contents
+        """
+        if self.scanner.fact_chunk is not None:
+            self.fact_chunk = FactChunk(
+                file,
+                self.scanner.format_chunk.chunk_offset,
+                self.scanner.format_chunk.chunk_offset,
+                self.scanner.format_chunk.chunk_name
+            )
+        else:
+            self.fact_chunk = None
 
-            self.normalized = False
+    def _read_data_chunk(self, file, s0: int, s1: int):
+        """
+        To further reduce the cognitive complexity of the functions, this will read the format chunk from the file
 
-            return
+        :param file:
+            The file reader that provides access to the file's contents
+        :param s0:
+            The start sample for reading the data from the file
+        :param s1:
+            The end sample for reading the data from the file
+        """
+        self.data_chunk = DataChunk(
+            file,
+            self.scanner.data_chunk.chunk_offset,
+            self.scanner.data_chunk.chunk_size,
+            self.scanner.data_chunk.chunk_name,
+            self.format_chunk,
+            self.peak_chunk,
+            s0,
+            s1,
+            self.normalized
+        )
 
-        if not isinstance(path, str):
-            raise ValueError("You must provide the path to the file")
+    def _read_file(self, path: str, s0: int, s1: int, get_peak: bool):
+        """
+        This function reads the contents of the WaveFile based on the canonical format.
 
-        if not os.path.exists(path):
-            raise ValueError("The supplied path ({})does not lead to a valid file".format(path))
+        :param path:
+            The path to the file that we want to read.
+        :param s0:
+            The start sample for reading the data from the file
+        :param s1:
+            The end sample for reading the data from the file
+        """
 
+        #   Store the name of the file within the property
         self.filename = path
 
         #   Parse the chunks
-
         self.scanner = ChunkScanner(self.filename)
 
         #   Now open the file and read the information from the format and peak chunks for the class
-
         with open(self.filename, 'rb') as file:
+            #   Call functions within the protected section of the class to read the various chunks, if they exist
+            #   within the file
+            self._read_format_chunk(file)
+            self._read_peak_chunk(file)
+            self._read_list_chunk(file)
+            self._read_xml_chunk(file)
+            self._read_fact_chunk(file)
+            self._read_data_chunk(file, s0, s1)
 
-            #   The format chunk is required by all wav files
-            self.format_chunk = FormatChunk(file,
-                                            self.scanner.format_chunk.chunk_offset,
-                                            self.scanner.format_chunk.chunk_size,
-                                            self.scanner.format_chunk.chunk_name)
-            self.sample_rate = self.format_chunk.sample_rate
+            #   If the peak chunk was not read from the file, we need to create one from the data that was read from
+            #   the wav file.
 
-            #   If there is a peak chunk, read it
+            if self.peak_chunk is None and get_peak:
+                self.peak_chunk = PeakChunk()
+                self.peak_chunk.peak_amplitude = np.max(self.data_chunk.waveform, axis=0)
+                self.peak_chunk.peak_sample = np.argmax(self.data_chunk.waveform, axis=0)
 
-            if self.scanner.peak_chunk is not None:
-                self.peak_chunk = PeakChunk(file,
-                                            self.scanner.peak_chunk.chunk_offset,
-                                            self.scanner.peak_chunk.chunk_size,
-                                            self.scanner.peak_chunk.chunk_name,
-                                            self.format_chunk.channel_count)
-            else:
-                self.peak_chunk = None
+        #   Create the data and build the information for the generic_time_waveform
+        super().__init__(self.data_chunk.waveform, self.format_chunk.sample_rate, self.start_time)
 
-            #   If there is a list chunk, read it
+    def _build_waveform(self, fs=None, samples=None, time=None):
+        """
+        This function permits the construction of the waveform from the arguments passed to the constructor rather
+        than reading the file.
 
-            if self.scanner.list_chunk is not None:
-                self.list_chunk = ListChunk(file,
-                                            self.scanner.list_chunk.chunk_size,
-                                            self.scanner.list_chunk.chunk_offset,
-                                            self.scanner.list_chunk.chunk_name)
-                if self.list_chunk.cropping_information is not None:
-                    if self.list_chunk.cropping_information == "normalized":
-                        self.normalized = True
-                    else:
-                        self.normalized = False
-                else:
-                    self.normalized = False
+        :param fs: int - the number of samples per second.  This facilitates calling the based class with the required
+            data
+        :param samples: ndarray - the actual samples to define the waveform
+        :param time: float or datetime - the time of the first sample
+        """
+        if (fs is None) and (samples is None) and (time is None):
+            #   Build a blank Waveform
+            self.list_chunk = ListChunk()
+            self.format_chunk = FormatChunk()
+            self.samples = None
+            self.start_time = None
+            self.sample_rate = None
+            self.peak_chunk = None
+            self.normalized = False
+        elif (fs is not None) and (samples is not None):
+            #   Construct a waveform from the information passed to the function
+            #
+            #   If the time is not specified, the set it to floating point zero
+            if time is None:
+                t0 = 0
             else:
-                self.list_chunk = ListChunk()
-                self.normalized = False
-            time0 = self.list_chunk.time0
+                t0 = time
 
-            if self.scanner.xml_chunk is not None:
-                self.xml_chunk = XMLChunk(file,
-                                          self.scanner.xml_chunk.chunk_size,
-                                          self.scanner.xml_chunk.chunk_offset,
-                                          self.scanner.xml_chunk.chunk_name)
+            #   Call the parent constructor
+            super().__init__(samples, sample_rate=fs, start_time=t0)
 
-                time0 = self.xml_chunk.start_time
-            else:
-                self.xml_chunk = None
+            #   Now build the format chunk from this information
+            self.format_chunk = FormatChunk()
 
-            if self.scanner.fact_chunk is not None:
-                self.fact_chunk = FactChunk(file,
-                                            self.scanner.format_chunk.chunk_offset,
-                                            self.scanner.format_chunk.chunk_offset,
-                                            self.scanner.format_chunk.chunk_name)
+            #   Specify the channel count within the Format Chunk
+            if len(self.samples.shape) == 1:
+                self.format_chunk.channel_count = 1
             else:
-                self.fact_chunk = None
+                self.format_chunk.channel_count = self.samples.shape[1]
 
-            #   Read the data chunk, which is also required by all Wav files
+            #   Create an empty peak chunk and a blank list chunk
+            self.peak_chunk = None
+            self.list_chunk = ListChunk()
 
-            self.data_chunk = DataChunk(file,
-                                        self.scanner.data_chunk.chunk_offset,
-                                        self.scanner.data_chunk.chunk_size,
-                                        self.scanner.data_chunk.chunk_name,
-                                        self.format_chunk,
-                                        self.peak_chunk,
-                                        s0,
-                                        s1,
-                                        self.normalized)
+            #   Since the contents of the WaveFile use the ListChunk's start_time, let's overwrite the representation
+            #   of the start time now to ensure that it is stored in the list chunk
+            self.start_time = t0
 
-            #   If the peak chunk was not read from the file, we need to create one from the data that was read from
-            #   the wav file.
+        self.normalized = False
 
-            if self.peak_chunk is None and get_peak:
-                self.peak_chunk = PeakChunk()
-                self.peak_chunk.peak_amplitude = np.max(self.data_chunk.waveform, axis=0)
-                self.peak_chunk.peak_sample = np.argmax(self.data_chunk.waveform, axis=0)
+    def __init__(
+            self, path=None, s0: int = None, s1: int = None, fs: int = None, samples=None, time=None,
+            get_peak: bool = True):
+        """
+        This constructor reads the chunks from the wave file and then processes those that are canonical.
 
-        #   Create the data and build the information for the generic_time_waveform
+        :param path: str - the full path to the file that we want to read
+        :param s0: int - the starting sample for the reading of the audio file
+        :param s1: int - the ending sample for the reading of the audio file
+        :param fs: int - the number of samples per second.  This facilitates calling the based class with the required
+            data
+        :param samples: ndarray - the actual samples to define the waveform
+        :param time: float or datetime - the time of the first sample
+        :param get_peak: bool - whether the constructor should get the peak value (and create the peak chunk).
+        Getting this value doubles memory usage.
+        """
 
-        super().__init__(self.data_chunk.waveform, self.format_chunk.sample_rate, time0)
+        # warnings.warn('Test for Insert Start Time using wfm.start_time=...is failing.')
+        # TODO - Correct the wfm.start_time setting feature.
+
+        if path is None:
+            self._build_waveform(fs, samples, time)
+        elif path is not None:
+            if not isinstance(path, str):
+                raise ValueError("You must provide the path to the file")
+
+            if not os.path.exists(path):
+                raise ValueError("The supplied path ({})does not lead to a valid file".format(path))
+
+            self._read_file(path, s0, s1, get_peak)
 
     @property
     def full_path(self):
         """
         The fully realized path to the file that was read
         """
 
@@ -1751,14 +1883,31 @@
     def track_number(self):
         return self.list_chunk.track_number
 
     @track_number.setter
     def track_number(self, value):
         self.list_chunk.meta_data['track_no'] = value
 
+    @property
+    def start_time(self):
+        if isinstance(self.list_chunk.meta_data['creation_date'], str):
+            if self.list_chunk.meta_data['creation_date'].isdigit():
+                return float(self.list_chunk.meta_data['creation_date'])
+            else:
+                try:
+                    return datetime.strptime(self.list_chunk.meta_data['creation_date'], "%Y-%m-%d %H:%M:%S.%f")
+                except ValueError:
+                    return datetime.strptime(self.list_chunk.meta_data['creation_date'], "%Y-%m-%d %H:%M:%S")
+        else:
+            return self.list_chunk.meta_data['creation_date']
+
+    @start_time.setter
+    def start_time(self, value):
+        self.list_chunk.meta_data['creation_date'] = value
+
     def save(self, path):
         """
         This function will save the data to a canonical wav formatted file with appropriate scaling to recover the
         actual Pascal values.
 
         :param path: str - the output path for the scaled canonical wav format
         """
@@ -1809,30 +1958,32 @@
 
             samples_to_write = np.reshape(self.samples, (np.product(self.samples.shape),))
             file.write(samples_to_write.astype("<f").tobytes())
 
             #   Write the LIST chunk
 
             # if self.list_chunk is not None: # There will always be a list chunk
-            if self.creation_date is not None:
-                self.list_chunk.time0 = self.creation_date
-            else:
-                #   To ensure that the wave file can be saved without saving the start time as a start time
-                if self.start_time is not None and not isinstance(self.start_time, datetime):
+            if self.creation_date is None:
+                self.creation_date = datetime.now()
+            if self.start_time is not None:
+                if not isinstance(self.start_time, datetime):
                     self.list_chunk.time0 = datetime.now()
+                else:
+                    self.list_chunk.time0 = self.start_time
+
             self.list_chunk.write_chunk(file)
 
             #   Get the current number of bytes within the file
 
             file_size = file.tell()
 
             #   Search for the file size - 8 within the header and update the information
 
             file.seek(4, 0)
-            file.write(struct.pack("<i", file_size-8))
+            file.write(struct.pack("<i", file_size - 8))
 
     def resample_16kHz_16bit(self, channel_index: int = 0):
         """
         In preparation for the transcription of the waveform with the Vosk wrapping of the Kaldi models we need to
         transform this signal to a 16 Khz, 16-bit signal.  This function performs the resmapling and scaling and returns
         the byte-array that is directly provided to the Vosk interface.
```

### Comparing `PyTimbre-0.7.2/src/pytimbre/spectral/acoustic_weights.py` & `PyTimbre-0.7.3/src/pytimbre/spectral/acoustic_weights.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.7.2/src/pytimbre/spectral/fractional_octave_band.py` & `PyTimbre-0.7.3/src/pytimbre/spectral/fractional_octave_band.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.7.2/src/pytimbre/spectral/fundamental_frequency.py` & `PyTimbre-0.7.3/src/pytimbre/spectral/fundamental_frequency.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.7.2/src/pytimbre/spectral/spectra.py` & `PyTimbre-0.7.3/src/pytimbre/spectral/spectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -707,27 +707,28 @@
         sens *= -1
         sens = 10.0 ** sens
 
         return sens
 
     def get_average_features(
             self, include_sq_metrics: bool = True, include_temporal_features: bool = True,
-            include_spectral_features: bool = True, include_harmonic_features: bool = True
+            include_spectral_features: bool = True, include_harmonic_features: bool = True,
+            include_speech_features: bool = True
             ):
         """
         This will return a dict of the various elements within the spectrum and waveform (if it was used to create the
         spectrogram object) with any time variant elements averaged.
         """
 
         #   Create the dictionary that will hold the data
         features = dict()
 
         #   If there is a waveform inside the Spectrum object, and we desire the temporal statistics
         if self.waveform is not None and include_temporal_features:
-            features = self.waveform.get_features(include_sq_metrics)
+            features = self.waveform.get_features(include_sq_metrics, include_speech_features)
             features['zero_crossing_rate'] = np.mean(features['zero crossing rate'])
             auto_correlation_coefficients = np.mean(features['auto-correlation'], axis=0)
 
             if include_sq_metrics:
                 features['loudness'] = np.mean(features['loudness'])
                 features['sharpness'] = np.mean(features['sharpness'])
                 features['roughness'] = np.mean(features['roughness'])
@@ -1201,14 +1202,15 @@
         s = Spectrum()
         s.frequencies = f_fob
         s.pressures_pascals = p_fob
         s.start_fractional_octave_frequency = f0
         s.stop_fractional_octave_frequency = f1
         s.fractional_octave_bandwidth = bandwidth
         s._time0 = self.time
+        s._waveform = self.waveform
 
         return s
 
 
 class SpectrumByDigitalFilters(Spectrum):
     """
     This class differs from the previous classes in that the determination of the spectrum is accomplished through an
```

### Comparing `PyTimbre-0.7.2/src/pytimbre/spectral/spectrogram.py` & `PyTimbre-0.7.3/src/pytimbre/spectral/spectrogram.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.7.2/src/pytimbre/spectral/swipe.py` & `PyTimbre-0.7.3/src/pytimbre/spectral/swipe.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,378 +1,378 @@
-from scipy import interpolate
-import numpy as np
-# import librosa
-import scipy.signal
-from .spectra import Spectrum
-
-"""
-| Description: libf0 SWIPE implementation
-| Contributors: Sebastian Rosenzweig, Vojtěch Pešek, Simon Schwär, Meinard Müller
-| License: The MIT license, https://opensource.org/licenses/MIT
-| This file is part of libf0.
-"""
-"""
-This file was downloaded on 1 April 2023, from https://github.com/groupmm/libf0. This swipe.py file was integrated into
-the structure of the PyTimbre module to facilitate the calculation of the fundamental frequency. However, there are a
-number of dependencies that were not required by PyTimbre. 
-
-2023_04_01 - FSM - Function arguments were normalized to the standard Python rules.
-2023-04-06 - FSM - Updated the swipe function to use the SciPy.Signal.STFT function rather than librosa
-2023-04-06 - FSM - Removed all functions that rely on librosa
-"""
-
-
-def swipe_spectral_estimation(x: Spectrum, hop_size: float = 256, minimum_frequency: float = 10.0,
-                              maximum_frequency: float = 10000, pitch_resolution: float = 1 / 100,
-                              erb_resolution: float = 0.1,
-                              strength_threshold: float = 0):
-    if x.waveform is None:
-        raise ValueError("At this point, you must provide a Spectrum object that has been created from a waveform")
-    t = x.time
-
-    # Compute pitch candidates
-    pc = 2 ** np.arange(np.log2(minimum_frequency), np.log2(maximum_frequency), pitch_resolution)
-
-    # Pitch strength matrix
-    S = np.zeros((len(pc),))
-
-    # Determine P2-WSs [max, min]
-    log_ws = np.round(np.log2(np.divide(8 * x.waveform.sample_rate, [minimum_frequency, maximum_frequency])))
-
-    # P2-WSs - window sizes in samples
-    ws = len(x.frequencies)
-
-    # Determine window sizes used by each pitch candidate
-    log2pc = np.arange(np.log2(minimum_frequency), np.log2(maximum_frequency), pitch_resolution)
-    d = log2pc - np.log2(np.divide(8 * x.waveform.sample_rate, ws))
-
-    # Create ERBs spaced frequencies (in Hertz)
-    f_erbs = erbs2hz(np.arange(hz2erbs(pc[0] / 4), hz2erbs(x.waveform.sample_rate / 2), erb_resolution))
-
-    #   Resample the frequency spectrum to the ERB frequencies
-    loudness = interpolate.splev(f_erbs, interpolate.splrep(x.frequencies, x.pressures_pascals ** 2))
-    # loudness = np.sqrt(magnitude)
-
-    pc_to_compute = pc
-
-    # Normalize loudness
-    normalization_loudness = np.full_like(loudness, np.sqrt(np.sum(loudness * loudness, axis=0)))
-    with np.errstate(divide='ignore', invalid='ignore'):
-        loudness = loudness / normalization_loudness
-
-    # Create pitch salience matrix
-    S = np.zeros((len(pc_to_compute),))
-
-    for j in range(0, len(pc_to_compute)):
-        S[j] = pitch_strength_one(f_erbs, loudness, pc_to_compute[j])
-
-    # pitch_strength = pitch_strength_all_candidates(f_erbs, loudness, pc_to_compute)
-
-    pitches, strength = parabolic_interpolation(S, strength_threshold, pc)
-
-    if np.isnan(pitches):
-        pitches = 0  # avoid NaN output
-
-    return pitches, t, strength
-
-
-def swipe(samples, sample_rate: float = 22050, hop_size: float = 256, minimum_frequency: float = 55.0,
-          maximum_frequency: float = 1760.0, pitch_resolution: float = 1 / 96, erb_resolution: float = 0.1,
-          strength_threshold: float = 0):
-    """
-    Implementation of a sawtooth waveform inspired pitch estimator (SWIPE).
-    This version of the algorithm follows the original implementation, see `swipe_slim` for a more efficient
-    alternative.
-
-    .. [#] Arturo Camacho and John G. Harris,
-       "A sawtooth waveform inspired pitch estimator for speech and music."
-       The Journal of the Acoustical Society of America, vol. 124, no. 3, pp. 1638–1652, Sep. 2008
-
-    Parameters
-    ----------
-    samples : ndarray
-        Audio signal
-    sample_rate : int
-        Sampling rate
-    hop_size : int
-        Hop size
-    minimum_frequency : float or int
-        Minimal frequency
-    maximum_frequency : float or int
-        Maximal frequency
-    pitch_resolution : float
-        resolution of the pitch candidate bins in octaves (default value = 1/96 -> 96 bins per octave)
-    erb_resolution : float
-        resolution of the ERB bands (default value = 0.1)
-    strength_threshold : float
-        confidence threshold [0, 1] for the pitch detection (default value = 0)
-
-    Returns
-    -------
-    f0 : ndarray
-        Estimated F0-trajectory
-    t : ndarray
-        Time axis
-    strength : ndarray
-        Confidence/Pitch Strength
-
-    Remarks/Development
-    2023-04-01 - FSM - updated the argument names, and put the parameter helpers into the list
-    """
-
-    t = np.arange(0, len(samples), hop_size) / sample_rate  # Times
-
-    # Compute pitch candidates
-    pc = 2 ** np.arange(np.log2(minimum_frequency), np.log2(maximum_frequency), pitch_resolution)
-
-    # Pitch strength matrix
-    S = np.zeros((len(pc), len(t)))
-
-    # Determine P2-WSs [max, min]
-    log_ws = np.round(np.log2(np.divide(8 * sample_rate, [minimum_frequency, maximum_frequency])))
-
-    # P2-WSs - window sizes in samples
-    ws = 2 ** np.arange(log_ws[0], log_ws[1] - 1, -1, dtype=np.int32)
-
-    # Determine window sizes used by each pitch candidate
-    log2pc = np.arange(np.log2(minimum_frequency), np.log2(maximum_frequency), pitch_resolution)
-    d = log2pc - np.log2(np.divide(8 * sample_rate, ws[0]))
-
-    # Create ERBs spaced frequencies (in Hertz)
-    f_erbs = erbs2hz(np.arange(hz2erbs(pc[0] / 4), hz2erbs(sample_rate / 2), erb_resolution))
-
-    for i in range(0, len(ws)):
-        N = ws[i]
-        hop_size = int(N / 2)
-
-        x_zero_padded = np.concatenate([samples, np.zeros(N)])
-
-        f, ti, x = scipy.signal.stft(x_zero_padded,
-                                     fs=sample_rate,
-                                     nperseg=hop_size,
-                                     nfft=N,
-                                     scaling='psd',
-                                     boundary='zeros',
-                                     padded=True)
-
-        ti = np.insert(ti, 0, 0)
-        ti = np.delete(ti, -1)
-
-        spectrum = np.abs(x)
-        magnitude = resample_ferbs(spectrum, f, f_erbs)
-        loudness = np.sqrt(magnitude)
-
-        # Select candidates that use this window size
-        # First window
-        if i == 0:
-            j = np.argwhere(d < 1).flatten()
-            k = np.argwhere(d[j] > 0).flatten()
-        # Last Window
-        elif i == len(ws) - 1:
-            j = np.argwhere(d - i > -1).flatten()
-            k = np.argwhere(d[j] - i < 0).flatten()
-        else:
-            j = np.argwhere(np.abs(d - i) < 1).flatten()
-            k = np.arange(0, len(j))
-
-        pc_to_compute = pc[j]
-
-        pitch_strength = pitch_strength_all_candidates(f_erbs, loudness, pc_to_compute)
-
-        resampled_pitch_strength = resample_time(pitch_strength, t, ti)
-
-        lambda_ = d[j[k]] - i
-        mu = np.ones(len(j))
-        mu[k] = 1 - np.abs(lambda_)
-
-        S[j, :] = S[j, :] + np.multiply(
-            np.ones(resampled_pitch_strength.shape) * mu.reshape((mu.shape[0], 1)),
-            resampled_pitch_strength
-        )
-
-    # Fine-tune the pitch using parabolic interpolation
-    pitches, strength = parabolic_int(S, strength_threshold, pc)
-
-    pitches[np.where(np.isnan(pitches))] = 0  # avoid NaN output
-
-    return pitches, t, strength
-
-
-def nyquist(sample_rate):
-    """Nyquist Frequency"""
-    return sample_rate / 2
-
-
-def frequency_coefficients(k, fft_size, sample_rate):
-    """Physical frequency of STFT coefficients"""
-    return (k * sample_rate) / fft_size
-
-
-def time_values(m, hop_size, sample_rate):
-    """Physical time of STFT coefficients"""
-    return m * hop_size / sample_rate
-
-
-def hz2erbs(hz):
-    """Convert Hz to ERB scale"""
-    return 21.4 * np.log10(1 + hz / 229)
-
-
-def erbs2hz(erbs):
-    """Convert ERB to Hz"""
-    return (10 ** np.divide(erbs, 21.4) - 1) * 229
-
-
-def pitch_strength_all_candidates(ferbs, loudness, pitch_candidates):
-    """Compute pitch strength for all pitch candidates"""
-    # Normalize loudness
-    normalization_loudness = np.full_like(loudness, np.sqrt(np.sum(loudness * loudness, axis=0)))
-    with np.errstate(divide='ignore', invalid='ignore'):
-        loudness = loudness / normalization_loudness
-
-    # Create pitch salience matrix
-    S = np.zeros((len(pitch_candidates), loudness.shape[1]))
-
-    for j in range(0, len(pitch_candidates)):
-        S[j, :] = pitch_strength_one(ferbs, loudness, pitch_candidates[j])
-    return S
-
-
-def pitch_strength_one(erbs_frequencies, normalized_loudness, pitch_candidate):
-    """Compute pitch strength for one pitch candidate"""
-    number_of_harmonics = np.floor(erbs_frequencies[-1] / pitch_candidate - 0.75).astype(np.int32)
-    k = np.zeros(erbs_frequencies.shape)
-
-    # f_prime / f
-    q = erbs_frequencies / pitch_candidate
-
-    for i in np.concatenate(([1], primes(number_of_harmonics))):
-        a = np.abs(q - i)
-        p = a < 0.25
-        k[p] = np.cos(np.dot(2 * np.pi, q[p]))
-        v = np.logical_and(0.25 < a, a < 0.75)
-        k[v] = k[v] + np.cos(np.dot(2 * np.pi, q[v])) / 2
-
-    # Apply envelope
-    k = np.multiply(k, np.sqrt(1.0 / erbs_frequencies))
-
-    # K+-normalize kernel
-    k = k / np.linalg.norm(k[k > 0])
-
-    # Compute pitch strength
-    S = np.dot(k, normalized_loudness)
-    return S
-
-
-def resample_ferbs(spectrum, f, ferbs):
-    """Resample to ERB scale"""
-
-    magnitude = np.zeros((len(ferbs), spectrum.shape[1]))
-
-    for t in range(spectrum.shape[1]):
-        spl = interpolate.splrep(f, spectrum[:, t])
-        interpolate.splev(ferbs, spl)
-
-        magnitude[:, t] = interpolate.splev(ferbs, spl)
-
-    return np.maximum(magnitude, 0)
-
-
-def resample_time(pitch_strength, resampled_time, ti):
-    """Resample time axis"""
-    if pitch_strength.shape[1] > 0:
-        pitch_strength = interpolate_one_candidate(pitch_strength, ti, resampled_time)
-    else:
-        pitch_strength = np.kron(np.ones((len(pitch_strength), len(resampled_time))), np.NaN)
-    return pitch_strength
-
-
-def interpolate_one_candidate(pitch_strength, ti, resampled_time):
-    """Interpolate time axis"""
-    pitch_strength_interpolated = np.zeros((pitch_strength.shape[0], len(resampled_time)))
-
-    for s in range(pitch_strength.shape[0]):
-        t_i = interpolate.interp1d(ti, pitch_strength[s, :], 'linear', bounds_error=True)
-        pitch_strength_interpolated[s, :] = t_i(resampled_time)
-
-    return pitch_strength_interpolated
-
-
-def parabolic_int(pitch_strength, strength_threshold, pc):
-    """Parabolic interpolation between pitch candidates using pitch strength"""
-    p = np.full((pitch_strength.shape[1],), np.NaN)
-    s = np.full((pitch_strength.shape[1],), np.NaN)
-
-    for j in range(pitch_strength.shape[1]):
-        i = np.argmax(pitch_strength[:, j])
-        s[j] = pitch_strength[i, j]
-
-        if s[j] < strength_threshold:
-            continue
-
-        if i == 0:
-            p[j] = pc[0]
-        elif i == len(pc) - 1:
-            p[j] = pc[0]
-        else:
-            I = np.arange(i - 1, i + 2)
-            tc = 1 / pc[I]
-            ntc = np.dot((tc / tc[1] - 1), 2 * np.pi)
-            if np.any(np.isnan(pitch_strength[I, j])):
-                s[j] = np.nan
-                p[j] = np.nan
-            else:
-                c = np.polyfit(ntc, pitch_strength[I, j], 2)
-                ftc = 1 / 2 ** np.arange(np.log2(pc[I[0]]), np.log2(pc[I[2]]), 1 / 12 / 64)
-                nftc = np.dot((ftc / tc[1] - 1), 2 * np.pi)
-                poly = np.polyval(c, nftc)
-                k = np.argmax(poly)
-                s[j] = poly[k]
-                p[j] = 2 ** (np.log2(pc[I[0]]) + k / 12 / 64)
-    return p, s
-
-
-def parabolic_interpolation(pitch_strength, strength_threshold, pc):
-    """Parabolic interpolation between pitch candidates using pitch strength"""
-
-    i = np.argmax(pitch_strength)
-    strength = pitch_strength[i]
-
-    if strength < strength_threshold:
-        return np.nan, np.nan
-
-    if i == 0:
-        return pc[0], pitch_strength[0]
-    elif i == len(pc) - 1:
-        return pc[-1], pitch_strength[-1]
-    else:
-        I = np.arange(i - 1, i + 2)
-        tc = 1 / pc[I]
-        ntc = np.dot((tc / tc[1] - 1), 2 * np.pi)
-        if np.any(np.isnan(pitch_strength[I])):
-            s = np.nan
-            p = np.nan
-        else:
-            c = np.polyfit(ntc, pitch_strength[I], 2)
-            ftc = 1 / 2 ** np.arange(np.log2(pc[I[0]]), np.log2(pc[I[2]]), 1 / 12 / 64)
-            nftc = np.dot((ftc / tc[1] - 1), 2 * np.pi)
-            poly = np.polyval(c, nftc)
-            k = np.argmax(poly)
-            s = poly[k]
-            p = 2 ** (np.log2(pc[I[0]]) + k / 12 / 64)
-        return p, s
-
-
-def primes(n):
-    """Returns a set of n prime numbers"""
-    small_primes = np.array([2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89,
-                             97, 101, 103, 107, 109, 113, 127, 131, 137, 139, 149, 151, 157, 163, 167, 173, 179, 181,
-                             191, 193, 197, 199, 211, 223, 227, 229, 233, 239, 241, 251, 257, 263, 269, 271, 277, 281,
-                             283, 293, 307, 311, 313, 317, 331, 337, 347, 349, 353, 359, 367, 373, 379, 383, 389, 397,
-                             401, 409, 419, 421, 431, 433, 439, 443, 449, 457, 461, 463, 467, 479, 487, 491, 499, 503,
-                             509, 521, 523, 541, 547, 557, 563, 569, 571, 577, 587, 593, 599, 601, 607, 613, 617, 619,
-                             631, 641, 643, 647, 653, 659, 661, 673, 677, 683, 691, 701, 709, 719, 727, 733, 739, 743,
-                             751, 757, 761, 769, 773, 787, 797, 809, 811, 821, 823, 827, 829, 839, 853, 857, 859, 863,
-                             877, 881, 883, 887, 907, 911, 919, 929, 937, 941, 947, 953, 967, 971, 977, 983, 991, 997])
-
-    b = small_primes <= n
-    return small_primes[b]
+from scipy import interpolate
+import numpy as np
+# import librosa
+import scipy.signal
+from .spectra import Spectrum
+
+"""
+| Description: libf0 SWIPE implementation
+| Contributors: Sebastian Rosenzweig, Vojtěch Pešek, Simon Schwär, Meinard Müller
+| License: The MIT license, https://opensource.org/licenses/MIT
+| This file is part of libf0.
+"""
+"""
+This file was downloaded on 1 April 2023, from https://github.com/groupmm/libf0. This swipe.py file was integrated into
+the structure of the PyTimbre module to facilitate the calculation of the fundamental frequency. However, there are a
+number of dependencies that were not required by PyTimbre. 
+
+2023_04_01 - FSM - Function arguments were normalized to the standard Python rules.
+2023-04-06 - FSM - Updated the swipe function to use the SciPy.Signal.STFT function rather than librosa
+2023-04-06 - FSM - Removed all functions that rely on librosa
+"""
+
+
+def swipe_spectral_estimation(x: Spectrum, hop_size: float = 256, minimum_frequency: float = 10.0,
+                              maximum_frequency: float = 10000, pitch_resolution: float = 1 / 100,
+                              erb_resolution: float = 0.1,
+                              strength_threshold: float = 0):
+    if x.waveform is None:
+        raise ValueError("At this point, you must provide a Spectrum object that has been created from a waveform")
+    t = x.time
+
+    # Compute pitch candidates
+    pc = 2 ** np.arange(np.log2(minimum_frequency), np.log2(maximum_frequency), pitch_resolution)
+
+    # Pitch strength matrix
+    S = np.zeros((len(pc),))
+
+    # Determine P2-WSs [max, min]
+    log_ws = np.round(np.log2(np.divide(8 * x.waveform.sample_rate, [minimum_frequency, maximum_frequency])))
+
+    # P2-WSs - window sizes in samples
+    ws = len(x.frequencies)
+
+    # Determine window sizes used by each pitch candidate
+    log2pc = np.arange(np.log2(minimum_frequency), np.log2(maximum_frequency), pitch_resolution)
+    d = log2pc - np.log2(np.divide(8 * x.waveform.sample_rate, ws))
+
+    # Create ERBs spaced frequencies (in Hertz)
+    f_erbs = erbs2hz(np.arange(hz2erbs(pc[0] / 4), hz2erbs(x.waveform.sample_rate / 2), erb_resolution))
+
+    #   Resample the frequency spectrum to the ERB frequencies
+    loudness = interpolate.splev(f_erbs, interpolate.splrep(x.frequencies, x.pressures_pascals ** 2))
+    # loudness = np.sqrt(magnitude)
+
+    pc_to_compute = pc
+
+    # Normalize loudness
+    normalization_loudness = np.full_like(loudness, np.sqrt(np.sum(loudness * loudness, axis=0)))
+    with np.errstate(divide='ignore', invalid='ignore'):
+        loudness = loudness / normalization_loudness
+
+    # Create pitch salience matrix
+    S = np.zeros((len(pc_to_compute),))
+
+    for j in range(0, len(pc_to_compute)):
+        S[j] = pitch_strength_one(f_erbs, loudness, pc_to_compute[j])
+
+    # pitch_strength = pitch_strength_all_candidates(f_erbs, loudness, pc_to_compute)
+
+    pitches, strength = parabolic_interpolation(S, strength_threshold, pc)
+
+    if np.isnan(pitches):
+        pitches = 0  # avoid NaN output
+
+    return pitches, t, strength
+
+
+def swipe(samples, sample_rate: float = 22050, hop_size: float = 256, minimum_frequency: float = 55.0,
+          maximum_frequency: float = 1760.0, pitch_resolution: float = 1 / 96, erb_resolution: float = 0.1,
+          strength_threshold: float = 0):
+    """
+    Implementation of a sawtooth waveform inspired pitch estimator (SWIPE).
+    This version of the algorithm follows the original implementation, see `swipe_slim` for a more efficient
+    alternative.
+
+    .. [#] Arturo Camacho and John G. Harris,
+       "A sawtooth waveform inspired pitch estimator for speech and music."
+       The Journal of the Acoustical Society of America, vol. 124, no. 3, pp. 1638–1652, Sep. 2008
+
+    Parameters
+    ----------
+    samples : ndarray
+        Audio signal
+    sample_rate : int
+        Sampling rate
+    hop_size : int
+        Hop size
+    minimum_frequency : float or int
+        Minimal frequency
+    maximum_frequency : float or int
+        Maximal frequency
+    pitch_resolution : float
+        resolution of the pitch candidate bins in octaves (default value = 1/96 -> 96 bins per octave)
+    erb_resolution : float
+        resolution of the ERB bands (default value = 0.1)
+    strength_threshold : float
+        confidence threshold [0, 1] for the pitch detection (default value = 0)
+
+    Returns
+    -------
+    f0 : ndarray
+        Estimated F0-trajectory
+    t : ndarray
+        Time axis
+    strength : ndarray
+        Confidence/Pitch Strength
+
+    Remarks/Development
+    2023-04-01 - FSM - updated the argument names, and put the parameter helpers into the list
+    """
+
+    t = np.arange(0, len(samples), hop_size) / sample_rate  # Times
+
+    # Compute pitch candidates
+    pc = 2 ** np.arange(np.log2(minimum_frequency), np.log2(maximum_frequency), pitch_resolution)
+
+    # Pitch strength matrix
+    S = np.zeros((len(pc), len(t)))
+
+    # Determine P2-WSs [max, min]
+    log_ws = np.round(np.log2(np.divide(8 * sample_rate, [minimum_frequency, maximum_frequency])))
+
+    # P2-WSs - window sizes in samples
+    ws = 2 ** np.arange(log_ws[0], log_ws[1] - 1, -1, dtype=np.int32)
+
+    # Determine window sizes used by each pitch candidate
+    log2pc = np.arange(np.log2(minimum_frequency), np.log2(maximum_frequency), pitch_resolution)
+    d = log2pc - np.log2(np.divide(8 * sample_rate, ws[0]))
+
+    # Create ERBs spaced frequencies (in Hertz)
+    f_erbs = erbs2hz(np.arange(hz2erbs(pc[0] / 4), hz2erbs(sample_rate / 2), erb_resolution))
+
+    for i in range(0, len(ws)):
+        N = ws[i]
+        hop_size = int(N / 2)
+
+        x_zero_padded = np.concatenate([samples, np.zeros(N)])
+
+        f, ti, x = scipy.signal.stft(x_zero_padded,
+                                     fs=sample_rate,
+                                     nperseg=hop_size,
+                                     nfft=N,
+                                     scaling='psd',
+                                     boundary='zeros',
+                                     padded=True)
+
+        ti = np.insert(ti, 0, 0)
+        ti = np.delete(ti, -1)
+
+        spectrum = np.abs(x)
+        magnitude = resample_ferbs(spectrum, f, f_erbs)
+        loudness = np.sqrt(magnitude)
+
+        # Select candidates that use this window size
+        # First window
+        if i == 0:
+            j = np.argwhere(d < 1).flatten()
+            k = np.argwhere(d[j] > 0).flatten()
+        # Last Window
+        elif i == len(ws) - 1:
+            j = np.argwhere(d - i > -1).flatten()
+            k = np.argwhere(d[j] - i < 0).flatten()
+        else:
+            j = np.argwhere(np.abs(d - i) < 1).flatten()
+            k = np.arange(0, len(j))
+
+        pc_to_compute = pc[j]
+
+        pitch_strength = pitch_strength_all_candidates(f_erbs, loudness, pc_to_compute)
+
+        resampled_pitch_strength = resample_time(pitch_strength, t, ti)
+
+        lambda_ = d[j[k]] - i
+        mu = np.ones(len(j))
+        mu[k] = 1 - np.abs(lambda_)
+
+        S[j, :] = S[j, :] + np.multiply(
+            np.ones(resampled_pitch_strength.shape) * mu.reshape((mu.shape[0], 1)),
+            resampled_pitch_strength
+        )
+
+    # Fine-tune the pitch using parabolic interpolation
+    pitches, strength = parabolic_int(S, strength_threshold, pc)
+
+    pitches[np.where(np.isnan(pitches))] = 0  # avoid NaN output
+
+    return pitches, t, strength
+
+
+def nyquist(sample_rate):
+    """Nyquist Frequency"""
+    return sample_rate / 2
+
+
+def frequency_coefficients(k, fft_size, sample_rate):
+    """Physical frequency of STFT coefficients"""
+    return (k * sample_rate) / fft_size
+
+
+def time_values(m, hop_size, sample_rate):
+    """Physical time of STFT coefficients"""
+    return m * hop_size / sample_rate
+
+
+def hz2erbs(hz):
+    """Convert Hz to ERB scale"""
+    return 21.4 * np.log10(1 + hz / 229)
+
+
+def erbs2hz(erbs):
+    """Convert ERB to Hz"""
+    return (10 ** np.divide(erbs, 21.4) - 1) * 229
+
+
+def pitch_strength_all_candidates(ferbs, loudness, pitch_candidates):
+    """Compute pitch strength for all pitch candidates"""
+    # Normalize loudness
+    normalization_loudness = np.full_like(loudness, np.sqrt(np.sum(loudness * loudness, axis=0)))
+    with np.errstate(divide='ignore', invalid='ignore'):
+        loudness = loudness / normalization_loudness
+
+    # Create pitch salience matrix
+    S = np.zeros((len(pitch_candidates), loudness.shape[1]))
+
+    for j in range(0, len(pitch_candidates)):
+        S[j, :] = pitch_strength_one(ferbs, loudness, pitch_candidates[j])
+    return S
+
+
+def pitch_strength_one(erbs_frequencies, normalized_loudness, pitch_candidate):
+    """Compute pitch strength for one pitch candidate"""
+    number_of_harmonics = np.floor(erbs_frequencies[-1] / pitch_candidate - 0.75).astype(np.int32)
+    k = np.zeros(erbs_frequencies.shape)
+
+    # f_prime / f
+    q = erbs_frequencies / pitch_candidate
+
+    for i in np.concatenate(([1], primes(number_of_harmonics))):
+        a = np.abs(q - i)
+        p = a < 0.25
+        k[p] = np.cos(np.dot(2 * np.pi, q[p]))
+        v = np.logical_and(0.25 < a, a < 0.75)
+        k[v] = k[v] + np.cos(np.dot(2 * np.pi, q[v])) / 2
+
+    # Apply envelope
+    k = np.multiply(k, np.sqrt(1.0 / erbs_frequencies))
+
+    # K+-normalize kernel
+    k = k / np.linalg.norm(k[k > 0])
+
+    # Compute pitch strength
+    S = np.dot(k, normalized_loudness)
+    return S
+
+
+def resample_ferbs(spectrum, f, ferbs):
+    """Resample to ERB scale"""
+
+    magnitude = np.zeros((len(ferbs), spectrum.shape[1]))
+
+    for t in range(spectrum.shape[1]):
+        spl = interpolate.splrep(f, spectrum[:, t])
+        interpolate.splev(ferbs, spl)
+
+        magnitude[:, t] = interpolate.splev(ferbs, spl)
+
+    return np.maximum(magnitude, 0)
+
+
+def resample_time(pitch_strength, resampled_time, ti):
+    """Resample time axis"""
+    if pitch_strength.shape[1] > 0:
+        pitch_strength = interpolate_one_candidate(pitch_strength, ti, resampled_time)
+    else:
+        pitch_strength = np.kron(np.ones((len(pitch_strength), len(resampled_time))), np.NaN)
+    return pitch_strength
+
+
+def interpolate_one_candidate(pitch_strength, ti, resampled_time):
+    """Interpolate time axis"""
+    pitch_strength_interpolated = np.zeros((pitch_strength.shape[0], len(resampled_time)))
+
+    for s in range(pitch_strength.shape[0]):
+        t_i = interpolate.interp1d(ti, pitch_strength[s, :], 'linear', bounds_error=True)
+        pitch_strength_interpolated[s, :] = t_i(resampled_time)
+
+    return pitch_strength_interpolated
+
+
+def parabolic_int(pitch_strength, strength_threshold, pc):
+    """Parabolic interpolation between pitch candidates using pitch strength"""
+    p = np.full((pitch_strength.shape[1],), np.NaN)
+    s = np.full((pitch_strength.shape[1],), np.NaN)
+
+    for j in range(pitch_strength.shape[1]):
+        i = np.argmax(pitch_strength[:, j])
+        s[j] = pitch_strength[i, j]
+
+        if s[j] < strength_threshold:
+            continue
+
+        if i == 0:
+            p[j] = pc[0]
+        elif i == len(pc) - 1:
+            p[j] = pc[0]
+        else:
+            I = np.arange(i - 1, i + 2)
+            tc = 1 / pc[I]
+            ntc = np.dot((tc / tc[1] - 1), 2 * np.pi)
+            if np.any(np.isnan(pitch_strength[I, j])):
+                s[j] = np.nan
+                p[j] = np.nan
+            else:
+                c = np.polyfit(ntc, pitch_strength[I, j], 2)
+                ftc = 1 / 2 ** np.arange(np.log2(pc[I[0]]), np.log2(pc[I[2]]), 1 / 12 / 64)
+                nftc = np.dot((ftc / tc[1] - 1), 2 * np.pi)
+                poly = np.polyval(c, nftc)
+                k = np.argmax(poly)
+                s[j] = poly[k]
+                p[j] = 2 ** (np.log2(pc[I[0]]) + k / 12 / 64)
+    return p, s
+
+
+def parabolic_interpolation(pitch_strength, strength_threshold, pc):
+    """Parabolic interpolation between pitch candidates using pitch strength"""
+
+    i = np.argmax(pitch_strength)
+    strength = pitch_strength[i]
+
+    if strength < strength_threshold:
+        return np.nan, np.nan
+
+    if i == 0:
+        return pc[0], pitch_strength[0]
+    elif i == len(pc) - 1:
+        return pc[-1], pitch_strength[-1]
+    else:
+        I = np.arange(i - 1, i + 2)
+        tc = 1 / pc[I]
+        ntc = np.dot((tc / tc[1] - 1), 2 * np.pi)
+        if np.any(np.isnan(pitch_strength[I])):
+            s = np.nan
+            p = np.nan
+        else:
+            c = np.polyfit(ntc, pitch_strength[I], 2)
+            ftc = 1 / 2 ** np.arange(np.log2(pc[I[0]]), np.log2(pc[I[2]]), 1 / 12 / 64)
+            nftc = np.dot((ftc / tc[1] - 1), 2 * np.pi)
+            poly = np.polyval(c, nftc)
+            k = np.argmax(poly)
+            s = poly[k]
+            p = 2 ** (np.log2(pc[I[0]]) + k / 12 / 64)
+        return p, s
+
+
+def primes(n):
+    """Returns a set of n prime numbers"""
+    small_primes = np.array([2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89,
+                             97, 101, 103, 107, 109, 113, 127, 131, 137, 139, 149, 151, 157, 163, 167, 173, 179, 181,
+                             191, 193, 197, 199, 211, 223, 227, 229, 233, 239, 241, 251, 257, 263, 269, 271, 277, 281,
+                             283, 293, 307, 311, 313, 317, 331, 337, 347, 349, 353, 359, 367, 373, 379, 383, 389, 397,
+                             401, 409, 419, 421, 431, 433, 439, 443, 449, 457, 461, 463, 467, 479, 487, 491, 499, 503,
+                             509, 521, 523, 541, 547, 557, 563, 569, 571, 577, 587, 593, 599, 601, 607, 613, 617, 619,
+                             631, 641, 643, 647, 653, 659, 661, 673, 677, 683, 691, 701, 709, 719, 727, 733, 739, 743,
+                             751, 757, 761, 769, 773, 787, 797, 809, 811, 821, 823, 827, 829, 839, 853, 857, 859, 863,
+                             877, 881, 883, 887, 907, 911, 919, 929, 937, 941, 947, 953, 967, 971, 977, 983, 991, 997])
+
+    b = small_primes <= n
+    return small_primes[b]
```

### Comparing `PyTimbre-0.7.2/src/pytimbre/spectral/time_histories.py` & `PyTimbre-0.7.3/src/pytimbre/spectral/time_histories.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.7.2/src/pytimbre/waveform.py` & `PyTimbre-0.7.3/src/pytimbre/waveform.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import statsmodels.api as sm
 import colorednoise as cn
 import warnings
 from typing import Dict, Tuple
 import numpy.typing as npt
 from .yin import yin
 import warnings
+from python_speech_features import mfcc, ssc, fbank, logfbank
 
 
 class WindowingMethods(Enum):
     """
     The available windowing methods for the waveform
     """
 
@@ -367,15 +368,14 @@
         return self._temporal_threshold_finding
 
     @temporal_threshold_finding.setter
     def temporal_threshold_finding(self,value):
         self._temporal_threshold_finding = value
 
 
-
     @property
     def attack(self):
         if self._addresses is None:
             self._calculate_signal_envelope()
             self._log_attack, self._increase, self._decrease, self._addresses = self.calculate_log_attack()
 
         return self._addresses[0]
@@ -1983,15 +1983,15 @@
             freq = np.mean(frequencies)
 
             calibration = (abs(freq - 1000) < 0.1 * 1000) or \
                           (abs(freq - 250) < 0.1 * 250)
 
         return calibration, freq
 
-    def get_features(self, include_sq_metrics: bool = True):
+    def get_features(self, include_sq_metrics: bool = True, include_speech_features: bool = True):
         """
         This function calculates the various features within the global time analysis and stores the results in the
         class object.  At the end, a dictionary of the values is available and returned to the calling function.
 
         Returns
         -------
         features : dict()
@@ -2013,14 +2013,26 @@
                         'auto-correlation': self.auto_correlation,
                         'zero crossing rate': self.zero_crossing_rate}
 
             if include_sq_metrics:
                 features['loudness'] = self.loudness
                 features['roughness'] = self.roughness
                 features['sharpness'] = self.sharpness
+
+            if include_speech_features:
+                from python_speech_features import mfcc, fbank, ssc, logfbank
+
+                vect = np.mean(mfcc(self.samples, self.sample_rate), axis=0)
+                for index in range(len(vect)):
+                    features['mfcc_{:02.0f}'.format(index)] = vect[index]
+
+                vect = np.mean(ssc(self.samples, self.sample_rate), axis=0)
+                for index in range(len(vect)):
+                    features['ssc_{:02.0f}'.format(index)] = vect[index]
+
         elif self.is_impulsive:
             features = {'a-duration': self.a_duration,
                         'equivalent level (T)': self.leqT,
                         'equivalent level a-weighted (T)': self.liaeqT,
                         'equivalent level a-weighted (8 hr)': self.liaeq8hr,
                         'equivalent level a-weighted (100ms)': self.liaeq100ms,
                         'peak level (dB)': self.peak_level,
```

### Comparing `PyTimbre-0.7.2/src/pytimbre/yin.py` & `PyTimbre-0.7.3/src/pytimbre/yin.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,236 +1,236 @@
-"""
-| Description: libf0 YIN implementation
-| Contributors: Sebastian Rosenzweig, Simon Schwär, Edgar Suárez, Meinard Müller
-| License: The MIT license, https://opensource.org/licenses/MIT
-| This file is part of libf0.
-"""
-import numpy as np
-
-
-def yin(x, Fs=22050, N=2048, H=256, F_min=55.0, F_max=1760.0, threshold=0.15, verbose=False):
-    """
-    Implementation of the YIN algorithm.
-
-    .. [#] Alain De Cheveigné and Hideki Kawahara.
-        "YIN, a fundamental frequency estimator for speech and music."
-        The Journal of the Acoustical Society of America 111.4 (2002): 1917-1930.
-
-    Parameters
-    ----------
-    x : ndarray [shape=(L, )], real - valued
-        Audio signal
-    Fs : int
-        Sampling frequency
-    N : int
-        Window size
-    H : int
-        Hop size
-    F_min : float
-        Minimal frequency
-    F_max : float
-        Maximal frequency
-    threshold : float
-        Threshold for cumulative mean normalized difference function
-    verbose : bool
-        Switch to activate/deactivate status bar
-
-    Returns
-    -------
-    f0 : ndarray
-        Estimated F0-trajectory
-    t : ndarray
-        Time axis
-    ap: ndarray
-        Aperiodicity (indicator for voicing: the lower, the more reliable the estimate)
-    """
-
-    if F_min > F_max:
-        raise ValueError("F_min must be smaller than F_max!")
-
-    if F_min < Fs/N:        
-        raise ValueError(f"The condition (F_min >= Fs/N) was not met. With Fs = {Fs}, N = {N} and F_min = {F_min} you have "
-                 f"the following options: \n1) Set F_min >= {np.ceil(Fs/N)} Hz. \n2) Set N >= {np.ceil(Fs/F_min).astype(int)}. \n3) Set Fs <= {np.floor(F_min * N)} Hz.")
-
-    x_pad = np.concatenate((np.zeros(N//2), x, np.zeros(N//2)))  # Add zeros for centered estimates
-    M = int(np.floor((len(x_pad) - N) / H)) + 1  # Compute number of estimates that will be generated
-    f0 = np.zeros(M)  # Estimated fundamental frequencies (0 for unspecified frames)
-    t = np.arange(M)*H/Fs  # Time axis
-    ap = np.zeros(M)  # Aperiodicity
-
-    lag_min = max(int(np.ceil(Fs / F_max)), 1)  # lag of maximal frequency in samples
-    lag_max = int(np.ceil(Fs / F_min))  # lag of minimal frequency in samples
-
-    for m in range(M):
-        if verbose:
-            print(f"YIN Progress: {np.ceil(100*m/M).astype(int)}%", end='\r')
-        # Take a frame from input signal
-        frame = x_pad[m*H:m*H + N]
-
-        # Cumulative Mean Normalized Difference Function
-        cmndf = cumulative_mean_normalized_difference_function(frame, lag_max)
-
-        # Absolute Thresholding
-        lag_est = absolute_thresholding(cmndf, threshold, lag_min, lag_max, parabolic_interp=True)
-
-        # Refine estimate by constraining search to vicinity of best local estimate (default: +/- 25 cents)
-        tol_cents = 25
-        lag_min_local = int(np.round(Fs / ((Fs / lag_est) * 2 ** (tol_cents/1200))))
-        if lag_min_local < lag_min:
-            lag_min_local = lag_min
-        lag_max_local = int(np.round(Fs / ((Fs / lag_est) * 2 ** (-tol_cents/1200))))
-        if lag_max_local > lag_max:
-            lag_max_local = lag_max
-        lag_new = absolute_thresholding(cmndf, threshold=np.inf, lag_min=lag_min_local, lag_max=lag_max_local,
-                                        parabolic_interp=True)
-
-        # Compute Fundamental Frequency Estimate
-        f0[m] = Fs / lag_new
-
-        # Compute Aperiodicity
-        ap[m] = aperiodicity(frame, lag_new)
-
-    return f0, t, ap
-
-
-def cumulative_mean_normalized_difference_function(frame, lag_max):
-    """
-    Computes Cumulative Mean Normalized Difference Function (CMNDF).
-
-    Parameters
-    ----------
-    frame : ndarray
-        Audio frame
-    lag_max : int
-        Maximum expected lag in the CMNDF
-
-    Returns
-    -------
-    cmndf : ndarray
-        Cumulative Mean Normalized Difference Function
-    """
-
-    cmndf = np.zeros(lag_max+1)  # Initialize CMNDF
-    cmndf[0] = 1
-    diff_mean = 0
-
-    for tau in range(1, lag_max+1):
-        # Difference function
-        diff = np.sum((frame[0:-tau] - frame[0 + tau:]) ** 2)
-        # Iterative mean of the difference function
-        diff_mean = diff_mean*(tau-1)/tau + diff/tau
-
-        cmndf[tau] = diff / (diff_mean + np.finfo(np.float64).eps)
-
-    return cmndf
-
-
-def absolute_thresholding(cmndf, threshold, lag_min, lag_max, parabolic_interp=True):
-    """
-    Absolute thresholding:
-    Set an absolute threshold and choose the smallest value of tau that gives a minimum of d' deeper than that
-    threshold. If none is found, the global minimum is chosen instead.
-
-    Parameters
-    ----------
-    cmndf : ndarray
-        Cumulative Mean Normalized Difference Function
-    threshold : float
-        Threshold
-    lag_min : float
-        Minimal lag
-    lag_max : float
-        Maximal lag
-    parabolic_interp : bool
-        Switch to activate/deactivate parabolic interpolation
-
-    Returns
-    -------
-
-    """
-
-    # take shortcut if search range only allows for one possible lag
-    if lag_min == lag_max:
-        return lag_min
-
-    # find local minima below absolute threshold in interval [lag_min:lag_max]
-    local_min_idxs = (np.argwhere((cmndf[1:-1] < cmndf[0:-2]) & (cmndf[1:-1] < cmndf[2:]))).flatten() + 1
-    below_thr_idxs = np.argwhere(cmndf[lag_min:lag_max] < threshold).flatten() + lag_min
-    # numba compatible intersection of indices sets
-    min_idxs = np.unique(np.array([i for i in local_min_idxs for j in below_thr_idxs if i == j]))
-
-    # if no local minima below threshold are found, return global minimum
-    if not min_idxs.size:
-        return np.argmin(cmndf[lag_min:lag_max]) + lag_min
-
-    # find first local minimum
-    lag = np.min(min_idxs)  # choose first local minimum
-
-    # Optional: Parabolic Interpolation of local minima
-    if parabolic_interp:
-        lag_corr, cmndf[lag] = parabolic_interpolation(cmndf[lag-1], cmndf[lag], cmndf[lag+1])
-        lag += lag_corr
-
-    return lag
-
-
-def parabolic_interpolation(y1, y2, y3):
-    """
-    Parabolic interpolation of an extremal value given three samples with equal spacing on the x-axis.
-    The middle value y2 is assumed to be the extremal sample of the three.
-
-    Parameters
-    ----------
-    y1: f(x1)
-    y2: f(x2)
-    y3: f(x3)
-
-    Returns
-    -------
-    x_interp: Interpolated x-value (relative to x3-x2)
-    y_interp: Interpolated y-value, f(x_interp)
-    """
-
-    a = np.finfo(np.float64).eps + (y1 + y3 - 2 * y2) / 2
-    b = (y3 - y1) / 2
-    x_interp = -b / (2 * a)
-    y_interp = y2 - (b ** 2) / (4 * a)
-
-    return x_interp, y_interp
-
-
-def aperiodicity(frame, lag_est):
-    """
-    Compute aperiodicity of given frame (serves as indicator for reliability or voicing detection).
-
-    Parameters
-    ----------
-    frame : ndarray
-        Frame
-    lag_est : float
-        Estimated lag
-
-    Returns
-    -------
-    ap: float
-        Aperiodicity (the lower, the more reliable the estimate)
-    """
-
-    lag_int = int(np.floor(lag_est))  # uncorrected period estimate
-    frac = lag_est - lag_int  # residual
-
-    # Pad frame to insure constant size
-    frame_pad = np.concatenate((frame, np.flip(frame)))  # mirror padding
-
-    # Shift frame by estimated period
-    if frac == 0:
-        frame_shift = frame_pad[lag_int:lag_int+len(frame)]
-    else:
-        # linear interpolation between adjacent shifts
-        frame_shift = (1 - frac) * frame_pad[lag_int:lag_int+len(frame)] + \
-                      frac * frame_pad[lag_int+1:lag_int+1+len(frame)]
-
-    pwr = (np.mean(frame ** 2) + np.mean(frame_shift ** 2)) / 2  # average power over fixed and shifted frame
-    res = np.mean((frame - frame_shift) ** 2) / 2  # residual power
-    ap = res / (pwr + np.finfo(np.float64).eps)
-
-    return ap
+"""
+| Description: libf0 YIN implementation
+| Contributors: Sebastian Rosenzweig, Simon Schwär, Edgar Suárez, Meinard Müller
+| License: The MIT license, https://opensource.org/licenses/MIT
+| This file is part of libf0.
+"""
+import numpy as np
+
+
+def yin(x, Fs=22050, N=2048, H=256, F_min=55.0, F_max=1760.0, threshold=0.15, verbose=False):
+    """
+    Implementation of the YIN algorithm.
+
+    .. [#] Alain De Cheveigné and Hideki Kawahara.
+        "YIN, a fundamental frequency estimator for speech and music."
+        The Journal of the Acoustical Society of America 111.4 (2002): 1917-1930.
+
+    Parameters
+    ----------
+    x : ndarray [shape=(L, )], real - valued
+        Audio signal
+    Fs : int
+        Sampling frequency
+    N : int
+        Window size
+    H : int
+        Hop size
+    F_min : float
+        Minimal frequency
+    F_max : float
+        Maximal frequency
+    threshold : float
+        Threshold for cumulative mean normalized difference function
+    verbose : bool
+        Switch to activate/deactivate status bar
+
+    Returns
+    -------
+    f0 : ndarray
+        Estimated F0-trajectory
+    t : ndarray
+        Time axis
+    ap: ndarray
+        Aperiodicity (indicator for voicing: the lower, the more reliable the estimate)
+    """
+
+    if F_min > F_max:
+        raise ValueError("F_min must be smaller than F_max!")
+
+    if F_min < Fs/N:        
+        raise ValueError(f"The condition (F_min >= Fs/N) was not met. With Fs = {Fs}, N = {N} and F_min = {F_min} you have "
+                 f"the following options: \n1) Set F_min >= {np.ceil(Fs/N)} Hz. \n2) Set N >= {np.ceil(Fs/F_min).astype(int)}. \n3) Set Fs <= {np.floor(F_min * N)} Hz.")
+
+    x_pad = np.concatenate((np.zeros(N//2), x, np.zeros(N//2)))  # Add zeros for centered estimates
+    M = int(np.floor((len(x_pad) - N) / H)) + 1  # Compute number of estimates that will be generated
+    f0 = np.zeros(M)  # Estimated fundamental frequencies (0 for unspecified frames)
+    t = np.arange(M)*H/Fs  # Time axis
+    ap = np.zeros(M)  # Aperiodicity
+
+    lag_min = max(int(np.ceil(Fs / F_max)), 1)  # lag of maximal frequency in samples
+    lag_max = int(np.ceil(Fs / F_min))  # lag of minimal frequency in samples
+
+    for m in range(M):
+        if verbose:
+            print(f"YIN Progress: {np.ceil(100*m/M).astype(int)}%", end='\r')
+        # Take a frame from input signal
+        frame = x_pad[m*H:m*H + N]
+
+        # Cumulative Mean Normalized Difference Function
+        cmndf = cumulative_mean_normalized_difference_function(frame, lag_max)
+
+        # Absolute Thresholding
+        lag_est = absolute_thresholding(cmndf, threshold, lag_min, lag_max, parabolic_interp=True)
+
+        # Refine estimate by constraining search to vicinity of best local estimate (default: +/- 25 cents)
+        tol_cents = 25
+        lag_min_local = int(np.round(Fs / ((Fs / lag_est) * 2 ** (tol_cents/1200))))
+        if lag_min_local < lag_min:
+            lag_min_local = lag_min
+        lag_max_local = int(np.round(Fs / ((Fs / lag_est) * 2 ** (-tol_cents/1200))))
+        if lag_max_local > lag_max:
+            lag_max_local = lag_max
+        lag_new = absolute_thresholding(cmndf, threshold=np.inf, lag_min=lag_min_local, lag_max=lag_max_local,
+                                        parabolic_interp=True)
+
+        # Compute Fundamental Frequency Estimate
+        f0[m] = Fs / lag_new
+
+        # Compute Aperiodicity
+        ap[m] = aperiodicity(frame, lag_new)
+
+    return f0, t, ap
+
+
+def cumulative_mean_normalized_difference_function(frame, lag_max):
+    """
+    Computes Cumulative Mean Normalized Difference Function (CMNDF).
+
+    Parameters
+    ----------
+    frame : ndarray
+        Audio frame
+    lag_max : int
+        Maximum expected lag in the CMNDF
+
+    Returns
+    -------
+    cmndf : ndarray
+        Cumulative Mean Normalized Difference Function
+    """
+
+    cmndf = np.zeros(lag_max+1)  # Initialize CMNDF
+    cmndf[0] = 1
+    diff_mean = 0
+
+    for tau in range(1, lag_max+1):
+        # Difference function
+        diff = np.sum((frame[0:-tau] - frame[0 + tau:]) ** 2)
+        # Iterative mean of the difference function
+        diff_mean = diff_mean*(tau-1)/tau + diff/tau
+
+        cmndf[tau] = diff / (diff_mean + np.finfo(np.float64).eps)
+
+    return cmndf
+
+
+def absolute_thresholding(cmndf, threshold, lag_min, lag_max, parabolic_interp=True):
+    """
+    Absolute thresholding:
+    Set an absolute threshold and choose the smallest value of tau that gives a minimum of d' deeper than that
+    threshold. If none is found, the global minimum is chosen instead.
+
+    Parameters
+    ----------
+    cmndf : ndarray
+        Cumulative Mean Normalized Difference Function
+    threshold : float
+        Threshold
+    lag_min : float
+        Minimal lag
+    lag_max : float
+        Maximal lag
+    parabolic_interp : bool
+        Switch to activate/deactivate parabolic interpolation
+
+    Returns
+    -------
+
+    """
+
+    # take shortcut if search range only allows for one possible lag
+    if lag_min == lag_max:
+        return lag_min
+
+    # find local minima below absolute threshold in interval [lag_min:lag_max]
+    local_min_idxs = (np.argwhere((cmndf[1:-1] < cmndf[0:-2]) & (cmndf[1:-1] < cmndf[2:]))).flatten() + 1
+    below_thr_idxs = np.argwhere(cmndf[lag_min:lag_max] < threshold).flatten() + lag_min
+    # numba compatible intersection of indices sets
+    min_idxs = np.unique(np.array([i for i in local_min_idxs for j in below_thr_idxs if i == j]))
+
+    # if no local minima below threshold are found, return global minimum
+    if not min_idxs.size:
+        return np.argmin(cmndf[lag_min:lag_max]) + lag_min
+
+    # find first local minimum
+    lag = np.min(min_idxs)  # choose first local minimum
+
+    # Optional: Parabolic Interpolation of local minima
+    if parabolic_interp:
+        lag_corr, cmndf[lag] = parabolic_interpolation(cmndf[lag-1], cmndf[lag], cmndf[lag+1])
+        lag += lag_corr
+
+    return lag
+
+
+def parabolic_interpolation(y1, y2, y3):
+    """
+    Parabolic interpolation of an extremal value given three samples with equal spacing on the x-axis.
+    The middle value y2 is assumed to be the extremal sample of the three.
+
+    Parameters
+    ----------
+    y1: f(x1)
+    y2: f(x2)
+    y3: f(x3)
+
+    Returns
+    -------
+    x_interp: Interpolated x-value (relative to x3-x2)
+    y_interp: Interpolated y-value, f(x_interp)
+    """
+
+    a = np.finfo(np.float64).eps + (y1 + y3 - 2 * y2) / 2
+    b = (y3 - y1) / 2
+    x_interp = -b / (2 * a)
+    y_interp = y2 - (b ** 2) / (4 * a)
+
+    return x_interp, y_interp
+
+
+def aperiodicity(frame, lag_est):
+    """
+    Compute aperiodicity of given frame (serves as indicator for reliability or voicing detection).
+
+    Parameters
+    ----------
+    frame : ndarray
+        Frame
+    lag_est : float
+        Estimated lag
+
+    Returns
+    -------
+    ap: float
+        Aperiodicity (the lower, the more reliable the estimate)
+    """
+
+    lag_int = int(np.floor(lag_est))  # uncorrected period estimate
+    frac = lag_est - lag_int  # residual
+
+    # Pad frame to insure constant size
+    frame_pad = np.concatenate((frame, np.flip(frame)))  # mirror padding
+
+    # Shift frame by estimated period
+    if frac == 0:
+        frame_shift = frame_pad[lag_int:lag_int+len(frame)]
+    else:
+        # linear interpolation between adjacent shifts
+        frame_shift = (1 - frac) * frame_pad[lag_int:lag_int+len(frame)] + \
+                      frac * frame_pad[lag_int+1:lag_int+1+len(frame)]
+
+    pwr = (np.mean(frame ** 2) + np.mean(frame_shift ** 2)) / 2  # average power over fixed and shifted frame
+    res = np.mean((frame - frame_shift) ** 2) / 2  # residual power
+    ap = res / (pwr + np.finfo(np.float64).eps)
+
+    return ap
```

