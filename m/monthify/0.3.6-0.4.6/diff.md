# Comparing `tmp/monthify-0.3.6.tar.gz` & `tmp/monthify-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monthify-0.3.6.tar", max compression
+gzip compressed data, was "monthify-0.4.6.tar", max compression
```

## Comparing `monthify-0.3.6.tar` & `monthify-0.4.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1133 2023-05-18 06:24:22.438685 monthify-0.3.6/README.md
--rw-r--r--   0        0        0      435 2023-06-17 20:51:52.540666 monthify-0.3.6/monthify/__init__.py
--rw-r--r--   0        0        0       68 2023-05-18 06:24:22.439685 monthify-0.3.6/monthify/__main__.py
--rw-r--r--   0        0        0     1610 2023-06-17 20:51:52.540666 monthify-0.3.6/monthify/args.py
--rw-r--r--   0        0        0     1103 2023-06-17 20:51:52.540666 monthify-0.3.6/monthify/auth.py
--rw-r--r--   0        0        0      811 2023-06-17 20:51:52.540666 monthify-0.3.6/monthify/config.py
--rw-r--r--   0        0        0     2916 2023-06-17 20:51:52.540666 monthify-0.3.6/monthify/main.py
--rw-r--r--   0        0        0    18736 2023-06-23 22:28:01.461301 monthify-0.3.6/monthify/script.py
--rw-r--r--   0        0        0      769 2023-06-17 20:51:52.541666 monthify-0.3.6/monthify/track.py
--rw-r--r--   0        0        0     1185 2023-05-27 02:42:22.456255 monthify-0.3.6/monthify/utils.py
--rw-r--r--   0        0        0      815 2023-06-23 22:28:01.462301 monthify-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 monthify-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1133 2023-05-18 06:24:22.438685 monthify-0.4.6/README.md
+-rw-r--r--   0        0        0      735 2023-07-02 01:29:05.096437 monthify-0.4.6/monthify/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-18 06:24:22.439685 monthify-0.4.6/monthify/__main__.py
+-rw-r--r--   0        0        0     1739 2023-08-01 19:57:31.582312 monthify-0.4.6/monthify/args.py
+-rw-r--r--   0        0        0     1103 2023-07-02 01:14:09.885599 monthify-0.4.6/monthify/auth.py
+-rw-r--r--   0        0        0      811 2023-07-02 01:14:09.885599 monthify-0.4.6/monthify/config.py
+-rw-r--r--   0        0        0     3319 2023-08-01 20:00:17.933206 monthify-0.4.6/monthify/main.py
+-rw-r--r--   0        0        0    19913 2023-08-01 20:00:17.934206 monthify-0.4.6/monthify/script.py
+-rw-r--r--   0        0        0      769 2023-06-17 20:51:52.541666 monthify-0.4.6/monthify/track.py
+-rw-r--r--   0        0        0     1980 2023-08-01 19:57:31.582312 monthify-0.4.6/monthify/utils.py
+-rw-r--r--   0        0        0      815 2023-08-01 20:01:13.479811 monthify-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 monthify-0.4.6/PKG-INFO
```

### Comparing `monthify-0.3.6/README.md` & `monthify-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `monthify-0.3.6/monthify/args.py` & `monthify-0.4.6/monthify/args.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from argparse import ArgumentParser, Namespace
 
 from monthify import appname
 from monthify.config import Config
 
 
 def get_args(config: Config) -> ArgumentParser:
-    parser = ArgumentParser(
-        prog=appname.lower(), description="Sorts saved spotify tracks by month saved"
-    )
+    parser = ArgumentParser(prog=appname.lower(), description="Sorts saved spotify tracks by month saved")
 
     creation_group = parser.add_mutually_exclusive_group()
 
     parser.add_argument(
         "--CLIENT_ID",
         metavar="client_id",
         type=str,
@@ -40,14 +38,18 @@
         "-v",
         default=False,
         required=False,
         action="store_true",
         help="Displays version then exits",
     )
 
+    parser.add_argument(
+        "--public", default=False, required=False, action="store_true", help="Set created playlists to public"
+    )
+
     creation_group.add_argument(
         "--skip-playlist-creation",
         default=False,
         required=False,
         action="store_true",
         help="Skips playlist generation automatically",
     )
```

