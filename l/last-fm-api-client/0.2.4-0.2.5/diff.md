# Comparing `tmp/last_fm_api_client-0.2.4.tar.gz` & `tmp/last_fm_api_client-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "last_fm_api_client-0.2.4.tar", max compression
+gzip compressed data, was "last_fm_api_client-0.2.5.tar", max compression
```

## Comparing `last_fm_api_client-0.2.4.tar` & `last_fm_api_client-0.2.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-28 17:55:46.624956 last_fm_api_client-0.2.4/last_fm_api_client/__init__.py
--rw-r--r--   0        0        0    11414 2023-06-03 18:30:38.302558 last_fm_api_client-0.2.4/last_fm_api_client/client.py
--rw-r--r--   0        0        0    11259 2023-08-01 18:59:03.534089 last_fm_api_client-0.2.4/last_fm_api_client/models.py
--rw-r--r--   0        0        0      383 2023-08-01 18:59:03.541881 last_fm_api_client-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1602 2023-08-01 18:59:03.538364 last_fm_api_client-0.2.4/README.md
--rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 last_fm_api_client-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-28 17:55:46.624956 last_fm_api_client-0.2.5/last_fm_api_client/__init__.py
+-rw-r--r--   0        0        0    12051 2023-08-01 19:06:20.154604 last_fm_api_client-0.2.5/last_fm_api_client/client.py
+-rw-r--r--   0        0        0    11660 2023-08-01 19:06:20.147585 last_fm_api_client-0.2.5/last_fm_api_client/models.py
+-rw-r--r--   0        0        0      383 2023-08-01 19:07:19.031188 last_fm_api_client-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1684 2023-08-01 19:07:25.811248 last_fm_api_client-0.2.5/README.md
+-rw-r--r--   0        0        0     2146 1970-01-01 00:00:00.000000 last_fm_api_client-0.2.5/PKG-INFO
```

### Comparing `last_fm_api_client-0.2.4/last_fm_api_client/client.py` & `last_fm_api_client-0.2.5/last_fm_api_client/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import datetime
 import logging
-from typing import Optional, Dict, Callable, Union
+from typing import Callable, Union
 from .models import *
 
-import pytz
 import requests
 
 logging.basicConfig(level=logging.DEBUG)
 # Define a custom exception class for API-related errors
 class LastFMClientError(Exception):
     pass
 
+
 # ...and for 404s
 class LastFMDataNotFound(Exception):
     pass
 
+
 class Client:
-    def __init__(self, api_key:str, user_agent:str, base_url:Optional[str]=None):
+    def __init__(self, api_key: str, user_agent: str, base_url: Optional[str] = None):
         """initializes an API client.
 
         :param api_key The Last.FM API key to use.
 
         :param user_agent An identificable user agent. Wanted by the Last.FM API:
         "Please use an identifiable User-Agent header on all requests. This helps our logging and reduces the risk of you getting banned."."""
         self.api_key = api_key
@@ -28,15 +28,20 @@
         self.logger = logging.getLogger(__name__)
         if base_url is None:
             base_url = "https://ws.audioscrobbler.com/2.0"
         else:
             base_url = base_url.strip("/")
         self.base_url = base_url
 
