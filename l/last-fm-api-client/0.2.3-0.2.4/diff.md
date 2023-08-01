# Comparing `tmp/last_fm_api_client-0.2.3.tar.gz` & `tmp/last_fm_api_client-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "last_fm_api_client-0.2.3.tar", max compression
+gzip compressed data, was "last_fm_api_client-0.2.4.tar", max compression
```

## Comparing `last_fm_api_client-0.2.3.tar` & `last_fm_api_client-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-28 17:55:46.624956 last_fm_api_client-0.2.3/last_fm_api_client/__init__.py
--rw-r--r--   0        0        0    11414 2023-06-03 18:30:38.302558 last_fm_api_client-0.2.3/last_fm_api_client/client.py
--rw-r--r--   0        0        0    10190 2023-07-12 19:01:01.648159 last_fm_api_client-0.2.3/last_fm_api_client/models.py
--rw-r--r--   0        0        0      383 2023-07-12 19:01:19.291143 last_fm_api_client-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1204 2023-07-12 19:01:01.642144 last_fm_api_client-0.2.3/README.md
--rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 last_fm_api_client-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-28 17:55:46.624956 last_fm_api_client-0.2.4/last_fm_api_client/__init__.py
+-rw-r--r--   0        0        0    11414 2023-06-03 18:30:38.302558 last_fm_api_client-0.2.4/last_fm_api_client/client.py
+-rw-r--r--   0        0        0    11259 2023-08-01 18:59:03.534089 last_fm_api_client-0.2.4/last_fm_api_client/models.py
+-rw-r--r--   0        0        0      383 2023-08-01 18:59:03.541881 last_fm_api_client-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1602 2023-08-01 18:59:03.538364 last_fm_api_client-0.2.4/README.md
+-rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 last_fm_api_client-0.2.4/PKG-INFO
```

### Comparing `last_fm_api_client-0.2.3/last_fm_api_client/client.py` & `last_fm_api_client-0.2.4/last_fm_api_client/client.py`

 * *Files identical despite different names*

### Comparing `last_fm_api_client-0.2.3/last_fm_api_client/models.py` & `last_fm_api_client-0.2.4/last_fm_api_client/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import datetime
 
 import dateutil.parser
-from pydantic import BaseModel, Field, validator
-from typing import List, Optional, Dict, Union
+from pydantic import BaseModel, Field, validator, BeforeValidator
+from typing import List, Optional, Dict, Any
 from bs4 import BeautifulSoup
 
+def convert_non_list_to_list(cls, value)->List[Any]:
+    """Last.FM seems to sometimes return the item outside of a list and just by itself
+    if there is just one item entry. This was troublesome since I thought it used lists
+    and I had writen all my models like that. """
+    return value if isinstance(value, list) else [value]
+
 # Functions used to normalize Last.FM data types
 def convert_empty_string_to_none(cls, value)->Optional[str]:
     """Converts an empty string to None."""
     return value if value != "" else None
 
 def convert_number_to_bool(cls, value)->bool:
     """Converts a 1 to True and 0 to False."""
@@ -35,19 +41,25 @@
         return parsed_content
     else:
         return None
 
 def ensure_images_exist(cls, value)->Optional[List["Image"]]:
     """Since Last.FM may return an image list with images, but all are empty, we need a check to ensure
     that that isn't the case."""
-    if "image" not in [None, ""] and value is not None: # If the image is not empty
+    result = []
+    if value is not None: # If the image is not empty
         # Check all images.
+        if not isinstance(value, list):
+            value = [value]
         for image in value:
             if image.get("#text", None) not in [None, ""]:
-               return value # If not empty, return the input value for further parsing
+                # If not empty, return the input value for further parsing
+                result.append(image)
+        if len(result) > 0:
+            return result
     return None # If all images are empty or no images are set, we will get here.
 
 # Some generic classes: belongs to multiple model types
 class Image(BaseModel):
     """Represents an image of a certain size. Could be both artist and album images."""
     size: Optional[str]
     url: Optional[str] = Field(alias="#text")