### Comparing `monthify-0.3.6/monthify/auth.py` & `monthify-0.4.6/monthify/auth.py`

 * *Files identical despite different names*

### Comparing `monthify-0.3.6/monthify/config.py` & `monthify-0.4.6/monthify/config.py`

 * *Files identical despite different names*

### Comparing `monthify-0.3.6/monthify/main.py` & `monthify-0.4.6/monthify/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #! /usr/bin/python3
 import sys
 from importlib.metadata import version
+from time import perf_counter
 
 from appdirs import user_data_dir
 from requests.exceptions import ConnectionError, ReadTimeout
 
-from monthify import ERROR, appauthor, appname, console
+from monthify import ERROR, appauthor, appname, console, logger
 from monthify.args import get_args, parse_args
 from monthify.auth import Auth
 from monthify.config import Config
 from monthify.script import Monthify
 
 appdata_location = user_data_dir(appname, appauthor)
 
@@ -20,14 +21,15 @@
 
 VERSION = args.version
 
 if VERSION:
     console.print(f"v{version('monthify')}")
     sys.exit(0)
 
+MAKE_PUBLIC = args.public
 SKIP_PLAYLIST_CREATION = args.skip_playlist_creation
 CREATE_PLAYLIST = args.create_playlists
 LOGOUT = args.logout
 
 if not config.is_using_config_file():
     CLIENT_ID = args.CLIENT_ID
     CLIENT_SECRET = args.CLIENT_SECRET
@@ -38,17 +40,16 @@
     if not config_args["CLIENT_ID"] or not config_args["CLIENT_SECRET"]:
         console.print("Spotify keys not found in config file")
         sys.exit(1)
     CLIENT_ID = config_args["CLIENT_ID"]
     CLIENT_SECRET = config_args["CLIENT_SECRET"]
 
 if not CLIENT_ID or not CLIENT_SECRET:
-    console.print(
-        "Client id and secret needed to connect to spotify's servers", style=ERROR
-    )
+    console.print("Client id and secret needed to connect to spotify's servers", style=ERROR)
+    logger.error("Client id and secret id not provided, exiting...")
     sys.exit(1)
 
 
 def run():
     try:
         controller = Monthify(
             Auth(
@@ -56,21 +57,24 @@
                 CLIENT_SECRET=CLIENT_SECRET,
                 LOCATION=appdata_location,
                 REDIRECT="https://open.spotify.com/",
                 SCOPES=(
                     "user-library-read",
                     "playlist-read-private",
                     "playlist-modify-private",
+                    "playlist-modify-public",
                 ),
             ),
             SKIP_PLAYLIST_CREATION=SKIP_PLAYLIST_CREATION,
             LOGOUT=LOGOUT,
             CREATE_PLAYLIST=CREATE_PLAYLIST,
+            MAKE_PUBLIC=MAKE_PUBLIC,
         )
 
+        t0 = perf_counter()
         # Starting info
         controller.starting()
 
         # Get user saved tracks
         controller.get_saved_track_info()
 
         # Generate names of playlists based on month and year saved tracks were added
@@ -79,23 +83,26 @@
         # Create playlists based on month and year
         controller.create_monthly_playlists()
 
         # Retrieve playlist ids of created playlists
         controller.get_monthly_playlist_ids()
 
         # Add saved tracks to created playlists by month and year
-        controller.sort_tracks_by_month()
+        controller.sort_all_tracks_by_month()
 
         # Update last run time
         controller.update_last_run()
+
+        logger.debug(f"Program completed in {perf_counter() - t0:.2f} s")
     except KeyboardInterrupt:
         console.print("Exiting...")
-    except (ConnectionError, ReadTimeout):
+    except (ConnectionError, ReadTimeout) as e:
         console.print(
             "Cannot connect to Spotify servers, please check your internet connection and try again",
             style=ERROR,
         )
