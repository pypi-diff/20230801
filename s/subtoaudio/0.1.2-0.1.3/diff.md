# Comparing `tmp/subtoaudio-0.1.2.tar.gz` & `tmp/subtoaudio-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subtoaudio-0.1.2.tar", last modified: Fri Jul 21 20:39:26 2023, max compression
+gzip compressed data, was "subtoaudio-0.1.3.tar", last modified: Tue Aug  1 03:58:10 2023, max compression
```

## Comparing `subtoaudio-0.1.2.tar` & `subtoaudio-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 20:39:26.888094 subtoaudio-0.1.2/
--rw-rw-rw-   0        0        0    16725 2023-07-21 03:01:38.000000 subtoaudio-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2821 2023-07-21 20:39:26.883094 subtoaudio-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2163 2023-07-21 20:34:28.000000 subtoaudio-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 20:39:26.923094 subtoaudio-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      963 2023-07-21 20:35:59.000000 subtoaudio-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:39:26.823094 subtoaudio-0.1.2/subtoaudio/
--rw-rw-rw-   0        0        0       34 2023-07-21 03:01:38.000000 subtoaudio-0.1.2/subtoaudio/__init__.py
--rw-rw-rw-   0        0        0     5131 2023-07-21 03:01:38.000000 subtoaudio-0.1.2/subtoaudio/subtoaudio.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:39:26.878094 subtoaudio-0.1.2/subtoaudio.egg-info/
--rw-rw-rw-   0        0        0     2821 2023-07-21 20:39:25.000000 subtoaudio-0.1.2/subtoaudio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-21 20:39:25.000000 subtoaudio-0.1.2/subtoaudio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 20:39:25.000000 subtoaudio-0.1.2/subtoaudio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-21 20:39:25.000000 subtoaudio-0.1.2/subtoaudio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-21 20:39:25.000000 subtoaudio-0.1.2/subtoaudio.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 03:58:10.515459 subtoaudio-0.1.3/
+-rw-rw-rw-   0        0        0    16725 2023-07-31 11:18:40.000000 subtoaudio-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3698 2023-08-01 03:58:10.515459 subtoaudio-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3013 2023-07-31 11:18:40.000000 subtoaudio-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 03:58:10.530459 subtoaudio-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-07-31 11:18:40.000000 subtoaudio-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:58:10.465459 subtoaudio-0.1.3/subtoaudio/
+-rw-rw-rw-   0        0        0       34 2023-07-31 11:18:40.000000 subtoaudio-0.1.3/subtoaudio/__init__.py
+-rw-rw-rw-   0        0        0     8247 2023-07-31 11:18:40.000000 subtoaudio-0.1.3/subtoaudio/subtoaudio.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:58:10.505459 subtoaudio-0.1.3/subtoaudio.egg-info/
+-rw-rw-rw-   0        0        0     3698 2023-08-01 03:58:08.000000 subtoaudio-0.1.3/subtoaudio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-08-01 03:58:08.000000 subtoaudio-0.1.3/subtoaudio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 03:58:08.000000 subtoaudio-0.1.3/subtoaudio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-08-01 03:58:08.000000 subtoaudio-0.1.3/subtoaudio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-01 03:58:08.000000 subtoaudio-0.1.3/subtoaudio.egg-info/top_level.txt
```

### Comparing `subtoaudio-0.1.2/LICENSE` & `subtoaudio-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `subtoaudio-0.1.2/PKG-INFO` & `subtoaudio-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: subtoaudio
-Version: 0.1.2
-Summary: Subtitle to audio, generate speech from any subtitle file
+Version: 0.1.3
+Summary: Subtitle to Audio, generate audio or speech from any subtitle file
 Home-page: https://github.com/bnsantoso/
 Author: Bagas NS
 Author-email: bagassantoso71@gmail.com
 License: MPL 2.0
 Keywords: subtitle,tts,text to audio,subtitle to audio,subtitle to speech
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/bnsantoso)
 
 # Subtitle to Audio
 Subtitle to audio, generate audio from any subtitle file using Coqui-ai TTS and synchronize the audio timing according to subtitle time.
 
 ## Dependencies
-[ffmpeg](https://ffmpeg.org/), [pydub](https://github.com/jiaaro/pydub), [librosa](https://github.com/librosa/librosa), [coqui-ai TTS](https://github.com/coqui-ai/TTS/)
+[ffmpeg](https://ffmpeg.org/), [pydub](https://github.com/jiaaro/pydub), [librosa](https://github.com/librosa/librosa), [coqui-ai TTS](https://github.com/coqui-ai/TTS/), [ffmpeg-python](https://github.com/kkroening/ffmpeg-python)
 
 ## Installation
 
 ```bash
 pip install git+https://github.com/bnsantoso/sub-to-audio
 ```
 ```bash