-    def generate_request_kwargs(self, api_method:str, request_parameters:Optional[Dict]=None, request_method:Optional[str]=None)->Dict:
+    def generate_request_kwargs(
+        self,
+        api_method: str,
+        request_parameters: Optional[Dict] = None,
+        request_method: Optional[str] = None,
+    ) -> Dict:
         """Last.FM uses URL parameters to add request data. This function builds a request containing
         that.
 
         :param api_method The Last.FM method to access, for example user.getRecentTracks.
 
         :param request_parameters: The parameters to include in the request (URL parameters). (This function adds format, method (api_method)
         and API key methods automagically)
@@ -52,57 +57,77 @@
         request_parameters["api_key"] = self.api_key
         request_parameters["format"] = "json"
         # Generate final kwargs to pass to requests.Request
         request_kwargs = {
             "url": self.base_url,
             "params": request_parameters,
             "method": request_method,
-            "headers": {
-                "User-Agent": self.user_agent
-            }
+            "headers": {"User-Agent": self.user_agent},
         }
-        self.logger.debug(f"Generated request parameters for a request to {api_method}: {request_kwargs}.")
+        self.logger.debug(
+            f"Generated request parameters for a request to {api_method}: {request_kwargs}."
+        )
         return request_kwargs
 
-
-    def send_request(self, api_method:str, request_parameters:Optional[Dict]=None, request_method:Optional[str]=None)->Union[
-        GetAlbumDetailsResponse, GetArtistResponse, GetTagInfoResponse, GetRecentTracksResponse
+    def send_request(
+        self,
+        api_method: str,
+        request_parameters: Optional[Dict] = None,
+        request_method: Optional[str] = None,
+    ) -> Union[
+        GetAlbumDetailsResponse,
+        GetArtistResponse,
+        GetTagInfoResponse,
+        GetRecentTracksResponse,
     ]:
         """Sends a Last.FM request and handles the response.
 
         :param api_method The Last.FM method to access, for example user.getRecentTracks.
 
         :param request_parameters: The parameters to include in the request (URL parameters). (This function adds format, method (api_method)
         and API key methods automagically)
 
         :param request_method: Optional argument to send any other request than a GET request. At least most endpoints in the API use GET
         request methods.
         """
         self.logger.debug(f"Sending a Last.FM request to {api_method}...")
         # Prepare request
-        request_kwargs = self.generate_request_kwargs(api_method, request_parameters, request_method)
+        request_kwargs = self.generate_request_kwargs(
+            api_method, request_parameters, request_method
+        )
         self.logger.debug("Sending a request...")
         response = requests.request(**request_kwargs)
         if response.status_code == 200:
             try:
                 response_json = response.json()
                 self.logger.debug(f"Last.FM responsed with JSON: {response_json}")
-                return METHOD_TO_MODEL[api_method].parse_obj(response_json) # Return the response
+                return METHOD_TO_MODEL[api_method].parse_obj(
+                    response_json
+                )  # Return the response
             except Exception as e:
-                error_message = f"Failed to decode response JSON. Original exception: {e}"
+                error_message = (
+                    f"Failed to decode response JSON. Original exception: {e}"
+                )
                 self.logger.critical(error_message, exc_info=True)
                 raise LastFMClientError(error_message)
         elif response.status_code == 404:
             raise LastFMDataNotFound("The Last.FM server responded with 404.")
         else:
             error_message = f"Unexpected status code returned from the Last.FM API: {response.status_code}. Please look into changing request parameters etc."
             self.logger.critical(error_message)
             raise LastFMClientError(error_message)
 
-    def handle_pagination(self, page_number, request_next:Callable, get_total_page_number:Callable, expand_response:Callable, previous_content=None):
+    def handle_pagination(
+        self,
+        page_number,
+        request_next: Callable,
+        get_total_page_number: Callable,
+        expand_response: Callable,
+        previous_content=None,
+    ):
         """A pagination handler. Will request an API method and keep adding data if there is more to it.
 
         :param page_number: The page number to retrieve.
 
         :param request_next: A function that will re-run the same request but with a new page number.
         This function receives a parameter: foo(new_page_number) and should return the response in the applicable model.
 
@@ -115,22 +140,34 @@
 
         :param previous_content: None on the first call, <data model with list inside> on subsequent calls"""
         self.logger.debug(f"Getting page: {page_number}...")
         response = request_next(page_number)
         self.logger.debug(f"Content for page {page_number} retrieved.")
         previous_content = expand_response(previous_content, response)
         total_page_number = get_total_page_number(response)
-        if total_page_number == page_number or total_page_number == 0: # Last.FM returns 0 if there is nothing.
-            self.logger.debug(f"Done handling pagination: {page_number} is the last page.")
+        if (
+            total_page_number == page_number or total_page_number == 0
+        ):  # Last.FM returns 0 if there is nothing.
+            self.logger.debug(
+                f"Done handling pagination: {page_number} is the last page."
+            )
             return previous_content
         else:
             self.logger.debug("Getting the next page...")
-            self.handle_pagination(page_number+1, request_next, get_total_page_number, expand_response, previous_content)
-
-    def get_album(self, artist:str, album:str, autocorrect:Optional[bool]=None)->GetAlbumDetailsResponse:
+            self.handle_pagination(
+                page_number + 1,
+                request_next,
+                get_total_page_number,
+                expand_response,
+                previous_content,
+            )
+
+    def get_album(
+        self, artist: str, album: str, autocorrect: Optional[bool] = None
+    ) -> GetAlbumDetailsResponse:
         """Retrieves information for an album.
 
         :param artist: The name of the album artist.
 
         :paran album: The name of the album.
 
         :param autocorrect From the Last.FM API docs:
