# Comparing `tmp/hp2p-api-0.0.2.tar.gz` & `tmp/hp2p-api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hp2p-api-0.0.2.tar", last modified: Mon Jun  5 07:32:33 2023, max compression
+gzip compressed data, was "hp2p-api-0.0.3.tar", last modified: Tue Aug  1 10:38:54 2023, max compression
```

## Comparing `hp2p-api-0.0.2.tar` & `hp2p-api-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-06-05 07:32:33.357616 hp2p-api-0.0.2/
--rw-r--r--   0 jay        (501) staff       (20)     1064 2022-10-25 09:30:30.000000 hp2p-api-0.0.2/LICENSE
--rw-r--r--   0 jay        (501) staff       (20)      345 2023-06-05 07:32:33.356865 hp2p-api-0.0.2/PKG-INFO
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-06-05 07:32:33.351367 hp2p-api-0.0.2/hp2p_api.egg-info/
--rw-r--r--   0 jay        (501) staff       (20)      345 2023-06-05 07:32:33.000000 hp2p-api-0.0.2/hp2p_api.egg-info/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      280 2023-06-05 07:32:33.000000 hp2p-api-0.0.2/hp2p_api.egg-info/SOURCES.txt
--rw-r--r--   0 jay        (501) staff       (20)        1 2023-06-05 07:32:33.000000 hp2p-api-0.0.2/hp2p_api.egg-info/dependency_links.txt
--rw-r--r--   0 jay        (501) staff       (20)        1 2023-06-05 07:31:10.000000 hp2p-api-0.0.2/hp2p_api.egg-info/not-zip-safe
--rw-r--r--   0 jay        (501) staff       (20)       29 2023-06-05 07:32:33.000000 hp2p-api-0.0.2/hp2p_api.egg-info/requires.txt
--rw-r--r--   0 jay        (501) staff       (20)        8 2023-06-05 07:32:33.000000 hp2p-api-0.0.2/hp2p_api.egg-info/top_level.txt
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-06-05 07:32:33.355501 hp2p-api-0.0.2/hp2papi/
--rw-r--r--   0 jay        (501) staff       (20)     1711 2023-06-05 07:31:56.000000 hp2p-api-0.0.2/hp2papi/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     3023 2023-05-16 09:53:35.000000 hp2p-api-0.0.2/hp2papi/api.py
--rw-r--r--   0 jay        (501) staff       (20)     5344 2023-05-16 09:53:35.000000 hp2p-api-0.0.2/hp2papi/api_func.py
--rw-r--r--   0 jay        (501) staff       (20)    15657 2023-05-16 09:53:35.000000 hp2p-api-0.0.2/hp2papi/classes.py
--rw-r--r--   0 jay        (501) staff       (20)       38 2023-06-05 07:32:33.357846 hp2p-api-0.0.2/setup.cfg
--rw-r--r--   0 jay        (501) staff       (20)      572 2023-06-05 07:31:49.000000 hp2p-api-0.0.2/setup.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-08-01 10:38:54.155776 hp2p-api-0.0.3/
+-rw-r--r--   0 jay        (501) staff       (20)     1064 2023-06-08 04:45:47.000000 hp2p-api-0.0.3/LICENSE
+-rw-r--r--   0 jay        (501) staff       (20)      345 2023-08-01 10:38:54.155660 hp2p-api-0.0.3/PKG-INFO
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-08-01 10:38:54.154811 hp2p-api-0.0.3/hp2p_api.egg-info/
+-rw-r--r--   0 jay        (501) staff       (20)      345 2023-08-01 10:38:54.000000 hp2p-api-0.0.3/hp2p_api.egg-info/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)      323 2023-08-01 10:38:54.000000 hp2p-api-0.0.3/hp2p_api.egg-info/SOURCES.txt
+-rw-r--r--   0 jay        (501) staff       (20)        1 2023-08-01 10:38:54.000000 hp2p-api-0.0.3/hp2p_api.egg-info/dependency_links.txt
+-rw-r--r--   0 jay        (501) staff       (20)        1 2023-08-01 10:38:54.000000 hp2p-api-0.0.3/hp2p_api.egg-info/not-zip-safe
+-rw-r--r--   0 jay        (501) staff       (20)       29 2023-08-01 10:38:54.000000 hp2p-api-0.0.3/hp2p_api.egg-info/requires.txt
+-rw-r--r--   0 jay        (501) staff       (20)        8 2023-08-01 10:38:54.000000 hp2p-api-0.0.3/hp2p_api.egg-info/top_level.txt
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-08-01 10:38:54.155495 hp2p-api-0.0.3/hp2papi/
+-rw-r--r--   0 jay        (501) staff       (20)     1711 2023-08-01 10:38:14.000000 hp2p-api-0.0.3/hp2papi/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     3211 2023-08-01 05:18:29.000000 hp2p-api-0.0.3/hp2papi/api.py
+-rw-r--r--   0 jay        (501) staff       (20)     6023 2023-08-01 10:35:27.000000 hp2p-api-0.0.3/hp2papi/api_func.py
+-rw-r--r--   0 jay        (501) staff       (20)     3654 2023-08-01 09:48:10.000000 hp2p-api-0.0.3/hp2papi/api_pb2.py
+-rw-r--r--   0 jay        (501) staff       (20)     2410 2023-08-01 10:06:45.000000 hp2p-api-0.0.3/hp2papi/api_pb2_grpc.py
+-rw-r--r--   0 jay        (501) staff       (20)    16704 2023-08-01 08:58:33.000000 hp2p-api-0.0.3/hp2papi/classes.py
+-rw-r--r--   0 jay        (501) staff       (20)       38 2023-08-01 10:38:54.155812 hp2p-api-0.0.3/setup.cfg
+-rw-r--r--   0 jay        (501) staff       (20)      572 2023-08-01 10:38:07.000000 hp2p-api-0.0.3/setup.py
```

### Comparing `hp2p-api-0.0.2/LICENSE` & `hp2p-api-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hp2p-api-0.0.2/hp2papi/__init__.py` & `hp2p-api-0.0.3/hp2papi/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,10 +47,10 @@
 #     "ModificationRequest",
 
 #     "Creation",
 # ]
 
 __all__ = []
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 __Init()
```

### Comparing `hp2p-api-0.0.2/hp2papi/api.py` & `hp2p-api-0.0.3/hp2papi/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,28 +28,39 @@
 
 @version 0.1
 @author jaylee@jayb.kr
 """
 
 from typing import Callable
 from .classes import *
-from .api_func import __CheckRequest, __Creation, __Query, __Modification, __Join, __SearchPeer, __SendData, __Leave, __Removal, __SetNotificatonListener
+from .api_func import __CheckRequest, __Creation, __Query, __Modification, __Join, __SearchPeer, __SendData, __Leave, __Removal, __SetNotificatonListener, __SetGrpcPort, __apapap
 
 __all__ = [
+    "SetGrpcPort",
+    "apapap",
     "Creation",
     "Query",
     "Modification",
     "Join",
     "SearchPeer",
     "SendData",
     "Leave",
     "Removal",
     "SetNotificatonListener",
 ]
 
+def SetGrpcPort(port: int) -> None:
+    """
+    gRPC 포트 설정
+    """
+    __SetGrpcPort(port)
+
+def apapap():
+    __apapap()
+
 def Creation(req: CreationRequest) -> CreationResponse:
     """
     신규 서비스 세션 생성
     """
     return __CheckRequest(req, __Creation)
 
 def Query(overlayId: str = None, title: str = None, description: str = None) -> QueryResponse:
```

### Comparing `hp2p-api-0.0.2/hp2papi/api_func.py` & `hp2p-api-0.0.3/hp2papi/api_func.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,30 +17,53 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
+import sys
+aaa  = sys.path
 from .classes import *
 #from collections.abc import Callable
 from typing import Callable
+import grpc
+from .api_pb2 import *
+from .api_pb2_grpc import *
+
 
 __notificationListeners = dict()
+__grpcPort = 50051
+
+def __SetGrpcPort(port: int) -> None:
+    global __grpcPort
+    __grpcPort = port
+
+def __GrpcStart() -> None:
+    server = grpc.aio.server(grpc.ThreadPoolExecutor(max_workers=10))
+    add_Hp2pApiProtoServicer_to_server(Hp2pApiProtoServicer(), server)
+    server.add_insecure_port('[::]:' + str(__grpcPort))
+    server.start()
+    print("Python gRPC Server is running on port " + str(__grpcPort))
+    server.wait_for_termination()
 
 def __Init():
+    __GrpcStart()
     print("Peer API init.")
 
 def __CheckRequest(req: Request, func: Callable[[Request], Response]) -> Response:
     if not req or not req.mandatoryCheck():
         return Response(ResponseCode.WrongRequest)
     
     return func(req)
 
 def __Creation(req: CreationRequest) -> CreationResponse:
+    if not req or not req.mandatoryCheck():
+        return CreationResponse(code=ResponseCode.WrongRequest)
+    
     return CreationResponse(code=ResponseCode.Success, overlayId="temp_overlay_id")
 
 def __Query(overlayId: str = None, title: str = None, description: str = None) -> QueryResponse:
     response = QueryResponse(ResponseCode.Success)
     response.overlay = [
         Overlay("temp_overlay_id1", "temp_title1", "temp_description1", "temp_owner_id1"),
         Overlay("temp_overlay_id2", "temp_title2", "temp_description2", "temp_owner_id2", OverlayClosed.SetAccessKey),
@@ -69,15 +92,15 @@
     faceChannel.keypointsType = "68points"
     
     audioChannel = ChannelAudio()
     audioChannel.channelId = "chid3"
     audioChannel.codec = AudioCodec.AAC
     audioChannel.sampleRate = AudioSampleRate.Is44100
     audioChannel.bitrate = AudioBitrate.Is128kbps
-    audioChannel.mono = AudioMono.Stereo
+    audioChannel.mono = AudioChannelType.Stereo
 
     textChannel = ChannelText()
     textChannel.channelId = "chid4"
     textChannel.sourceList = [ "*" ]
     textChannel.format = TextFormat.Plain
 
     response.channelList = [ serviceControlChannel, faceChannel, audioChannel, textChannel ]
```

### Comparing `hp2p-api-0.0.2/hp2papi/classes.py` & `hp2p-api-0.0.3/hp2papi/classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "ResponseCode",
     "DataType",
     "ChannelType",
     "FeatureBasedVideoMode",
     "AudioCodec",
     "AudioSampleRate",
     "AudioBitrate",
-    "AudioMono",
+    "AudioChannelType",
     "TextFormat",
     "Response",
     "OverlayClosed",
     "Overlay",
     "QueryResponse",
     "ChannelServiceControl",
     "ChannelFeatureBasedVideo",
@@ -82,14 +82,21 @@
 class ChannelType(Enum):
     ServiceControl = "control"
     FeatureBasedVideo = "feature/face"
     Audio = "audio"
     Text = "text"
 
 @unique
+class FeatureBasedVideoTarget(Enum):
+    Face = "face"
+    Body = "body"
+    Hands = "hands"
+    Pose = "pose"
+
+@unique
 class FeatureBasedVideoMode(Enum):
     KeypointsDescriptionMode = "KDM"
     SharedNeuralNetworkMode = "SNNM"
 
 @unique
 class AudioCodec(Enum):
     AAC = "AAC"
@@ -111,22 +118,26 @@
 class AudioBitrate(Enum):
     Is128kbps = "128kbps"
     Is192kbps = "192kbps"
     Is256kbps = "256kbps"
     Is320kbps = "320kbps"
 
 @unique
-class AudioMono(Enum):
+class AudioChannelType(Enum):
     Mono = "mono"
     Stereo = "stereo"
 
 @unique
 class TextFormat(Enum):
-    Plain = "Plain"
-    Json = "JSON"
+    Plain = "text/plain"
+    Json = "application/json"
+
+@unique
+class TextEncoding(Enum):
+    UTF8 = "UTF-8"
 
 @unique
 class OverlayClosed(Enum):
     Open = 0
     SetAccessKey = 1
     SetPeerList = 2
 
@@ -156,14 +167,16 @@
 @dataclass
 class Channel:
     channelId: str = None
     channelType: ChannelType = None
     sourceList: List[str] = None
 
     def mandatoryCheck(self) -> bool:
+        if not _check(self.channelId) or len(self.channelId) <= 0:
+            return False
         if not _check(self.channelType):
             return False
         
         return True
 
 @dataclass
 class Overlay:
@@ -195,45 +208,51 @@
 class ChannelFeatureBasedVideo(Channel):
     """
     feature를 위한 채널
     """
     def __init__(
         self,
         channelId: str = None,
+        target: FeatureBasedVideoTarget = None,
         mode: FeatureBasedVideoMode = None,
         resolution: str = None,
         framerate: str = None,
         keypointsType: str = None,
         modelLink: str = None,
         hash: str = None,
         dimension: str = None,
     ):
         self.channelId = channelId
+        self.target = target
         self.channelType = ChannelType.FeatureBasedVideo
         self.mode = mode
         self.resolution = resolution
         self.framerate = framerate
         self.keypointsType = keypointsType
         self.modelLink = modelLink
         self.hash = hash
         self.dimension = dimension
 
+    target: FeatureBasedVideoTarget = None
     mode: FeatureBasedVideoMode = None
     resolution: str = None
     framerate: str = None
     keypointsType: str = None
     modelLink: str = None
     hash: str = None
     dimension: str = None
 
     def mandatoryCheck(self) -> bool:
         if not super().mandatoryCheck():
             return False
         
-        if not _check(self.mode):
+        if not _check(self.target) or len(self.target) <= 0 or self.target not in FeatureBasedVideoTarget:
+            return False
+
+        if not _check(self.mode) or self.mode not in FeatureBasedVideoMode:
             return False
         
         if self.mode is FeatureBasedVideoMode.KeypointsDescriptionMode:
             if not _check(self.resolution):
                 return False
             if not _check(self.framerate):
                 return False
@@ -257,62 +276,67 @@
     """
     def __init__(
         self,
         channelId: str = None,
         codec: AudioCodec = None,
         sampleRate: AudioSampleRate = None,
         bitrate: AudioBitrate = None,
-        mono: AudioMono = None
+        channelType: AudioChannelType = None
     ):
         self.channelId = channelId
         self.channelType = ChannelType.Audio
         self.codec = codec
         self.sampleRate = sampleRate
         self.bitrate = bitrate