+        logger.error(f"Could not connect to Spotify servers, stacktrace:\n{e.strerror}")
         sys.exit(1)
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `monthify-0.3.6/monthify/script.py` & `monthify-0.4.6/monthify/script.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,81 +1,77 @@
 # Script
 import sys
+from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
-from os import makedirs, remove, stat
+from os import remove, stat
 from os.path import exists
 from pathlib import Path
-from typing import Any, Generator, Iterable, List, Optional, Reversible, Tuple
+from time import perf_counter
+from typing import Iterable, Iterator, List, Optional, Reversible, Tuple
 
 from cachetools import TTLCache, cached
-from loguru import logger
 
-from monthify import ERROR, SUCCESS, appdata_location, console
+from monthify import ERROR, SUCCESS, appdata_location, console, logger
 from monthify.auth import Auth
 from monthify.track import Track
 from monthify.utils import conditional_decorator, normalize_text, sort_chronologically
 
 MAX_RESULTS = 10000
 CACHE_LIFETIME = 30
+MAX_WORKERS = 3
 
-makedirs(f"{appdata_location}/logs", exist_ok=True)
-logger.add(sys.stderr, format="{time} {level} {message}", filter="monthify", level="INFO")
-logger.remove()
-logger.add(f"{appdata_location}/logs/monthify.log", rotation="00:00", compression="zip")
 existing_playlists_file = f"{appdata_location}/existing_playlists_file.dat"
 last_run_file = f"{appdata_location}/last_run.txt"
 last_run_format = "%Y-%m-%d %H:%M:%S"
 saved_tracks_cache: TTLCache = TTLCache(maxsize=1000, ttl=86400)
 saved_playlists_cache: TTLCache = TTLCache(maxsize=1000, ttl=86400)
 user_cache: TTLCache = TTLCache(maxsize=1, ttl=86400)
+playlist_items_cache: TTLCache = TTLCache(maxsize=100, ttl=86400)
 
 
 class Monthify:
-    total_tracks_added = 0
-
     def __init__(
         self,
         auth: Auth,
         SKIP_PLAYLIST_CREATION: bool,
         LOGOUT: bool,
         CREATE_PLAYLIST: bool,
+        MAKE_PUBLIC: bool,
     ):
+        self.MAKE_PUBLIC = MAKE_PUBLIC
         self.LOGOUT = LOGOUT
         self.logout()
         authentication = auth
         self.sp = authentication.get_spotipy()
         self.SKIP_PLAYLIST_CREATION = SKIP_PLAYLIST_CREATION
         self.CREATE_PLAYLIST = CREATE_PLAYLIST
         self.has_created_playlists = False
         self.current_username: str
         self.current_display_name: str
         self.playlist_names: List[Tuple[str, str]]
+        self.total_tracks_added = 0
         self.already_created_playlists_exists = False
         if exists(existing_playlists_file) and stat(existing_playlists_file).st_size != 0:
             if (
                 datetime.now() - datetime.fromtimestamp(Path(existing_playlists_file).stat().st_ctime)
             ).days >= CACHE_LIFETIME:
                 remove(existing_playlists_file)
-                self.already_created_playlists = []
+                self.already_created_playlists = set([])
                 self.already_created_playlists_exists = False
             else:
                 with open(existing_playlists_file, "r", encoding="utf_8") as f:
-                    self.already_created_playlists = list(f.read().splitlines())
+                    self.already_created_playlists = set(f.read().splitlines())
                     self.already_created_playlists_exists = True
         else:
-            self.already_created_playlists = []
+            self.already_created_playlists = set([])
             self.already_created_playlists_exists = False
 
-        self.already_created_playlists_inter: List[str] = []
-        if exists(last_run_file):
-            if stat(last_run_file).st_size != 0:
-                with open(last_run_file, "r", encoding="utf_8") as f:
-                    self.last_run = f.read()
-            else:
-                self.last_run = ""
+        if exists(last_run_file) and stat(last_run_file).st_size != 0:
+            with open(last_run_file, "r", encoding="utf_8") as f:
+                self.last_run = f.read()
         else:
             self.last_run = ""
 
         self.playlist_names_with_id: List[Tuple[str, str, str]] = []
         self.name = """
         ___  ___            _   _     _  __       
         |  \/  |           | | | |   (_)/ _|      
@@ -162,86 +158,87 @@
         """
 
         logger.info("Starting user saved playlists fetch")
         results = self.get_results(self.sp.current_user_playlists(limit=50))
         logger.info("Ending user saved playlists fetch")
         return results
 
+    @cached(playlist_items_cache)
     def get_playlist_items(self, playlist_id: str) -> List[dict]:
         """
         Retrieves all the tracks in a specified spotify playlist identified by playlist id
         """
 
         logger.info(f"Starting playlist item fetch\n id: {playlist_id}", playlist_id)
         results = self.get_results(self.sp.playlist_items(playlist_id=playlist_id, fields=None, limit=20))
         logger.info(f"Ending playlist item fetch\n id: {playlist_id}")
         return results
 
-    def create_playlist(self, name: str) -> None:
+    def create_playlist(self, name: str) -> str:
         """
         Creates playlist with name var checking if the playlist already exists in the user's library,
         if it does the user is informed
         """
 
         sp = self.sp
         playlists = self.get_user_saved_playlists()
-        already_created_playlists: List[str] = []
         created_playlists = []
-        count = 0
         logger.info(f"Playlist creation called {name}")
+        t0 = perf_counter()
+        log = ""
+
         for item in playlists:
             if normalize_text(item["name"]) == normalize_text(name):
-                count += 1
-                console.print(f"Playlist {name} already exists")
-                self.already_created_playlists_inter.append(name)
+                log += f"Playlist {name} already exists"
+                self.already_created_playlists.add(name)
                 logger.info(f"Playlist already exists {name}")
-                return
-        if count != 0:
-            console.print(f"Playlist {name} already exists")
-        else:
-            console.print(f"Creating playlist {name}")
-            logger.info(f"Creating playlist {name}")
-            playlist = sp.user_playlist_create(
-                user=self.current_username,
-                name=name,
-                public=False,
-                collaborative=False,
-                description=f"{name}",
-            )
-            created_playlists.append(playlist)
-            console.print(f"Added {name} playlist")
-            logger.info(f"Added {name} playlist")
-        self.has_created_playlists = True if len(created_playlists) > 0 else False
-        self.already_created_playlists_inter = already_created_playlists
+                logger.debug(f"Playlist creation took {perf_counter() - t0} s")
+                return log
+
+        logger.debug(f"Playlist creation took {perf_counter() - t0} s")
+        log += "\n" f"Creating playlist {name}"
+        logger.info(f"Creating playlist {name}")
+        playlist = sp.user_playlist_create(
+            user=self.current_username,
+            name=name,
+            public=self.MAKE_PUBLIC,
+            collaborative=False,
+            description=f"{name}",
+        )
+        created_playlists.append(playlist)
+        log += "\n" f"Added {name} playlist"
+        log += "\n"
+        logger.info(f"Added {name} playlist")
+        self.has_created_playlists = len(created_playlists) > 0
+        return log
 
     def get_saved_track_info(self) -> None:
         """
         Calls the get_saved_track_gen function at program's start to cache the user's saved tracks
         """
 
         with console.status("Retrieving user saved tracks"):
             self.get_saved_track_gen()
 
-    def get_saved_track_gen(self) -> Generator[Track, Any, None]:
+    def get_saved_track_gen(self) -> Iterator[Track]:
         """
         Collates the user's saved tracks and adds them to a list as a Track type
         """
 
         tracks = self.get_user_saved_tracks()
         logger.info("Retrieving saved track info")
-        track_list = (
+        return (
             Track(
                 title=item["track"]["name"],
                 artist=item["track"]["artists"][0]["name"],
                 added_at=item["added_at"],
                 uri=item["track"]["uri"],
             )
             for item in tracks
         )
-        return track_list
 
     def get_playlist_names_names(self):
         """
         Generates month playlist names using the added_at attribute of the Track type
         """
 
         logger.info("Generating playlist names")
@@ -277,21 +274,24 @@
         if status is True:
             console.print("Playlist generation skipped")
             logger.info("Playlist generation skipped")
         else:
             logger.info("Playlist generation starting")
             if playlists is None:
                 RuntimeError("Playlists have not passed been passed to skip function")
-            for month, year in reversed(self.playlist_names):
-                playlist_name = str(month + " '" + year[2:])
-                if playlist_name in self.already_created_playlists and playlist_name in playlists:
-                    console.print(f"{month} '{year[2:]} playlist already exists")
-                else:
-                    name = month + " '" + year[2:]
-                    self.create_playlist(name)
+            t0 = perf_counter()
+            with ThreadPoolExecutor(max_workers=MAX_WORKERS) as executor:
+                playlist_names = [str(month + " '" + year[2:]) for month, year in self.playlist_names]
+
+                logs = executor.map(self.create_playlist, playlist_names)
+                for log in logs:
+                    if log is not None:
+                        console.print(log)
+
+            logger.debug(f"Entire playlist generation took {perf_counter() - t0} s")
 
     def create_monthly_playlists(self):
         """
         Creates playlists in user's library based on generated playlist names
         """
 
         logger.info("Creating playlists")
@@ -300,15 +300,15 @@
 
         monthly_ran = False
         last_run = datetime.now().strftime(last_run_format) if not self.last_run else self.last_run
 
         has_month_passed = datetime.strptime(last_run, last_run_format).strftime("%B") != datetime.now().strftime("%B")
         if has_month_passed and self.already_created_playlists_exists is False:
             self.skip(False, spotify_playlists)
-        elif has_month_passed is False and self.already_created_playlists_exists:
+        elif not has_month_passed and self.already_created_playlists_exists:
             monthly_ran = True
 
         if self.CREATE_PLAYLIST is False:
             if self.SKIP_PLAYLIST_CREATION is False and monthly_ran is False:
                 console.print("Playlist generation has not occured this month, Generating Playlists...")
                 logger.info("Requesting playlist creation")
                 self.skip(False, spotify_playlists)
@@ -321,32 +321,25 @@
                 logger.info("Requesting playlist creation")
 
                 if not console.input("> ").lower().startswith("y"):
                     self.skip(True)
                 else:
                     self.skip(False, spotify_playlists)
 
-            elif self.already_created_playlists_exists is False:
+            elif not self.already_created_playlists_exists:
                 console.print("Somehow the playlists do not exist. Generating Playlists...")
                 logger.info("Requesting playlist creation")
                 self.skip(False, spotify_playlists)
 
             else:
                 self.skip(True)
 
         else:
             self.skip(False, spotify_playlists)
 
-        if self.already_created_playlists_inter:
-            self.already_created_playlists = [
-                *self.already_created_playlists,
-                *self.already_created_playlists_inter,
-            ]
-            self.already_created_playlists = list(dict.fromkeys(self.already_created_playlists))
-
         if self.already_created_playlists:
             with open(existing_playlists_file, "w", encoding="utf_8") as f:
                 f.write("\n".join(self.already_created_playlists))
 
     def add_to_playlist(self, tracks: Reversible[Track], playlist_id: str) -> None:
         """
         Add a list of tracks to a specified playlist using playlist id
@@ -354,54 +347,83 @@
 
         logger.info(
             "Attempting to add tracks to playlist: {playlist}\ntracks: {tracks} ",
             tracks=tracks,
             playlist=str(playlist_id),
         )
         playlist_items = self.get_playlist_items(playlist_id)
-        to_be_added_uris: list[str] = []
+        to_be_added_uris: List[str] = []
 
         playlist_uris: Iterable[str] = tuple(item["track"]["uri"] for item in playlist_items)
+        log: str = ""
 
         for track in reversed(tracks):
             if track.uri in playlist_uris:
                 logger.info(f"Track: {track} already in playlist: {str(playlist_id)}")
                 track_url = f'https://open.{track.uri.replace(":", "/").replace("spotify", "spotify.com")}'
-                console.print(
+                log += (
+                    "\n"
                     f"[bold red][-][/bold red]\t[link={track_url}][cyan]{track.title} by {track.artist}[/cyan][/link]"
                     " already exists in the playlist"
                 )
             else:
                 logger.info(f"Track: {track} will be added to playlist: {str(playlist_id)}")
                 track_url = f'https://open.{track.uri.replace(":", "/").replace("spotify", "spotify.com")}'
-                console.print(
+                log += (
+                    "\n"
                     f"[bold green][+][/bold green]\t[link={track_url}][bold green]{track.title} by {track.artist}"
                     "[/bold green][/link]"
                     " will be added to the playlist "
                 )
                 to_be_added_uris.append(track.uri)
+        log += "\n"
 
         if not to_be_added_uris:
             logger.info("No tracks to add to playlist: {playlist}", playlist=playlist_id)
-            console.print("\t\n")
+            log += "\t\n"
         else:
             logger.info(
                 "Adding tracks: {tracks} to playlist: {playlist}",
                 tracks=(" ".join(to_be_added_uris)),
                 playlist=playlist_id,
             )
             to_be_added_uris_chunks = tuple(to_be_added_uris[x : x + 100] for x in range(0, len(to_be_added_uris), 100))
             for chunk in to_be_added_uris_chunks:
                 self.sp.playlist_add_items(playlist_id=playlist_id, items=chunk)
-            console.print("\n")
+            log += "\n"
             self.total_tracks_added += len(to_be_added_uris)
 
         logger.info("Ended track addition")
+        return log
+
+    def sort_tracks_by_month(self, playlist: List[Tuple[str, str, str]]) -> List[str]:
+        month, year, playlist_id = playlist
+        playlist_url = f"https://open.spotify.com/playlist/{playlist_id}"
+        playlist_name = f"{month} '{year[2:]}"
+        logger.info("Sorting into playlist: {playlist}", playlist=playlist_name)
+        log = []
+
+        tracks = tuple(track for track in self.get_saved_track_gen() if track.track_month == (month, year))
+        if not tracks:
+            return
+        else:
+            log.append(f"Sorting into playlist [link={playlist_url}]{playlist_name}[/link]")
+            log.append("\t\n")
+
+            logger.info(
+                "Adding tracks to playlist: {playlist}",
+                playlist=str(playlist_id),
+            )
+            t0 = perf_counter()
+            addedLog = self.add_to_playlist(tracks, playlist_id)
+            logger.debug(f"Finished adding tracks to playlist: {str(playlist_id)} in {perf_counter() - t0:.2f}s")
+            log.append(addedLog)
+            return log
 
-    def sort_tracks_by_month(self):
+    def sort_all_tracks_by_month(self):
         """
         Sorts saved tracks into appropriate monthly playlist
         """
 
         log = logger.bind(
             playlist_names=self.playlist_names_with_id,
             tracks=[track.title for track in self.get_saved_track_gen()],
@@ -423,36 +445,50 @@
             console.print(
                 f"Something has gone wrong error='{error}',"
                 " please run the program again with the --create-playlists flag",
                 style=ERROR,
             )
             sys.exit(1)
 
+        t0 = perf_counter()
         with console.status("Sorting Tracks"):
-            for month, year, playlist_id in self.playlist_names_with_id:
-                logger.info("Sorting into playlist: {playlist}", playlist=(month, year[2:]))
-                playlist_url = f"https://open.spotify.com/playlist/{playlist_id}"
-                playlist_name = f"{month} '{year[2:]}"
-
-                console.rule(f"Sorting into playlist [link={playlist_url}]{playlist_name}[/link]")
-                console.print("\t\n")
-                tracks = tuple(track for track in self.get_saved_track_gen() if track.track_month == (month, year))
-                if not tracks:
-                    break
-                else:
-                    logger.info(
-                        "Adding tracks to playlist: {playlist}",
-                        playlist=str(playlist_id),
-                    )
-                    self.add_to_playlist(tracks, playlist_id)
+            with ThreadPoolExecutor(max_workers=MAX_WORKERS) as executor:
+                logs = executor.map(self.sort_tracks_by_month, self.playlist_names_with_id)
+                for log in logs:
+                    console.rule(log[0])
+                    console.print("".join(log[1:]), end="")
+
+        logger.debug(f"Finished sorting tracks in {perf_counter() - t0:.2f}s")
 
         count = ""
         if self.total_tracks_added == 0:
             count = "No new tracks added"
         elif self.total_tracks_added == 1:
             count = "One track added"
         elif self.total_tracks_added > 1:
             count = f"Total tracks added to playlists: {self.total_tracks_added}"
 
         console.print(count)
         console.print("Finished playlist sort")
         logger.info("Finished script execution")
+
+    def clean_playlist(self, playlist_id: str):
+        counts = dict()
+        tracks_to_remove = []
+        items = self.get_playlist_items(playlist_id)
+        snapshot_id = self.sp.playlist(playlist_id, fields="snapshot_id")["snapshot_id"]
+        for idx, item in enumerate(items):
+            counts[item["track"]["uri"]] = {
+                "count": (counts.get(item["track"]["uri"], {"count": 0, "positions": []}))["count"] + 1,
+                "positions": [idx + 1],
+            }
+
+        for item_id, values in counts.items():
+            if values["count"] > 1:
+                tracks_to_remove.append({"uri": item_id.split(":")[2], "positions": values["positions"]})
+
+        if tracks_to_remove:
+            tracks_to_remove_chunks = (tracks_to_remove[x : x + 100] for x in range(0, len(tracks_to_remove), 100))
+            for chunk in tracks_to_remove_chunks:
+                self.sp.playlist_remove_specific_occurrences_of_items(
+                    playlist_id=playlist_id, items=chunk, snapshot_id=snapshot_id
+                )
```