@@ -139,18 +176,23 @@
         request_parameters = {
             "artist": artist,
             "album": album,
         }
         if autocorrect is None:
             autocorrect = True
         # Translate True or False into 1 or 0.
-        request_parameters["autocorrect"]:str = "1" if autocorrect else "0"
+        request_parameters["autocorrect"]: str = "1" if autocorrect else "0"
         return self.send_request("album.getInfo", request_parameters)
 
-    def get_artist(self, artist:str, autocorrect:Optional[bool]=None, language:Optional[str]=None)->GetArtistResponse:
+    def get_artist(
+        self,
+        artist: str,
+        autocorrect: Optional[bool] = None,
+        language: Optional[str] = None,
+    ) -> GetArtistResponse:
         """Retrieves information for an artist.
 
         :param artist: The aritst name to retrieve.
 
         :param autocorrect: From the Last.FM API docs:
         Transform misspelled artist names into correct artist names, returning the correct version instead.
         The corrected artist name will be returned in the response.
@@ -165,66 +207,76 @@
         # Translate True or False into 1 or 0.
         request_parameters["autocorrect"]: str = "1" if autocorrect else "0"
         # Add language if set
         if language is not None:
             request_parameters["language"] = language
         return self.send_request("artist.getInfo", request_parameters)
 
-    def get_tag(self, tag_name:str)->GetTagInfoResponse:
+    def get_tag(self, tag_name: str) -> GetTagInfoResponse:
         """Retrieves information about a tag.
 
         :param tag_name: The tag name to retrieve."""
-        request_parameters = {
-            "tag": tag_name
-        }
+        request_parameters = {"tag": tag_name}
         response = self.send_request("tag.getInfo", request_parameters)
         # Detect empty tags
         if response.tag.total == 0 and response.tag.reach == 0:
             raise LastFMDataNotFound("The tag you requested was not found.")
         return response
 
-    def get_scrobbles(self, user, from_time:Optional[datetime.datetime]=None, to_time:Optional[datetime.datetime]=None, limit:Optional[int]=None)->GetRecentTracksResponse:
+    def get_scrobbles(
+        self,
+        user,
+        from_time: Optional[datetime.datetime] = None,
+        to_time: Optional[datetime.datetime] = None,
+        limit: Optional[int] = None,
+    ) -> GetRecentTracksResponse:
         """Gets scrobbles for a certain user.
 
         :param user: The user to retrieve scrobbles for.
 
         :param from_time: A time interval (start time) to get scrobbles within
 
         :param to_time A time interval (end time) to get scrobbles within"""
         # Fill out limit and page if not set
         if limit is None:
             limit = 200
 
-        def get_scrobble_page(page_number:int)->GetRecentTracksResponse:
+        def get_scrobble_page(page_number: int) -> GetRecentTracksResponse:
             """Retrieves the scrobbles on a certain page number.
 
             :param page_number: The page number"""
-            request_parameters = {
-                "user": user,
-                "limit": limit,
-                "page": page_number
-            }
+            request_parameters = {"user": user, "limit": limit, "page": page_number}
             # The from time and to time should be unix timestamps. Perform the conversion
             if from_time is not None:
-                request_parameters["from"]:int = round(from_time.timestamp())
+                request_parameters["from"]: int = round(from_time.timestamp())
             if to_time is not None:
-                request_parameters["to"]:int = round(to_time.timestamp())
+                request_parameters["to"]: int = round(to_time.timestamp())
             return self.send_request("user.getRecentTracks", request_parameters)
 
-        def get_total_page_number(response:GetRecentTracksResponse)->int:
+        def get_total_page_number(response: GetRecentTracksResponse) -> int:
             """Gets the total page number of scrobbles."""
             return response.recenttracks.attr.total_pages
 
-        def expand_response(previous_content:Optional[GetRecentTracksResponse], new_content:Optional[GetRecentTracksResponse])->GetRecentTracksResponse:
+        def expand_response(
+            previous_content: Optional[GetRecentTracksResponse],
+            new_content: Optional[GetRecentTracksResponse],
+        ) -> GetRecentTracksResponse:
             """'Adds together' two different responses: one that is has data from the previous page(s)
             and one that is the current response
 
             :param previous_content: The previous response that contains data from the previous pages.
 
             :param new_content: A response that contains data from the current page to be added on to previous data."""
             if previous_content is not None:
-                previous_content.recenttracks.track.extend(new_content.recenttracks.track)
-                previous_content.recenttracks.attr = new_content.recenttracks.attr # Update the attribute
-                return previous_content # Return the updated content
+                previous_content.recenttracks.track.extend(
+                    new_content.recenttracks.track
+                )
+                previous_content.recenttracks.attr = (
+                    new_content.recenttracks.attr
+                )  # Update the attribute
+                return previous_content  # Return the updated content
             else:
-                return new_content # Return the new content on first response
-        return self.handle_pagination(1, get_scrobble_page, get_total_page_number, expand_response)
+                return new_content  # Return the new content on first response
+
+        return self.handle_pagination(
+            1, get_scrobble_page, get_total_page_number, expand_response
+        )
```

### Comparing `last_fm_api_client-0.2.4/last_fm_api_client/models.py` & `last_fm_api_client-0.2.5/last_fm_api_client/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,233 +1,308 @@
 import datetime
 
 import dateutil.parser
-from pydantic import BaseModel, Field, validator, BeforeValidator
+from pydantic import BaseModel, Field, validator
 from typing import List, Optional, Dict, Any
 from bs4 import BeautifulSoup
 
-def convert_non_list_to_list(cls, value)->List[Any]:
+
+def convert_non_list_to_list(cls, value) -> List[Any]:
     """Last.FM seems to sometimes return the item outside of a list and just by itself
     if there is just one item entry. This was troublesome since I thought it used lists