@@ -37,15 +37,15 @@
 ## Example usage
 
 Basic use is very similiar to [Coqui-ai TTS](https://github.com/coqui-ai/TTS/), you can check their [documentation](https://tts.readthedocs.io/en/latest/inference.html).
 
 ```python
 from subtoaudio import SubToAudio
 
-#Using the Fairseq English speaker model as the default, the code will output 'output.wav' in the current directory.
+#Using the Fairseq English speaker model as the default, the code will output 'yoursubtitle.wav' in the current directory.
 sub = SubToAudio(gpu=True)
 subtitle = sub.subtitle("yoursubtitle.srt")
 sub.convert_to_audio(data=subtitle)
 
 #you can choose 1100 different language using fairseq model
 sub = SubToAudio(language='<lang-iso_code>')
 subtitle = sub.subtitle("yoursubtitle.ass")
@@ -62,12 +62,30 @@
 sub.convert_to_audio(data=subtitle)
 
 #By default, it is using "speaker=tts.speakers[0]/None, language=tts.languages[0]/None, speaker_wav=None"
 sub = SubToAudio(model_name="tts_models/multilingual/multi-dataset/your_tts")
 subtitle = sub.subtitle("yoursubtitle.srt")
 sub.convert_to_audio(data=subtitle, language="en", speaker="speakername", speaker_wav="your/path/speaker.wav", output_path="subtitle.wav")
 
+#Change the tempo or speech rate of all audio files , default is 1.2
+sub = SubToAudio(gpu=True)
+subtitle = sub.subtitle("yoursubtitle.srt")
+sub.convert_to_audio(data=subtitle, tempo_mode="all", tempo_speed=1.3)
+
+#Change tempo or speech rate to audio that doesn't match the subtitle duration
+sub = SubToAudio(gpu=True)
+subtitle = sub.subtitle("yoursubtitle.srt")
+sub.convert_to_audio(data=subtitle, tempo_mode="overflow")
+
+#Limit tempo speed on the overflow mode 
+sub.convert_to_audio(data=subtitle, tempo_mode="overflow", tempo_limit=1.2)
+
+#Save temporary audio to current folder
+sub = SubToAudio(model_name="tts_models/multilingual/multi-dataset/your_tts")
+subtitle = sub.subtitle("yoursubtitle.srt")
+sub.convert_to_audio(data=subtitle, output_path="subtitle.wav", save_temp=True)
+
 ```
 
 ### Citation 
 Eren, G., & The Coqui TTS Team. (2021). Coqui TTS (Version 1.4) [Computer software]. https://doi.org/10.5281/zenodo.6334862
```

### Comparing `subtoaudio-0.1.2/README.md` & `subtoaudio-0.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/bnsantoso)
 
 # Subtitle to Audio
 Subtitle to audio, generate audio from any subtitle file using Coqui-ai TTS and synchronize the audio timing according to subtitle time.
 
 ## Dependencies