@@ -94,15 +106,16 @@
     name: str
     total: int
     reach: int
     wiki: TagDetailsWiki
 
 class Tags(BaseModel):
     """Represents a list of tags or a single tag under the "tags" key (new since v0.2.3)."""
-    tag: Union[List[Tag], Tag]
+    tag: List[Tag]
+    _normalize_tag = validator("tag", allow_reuse=True, pre=True)(convert_non_list_to_list)
 
 
 # Artist-related  things
 class ArtistStats(BaseModel):
     """Represents Last.FM stats for an artist."""
     listeners: int
     playcount: int
@@ -122,77 +135,80 @@
     # Add normalizers for converting content to plaintext
     _normalize_summary = validator("summary", allow_reuse=True, pre=True)(convert_html_to_raw_text)
     _normalize_content = validator("content", allow_reuse=True, pre=True)(convert_html_to_raw_text)
 
 class Artist(BaseModel):
     """Reprensts a simple artist model."""
     name: str
-    url: Optional[str]
-    image: Optional[List[Image]]
-    mbid: Optional[str]
+    url: Optional[str] = None
+    image: Optional[List[Image]] = None
+    mbid: Optional[str] = None
     # Ensure that Last.FM doesn't provide empty images
     _normalize_image = validator("image", always=True, pre=True, allow_reuse=True)(ensure_images_exist)
 
 class SimilarArtists(BaseModel):
     """Reprensts a list of similar artist for ArtistDetails."""
     artist: List[Artist]
 
 class ArtistDetails(BaseModel):
     """Represents data for an artist retrieved using the artist search method."""
     name: str
-    image: Optional[List[Image]]
-    url: Optional[str]
-    mbid: Optional[str]
+    image: Optional[List[Image]]  = None
+    url: Optional[str]  = None
+    mbid: Optional[str]  = None
     stats: ArtistStats
     similar: SimilarArtists # Forward-reference to the artist because it hasn't been created yet.
-    streamable: Optional[str]
-    ontour: Optional[str]
-    tags: Optional[Tags]
-    bio: Optional[ArtistBiography]
+    streamable: Optional[str]  = None
+    ontour: Optional[str] = None
+    tags: Optional[Tags] = None
+    bio: Optional[ArtistBiography]  = None
     # Add normalizer to convert streamable and ontour value to True or False
     _normalize_streamable = validator("streamable", allow_reuse=True)(convert_number_to_bool)
     _normalize_ontour = validator("ontour", allow_reuse=True)(convert_number_to_bool)
     # Ensure that Last.FM doesn't provide empty images
     _normalize_image = validator("image", always=True, pre=True, allow_reuse=True)(ensure_images_exist)
 
 # Track-related information
 class TrackAttr(BaseModel):
     """Represents attributes for a track on an album."""
     rank: int
 
 class Track(BaseModel):
     """Represents data for a track in the Last.FM database."""
-    duration: Optional[int]
+    duration: Optional[int]  = None
     artist: Artist
     url: str
     name: str
-    streamable: Optional[Dict]
+    streamable: Optional[Dict]  = None
     attr: Optional[TrackAttr] = Field(alias="@attr")
 
 
 class Tracks(BaseModel):
-    """Represents a list of tracks."""
-    track: List[Track]
+    """Represents a list of tracks or a single track under the "track" key (new since v0.2.4)"""
+    track: List[Track]  = None
+    _normalize_track = validator("track", allow_reuse=True, pre=True)(convert_non_list_to_list)
+
 
 class TracksUndetailed(BaseModel):
     """Represents a list of tracks in form of undetailed metadata."""
     track: List[UndetailedMetadata]
+    _normalize_track = validator("track", allow_reuse=True, pre=True)(convert_non_list_to_list)
 
 
 # Recent tracks. Note that Last.FM API calls them recenttracks rather than scrobbles,
 # so we go by that in the model naming
 class RecentTrack(BaseModel):
     """Represents a scrobbled track."""
     artist: UndetailedMetadata # The track artist(s)
     album: UndetailedMetadata # The album name
-    image: Optional[List[Image]] # The scrobble image
+    image: Optional[List[Image]] = None # The scrobble image
     mbid: str # A MusicBrainz ID
     date: Date # The data of the scrobble
     name: str # The name of the track