-    and I had writen all my models like that. """
+    and I had writen all my models like that."""
     return value if isinstance(value, list) else [value]
 
+
 # Functions used to normalize Last.FM data types
-def convert_empty_string_to_none(cls, value)->Optional[str]:
+def convert_empty_string_to_none(cls, value) -> Optional[str]:
     """Converts an empty string to None."""
     return value if value != "" else None
 
-def convert_number_to_bool(cls, value)->bool:
+
+def convert_number_to_bool(cls, value) -> bool:
     """Converts a 1 to True and 0 to False."""
     if value == "1":
         return True
     elif value == "0":
         return False
     else:
-        raise ValueError(f"Could not convert expected 1 or 0 to True or False: inptu string was: \"{value}\"")
+        raise ValueError(
+            f'Could not convert expected 1 or 0 to True or False: inptu string was: "{value}"'
+        )
+
 
-def convert_string_to_datetime(cls, value)->datetime:
+def convert_string_to_datetime(cls, value) -> datetime:
     """Converts a string to a datetime. All-inclusive to catch all possible formats."""
     return dateutil.parser.parse(value)
 
-def convert_unix_timestamp_to_datetime(cls, value)->datetime.datetime:
+
+def convert_unix_timestamp_to_datetime(cls, value) -> datetime.datetime:
     """Converts a unix timestamp to a datetime."""
     return datetime.datetime.fromtimestamp(int(value))
 
-def convert_html_to_raw_text(cls, value)->Optional[str]:
+
+def convert_html_to_raw_text(cls, value) -> Optional[str]:
     """Converts all HTML tags to text."""
     soup = BeautifulSoup(value, "html.parser")
-    parsed_content = " ".join(soup.find_all(text=True)).replace("\n", " ") # Make sure to remove any newlines.
+    parsed_content = " ".join(soup.find_all(text=True)).replace(
+        "\n", " "
+    )  # Make sure to remove any newlines.
     if len(parsed_content) > 0:
         return parsed_content
     else:
         return None
 
-def ensure_images_exist(cls, value)->Optional[List["Image"]]:
+
+def ensure_images_exist(cls, value) -> Optional[List["Image"]]:
     """Since Last.FM may return an image list with images, but all are empty, we need a check to ensure
     that that isn't the case."""
     result = []
-    if value is not None: # If the image is not empty
+    if value is not None:  # If the image is not empty
         # Check all images.
         if not isinstance(value, list):
             value = [value]
         for image in value:
             if image.get("#text", None) not in [None, ""]:
                 # If not empty, return the input value for further parsing
                 result.append(image)
         if len(result) > 0:
             return result
-    return None # If all images are empty or no images are set, we will get here.
+    return None  # If all images are empty or no images are set, we will get here.
+
 
 # Some generic classes: belongs to multiple model types
 class Image(BaseModel):
     """Represents an image of a certain size. Could be both artist and album images."""
+
     size: Optional[str]
     url: Optional[str] = Field(alias="#text")
     _normalize_size = validator("size", allow_reuse=True)(convert_empty_string_to_none)
     _normalize_url = validator("url", allow_reuse=True)(convert_empty_string_to_none)
 
 
 class Date(BaseModel):
     """Represents a certain date."""