-[ffmpeg](https://ffmpeg.org/), [pydub](https://github.com/jiaaro/pydub), [librosa](https://github.com/librosa/librosa), [coqui-ai TTS](https://github.com/coqui-ai/TTS/)
+[ffmpeg](https://ffmpeg.org/), [pydub](https://github.com/jiaaro/pydub), [librosa](https://github.com/librosa/librosa), [coqui-ai TTS](https://github.com/coqui-ai/TTS/), [ffmpeg-python](https://github.com/kkroening/ffmpeg-python)
 
 ## Installation
 
 ```bash
 pip install git+https://github.com/bnsantoso/sub-to-audio
 ```
 ```bash
@@ -21,15 +21,15 @@
 ## Example usage
 
 Basic use is very similiar to [Coqui-ai TTS](https://github.com/coqui-ai/TTS/), you can check their [documentation](https://tts.readthedocs.io/en/latest/inference.html).
 
 ```python
 from subtoaudio import SubToAudio
 
-#Using the Fairseq English speaker model as the default, the code will output 'output.wav' in the current directory.
+#Using the Fairseq English speaker model as the default, the code will output 'yoursubtitle.wav' in the current directory.
 sub = SubToAudio(gpu=True)
 subtitle = sub.subtitle("yoursubtitle.srt")
 sub.convert_to_audio(data=subtitle)
 
 #you can choose 1100 different language using fairseq model
 sub = SubToAudio(language='<lang-iso_code>')
 subtitle = sub.subtitle("yoursubtitle.ass")
@@ -46,12 +46,30 @@
 sub.convert_to_audio(data=subtitle)
 
 #By default, it is using "speaker=tts.speakers[0]/None, language=tts.languages[0]/None, speaker_wav=None"
 sub = SubToAudio(model_name="tts_models/multilingual/multi-dataset/your_tts")
 subtitle = sub.subtitle("yoursubtitle.srt")
 sub.convert_to_audio(data=subtitle, language="en", speaker="speakername", speaker_wav="your/path/speaker.wav", output_path="subtitle.wav")
 
+#Change the tempo or speech rate of all audio files , default is 1.2
+sub = SubToAudio(gpu=True)
+subtitle = sub.subtitle("yoursubtitle.srt")
+sub.convert_to_audio(data=subtitle, tempo_mode="all", tempo_speed=1.3)
+
+#Change tempo or speech rate to audio that doesn't match the subtitle duration
+sub = SubToAudio(gpu=True)
+subtitle = sub.subtitle("yoursubtitle.srt")
+sub.convert_to_audio(data=subtitle, tempo_mode="overflow")
+
+#Limit tempo speed on the overflow mode 
+sub.convert_to_audio(data=subtitle, tempo_mode="overflow", tempo_limit=1.2)
+
+#Save temporary audio to current folder
+sub = SubToAudio(model_name="tts_models/multilingual/multi-dataset/your_tts")
+subtitle = sub.subtitle("yoursubtitle.srt")
+sub.convert_to_audio(data=subtitle, output_path="subtitle.wav", save_temp=True)
+
 ```
 
 ### Citation 
 Eren, G., & The Coqui TTS Team. (2021). Coqui TTS (Version 1.4) [Computer software]. https://doi.org/10.5281/zenodo.6334862
```

### Comparing `subtoaudio-0.1.2/setup.py` & `subtoaudio-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 with open("README.md", "r", encoding="utf-8") as readme_file:
     README = readme_file.read()
 
 setup(
     name="subtoaudio",
     packages=find_packages(exclude=[]),
-    version="0.1.2",
+    version="0.1.3",
     license="MPL 2.0",
-    description="Subtitle to audio, generate speech from any subtitle file",
+    description="Subtitle to Audio, generate audio or speech from any subtitle file",
     author="Bagas NS",
     author_email="bagassantoso71@gmail.com",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bnsantoso/",
-    install_requires=["TTS","pydub","librosa",],
+    install_requires=["TTS","pydub","librosa","ffmpeg-python"],
     keywords=["subtitle", "tts", "text to audio", "subtitle to audio", "subtitle to speech",],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
         "Programming Language :: Python :: 3.9",
     ],
```

### Comparing `subtoaudio-0.1.2/subtoaudio/subtoaudio.py` & `subtoaudio-0.1.3/subtoaudio/subtoaudio.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import os
 import shutil
+import ffmpeg
 import librosa
 import tempfile
-import subprocess
 from TTS.api import TTS
 from pydub import AudioSegment
 
 class SubToAudio:
 
   def __init__( self,
                 model_name: str = None,
@@ -26,55 +26,93 @@
         print("English is default language")
         model_name = f"tts_models/{languages}/fairseq/vits"
       self.apitts = TTS(model_name=model_name, gpu=gpu, progress_bar=progress_bar)
     else:
       if config_path == None:
         print("Expecting config_path.json")
       else:
-        self.apitts = TTS(model_path=model_path, config_path=config_path, gpu=gpu, progress_bar=progress_bar)
+        self.apitts = TTS(model_path=model_path, 
+                          config_path=config_path, 
+                          gpu=gpu, 
+                          progress_bar=progress_bar)
 
   def subtitle(self, file_path:str):
-    with tempfile.NamedTemporaryFile(suffix=".srt") as temp_file:
+    self.name_path = file_path
+    with tempfile.NamedTemporaryFile(suffix=".srt", delete=False) as temp_file:
       temp_filename = temp_file.name
-      ffmpeg_command = f'ffmpeg -y -i "{file_path}" "{temp_filename}"'
-      subprocess.run(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+      input_stream = ffmpeg.input(file_path)
+      try:
+        ffmpeg.output(input_stream, temp_filename, y='-y').run()
+      except:
+        temp_file.close()
+        os.unlink(temp_filename)
+      temp_file.close()
       dictionary = self._extract_data_srt(temp_filename)
-      return dictionary
+      os.unlink(temp_filename)
+    return dictionary
 
   def convert_to_audio(self,
                        data=None,
                        speaker:str=None,
                        languages:str=None,
                        speaker_wav:str=None,
-                       output_path:str="output.wav",
+                       output_path:str=None,
+                       tempo_mode:str=None,
+                       tempo_speed:float=None,
+                       tempo_limit:float=None,
+                       save_temp:bool=False,
                       ):
+    
     try:
       if speaker == None:
         speaker = self.apitts.speakers[0]
         print(f"speaker is None, using '{speaker}' as default")
       if languages == None:
         languages = self.apitts.languages[0]
         print(f"Language is None, using '{languages}' as default")
     except:
       pass
 
-    if os.path.splitext(output_path)[1] != ".wav":
+    if output_path == None:
+      output_path = os.path.splitext(self.name_path)[0] + ".wav"
+    elif os.path.splitext(output_path)[1] != ".wav":
       output_path += ".wav"
 
+    if tempo_mode == "all":
+      if tempo_speed is None or not isinstance(tempo_speed, float):
+        tempo_speed = 1.2
+        print(f"tempo_speed speed is not Float")
+        print(f"tempo_speed change to default value '{tempo_speed}'")
+
     with tempfile.TemporaryDirectory() as temp_folder:
       print("Temporary folder:", temp_folder)
 
       for entry_data in data:
         audio_path = f"{temp_folder}/{entry_data['audio_name']}"
         self.apitts.tts_to_file(f"{entry_data['text']}",
                                 file_path=audio_path,
                                 speaker=speaker,
                                 language=languages,
                                 speaker_wav=speaker_wav)
-        audio_length = int(round(librosa.get_duration(path=audio_path),3) * 1000)
+        
+        if tempo_mode == "all":
+          self._tempo(mode=tempo_mode,audiopath = audio_path, 
+                      tempospeed = tempo_speed) 
+
+        elif tempo_mode == "overflow":
+          audio_length = self._audio_length(audio_path)
+          sub_time = entry_data['sub_time']
+          if audio_length > sub_time:
+            self._tempo(mode=tempo_mode,
+                        audiopath = audio_path, 
+                        audiolength=audio_length, 
+                        subtime=sub_time,
+                        tempolimit=tempo_limit)     
+
+        audio_length = self._audio_length(audio_path)
         entry_data['audio_length'] = audio_length
 
       for i in range(len(data)):
         if data[i]['audio_length'] > data[i]['sub_time']:
           shift_time = data[i]['audio_length'] - data[i]['sub_time'] + 50
           if i + 1 < len(data):
             data[i+1]['start_time'] += shift_time
@@ -89,14 +127,52 @@
         audio_path = f"{temp_folder}/{entry_data['audio_name']}"
         position = entry_data['start_time']
         overlay_audio = AudioSegment.from_file(audio_path)
         blank_base_audio = blank_base_audio.overlay(overlay_audio, position=position)
 
       blank_base_audio.export(output_path, format="wav")
 
+      if save_temp:
+        new_folder_name = os.path.splitext(self.name_path)[0]
+        self._move_tempaudio(temp_folder, new_folder_name)
+        pass
+  
+  def _tempo(self,
+             mode:str,
+             audiopath:str,
+             tempospeed:float=None,
+             audiolength:int=None,
+             subtime:int=None,
+             tempolimit:float=None,
+            ):
+            
+    if mode == "all":
+      atempo = tempospeed
+    if mode == "overflow":
+      atempo = audiolength / subtime
+      if tempolimit is not None and isinstance(tempolimit, float):
+        if atempo > tempolimit:
+          atempo = tempolimit
+
+    atempo = round(atempo, 2)
+    audio_out = audiopath+"temp.wav"
+    print(f"atempo {atempo}")
+    ffmpeg_command = (ffmpeg.input(audiopath).filter('atempo',atempo).output(audio_out))
+    try:
+      ffmpeg_command.run(capture_stdout=True, capture_stderr=True)
+    except ffmpeg.Error as e:
+        print('stdout:', e.stdout.decode('utf8'))
+        print('stderr:', e.stderr.decode('utf8'))
+        raise e
+    os.remove(audiopath)
+    os.rename(audio_out, audiopath)
+
+  def _audio_length(self, audio_path):
+    return int(round(librosa.get_duration(path=audio_path),3) * 1000)
+
   def _extract_data_srt(self, file_path):
     subtitle_data = []
     pattern = r'(\d+)\n([\d:,]+) --> ([\d:,]+)\n(.+?)\n\n'
 
     with open(file_path, 'r') as file:
         file_content = file.read()
 
@@ -131,7 +207,21 @@
     time_string = time_string.replace(":", "").replace(",", "")
     hours = int(time_string[:2])
     minutes = int(time_string[2:4])
     seconds = int(time_string[4:6])
     milliseconds = int(time_string[6:])
     total_milliseconds = (hours * 60 * 60 * 1000) + (minutes * 60 * 1000) + (seconds * 1000) + milliseconds
     return total_milliseconds
+
+  def _move_tempaudio(self, folder_path, new_folder):
+    try:
+        new_folder_path = os.path.join(os.getcwd(), new_folder)
+        os.mkdir(new_folder_path)
+        if not os.path.exists(new_folder_path):
+          os.mkdir(new_folder_path)
+        for item in os.listdir(folder_path):
+            item_path = os.path.join(folder_path, item)
+            if os.path.isfile(item_path):
+                shutil.move(item_path, new_folder)
+        print("Temp files moved successfully!")
+    except Exception as e:
+        print(f"Error occurred: {e}")
```

### Comparing `subtoaudio-0.1.2/subtoaudio.egg-info/PKG-INFO` & `subtoaudio-0.1.3/subtoaudio.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: subtoaudio
-Version: 0.1.2
-Summary: Subtitle to audio, generate speech from any subtitle file
+Version: 0.1.3
+Summary: Subtitle to Audio, generate audio or speech from any subtitle file
 Home-page: https://github.com/bnsantoso/
 Author: Bagas NS
 Author-email: bagassantoso71@gmail.com
 License: MPL 2.0
 Keywords: subtitle,tts,text to audio,subtitle to audio,subtitle to speech
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/bnsantoso)
 
 # Subtitle to Audio
 Subtitle to audio, generate audio from any subtitle file using Coqui-ai TTS and synchronize the audio timing according to subtitle time.
 
 ## Dependencies
-[ffmpeg](https://ffmpeg.org/), [pydub](https://github.com/jiaaro/pydub), [librosa](https://github.com/librosa/librosa), [coqui-ai TTS](https://github.com/coqui-ai/TTS/)
+[ffmpeg](https://ffmpeg.org/), [pydub](https://github.com/jiaaro/pydub), [librosa](https://github.com/librosa/librosa), [coqui-ai TTS](https://github.com/coqui-ai/TTS/), [ffmpeg-python](https://github.com/kkroening/ffmpeg-python)
 
 ## Installation
 
 ```bash
 pip install git+https://github.com/bnsantoso/sub-to-audio
 ```
 ```bash
@@ -37,15 +37,15 @@
 ## Example usage
 
 Basic use is very similiar to [Coqui-ai TTS](https://github.com/coqui-ai/TTS/), you can check their [documentation](https://tts.readthedocs.io/en/latest/inference.html).
 
 ```python
 from subtoaudio import SubToAudio
 
-#Using the Fairseq English speaker model as the default, the code will output 'output.wav' in the current directory.
+#Using the Fairseq English speaker model as the default, the code will output 'yoursubtitle.wav' in the current directory.
 sub = SubToAudio(gpu=True)
 subtitle = sub.subtitle("yoursubtitle.srt")
 sub.convert_to_audio(data=subtitle)
 
 #you can choose 1100 different language using fairseq model
 sub = SubToAudio(language='<lang-iso_code>')
 subtitle = sub.subtitle("yoursubtitle.ass")
@@ -62,12 +62,30 @@
 sub.convert_to_audio(data=subtitle)
 
 #By default, it is using "speaker=tts.speakers[0]/None, language=tts.languages[0]/None, speaker_wav=None"
 sub = SubToAudio(model_name="tts_models/multilingual/multi-dataset/your_tts")
 subtitle = sub.subtitle("yoursubtitle.srt")
 sub.convert_to_audio(data=subtitle, language="en", speaker="speakername", speaker_wav="your/path/speaker.wav", output_path="subtitle.wav")
 
+#Change the tempo or speech rate of all audio files , default is 1.2
+sub = SubToAudio(gpu=True)
+subtitle = sub.subtitle("yoursubtitle.srt")
+sub.convert_to_audio(data=subtitle, tempo_mode="all", tempo_speed=1.3)
+
+#Change tempo or speech rate to audio that doesn't match the subtitle duration
+sub = SubToAudio(gpu=True)
+subtitle = sub.subtitle("yoursubtitle.srt")
+sub.convert_to_audio(data=subtitle, tempo_mode="overflow")
+
+#Limit tempo speed on the overflow mode 
+sub.convert_to_audio(data=subtitle, tempo_mode="overflow", tempo_limit=1.2)
+
+#Save temporary audio to current folder
+sub = SubToAudio(model_name="tts_models/multilingual/multi-dataset/your_tts")
+subtitle = sub.subtitle("yoursubtitle.srt")
+sub.convert_to_audio(data=subtitle, output_path="subtitle.wav", save_temp=True)
+
 ```
 
 ### Citation 
 Eren, G., & The Coqui TTS Team. (2021). Coqui TTS (Version 1.4) [Computer software]. https://doi.org/10.5281/zenodo.6334862
```

