# Comparing `tmp/gitlab_sdk-0.2.0.tar.gz` & `tmp/gitlab_sdk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_sdk-0.2.0.tar", last modified: Mon Jul 31 13:20:14 2023, max compression
+gzip compressed data, was "gitlab_sdk-0.2.1.tar", last modified: Tue Aug  1 16:13:00 2023, max compression
```

## Comparing `gitlab_sdk-0.2.0.tar` & `gitlab_sdk-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:20:14.299667 gitlab_sdk-0.2.0/
--rw-r--r--   0 root         (0) root         (0)      322 2023-07-31 13:20:14.298667 gitlab_sdk-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3214 2023-07-31 13:20:01.000000 gitlab_sdk-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:20:14.297666 gitlab_sdk-0.2.0/gitlab_sdk/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-31 13:20:01.000000 gitlab_sdk-0.2.0/gitlab_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-31 13:20:01.000000 gitlab_sdk-0.2.0/gitlab_sdk/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1838 2023-07-31 13:20:01.000000 gitlab_sdk-0.2.0/gitlab_sdk/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:20:14.298667 gitlab_sdk-0.2.0/gitlab_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      322 2023-07-31 13:20:14.000000 gitlab_sdk-0.2.0/gitlab_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      293 2023-07-31 13:20:14.000000 gitlab_sdk-0.2.0/gitlab_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 13:20:14.000000 gitlab_sdk-0.2.0/gitlab_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-31 13:20:14.000000 gitlab_sdk-0.2.0/gitlab_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-31 13:20:14.000000 gitlab_sdk-0.2.0/gitlab_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 13:20:14.299667 gitlab_sdk-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-31 13:20:01.000000 gitlab_sdk-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:20:14.298667 gitlab_sdk-0.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 13:20:01.000000 gitlab_sdk-0.2.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2424 2023-07-31 13:20:01.000000 gitlab_sdk-0.2.0/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:13:00.632813 gitlab_sdk-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-08-01 16:13:00.631812 gitlab_sdk-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3214 2023-08-01 16:12:47.000000 gitlab_sdk-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:13:00.630813 gitlab_sdk-0.2.1/gitlab_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-08-01 16:12:47.000000 gitlab_sdk-0.2.1/gitlab_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-08-01 16:12:47.000000 gitlab_sdk-0.2.1/gitlab_sdk/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2445 2023-08-01 16:12:47.000000 gitlab_sdk-0.2.1/gitlab_sdk/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:13:00.631812 gitlab_sdk-0.2.1/gitlab_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-08-01 16:13:00.000000 gitlab_sdk-0.2.1/gitlab_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      293 2023-08-01 16:13:00.000000 gitlab_sdk-0.2.1/gitlab_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 16:13:00.000000 gitlab_sdk-0.2.1/gitlab_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-08-01 16:13:00.000000 gitlab_sdk-0.2.1/gitlab_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-08-01 16:13:00.000000 gitlab_sdk-0.2.1/gitlab_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 16:13:00.632813 gitlab_sdk-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-08-01 16:12:47.000000 gitlab_sdk-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:13:00.631812 gitlab_sdk-0.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 16:12:47.000000 gitlab_sdk-0.2.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2753 2023-08-01 16:12:47.000000 gitlab_sdk-0.2.1/tests/test_client.py
```

### Comparing `gitlab_sdk-0.2.0/README.md` & `gitlab_sdk-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gitlab_sdk-0.2.0/gitlab_sdk/client.py` & `gitlab_sdk-0.2.1/gitlab_sdk/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,67 @@
+"""
+This module provides a client interface for tracking events using Snowplow.
+"""
 from snowplow_tracker import EmitterConfiguration, SelfDescribingJson, Snowplow, Subject
 
 SCHEMAS = {
     "custom_event": "iglu:com.gitlab/custom_event/jsonschema/1-0-0",
     "user_context": "iglu:com.gitlab/user_context/jsonschema/1-0-0",
 }
 DEFAULT_TRACKER_NAMESPACE = "gitlab"
 
 
 class Client:
+    """
+    Client to interact with Snowplow and send tracking events.
+    """
+
     def __init__(
         self,
         app_id: str,
         host: str,
     ):
+        """
+        Initializes the Client with given app_id and host.
+
+        Args:
+            app_id (str): Application ID.
+            host (str): Host for the collector.
+        """
         emitter_config = EmitterConfiguration(batch_size=1)
         self.tracker = Snowplow.create_tracker(
             app_id=app_id,
             namespace=DEFAULT_TRACKER_NAMESPACE,
             endpoint=host,
             emitter_config=emitter_config,
         )
         self.user_id = None
         self.user_attributes = None
 
     def track(self, event_name: str, event_payload: dict):
+        """
+        Tracks a custom event.
+
+        Args:
+            event_name (str): Name of the event.
+            event_payload (dict): Event data payload.
+        """
         self_desc_json = SelfDescribingJson(
             SCHEMAS["custom_event"], {"name": event_name, "props": event_payload}
         )
 
         track_arguments = {"event_json": self_desc_json}
         self.__set_user_data(track_arguments)
 
         self.tracker.track_self_describing_event(**track_arguments)
 
     def identify(self, user_id, user_attributes=None):
+        """
+        Identifies the user with given ID and attributes.
+        """
         self.user_id = user_id
         if not user_attributes:
             return
 
         self.user_attributes = user_attributes
 
     def __set_user_data(self, track_arguments: dict):
```

### Comparing `gitlab_sdk-0.2.0/tests/test_client.py` & `gitlab_sdk-0.2.1/tests/test_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Tests for the gitlab_sdk.client Client class.
+"""
 import pytest
 from snowplow_tracker import SelfDescribingJson, Snowplow
 
 from gitlab_sdk import Client
 from gitlab_sdk.client import SCHEMAS
 
 app_id = "app_id"
@@ -10,53 +13,58 @@
 event_payload = {"pay": "load"}
 user_id = "12"
 user_attributes = {"user_name": "Matthew"}
 
 
 @pytest.fixture(autouse=True)
 def cleanup_after_test():
+    """Reset Snowplow after each test."""
     yield
     Snowplow.reset()
 
 
 def test_initializes_snowplow_tracker_correctly(mocker):
+    """Test if Snowplow initializes correctly when Client is instantiated."""
     mocked_tracker_creation = mocker.patch("snowplow_tracker.Snowplow.create_tracker")
 
     Client(app_id=app_id, host=host)
 
     creation_args = mocked_tracker_creation.call_args[1]
     assert creation_args["app_id"] == app_id
     assert creation_args["namespace"] == "gitlab"
     assert creation_args["endpoint"] == host
     assert creation_args["emitter_config"].batch_size == 1
 
 
 def test_track(mocker):
+    """Test if tracking works correctly."""
     mocked_track = mocker.patch("snowplow_tracker.Tracker.track_self_describing_event")
 
     Client(app_id=app_id, host=host).track(event_name, event_payload)
 
     track_args = mocked_track.call_args[1]
     assert list(track_args.keys()) == ["event_json"]
     assert track_args["event_json"].schema == SCHEMAS["custom_event"]
     assert track_args["event_json"].data == {"name": event_name, "props": event_payload}
 
 
 def test_identify_without_user_attributes(mocker):
+    """Test identifying user without user attributes."""
     mocked_set_subject = mocker.patch("snowplow_tracker.Tracker.set_subject")
 
     client = Client(app_id=app_id, host=host)
     client.identify(user_id)
     client.track(event_name, event_payload)
 
     subject = mocked_set_subject.call_args[0][0]
     assert subject.standard_nv_pairs["uid"] == user_id
 
 
 def test_identify_with_user_attributes(mocker):
+    """Test identifying user with user attributes."""
     mocked_set_subject = mocker.patch("snowplow_tracker.Tracker.set_subject")
     mocked_track = mocker.patch("snowplow_tracker.Tracker.track_self_describing_event")
 
     client = Client(app_id=app_id, host=host)
     client.identify(user_id, user_attributes)
     client.track(event_name, event_payload)
```