+
     timestamp: datetime.datetime = Field(alias="uts")
     text: str = Field(alias="#text")
-    _normalize_timestamp = validator("timestamp", allow_reuse=True, pre=True)(convert_unix_timestamp_to_datetime)
+    _normalize_timestamp = validator("timestamp", allow_reuse=True, pre=True)(
+        convert_unix_timestamp_to_datetime
+    )
+
 
 class UndetailedMetadata(BaseModel):
     """Represents data for an undetailed album or artist in Last.FM that only includes two keys: #text and mbid."""
+
     text: Optional[str] = Field(alias="#text")
     mbid: Optional[str]
     _normalize_text = validator("text", allow_reuse=True)(convert_empty_string_to_none)
     _normalize_mbid = validator("mbid", allow_reuse=True)(convert_empty_string_to_none)
 
+
 class LinkMetadata(BaseModel):
     """Represents data for a link in the Last.Fm page"""
+
     href: str
     text: Optional[str] = Field(alias="#text")
     rel: Optional[str]
 
 
 # Tags
 class Tag(BaseModel):
     """Represents data for a tag in the Last.FM database."""
+
     name: str
     url: Optional[str]
 
+
 class TagDetailsWiki(BaseModel):
     """Represents the wiki for a detailed tag in the Last.FM database (see TagDetails)"""
-    summary: Optional[str] # Summary of the tag
-    content: Optional[str] # Content of the tag description
+
+    summary: Optional[str]  # Summary of the tag
+    content: Optional[str]  # Content of the tag description
     # Add normalizers for converting content to plaintext
-    _normalize_summary = validator("summary", allow_reuse=True, pre=True)(convert_html_to_raw_text)
-    _normalize_content = validator("content", allow_reuse=True, pre=True)(convert_html_to_raw_text)
+    _normalize_summary = validator("summary", allow_reuse=True, pre=True)(
+        convert_html_to_raw_text
+    )
+    _normalize_content = validator("content", allow_reuse=True, pre=True)(
+        convert_html_to_raw_text
+    )
+
 
 class TagDetails(BaseModel):
     """Represents data for a detailed tag in the Last.FM database (as retrieved from the tag.getInfo) method"""
+
     name: str
     total: int
     reach: int
     wiki: TagDetailsWiki
 
+
 class Tags(BaseModel):
     """Represents a list of tags or a single tag under the "tags" key (new since v0.2.3)."""
+
     tag: List[Tag]
-    _normalize_tag = validator("tag", allow_reuse=True, pre=True)(convert_non_list_to_list)
+    _normalize_tag = validator("tag", allow_reuse=True, pre=True)(
+        convert_non_list_to_list
+    )
 
 
 # Artist-related  things
 class ArtistStats(BaseModel):
     """Represents Last.FM stats for an artist."""
+
     listeners: int
     playcount: int
 
+
 class ArtistBiographyLinks(BaseModel):
     """Represents the links in the biography of an artist."""
+
     link: LinkMetadata
 
+
 class ArtistBiography(BaseModel):
     """Represents the biography of an artist."""
+
     links: ArtistBiographyLinks
     published: datetime.datetime
-    summary: Optional[str] # Summary of the biography
-    content: Optional[str] # Content of the biography
+    summary: Optional[str]  # Summary of the biography
+    content: Optional[str]  # Content of the biography
     # Add converter/normalizer for the published field to datetime
-    _normalize_published = validator("published", allow_reuse=True, pre=True)(convert_string_to_datetime)
+    _normalize_published = validator("published", allow_reuse=True, pre=True)(
+        convert_string_to_datetime
+    )
     # Add normalizers for converting content to plaintext
-    _normalize_summary = validator("summary", allow_reuse=True, pre=True)(convert_html_to_raw_text)
-    _normalize_content = validator("content", allow_reuse=True, pre=True)(convert_html_to_raw_text)
+    _normalize_summary = validator("summary", allow_reuse=True, pre=True)(
+        convert_html_to_raw_text
+    )
+    _normalize_content = validator("content", allow_reuse=True, pre=True)(
+        convert_html_to_raw_text
+    )
+
 
 class Artist(BaseModel):
     """Reprensts a simple artist model."""
+
     name: str
     url: Optional[str] = None
     image: Optional[List[Image]] = None
     mbid: Optional[str] = None
     # Ensure that Last.FM doesn't provide empty images