-    url: Optional[str] # A link to the track
+    url: Optional[str] = None # A link to the track
     # Add validator for converting an empty MusicBrainz string to None
     _normalize_mbid = validator("mbid", allow_reuse=True)(convert_empty_string_to_none)
     # Ensure that Last.FM doesn't provide empty images
     _normalize_image = validator("image", always=True, pre=True, allow_reuse=True)(ensure_images_exist)
 
 class RecentTracksAttr(BaseModel):
     """Contains the metadata entry of RecentTracks, including username etc."""
@@ -203,26 +219,27 @@
     total_pages: int = Field(alias="totalPages")
     per_page: int = Field(alias="perPage")
 
 class RecentTracks(BaseModel):
     """Represents basically what is returned from user.getRecentTracks - but it is contained within the subkey"""
     track: List[RecentTrack]
     attr: RecentTracksAttr = Field(alias="@attr")
+    _normalize_track = validator("track", allow_reuse=True, pre=True)(convert_non_list_to_list)
 
 
 # Album-related
 class AlbumDetails(BaseModel):
     artist: str
     name: str
     listeners: int
     playcount: int
-    tracks: Optional[Tracks]
-    image: Optional[List[Image]]
-    url: Optional[str]
-    mbid: Optional[str]
+    tracks: Optional[Tracks] = None
+    image: Optional[List[Image]] = None
+    url: Optional[str] = None
+    mbid: Optional[str] = None
     tags: Tags
     # Add validator for converting an empty tags and tracks to an empty list
     @validator("tags", pre=True, always=True)
     def handle_unset_tag_list(cls, value):
         return value if value is not None and value != "" else Tags(tag=[])
     #... and for tracks too
     _normalize_tracks = validator("tracks", allow_reuse=True)(convert_empty_string_to_none)
```

### Comparing `last_fm_api_client-0.2.3/README.md` & `last_fm_api_client-0.2.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 The following [Last.FM API methods](https://www.last.fm/api/intro) are implemented:
 * `album.getInfo` - get information about an album
 * `artist.getInfo` - get information about an artist
 * `tag.getInfo` - get information about a tag
 * `user.getRecentTracks` - retrieve scrobbles
 
 ### Changelog:
+* `v0.2.4`: Improved deserialization for multiple fields and cases where the album only has one tag.
+This change throws things around a little bit - you do not no longer have to check that items are singular
+or a list, the module will handle that for you.
+
+  **Breaking changes**
+    * List fields will now always return a list.
+    * Multiple fields are now optional and may return `None`.
 * `v0.2.3`: Fixed a bug that crashed the deserialization if an album only had one tag, which made
 Last.FM return a dictionary rather than a list containing the tag.
 * `v0.2.2`: Fixed a bug related to the loading of album images.
   
   **Breaking changes**
     * The field `Image.size` is now optional and may return `None`.  
 * `v0.2.1`: Fixed empty album text being converted to None.
```

### Comparing `last_fm_api_client-0.2.3/PKG-INFO` & `last_fm_api_client-0.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: last-fm-api-client
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: William04A
 Author-email: 35110380+William04A@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,14 +23,21 @@
 The following [Last.FM API methods](https://www.last.fm/api/intro) are implemented:
 * `album.getInfo` - get information about an album
 * `artist.getInfo` - get information about an artist
 * `tag.getInfo` - get information about a tag
 * `user.getRecentTracks` - retrieve scrobbles
 
 ### Changelog:
+* `v0.2.4`: Improved deserialization for multiple fields and cases where the album only has one tag.
+This change throws things around a little bit - you do not no longer have to check that items are singular
+or a list, the module will handle that for you.
+
+  **Breaking changes**
+    * List fields will now always return a list.
+    * Multiple fields are now optional and may return `None`.
 * `v0.2.3`: Fixed a bug that crashed the deserialization if an album only had one tag, which made
 Last.FM return a dictionary rather than a list containing the tag.
 * `v0.2.2`: Fixed a bug related to the loading of album images.
   
   **Breaking changes**
     * The field `Image.size` is now optional and may return `None`.  
 * `v0.2.1`: Fixed empty album text being converted to None.
```