### Comparing `monthify-0.3.6/monthify/track.py` & `monthify-0.4.6/monthify/track.py`

 * *Files identical despite different names*

### Comparing `monthify-0.3.6/monthify/utils.py` & `monthify-0.4.6/monthify/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Utilities
 
 import datetime
-from typing import Tuple
+from typing import Iterable, List, Tuple
 
 
 def extract_month_and_year(date: str) -> Tuple[str, str]:
     """Extract month and year from date string"""
     datem = datetime.datetime.strptime(date, "%Y-%m-%dT%H:%M:%SZ")
     year = datem.year
     month = datem.strftime("%B")
     return str(month), str(year)
 
 
-def sort_chronologically(playlist_names: list) -> list[str]:
+def sort_chronologically(playlist_names: Iterable) -> List[str]:
     """Sort months and years chronologically for playlist names"""
     sorted_list = sorted(
         playlist_names,
         key=lambda d: (d[1], datetime.datetime.strptime(d[0], "%B")),
         reverse=True,
     )
     return sorted_list
@@ -37,7 +37,39 @@
             if getattr(self, attribute) is True:
                 return func(self)
             return dec(func)(self)
 
         return wrapper
 
     return decorator
+
+
+def strIsGreater(a: str, b: str) -> bool:
+    """
+    Compare two strings by summing their ascii values
+    """
+    if sum(ord(c) for c in a.lower()) > sum(ord(c) for c in b.lower()):
+        return True
+    return False
+
+
+def search_normalized(dataset: Iterable[str], target: str) -> bool:
+    """
+    Binary search for target in dataset
+    """
+    low = 0
+    high = len(dataset) - 1
+    sorted_dataset = sorted(dataset, key=lambda a: sum(ord(c) for c in a.lower()))
+
+    while low <= high:
+        mid = (high + low) // 2
+        guess = sorted_dataset[mid]
+
+        if normalize_text(guess) == normalize_text(target):
+            return True
+
+        if strIsGreater(guess, target):
+            high = mid - 1
+        else:
+            low = mid + 1
+
+    return False
```

### Comparing `monthify-0.3.6/pyproject.toml` & `monthify-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monthify"
-version = "0.3.6"
+version = "0.4.6"
 description = "Sorts liked spotify tracks into playlists by the month they were liked."
 authors = ["Madiba Hudson-Quansah <mhquansah@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 loguru = "^0.6.0"
```

### Comparing `monthify-0.3.6/PKG-INFO` & `monthify-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monthify
-Version: 0.3.6
+Version: 0.4.6
 Summary: Sorts liked spotify tracks into playlists by the month they were liked.
 Author: Madiba Hudson-Quansah
 Author-email: mhquansah@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