-    _normalize_image = validator("image", always=True, pre=True, allow_reuse=True)(ensure_images_exist)
+    _normalize_image = validator("image", always=True, pre=True, allow_reuse=True)(
+        ensure_images_exist
+    )
+
 
 class SimilarArtists(BaseModel):
     """Reprensts a list of similar artist for ArtistDetails."""
+
     artist: List[Artist]
 
+
 class ArtistDetails(BaseModel):
     """Represents data for an artist retrieved using the artist search method."""
+
     name: str
-    image: Optional[List[Image]]  = None
-    url: Optional[str]  = None
-    mbid: Optional[str]  = None
+    image: Optional[List[Image]] = None
+    url: Optional[str] = None
+    mbid: Optional[str] = None
     stats: ArtistStats
-    similar: SimilarArtists # Forward-reference to the artist because it hasn't been created yet.
-    streamable: Optional[str]  = None
+    similar: SimilarArtists  # Forward-reference to the artist because it hasn't been created yet.
+    streamable: Optional[str] = None
     ontour: Optional[str] = None
     tags: Optional[Tags] = None
-    bio: Optional[ArtistBiography]  = None
+    bio: Optional[ArtistBiography] = None
     # Add normalizer to convert streamable and ontour value to True or False
-    _normalize_streamable = validator("streamable", allow_reuse=True)(convert_number_to_bool)
+    _normalize_streamable = validator("streamable", allow_reuse=True)(
+        convert_number_to_bool
+    )
     _normalize_ontour = validator("ontour", allow_reuse=True)(convert_number_to_bool)
     # Ensure that Last.FM doesn't provide empty images
-    _normalize_image = validator("image", always=True, pre=True, allow_reuse=True)(ensure_images_exist)
+    _normalize_image = validator("image", always=True, pre=True, allow_reuse=True)(
+        ensure_images_exist
+    )
+
 
 # Track-related information
 class TrackAttr(BaseModel):
     """Represents attributes for a track on an album."""
+
     rank: int
 
+
 class Track(BaseModel):
     """Represents data for a track in the Last.FM database."""
-    duration: Optional[int]  = None
+
+    duration: Optional[int] = None
     artist: Artist
     url: str
     name: str
-    streamable: Optional[Dict]  = None
+    streamable: Optional[Dict] = None
     attr: Optional[TrackAttr] = Field(alias="@attr")
 
 
 class Tracks(BaseModel):
     """Represents a list of tracks or a single track under the "track" key (new since v0.2.4)"""
-    track: List[Track]  = None
-    _normalize_track = validator("track", allow_reuse=True, pre=True)(convert_non_list_to_list)
+
+    track: List[Track] = None
+    _normalize_track = validator("track", allow_reuse=True, pre=True)(
+        convert_non_list_to_list
+    )
 
 
 class TracksUndetailed(BaseModel):
     """Represents a list of tracks in form of undetailed metadata."""
+
     track: List[UndetailedMetadata]
-    _normalize_track = validator("track", allow_reuse=True, pre=True)(convert_non_list_to_list)
+    _normalize_track = validator("track", allow_reuse=True, pre=True)(
+        convert_non_list_to_list
+    )
 
 
 # Recent tracks. Note that Last.FM API calls them recenttracks rather than scrobbles,
 # so we go by that in the model naming
 class RecentTrack(BaseModel):
     """Represents a scrobbled track."""
-    artist: UndetailedMetadata # The track artist(s)
-    album: UndetailedMetadata # The album name
-    image: Optional[List[Image]] = None # The scrobble image
-    mbid: str # A MusicBrainz ID
-    date: Date # The data of the scrobble
-    name: str # The name of the track
-    url: Optional[str] = None # A link to the track
+
+    artist: UndetailedMetadata  # The track artist(s)
+    album: UndetailedMetadata  # The album name
+    image: Optional[List[Image]] = None  # The scrobble image
+    mbid: str  # A MusicBrainz ID
+    date: Date  # The data of the scrobble
+    name: str  # The name of the track
+    url: Optional[str] = None  # A link to the track
     # Add validator for converting an empty MusicBrainz string to None
     _normalize_mbid = validator("mbid", allow_reuse=True)(convert_empty_string_to_none)
     # Ensure that Last.FM doesn't provide empty images
-    _normalize_image = validator("image", always=True, pre=True, allow_reuse=True)(ensure_images_exist)
+    _normalize_image = validator("image", always=True, pre=True, allow_reuse=True)(
+        ensure_images_exist
+    )
+
 
 class RecentTracksAttr(BaseModel):
     """Contains the metadata entry of RecentTracks, including username etc."""