-        self.mono = mono
+        self.channelType = channelType
 
     codec: AudioCodec = None
     sampleRate: AudioSampleRate = None
     bitrate: AudioBitrate = None
-    mono: AudioMono = None
+    channelType: AudioChannelType = None
 
     def mandatoryCheck(self) -> bool:
         if not super().mandatoryCheck():
             return False
         
         if not _check(self.codec):
             return False
         if not _check(self.sampleRate):
             return False
         if not _check(self.bitrate):
             return False
-        if not _check(self.mono):
+        if not _check(self.channelType):
             return False
         
         return True
 
 @dataclass
 class ChannelText(Channel):
     """
     text를 위한 채널
     """
-    def __init__(self, channelId: str = None, format: TextFormat = None):
+    def __init__(self, channelId: str = None, format: TextFormat = TextFormat.Plain, encoding: TextEncoding = TextEncoding.UTF8):
         self.channelId = channelId
         self.channelType = ChannelType.Text
         self.format = format
+        self.encoding = encoding
 
     format: TextFormat = None
+    encoding: TextEncoding = None
     
     def mandatoryCheck(self) -> bool:
         if not super().mandatoryCheck():
             return False
         
         if not _check(self.format):
             return False
         
+        if not _check(self.encoding):
+            return False
+        
         return True
 
 @dataclass
 class CreationRequest(Request):
     """
     신규 서비스 생성 요청 Class
         mandatory:
@@ -335,14 +359,19 @@
             return False
         if not _check(self.ownerId):
             return False
         if not _check(self.adminKey):
             return False
         if not _check(self.channelList):
             return False
+        if not _check(self.channelList) or len(self.channelList) <= 0:
+            return False
+        for channel in self.channelList:
+            if not channel.mandatoryCheck():
+                return False
         
         return True
 
 @dataclass
 class CreationResponse(Response):
     overlayId: str = None
```

### Comparing `hp2p-api-0.0.2/setup.py` & `hp2p-api-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hp2p-api',
-    version='0.0.2',
+    version='0.0.3',
     description='An API for HP2P Peer',
     author='JAYB',
     author_email='jaylee@jayb.kr',
     url='https://github.com/ITU-T-SG11-Q8/Q.4102',
     install_requires=['grpcio', 'grpcio-tools', 'protobuf',],
     packages=find_packages(exclude=[]),
     keywords=['hp2p', 'hp2p-api'],
```