+
     user: str
     page: int
     total: int
     # Some camelCase to snake_case conversion done below
     total_pages: int = Field(alias="totalPages")
     per_page: int = Field(alias="perPage")
 
+
 class RecentTracks(BaseModel):
     """Represents basically what is returned from user.getRecentTracks - but it is contained within the subkey"""
+
     track: List[RecentTrack]
     attr: RecentTracksAttr = Field(alias="@attr")
-    _normalize_track = validator("track", allow_reuse=True, pre=True)(convert_non_list_to_list)
+    _normalize_track = validator("track", allow_reuse=True, pre=True)(
+        convert_non_list_to_list
+    )
 
 
 # Album-related
 class AlbumDetails(BaseModel):
     artist: str
     name: str
     listeners: int
@@ -237,37 +312,49 @@
     url: Optional[str] = None
     mbid: Optional[str] = None
     tags: Tags
     # Add validator for converting an empty tags and tracks to an empty list
     @validator("tags", pre=True, always=True)
     def handle_unset_tag_list(cls, value):
         return value if value is not None and value != "" else Tags(tag=[])
-    #... and for tracks too
-    _normalize_tracks = validator("tracks", allow_reuse=True)(convert_empty_string_to_none)
+
+    # ... and for tracks too
+    _normalize_tracks = validator("tracks", allow_reuse=True)(
+        convert_empty_string_to_none
+    )
     # Ensure that Last.FM doesn't provide empty images
-    _normalize_image = validator("image", always=True, pre=True, allow_reuse=True)(ensure_images_exist)
+    _normalize_image = validator("image", always=True, pre=True, allow_reuse=True)(
+        ensure_images_exist
+    )
 
 
 # Response models for API methods
 class GetRecentTracksResponse(BaseModel):
     """Represents a response for the user.getRecentTracks API method."""
+
     recenttracks: RecentTracks
 
+
 class GetAlbumDetailsResponse(BaseModel):
     """Represents a response for the album.getInfo API method."""
+
     album: AlbumDetails
 
+
 class GetArtistResponse(BaseModel):
     """Represents a response for the artist.getInfo API method."""
+
     artist: ArtistDetails
 
+
 class GetTagInfoResponse(BaseModel):
     """Represents a response for the tag.getInfo API method."""
+
     tag: TagDetails
 
+
 METHOD_TO_MODEL = {
     "user.getRecentTracks": GetRecentTracksResponse,
     "album.getInfo": GetAlbumDetailsResponse,
     "artist.getInfo": GetArtistResponse,
-    "tag.getInfo": GetTagInfoResponse
+    "tag.getInfo": GetTagInfoResponse,
 }
-
```

### Comparing `last_fm_api_client-0.2.4/README.md` & `last_fm_api_client-0.2.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,43 @@
-# Last.FM API Client
-
-A partially complete Python wrapper for the Last.FM API that implements the functions that I need for my Album of the day website.
-
-The wrapper uses `pydantic` models to parse responses which allows better type validation.
-
-### Implemented API methods
-
-The following [Last.FM API methods](https://www.last.fm/api/intro) are implemented:
-* `album.getInfo` - get information about an album
-* `artist.getInfo` - get information about an artist
-* `tag.getInfo` - get information about a tag
-* `user.getRecentTracks` - retrieve scrobbles
-
-### Changelog:
-* `v0.2.4`: Improved deserialization for multiple fields and cases where the album only has one tag.
-This change throws things around a little bit - you do not no longer have to check that items are singular
-or a list, the module will handle that for you.
-
-  **Breaking changes**
-    * List fields will now always return a list.
-    * Multiple fields are now optional and may return `None`.
-* `v0.2.3`: Fixed a bug that crashed the deserialization if an album only had one tag, which made
-Last.FM return a dictionary rather than a list containing the tag.
-* `v0.2.2`: Fixed a bug related to the loading of album images.
-  
-  **Breaking changes**
-    * The field `Image.size` is now optional and may return `None`.  
-* `v0.2.1`: Fixed empty album text being converted to None.
-* `v0.2.0`: Better handling of unset/empty Last.FM values.
-
-   **Breaking changes:**
-  * The field `Album.Tracks` is now optional and may return `None`.
-  * Same applies for all image fields.
-  * `v0.1.0`: Initial release
+# Last.FM API Client
+
+A partially complete Python wrapper for the Last.FM API that implements the functions that I need for my Album of the day website.
+
+The wrapper uses `pydantic` models to parse responses which allows better type validation.
+
+### Implemented API methods
+
+The following [Last.FM API methods](https://www.last.fm/api/intro) are implemented:
+
+- `album.getInfo` - get information about an album
+- `artist.getInfo` - get information about an artist
+- `tag.getInfo` - get information about a tag
+- `user.getRecentTracks` - retrieve scrobbles
+
+### Changelog:
+
+- `v.0.2.5`: Minor code quality changes. The module will also work with Pydantic versions that are not `v2.x.x`.
+
+- `v0.2.4`: Improved deserialization for multiple fields and cases where the album only has one tag.
+  This change throws things around a little bit - you do not no longer have to check that items are singular
+  or a list, the module will handle that for you.
+
+  **Breaking changes**
+  _ List fields will now always return a list.
+  _ Multiple fields are now optional and may return `None`.
+
+- `v0.2.3`: Fixed a bug that crashed the deserialization if an album only had one tag, which made
+  Last.FM return a dictionary rather than a list containing the tag.
+- `v0.2.2`: Fixed a bug related to the loading of album images.
+
+  **Breaking changes**
+
+  - The field `Image.size` is now optional and may return `None`.
+
+- `v0.2.1`: Fixed empty album text being converted to None.
+- `v0.2.0`: Better handling of unset/empty Last.FM values.
+
+  **Breaking changes:**
+
+  - The field `Album.Tracks` is now optional and may return `None`.
+  - Same applies for all image fields.
+  - `v0.1.0`: Initial release
```

### Comparing `last_fm_api_client-0.2.4/PKG-INFO` & `last_fm_api_client-0.2.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: last-fm-api-client
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: William04A
 Author-email: 35110380+William04A@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,33 +17,42 @@
 A partially complete Python wrapper for the Last.FM API that implements the functions that I need for my Album of the day website.
 
 The wrapper uses `pydantic` models to parse responses which allows better type validation.
 
 ### Implemented API methods
 
 The following [Last.FM API methods](https://www.last.fm/api/intro) are implemented:
-* `album.getInfo` - get information about an album
-* `artist.getInfo` - get information about an artist
-* `tag.getInfo` - get information about a tag
-* `user.getRecentTracks` - retrieve scrobbles
+
+- `album.getInfo` - get information about an album
+- `artist.getInfo` - get information about an artist
+- `tag.getInfo` - get information about a tag
+- `user.getRecentTracks` - retrieve scrobbles
 
 ### Changelog:
-* `v0.2.4`: Improved deserialization for multiple fields and cases where the album only has one tag.
-This change throws things around a little bit - you do not no longer have to check that items are singular
-or a list, the module will handle that for you.
+
+- `v.0.2.5`: Minor code quality changes. The module will also work with Pydantic versions that are not `v2.x.x`.
+
+- `v0.2.4`: Improved deserialization for multiple fields and cases where the album only has one tag.
+  This change throws things around a little bit - you do not no longer have to check that items are singular
+  or a list, the module will handle that for you.
 
   **Breaking changes**
-    * List fields will now always return a list.
-    * Multiple fields are now optional and may return `None`.
-* `v0.2.3`: Fixed a bug that crashed the deserialization if an album only had one tag, which made
-Last.FM return a dictionary rather than a list containing the tag.
-* `v0.2.2`: Fixed a bug related to the loading of album images.
-  
+  _ List fields will now always return a list.
+  _ Multiple fields are now optional and may return `None`.
+
+- `v0.2.3`: Fixed a bug that crashed the deserialization if an album only had one tag, which made
+  Last.FM return a dictionary rather than a list containing the tag.
+- `v0.2.2`: Fixed a bug related to the loading of album images.
+
   **Breaking changes**
-    * The field `Image.size` is now optional and may return `None`.  
-* `v0.2.1`: Fixed empty album text being converted to None.
-* `v0.2.0`: Better handling of unset/empty Last.FM values.
-
-   **Breaking changes:**
-  * The field `Album.Tracks` is now optional and may return `None`.
-  * Same applies for all image fields.
-  * `v0.1.0`: Initial release
+
+  - The field `Image.size` is now optional and may return `None`.
+
+- `v0.2.1`: Fixed empty album text being converted to None.
+- `v0.2.0`: Better handling of unset/empty Last.FM values.
+
+  **Breaking changes:**
+
+  - The field `Album.Tracks` is now optional and may return `None`.
+  - Same applies for all image fields.
+  - `v0.1.0`: Initial release
+
```

