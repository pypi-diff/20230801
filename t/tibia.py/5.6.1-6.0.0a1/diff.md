# Comparing `tmp/tibia.py-5.6.1.tar.gz` & `tmp/tibia.py-6.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tibia.py-5.6.1.tar", last modified: Tue Aug  1 14:05:30 2023, max compression
+gzip compressed data, was "tibia.py-6.0.0a1.tar", last modified: Fri Apr 28 02:33:28 2023, max compression
```

## Comparing `tibia.py-5.6.1.tar` & `tibia.py-6.0.0a1.tar`

### file list

```diff
@@ -1,58 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 14:05:30.268325 tibia.py-5.6.1/
--rw-rw-rw-   0        0        0    18300 2023-08-01 13:51:56.000000 tibia.py-5.6.1/CHANGELOG.rst
--rw-rw-rw-   0        0        0    11544 2023-07-05 20:29:37.000000 tibia.py-5.6.1/LICENSE
--rw-rw-rw-   0        0        0       83 2023-07-05 20:29:37.000000 tibia.py-5.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3874 2023-08-01 14:05:30.269325 tibia.py-5.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     2102 2023-08-01 13:43:59.000000 tibia.py-5.6.1/README.md
--rw-rw-rw-   0        0        0       54 2023-08-01 13:43:59.000000 tibia.py-5.6.1/requirements.txt
--rw-rw-rw-   0        0        0      399 2023-08-01 14:05:30.273325 tibia.py-5.6.1/setup.cfg
--rw-rw-rw-   0        0        0     3377 2023-08-01 13:43:59.000000 tibia.py-5.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 14:05:30.245316 tibia.py-5.6.1/tests/
--rw-rw-rw-   0        0        0        0 2023-07-05 20:29:37.000000 tibia.py-5.6.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1606 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/integration.py
--rw-rw-rw-   0        0        0    14231 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_bazaar.py
--rw-rw-rw-   0        0        0     9863 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_character.py
--rw-rw-rw-   0        0        0    15691 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_client.py
--rw-rw-rw-   0        0        0     5206 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_creature.py
--rw-rw-rw-   0        0        0      705 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_enums.py
--rw-rw-rw-   0        0        0      964 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_events.py
--rw-rw-rw-   0        0        0    14335 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_forums.py
--rw-rw-rw-   0        0        0    14465 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_guild.py
--rw-rw-rw-   0        0        0     6695 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_highscores.py
--rw-rw-rw-   0        0        0     6498 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_house.py
--rw-rw-rw-   0        0        0     2227 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_kill_statistics.py
--rw-rw-rw-   0        0        0     1855 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_leaderboards.py
--rw-rw-rw-   0        0        0     6855 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_new_changes.py
--rw-rw-rw-   0        0        0     3838 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_news.py
--rw-rw-rw-   0        0        0     4019 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_spell.py
--rw-rw-rw-   0        0        0      547 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_tibiapy.py
--rw-rw-rw-   0        0        0    11289 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_tournament.py
--rw-rw-rw-   0        0        0    15915 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_utils.py
--rw-rw-rw-   0        0        0     6561 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tests/tests_world.py
-drwxrwxrwx   0        0        0        0 2023-08-01 14:05:30.253316 tibia.py-5.6.1/tibia.py.egg-info/
--rw-rw-rw-   0        0        0     3874 2023-08-01 14:05:30.000000 tibia.py-5.6.1/tibia.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1097 2023-08-01 14:05:30.000000 tibia.py-5.6.1/tibia.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 14:05:30.000000 tibia.py-5.6.1/tibia.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-08-01 14:05:30.000000 tibia.py-5.6.1/tibia.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-08-01 14:05:30.000000 tibia.py-5.6.1/tibia.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 14:05:30.268325 tibia.py-5.6.1/tibiapy/
--rw-rw-rw-   0        0        0      813 2023-08-01 13:52:19.000000 tibia.py-5.6.1/tibiapy/__init__.py
--rw-rw-rw-   0        0        0    18874 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/abc.py
--rw-rw-rw-   0        0        0    64568 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/bazaar.py
--rw-rw-rw-   0        0        0    31177 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/character.py
--rw-rw-rw-   0        0        0    61932 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/client.py
--rw-rw-rw-   0        0        0    18209 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/creature.py
--rw-rw-rw-   0        0        0    13028 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/enums.py
--rw-rw-rw-   0        0        0     2087 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/errors.py
--rw-rw-rw-   0        0        0     8430 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/event.py
--rw-rw-rw-   0        0        0    53801 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/forum.py
--rw-rw-rw-   0        0        0    30916 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/guild.py
--rw-rw-rw-   0        0        0    14640 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/highscores.py
--rw-rw-rw-   0        0        0    21947 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/house.py
--rw-rw-rw-   0        0        0     6110 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/kill_statistics.py
--rw-rw-rw-   0        0        0     9242 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/leaderboard.py
--rw-rw-rw-   0        0        0    12853 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/news.py
--rw-rw-rw-   0        0        0    19736 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/spell.py
--rw-rw-rw-   0        0        0    30581 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/tournament.py
--rw-rw-rw-   0        0        0    21351 2023-08-01 13:43:59.000000 tibia.py-5.6.1/tibiapy/utils.py
--rw-rw-rw-   0        0        0    20853 2023-08-01 13:49:54.000000 tibia.py-5.6.1/tibiapy/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:28.537114 tibia.py-6.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    20334 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-04-28 02:33:28.537114 tibia.py-6.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-28 02:33:28.541114 tibia.py-6.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:28.521114 tibia.py-6.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_character.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_creature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14763 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_forums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_highscores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_house.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_kill_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_leaderboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_spell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_tibiapy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tests/tests_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:28.521114 tibia.py-6.0.0a1/tibia.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-04-28 02:33:28.000000 tibia.py-6.0.0a1/tibia.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-28 02:33:28.000000 tibia.py-6.0.0a1/tibia.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 02:33:28.000000 tibia.py-6.0.0a1/tibia.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-28 02:33:28.000000 tibia.py-6.0.0a1/tibia.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 02:33:28.000000 tibia.py-6.0.0a1/tibia.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:28.525114 tibia.py-6.0.0a1/tibiapy/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:28.529115 tibia.py-6.0.0a1/tibiapy/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13577 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/creature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/forum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/highscores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/house.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/kill_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/spell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/builders/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56147 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13943 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:28.533115 tibia.py-6.0.0a1/tibiapy/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16232 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/creature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/forum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/highscores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/house.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/kill_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/spell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/tibia_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/models/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:28.537114 tibia.py-6.0.0a1/tibiapy/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27479 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15091 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/creature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28691 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/forum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/highscores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/house.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/kill_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/spell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/parsers/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18006 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23767 2023-04-28 02:33:18.000000 tibia.py-6.0.0a1/tibiapy/utils.py
```

### Comparing `tibia.py-5.6.1/CHANGELOG.rst` & `tibia.py-6.0.0a1/CHANGELOG.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,637 +1,674 @@
-=========
-Changelog
-=========
-
-.. note::
-    Due to this library relying on external content, older versions are not guaranteed to work.
-    Try to always use the latest version.
-
-
-
-.. v5.6.1
-
-5.6.1 (2023-08-01)
-==================
-- Fixed parsing for world's creation date.
-
-
-.. v5.6.0
-
-5.6.0 (2023-02-17)
-==================
-- Added ``tier`` to items in auctions.
-
-
-.. v5.5.2
-
-5.5.2 (2022-09-02)
-==================
-- Fixed Houses section not parsing due to a change in the filters table.
-- Fixed status parameter not generating the correct URL in the houses section.
-
-.. v5.5.1
-
-5.5.1 (2022-08-02)
-==================
-- Adjusted parsing to support the changes related to mobile devices introduced on the day of this release. The following sections were affected:
-    - Highscores
-    - News
-    - Forums
-    - Spells
-
-.. v5.5.0
-
-5.5.0 (2022-07-27)
-==================
-- Added ``BOSS_POINTS`` to ``Category`` in highscores.
-
-
-.. v5.4.0
-
-5.4.0 (2022-07-23)
-==================
-- Added ``boss_points`` and ``bosstiary_progress`` to auctions.
-
-.. v5.3.0
-
-5.3.0 (2022-07-22)
-==================
-- Added support for Boostable Bosses.
-
-.. v5.2.1
-
-5.2.1 (2022-03-01)
-==================
-- Fixed bug in news ticker with a ``div`` tag failing to parse.
-- Updated code to detect the discussion thread link.
-
-.. v5.2.0
-
-5.2.0 (2021-12-31)
-==================
-- Added ``exalted_dust`` and ``exalted_dust_limit`` attributes to auctions.
-
-
-.. v5.1.0
-
-5.1.0 (2021-09-16)
-==================
-- Added ``traded`` attribute to death killers, to indicate that the killer was traded after the death occurred.
-- Properly handle deaths caused by summons of traded characters.
-
-.. v5.0.1
-
-5.0.1 (2021-08-26)
-==================
-- Fixed many sections not being parsed correctly due to changes to Tibia.com.
-    - Houses list
-    - News list
-    - Spells section
-    - Forums section
-- Fixed character's houses failing to parse due to a bug in the display in Tibia.com.
-    - Temporarily disabling this attribute.
-
-.. v5.0.0
-
-5.0.0 (2021-08-06)
-==================
-- Added parsing for Tibia Drome leaderboards, new ``Leaderboard`` class.
-    - Auxiliary classes ``LeaderboardEntry`` and ``LeaderboardRotation`` were added as well.
-    - New ``Client`` method: ``fetch_leaderboards``.
-- Added parsing for Spells library, new ``SpellsSection`` class.
-    - Auxiliary  classes ``Spell`` and ``SpellEntry``.
-    - New ``Client`` methods: ``fetch_spell`` and ``fetch_spells``
-- Fix last page of highscores having ``0`` as page value.
-- Using the ``Client`` class, you can now fetch and parse content from the test version of www.tibia.com when available.
-    - Note that if the test website has changes, parsing might not be possible.
-    - Internal URL attributes might still point to the regular website.
-- New ``HousesSection`` class, including the house filtering attributes.
-- New ``NewsArchive`` class, including the news filtering attributes.
-- New ``GuildsSection`` class, to replace the lists of ``GuildEntry``
-- Many "ListedObject" classes were renamed to "ObjectEntry", for details check the breaking changes below.
-- Fixed bug with other characters not being parsed.
-- Added ``traded`` attribute to ``LastPost`` class.
-- Added ``thread_starter_traded`` attribute to ``ThreadEntry``
-
-**Breaking Changes**:
-
-- Python 3.7 or higher is now required.
-- House classes no longer have ``get_list_url`` and ``list_from_content`` methods.
-- ``Client.fetch_world_houses`` now returns a ``HousesSection`` instance in its data attribute, instead of a list of ``ListedHouses``.
-- ``ListedHouse.highest_bid`` attribute now may be ``None`` if the house's auction has not yet started.
-- ``ListedHouse`` class renamed to ``HouseEntry``.
-- Removed deprecated property ``AuctionFilters.item``.
-- ``Client.fetch_news_archive``, ``Client.fetch_recent_news`` now returns an instance of ``NewsArchive`` in the ``data`` attribute.
-- ``ListedNews`` class renamed to ``NewsEntry``.
-- ``News`` and ``NewsEntry`` no longer have a ``get_list_url`` method.
-- ``ListedBoard`` class renamed to ``BoardEntry``.
-- ``ListedThread`` class renamed to ``ThreadEntry``.
-- ``ListedAnnouncement`` class renamed to ``AnnouncementEntry``.
-- ``ListedWorld`` class renamed to ``WorldEntry``.
-- ``ListedAuction`` class renamed to ``AuctionEntry``.
-- ``AuctionDetails`` class renamed to ``Auction``.
-- ``ListedGuild`` class renamed to ``GuildEntry``.
-- ``ListedTournament`` class renamed to ``TournamentEntry``.
-- ``Creature`` class renamed to ``CreatureEntry``.
-- ``CreatureDetail`` class renamed to ``Creature``.
-- ``Guild`` and ``GuildEntry`` class no longer have a ``get_list_url`` method.
-- Renamed ``begin_date`` parameter to ``start_date`` in ``fetch_news_archive``.
-- Renamed ``race`` attribute of ``CreatureEntry`` and ``Creature`` to ``identifier``, method parameters renamed as well.
-- ``CreaturesSection.from_boosted_creature_header`` renamed to ``CreaturesSection.boosted_creature_from_header``.
-
-
-.. v4.1.7
-
-4.1.7 (2021-06-30)
-==================
-- Fixed titles being parsed as part of the name for guild members with symbols in their name.
-
-.. v4.1.6
-
-4.1.6 (2021-06-28)
-==================
-- Fixed worlds not being parsed correctly again due to tournament worlds order changing. After this fix,
-  the order should not matter anymore.
-
-.. v4.1.5
-
-4.1.5 (2021-06-25)
-==================
-- Fixed parsing bug on characters, returning an incorrect exception when a character doesn't exist.
-
-.. v4.1.4
-
-4.1.4 (2021-06-17)
-==================
-- Fixed worlds not being parsed correctly due to tournament worlds order changing.
-
-.. v4.1.3
-
-4.1.3 (2021-05-12)
-==================
-- Fixed house transfer date not being parsed properly.
-
-
-.. v4.1.2
-
-4.1.2 (2021-04-27)
-==================
-- Fixed parsing errors for forum posts that contained a copy of the signature separator in the signature.
-
-.. v4.1.1
-
-4.1.1 (2021-04-19)
-==================
-- Fixed bug with extraneous character in some item descriptions, causing auction to give a parsing error.
-
-.. v4.1.0
-
-4.1.0 (2021-03-30)
-==================
-- Added ``prey_wildcards`` attribute to ``AuctionDetails``.
-- Added ``filters`` parameter to ``CharacterBazaar.get_auctions_history_url`` and ``Client.fetch_auction_history``.
-
-.. v4.0.0:
-
-4.0.0 (2021-03-10)
-==================
-- Breaking change: Removed ``BoostedCreature`` class, replaced by ``Creature`` class.
-    - Attributes should be compatible, ``image_url`` is a property of ``Creature``, calculated from its ``race`` attribute.
-- Added parsing and fetching for the Creature library section.
-    - Added ``CreatureSection``, ``Creature``, and ``CreatureDetail`` classes.
-- Added ``traded`` attribute to ``ForumAuthor``. Indicates if the author was a traded character.
-    - Previously, it would mark the author as a deleted character and its name would include ``(traded)``.
-- Fixed a bug with ``ForumBoards`` not parsing due to the cookies dialog that was added.
-- Added ``battleye_type`` attribute to ``ListedWorld`` and ``World`` classes. Indicates the type of BattlEye protection the world has.
-    - ``battleye_protected`` is now a property instead of an attribute.
-- Added ``YELLOW`` and ``GREEN`` aliases to all BattlEye related enums.
-- Fixed wrong timezone being used for forum related dates.
-
-.. v3.7.1:
-
-3.7.1 (2021-02-15)
-==================
-
-- Adjusted highscores parsing for upcoming Tibia.com changes.
-
-.. v3.7.0:
-
-3.7.0 (2021-02-09)
-==================
-
-- Parse familiars from auctions
-- Updated the way tooltips in auctions are parsed, the format changed, resulting in the previous code not working anymore.
-- Results count in bazaar pages are now properly parsed when there are comma thousand separators.
-- Item amounts are now more accurate instead of being based from their indicator (which was grouping them in thousands)
-
-
-.. v3.6.5:
-
-3.6.5 (2021-01-27)
-==================
-
-- Fixed auction history parsing breaking due to the cookie consent dialog.
-
-.. v3.6.4:
-
-3.6.4 (2021-01-26)
-==================
-
-- Fixed world list parsing breaking due to the cookie consent dialog.
-
-.. v3.6.3:
-
-3.6.3 (2021-01-14)
-==================
-
-- Fixed bug in guild names being parsed with Non-Breaking spaces instead of a regular space.
-
-.. v3.6.2:
-
-3.6.2 (2021-01-01)
-==================
-
-- Fixed bug in Event Calendar parsing.
-
-.. v3.6.1:
-
-3.6.1 (2020-12-28)
-==================
-
-- Fixed guild information being parsed incorrectly for characters in guilds containing "of the" in their name.
-
-.. v3.6.0:
-
-3.6.0 (2020-12-12)
-==================
-
-- Added support for the new filtering options in Highscores
-    - Added ``battleye_filter`` and ``pvp_types_filter`` attributes.
-- Added ``get_page_url()`` instance method to ``Highscores`` class.
-- Added ``previous_page_url`` and ``next_page_url`` properties.
-
-.. v3.5.7:
-
-3.5.7 (2020-12-04)
-==================
-
-- Fixed bug in Event Calendar parsing.
-
-
-.. v3.5.6:
-
-3.5.6 (2020-11-10)
-==================
-
-- Updated the URL used to fetch additional auction pages (items, mounts, outfits).
-
-.. v3.5.5:
-
-3.5.5 (2020-10-03)
-==================
-
-- Fixed charm expansion not being parsed correctly in auctions.
-
-.. v3.5.4:
-
-3.5.4 (2020-09-24)
-==================
-
-- Fetching auctions while skipping details is now faster.
-- Fixed bug in tournaments parsing.
-
-.. v3.5.3:
-
-3.5.3 (2020-09-24)
-==================
-
-- Fixed bug with ascending ordering (lowest / earliest) not being passed to the request URL.
-
-.. v3.5.2:
-
-3.5.2 (2020-09-23)
-==================
-
-- Fixed bug with auctions with more than 10 charms failing to parse.
-
-.. v3.5.1:
-
-3.5.1 (2020-09-22)
-==================
-
-- Fixed bug with recently traded characters in "other characters" section not being properly parsed.
-
-.. v3.5.0:
-
-3.5.0 (2020-09-22)
-==================
-
-- Added support for the new filtering options added to current auctions:
-    - Added new enumeration: ``AuctionSearchType``
-    - Renamed ``AuctionFilters`` attribute ``item`` to ``search_string``.
-      Property alias kept for backwards compatibility.
-    - Added new attribute ``AuctionFilters.search_type``
-
-.. v3.4.0:
-
-3.4.0 (2020-09-19)
-==================
-
-- Added option to only parse the listed information of an auction, to skip the rest of the parsing.
-- Fixed wrong type hint in ``ListedAuction`` for ``status``.
-
-.. v3.3.0:
-
-3.3.0 (2020-09-09)
-==================
-
-- Added support for the Character Bazaar
-    - Added classes: ``CharacterBazaar``, ``ListedAuction`` and ``AuctionDetails`` and many auxiliary classes.
-- Client methods throw a ``SiteMaintenanceError`` when Tibia.com is under maintenance, to be able to tell apart from
-  other network errors.
-
-.. v3.2.2:
-
-3.2.2 (2020-08-27)
-==================
-
-- Properly parse the name of recently traded characters.
-    - Added ``traded`` attribute to ``Character`` and ``OtherCharacter``.
-
-.. v3.2.1:
-
-3.2.1 (2020-08-25)
-==================
-
-- Fixed bug when parsing "other characters" from Tibia.com due to an unannounced change in the website.
-
-.. v3.2.0:
-
-3.2.0 (2020-08-10)
-==================
-
-- Added support for the new rules and score set added for the most recent Tournament.
-    - Added ``ScoreSet.creature_kills``
-    - Added ``ScoreSet.area_discovery``
-    - Added ``ScoreSet.skill_gain_loss``
-    - Added ``RuleSet.shared_xp_bonus``
-
-.. v3.1.0:
-
-3.1.0 (2020-07-29)
-==================
-
-- Added ``fetch_forum_post`` method to fetch a forum post directly.
-- Fixed bug with forum posts made by tournament characters.
-
-.. v3.0.3:
-
-3.0.3 (2020-07-28)
-==================
-
-- Fixed bug with character title being parsed incorrectly when the character has no title selected and a single unlocked title.
-
-.. v3.0.2:
-
-3.0.2 (2020-07-14)
-==================
-
-- Fixed values being mapped incorrectly for highscores.
-- ``ExpHighscoresEntry`` is now removed.
-
-.. v3.0.1:
-
-3.0.1 (2020-07-14)
-==================
-
-- ``Highscores.world`` is now ``None`` when the highscores are for all worlds.
-
-.. v3.0.0:
-
-3.0.0 (2020-07-13)
-==================
-- The ``Client`` class' methods now return their responses wrapped in a ``TibiaResponse`` object.
-  This contains information about Tibia.com's cache.
-- Added parsing for Guild wars.
-    - Added class ``GuildWars``
-    - Added class ``GuildWarsEntry``
-    - Added ``url_wars`` property and ``get_url_wars`` class method to all Guild classes.
-    - Added ``active_war`` attribute to ``Guild``.
-- Added parsing for the Tibia forums: Boards, Threads, Posts, Announcements
-    - Added classes ``ForumBoard`` and ``ListedBoard``
-    - Added classes ``ForumThread`` and ``ListedThread``
-    - Added classes ``ForumAnnouncement`` and ``ListedAnnouncement``
-    - Added classes ``ForumPost``
-    - Added auxiliary classes ``LastPost``,  ``ForumAuthor`` and ``ThreadStatus``.
-    - Added property ``thread_url`` to ``News``.
-- Updated highscores for Summer Update 2020:
-    - ``page`` and ``total_pages`` are now fields instead of properties.
-    - Added ``last_updated`` field.
-    - Added ``Category.GOSHNARS_TAINT`` and ``Category.CHARM_POINTS``.
-    - Added ``VocationFilter.NONE``.
-- Removed deprecated property ``house`` from ``Character``, use ``houses`` instead.
-- Removed support for Python 3.5.
-- Changed the hierarchy of base classes. Base classes no longer implement ``Serializable``, ``Serializable`` is now
-  directly implemented by most classes.
-- Removed TibiaData functionality.
-
-.. _v2.5.1:
-
-2.5.1 (2020-05-27)
-==================
-- Fixed bed count not being parsed on houses.
-
-.. _v2.5.0:
-
-2.5.0 (2020-05-22)
-==================
-- Added parsing of Tournaments and Tournament Leaderboards.
-- Fixed parsing errors with characters that had deaths by killers with "and" in their name.
-
-.. _v2.4.3:
-
-2.4.3 (2020-04-22)
-==================
-- Fixed an error when trying to parse a character with more deaths than what can be displayed in Tibia.com
-    - ``Character.deaths_truncated`` field was added to keep track of this case.
-
-.. _v2.4.2:
-
-2.4.2 (2020-02-26)
-==================
-- Fixed exception when attempting to parse highscores with no results (e.g. a new world on its first day).
-
-.. _v2.4.1:
-
-2.4.1 (2019-11-20)
-==================
-- Fixed incorrect argument name (house) in ``Character`` constructor.
-
-.. _v2.4.0:
-
-2.4.0 (2019-11-20)
-==================
-- Added support for multiple houses per character. Accessible on ``Character.houses`` field.
-- ``Character.house`` is now deprecated. It will contain the character's first house or ``None``.
-
-.. _v2.3.4:
-
-2.3.4 (2019-11-14)
-==================
-- Fixed bug with deaths not being parsed when a killer had ``and`` in their name.
-
-.. _v2.3.3:
-
-2.3.3 (2019-11-04)
-==================
-- Fixed bug with world parsing when there are more than 1000 players online.
-
-.. _v2.3.2:
-
-2.3.2 (2019-10-17)
-==================
-- Fixed incorrect highscores URL.
-
-.. _v2.3.1:
-
-2.3.1 (2019-10-06)
-==================
-- Fixed a bug with deaths not being parsed when a killer in assists had ``and`` in their name.
-
-.. _v2.3.0:
-
-2.3.0 (2019-09-16)
-==================
-- Added proxy option to client.
-
-.. _v2.2.6:
-
-2.2.6 (2019-09-01)
-==================
-- Fixed bug with account badges parsing failing when no badges were selected.
-
-.. _v2.2.5:
-
-2.2.5 (2019-08-22)
-==================
-
-- Fixed account badges parsing due to changes on the layout by CipSoft.
-
-.. _v2.2.4:
-
-2.2.4 (2019-08-20)
-==================
-
-- Disabled client compression for POST requests.
-
-.. _v2.2.3:
-
-2.2.3 (2019-08-17)
-==================
-
-- Enabled client side compression
-
-.. _v2.2.2:
-
-2.2.2 (2019-08-17)
-==================
-
-- Fixed killed by players and players kill stats being inverted for ``KillStatistics``
-
-.. _v2.2.1:
-
-2.2.1 (2019-08-10)
-==================
-
-- Fixed bug with character parsing failing when the guild rank is ``(member)``.
-
-.. _v2.2.0:
-
-2.2.0 (2019-08-08)
-==================
-
-- Added support for account badges and character titles.
-
-.. _v2.1.0:
-
-2.1.0 (2019-06-17)
-==================
-
-- Added ways to sort and filter House list results like in Tibia.com.
-- Added support to get the Boosted Creature of the day.
-
-.. _v2.0.1:
-
-2.0.1 (2019-06-04)
-==================
-
-- Replaced references to ``secure.tibia.com`` with ``www.tibia.com`` as the former always redirects to the front page.
-
-.. _v2.0.0:
-
-2.0.0 (2019-06-03)
-==================
-
-- Added asynchronous client to fetch and parse Tibia.com sections.
-- Added news parsing.
-- Added kill statistics parsing.
-- Added support for tournament worlds.
-- Added support for house prices with 'k' suffixes.
-
-.. _v1.1.3:
-
-1.1.3 (2019-01-29)
-==================
-
-- Fixed incorrect parsing of deaths with summons involved when parsing characters from TibiaData.
-
-.. _v1.1.2:
-
-1.1.2 (2019-01-22)
-==================
-
-- Fixed TibiaData URLs of tibia characters with special characters in their names. (e.g Himmelhüpferin)
-
-.. _v1.1.1:
-
-1.1.1 (2019-01-09)
-==================
-
-- Fixed character houses having attributes mixed up.
-
-.. _v1.1.0:
-
-1.1.0 (2019-01-09)
-==================
-
-- Parsing Highscores from Tibia.com and TibiaData.
-- Some strings from TibiaData had unpredictable trailing whitespaces,
-  all leading and trailing whitespaces are removed.
-- Added type hints to many variables and methods.
-
-.. _v1.0.0:
-
-1.0.0 (2018-12-23)
-==================
-
--  Added support for TibiaData JSON parsing. To have interoperability
-   between Tibia.com and TibiaData.
--  Added support for parsing Houses, House lists, World and World list
--  Added support for many missing attributes in Character and Guilds.
--  All objects are now serializable to JSON strings.
-
-.. _v0.1.0:
-
-0.1.0 (2018-08-17)
-==================
-
-Initial release:
-
--  Parses content from tibia.com
-
-   -  Character pages
-   -  Guild pages
-   -  Guild list pages
-
--  Parses content into JSON format strings.
--  Parses content into Python objects.
+=========
+Changelog
+=========
+
+.. note::
+    Due to this library relying on external content, older versions are not guaranteed to work.
+    Try to always use the latest version.
+
+.. v6.0.0
+
+6.0.0 (Unreleased)
+==================
+- Python 3.7 and below no longer supported.
+- All models are now Pydantic models, for better data validation, serialization and deserialization.
+- Models no longer contain methods to parse content, these have been moved to dedicated parser classes.
+- The location of models inside the module changed, so all imports need to be modified.
+- Model changes:
+    - Removed ``world`` from ``OnlineCharacter``.
+    - Removed ``category_icon`` from ``NewsEntry`` and ``News``.
+    - Added ``big_icon_url`` and ``small_icon_url`` to ``NewsCategory``
+    - ``Leaderboard.page`` renamed to ``current_page``.
+    - ``Highscores.page`` renamed to ``current_page``.
+    - Removed ``owner``, ``world``, ``status`` and ``type`` from ``GuildHouse``.
+    - Removed ``name`` from ``Death``.
+    - Removed ``owner``, ``status`` and ``type`` from ``CharacterHouse``.
+    - ``Auction`` renamed to ``AuctionDetails`` and is no longer a subclass of ``AuctionEntry``.
+    - ``AuctionEntry`` renamed to ``Auction``.
+    - ``CharacterBazaar.page`` renamed to ``current_page``.
+    - ``NewsArchive.categories`` and ``NewsArchive.types`` are now sets instead of lists.
+    - ``Character.account_status`` replaced with ``is_premium``.
+    - Renamed ``DisplayImage`` to ``ItemEntry``.
+    - Renamed ``DisplayMount`` to ``MountEntry``.
+    - Renamed ``DisplayOutfit`` to ``OutfitEntry``.
+    - Renamed ``DisplayFamiliar`` to ``FamiliarEntry``.
+    - Renamed ``page`` to ``current_page``, ``results`` to ``results_count``, and ``fully_fetched`` to ``is_fully_fetched`` in ``ItemSummary``, ``Mounts``, ``Familiars`` and ``Outfits``.
+    - Renamed ``CMPostArchive.page`` and ``CMPostArchive.posts`` to ``current_page`` and ``entries`` respectively.
+    - Renamed ``Killer``to ``DeathParticipant``
+    - Renamed ``ForumBoard.threads`` to ``entries``.
+    - Renamed ``ForumThread.posts`` to ``entries``.
+    - Added ``thread_starter_deleted`` to ``ThreadEntry``.
+    - ``ForumThread.previous_topic_number`` and ``ForumThread.next_topic_number`` may be ``None`` instead of ``0``.
+- Renamed ``Category`` to ``HighscoresCategory``.
+- Renamed ``BattlEyeTypeFilter`` to ``AuctionBattlEyeFilter``.
+- Renamed ``VocationFilter`` to ``HighscoresProfession``.
+- Renamed ``BattlEyeHighscoresFilter`` to ``HighscoresBattlEyeType``.
+- Renamed ``VocationAuctionFilter`` to ``AuctionVocationFilter``.
+- Renamed ``VocationSpellFilter`` to ``SpellVocationFilter``.
+- Renamed ``SkillFilter`` to ``AuctionSkillFilter``.
+- Added `ForumSection`` model and its respective parser, to fetch a list of board entries.
+- Removed ``get_url`` class methods from all models, replaced by functions in the urls package.
+- Fixed ``Character`` account badges not being parsed properly.
+
+
+
+.. v5.6.0
+
+5.6.0 (2023-02-17)
+==================
+- Added ``tier`` to items in auctions.
+
+
+.. v5.5.2
+
+5.5.2 (2022-09-02)
+==================
+- Fixed Houses section not parsing due to a change in the filters table.
+- Fixed status parameter not generating the correct URL in the houses section.
+
+.. v5.5.1
+
+5.5.1 (2022-08-02)
+==================
+- Adjusted parsing to support the changes related to mobile devices introduced on the day of this release. The following sections were affected:
+    - Highscores
+    - News
+    - Forums
+    - Spells
+
+.. v5.5.0
+
+5.5.0 (2022-07-27)
+==================
+- Added ``BOSS_POINTS`` to ``Category`` in highscores.
+
+
+.. v5.4.0
+
+5.4.0 (2022-07-23)
+==================
+- Added ``boss_points`` and ``bosstiary_progress`` to auctions.
+
+.. v5.3.0
+
+5.3.0 (2022-07-22)
+==================
+- Added support for Boostable Bosses.
+
+.. v5.2.1
+
+5.2.1 (2022-03-01)
+==================
+- Fixed bug in news ticker with a ``div`` tag failing to parse.
+- Updated code to detect the discussion thread link.
+
+.. v5.2.0
+
+5.2.0 (2021-12-31)
+==================
+- Added ``exalted_dust`` and ``exalted_dust_limit`` attributes to auctions.
+
+
+.. v5.1.0
+
+5.1.0 (2021-09-16)
+==================
+- Added ``traded`` attribute to death killers, to indicate that the killer was traded after the death occurred.
+- Properly handle deaths caused by summons of traded characters.
+
+.. v5.0.1
+
+5.0.1 (2021-08-26)
+==================
+- Fixed many sections not being parsed correctly due to changes to Tibia.com.
+    - Houses list
+    - News list
+    - Spells section
+    - Forums section
+- Fixed character's houses failing to parse due to a bug in the display in Tibia.com.
+    - Temporarily disabling this attribute.
+
+.. v5.0.0
+
+5.0.0 (2021-08-06)
+==================
+- Added parsing for Tibia Drome leaderboards, new ``Leaderboard`` class.
+    - Auxiliary classes ``LeaderboardEntry`` and ``LeaderboardRotation`` were added as well.
+    - New ``Client`` method: ``fetch_leaderboards``.
+- Added parsing for Spells library, new ``SpellsSection`` class.
+    - Auxiliary  classes ``Spell`` and ``SpellEntry``.
+    - New ``Client`` methods: ``fetch_spell`` and ``fetch_spells``
+- Fix last page of highscores having ``0`` as page value.
+- Using the ``Client`` class, you can now fetch and parse content from the test version of www.tibia.com when available.
+    - Note that if the test website has changes, parsing might not be possible.
+    - Internal URL attributes might still point to the regular website.
+- New ``HousesSection`` class, including the house filtering attributes.
+- New ``NewsArchive`` class, including the news filtering attributes.
+- New ``GuildsSection`` class, to replace the lists of ``GuildEntry``
+- Many "ListedObject" classes were renamed to "ObjectEntry", for details check the breaking changes below.
+- Fixed bug with other characters not being parsed.
+- Added ``traded`` attribute to ``LastPost`` class.
+- Added ``thread_starter_traded`` attribute to ``ThreadEntry``
+
+**Breaking Changes**:
+
+- Python 3.7 or higher is now required.
+- House classes no longer have ``get_list_url`` and ``list_from_content`` methods.
+- ``Client.fetch_world_houses`` now returns a ``HousesSection`` instance in its data attribute, instead of a list of ``ListedHouses``.
+- ``ListedHouse.highest_bid`` attribute now may be ``None`` if the house's auction has not yet started.
+- ``ListedHouse`` class renamed to ``HouseEntry``.
+- Removed deprecated property ``AuctionFilters.item``.
+- ``Client.fetch_news_archive``, ``Client.fetch_recent_news`` now returns an instance of ``NewsArchive`` in the ``data`` attribute.
+- ``ListedNews`` class renamed to ``NewsEntry``.
+- ``News`` and ``NewsEntry`` no longer have a ``get_list_url`` method.
+- ``ListedBoard`` class renamed to ``BoardEntry``.
+- ``ListedThread`` class renamed to ``ThreadEntry``.
+- ``ListedAnnouncement`` class renamed to ``AnnouncementEntry``.
+- ``ListedWorld`` class renamed to ``WorldEntry``.
+- ``ListedAuction`` class renamed to ``AuctionEntry``.
+- ``AuctionDetails`` class renamed to ``Auction``.
+- ``ListedGuild`` class renamed to ``GuildEntry``.
+- ``ListedTournament`` class renamed to ``TournamentEntry``.
+- ``Creature`` class renamed to ``CreatureEntry``.
+- ``CreatureDetail`` class renamed to ``Creature``.
+- ``Guild`` and ``GuildEntry`` class no longer have a ``get_list_url`` method.
+- Renamed ``begin_date`` parameter to ``start_date`` in ``fetch_news_archive``.
+- Renamed ``race`` attribute of ``CreatureEntry`` and ``Creature`` to ``identifier``, method parameters renamed as well.
+- ``CreaturesSection.from_boosted_creature_header`` renamed to ``CreaturesSection.boosted_creature_from_header``.
+
+
+.. v4.1.7
+
+4.1.7 (2021-06-30)
+==================
+- Fixed titles being parsed as part of the name for guild members with symbols in their name.
+
+.. v4.1.6
+
+4.1.6 (2021-06-28)
+==================
+- Fixed worlds not being parsed correctly again due to tournament worlds order changing. After this fix,
+  the order should not matter anymore.
+
+.. v4.1.5
+
+4.1.5 (2021-06-25)
+==================
+- Fixed parsing bug on characters, returning an incorrect exception when a character doesn't exist.
+
+.. v4.1.4
+
+4.1.4 (2021-06-17)
+==================
+- Fixed worlds not being parsed correctly due to tournament worlds order changing.
+
+.. v4.1.3
+
+4.1.3 (2021-05-12)
+==================
+- Fixed house transfer date not being parsed properly.
+
+
+.. v4.1.2
+
+4.1.2 (2021-04-27)
+==================
+- Fixed parsing errors for forum posts that contained a copy of the signature separator in the signature.
+
+.. v4.1.1
+
+4.1.1 (2021-04-19)
+==================
+- Fixed bug with extraneous character in some item descriptions, causing auction to give a parsing error.
+
+.. v4.1.0
+
+4.1.0 (2021-03-30)
+==================
+- Added ``prey_wildcards`` attribute to ``AuctionDetails``.
+- Added ``filters`` parameter to ``CharacterBazaar.get_auctions_history_url`` and ``Client.fetch_auction_history``.
+
+.. v4.0.0:
+
+4.0.0 (2021-03-10)
+==================
+- Breaking change: Removed ``BoostedCreature`` class, replaced by ``Creature`` class.
+    - Attributes should be compatible, ``image_url`` is a property of ``Creature``, calculated from its ``race`` attribute.
+- Added parsing and fetching for the Creature library section.
+    - Added ``CreatureSection``, ``Creature``, and ``CreatureDetail`` classes.
+- Added ``traded`` attribute to ``ForumAuthor``. Indicates if the author was a traded character.
+    - Previously, it would mark the author as a deleted character and its name would include ``(traded)``.
+- Fixed a bug with ``ForumBoards`` not parsing due to the cookies dialog that was added.
+- Added ``battleye_type`` attribute to ``ListedWorld`` and ``World`` classes. Indicates the type of BattlEye protection the world has.
+    - ``battleye_protected`` is now a property instead of an attribute.
+- Added ``YELLOW`` and ``GREEN`` aliases to all BattlEye related enums.
+- Fixed wrong timezone being used for forum related dates.
+
+.. v3.7.1:
+
+3.7.1 (2021-02-15)
+==================
+
+- Adjusted highscores parsing for upcoming Tibia.com changes.
+
+.. v3.7.0:
+
+3.7.0 (2021-02-09)
+==================
+
+- Parse familiars from auctions
+- Updated the way tooltips in auctions are parsed, the format changed, resulting in the previous code not working anymore.
+- Results count in bazaar pages are now properly parsed when there are comma thousand separators.
+- Item amounts are now more accurate instead of being based from their indicator (which was grouping them in thousands)
+
+
+.. v3.6.5:
+
+3.6.5 (2021-01-27)
+==================
+
+- Fixed auction history parsing breaking due to the cookie consent dialog.
+
+.. v3.6.4:
+
+3.6.4 (2021-01-26)
+==================
+
+- Fixed world list parsing breaking due to the cookie consent dialog.
+
+.. v3.6.3:
+
+3.6.3 (2021-01-14)
+==================
+
+- Fixed bug in guild names being parsed with Non-Breaking spaces instead of a regular space.
+
+.. v3.6.2:
+
+3.6.2 (2021-01-01)
+==================
+
+- Fixed bug in Event Calendar parsing.
+
+.. v3.6.1:
+
+3.6.1 (2020-12-28)
+==================
+
+- Fixed guild information being parsed incorrectly for characters in guilds containing "of the" in their name.
+
+.. v3.6.0:
+
+3.6.0 (2020-12-12)
+==================
+
+- Added support for the new filtering options in Highscores
+    - Added ``battleye_filter`` and ``pvp_types_filter`` attributes.
+- Added ``get_page_url()`` instance method to ``Highscores`` class.
+- Added ``previous_page_url`` and ``next_page_url`` properties.
+
+.. v3.5.7:
+
+3.5.7 (2020-12-04)
+==================
+
+- Fixed bug in Event Calendar parsing.
+
+
+.. v3.5.6:
+
+3.5.6 (2020-11-10)
+==================
+
+- Updated the URL used to fetch additional auction pages (items, mounts, outfits).
+
+.. v3.5.5:
+
+3.5.5 (2020-10-03)
+==================
+
+- Fixed charm expansion not being parsed correctly in auctions.
+
+.. v3.5.4:
+
+3.5.4 (2020-09-24)
+==================
+
+- Fetching auctions while skipping details is now faster.
+- Fixed bug in tournaments parsing.
+
+.. v3.5.3:
+
+3.5.3 (2020-09-24)
+==================
+
+- Fixed bug with ascending ordering (lowest / earliest) not being passed to the request URL.
+
+.. v3.5.2:
+
+3.5.2 (2020-09-23)
+==================
+
+- Fixed bug with auctions with more than 10 charms failing to parse.
+
+.. v3.5.1:
+
+3.5.1 (2020-09-22)
+==================
+
+- Fixed bug with recently traded characters in "other characters" section not being properly parsed.
+
+.. v3.5.0:
+
+3.5.0 (2020-09-22)
+==================
+
+- Added support for the new filtering options added to current auctions:
+    - Added new enumeration: ``AuctionSearchType``
+    - Renamed ``AuctionFilters`` attribute ``item`` to ``search_string``.
+      Property alias kept for backwards compatibility.
+    - Added new attribute ``AuctionFilters.search_type``
+
+.. v3.4.0:
+
+3.4.0 (2020-09-19)
+==================
+
+- Added option to only parse the listed information of an auction, to skip the rest of the parsing.
+- Fixed wrong type hint in ``ListedAuction`` for ``status``.
+
+.. v3.3.0:
+
+3.3.0 (2020-09-09)
+==================
+
+- Added support for the Character Bazaar
+    - Added classes: ``CharacterBazaar``, ``ListedAuction`` and ``AuctionDetails`` and many auxiliary classes.
+- Client methods throw a ``SiteMaintenanceError`` when Tibia.com is under maintenance, to be able to tell apart from
+  other network errors.
+
+.. v3.2.2:
+
+3.2.2 (2020-08-27)
+==================
+
+- Properly parse the name of recently traded characters.
+    - Added ``traded`` attribute to ``Character`` and ``OtherCharacter``.
+
+.. v3.2.1:
+
+3.2.1 (2020-08-25)
+==================
+
+- Fixed bug when parsing "other characters" from Tibia.com due to an unannounced change in the website.
+
+.. v3.2.0:
+
+3.2.0 (2020-08-10)
+==================
+
+- Added support for the new rules and score set added for the most recent Tournament.
+    - Added ``ScoreSet.creature_kills``
+    - Added ``ScoreSet.area_discovery``
+    - Added ``ScoreSet.skill_gain_loss``
+    - Added ``RuleSet.shared_xp_bonus``
+
+.. v3.1.0:
+
+3.1.0 (2020-07-29)
+==================
+
+- Added ``fetch_forum_post`` method to fetch a forum post directly.
+- Fixed bug with forum posts made by tournament characters.
+
+.. v3.0.3:
+
+3.0.3 (2020-07-28)
+==================
+
+- Fixed bug with character title being parsed incorrectly when the character has no title selected and a single unlocked title.
+
+.. v3.0.2:
+
+3.0.2 (2020-07-14)
+==================
+
+- Fixed values being mapped incorrectly for highscores.
+- ``ExpHighscoresEntry`` is now removed.
+
+.. v3.0.1:
+
+3.0.1 (2020-07-14)
+==================
+
+- ``Highscores.world`` is now ``None`` when the highscores are for all worlds.
+
+.. v3.0.0:
+
+3.0.0 (2020-07-13)
+==================
+- The ``Client`` class' methods now return their responses wrapped in a ``TibiaResponse`` object.
+  This contains information about Tibia.com's cache.
+- Added parsing for Guild wars.
+    - Added class ``GuildWars``
+    - Added class ``GuildWarsEntry``
+    - Added ``url_wars`` property and ``get_url_wars`` class method to all Guild classes.
+    - Added ``active_war`` attribute to ``Guild``.
+- Added parsing for the Tibia forums: Boards, Threads, Posts, Announcements
+    - Added classes ``ForumBoard`` and ``ListedBoard``
+    - Added classes ``ForumThread`` and ``ListedThread``
+    - Added classes ``ForumAnnouncement`` and ``ListedAnnouncement``
+    - Added classes ``ForumPost``
+    - Added auxiliary classes ``LastPost``,  ``ForumAuthor`` and ``ThreadStatus``.
+    - Added property ``thread_url`` to ``News``.
+- Updated highscores for Summer Update 2020:
+    - ``page`` and ``total_pages`` are now fields instead of properties.
+    - Added ``last_updated`` field.
+    - Added ``Category.GOSHNARS_TAINT`` and ``Category.CHARM_POINTS``.
+    - Added ``VocationFilter.NONE``.
+- Removed deprecated property ``house`` from ``Character``, use ``houses`` instead.
+- Removed support for Python 3.5.
+- Changed the hierarchy of base classes. Base classes no longer implement ``Serializable``, ``Serializable`` is now
+  directly implemented by most classes.
+- Removed TibiaData functionality.
+
+.. _v2.5.1:
+
+2.5.1 (2020-05-27)
+==================
+- Fixed bed count not being parsed on houses.
+
+.. _v2.5.0:
+
+2.5.0 (2020-05-22)
+==================
+- Added parsing of Tournaments and Tournament Leaderboards.
+- Fixed parsing errors with characters that had deaths by killers with "and" in their name.
+
+.. _v2.4.3:
+
+2.4.3 (2020-04-22)
+==================
+- Fixed an error when trying to parse a character with more deaths than what can be displayed in Tibia.com
+    - ``Character.deaths_truncated`` field was added to keep track of this case.
+
+.. _v2.4.2:
+
+2.4.2 (2020-02-26)
+==================
+- Fixed exception when attempting to parse highscores with no results (e.g. a new world on its first day).
+
+.. _v2.4.1:
+
+2.4.1 (2019-11-20)
+==================
+- Fixed incorrect argument name (house) in ``Character`` constructor.
+
+.. _v2.4.0:
+
+2.4.0 (2019-11-20)
+==================
+- Added support for multiple houses per character. Accessible on ``Character.houses`` field.
+- ``Character.house`` is now deprecated. It will contain the character's first house or ``None``.
+
+.. _v2.3.4:
+
+2.3.4 (2019-11-14)
+==================
+- Fixed bug with deaths not being parsed when a killer had ``and`` in their name.
+
+.. _v2.3.3:
+
+2.3.3 (2019-11-04)
+==================
+- Fixed bug with world parsing when there are more than 1000 players online.
+
+.. _v2.3.2:
+
+2.3.2 (2019-10-17)
+==================
+- Fixed incorrect highscores URL.
+
+.. _v2.3.1:
+
+2.3.1 (2019-10-06)
+==================
+- Fixed a bug with deaths not being parsed when a killer in assists had ``and`` in their name.
+
+.. _v2.3.0:
+
+2.3.0 (2019-09-16)
+==================
+- Added proxy option to client.
+
+.. _v2.2.6:
+
+2.2.6 (2019-09-01)
+==================
+- Fixed bug with account badges parsing failing when no badges were selected.
+
+.. _v2.2.5:
+
+2.2.5 (2019-08-22)
+==================
+
+- Fixed account badges parsing due to changes on the layout by CipSoft.
+
+.. _v2.2.4:
+
+2.2.4 (2019-08-20)
+==================
+
+- Disabled client compression for POST requests.
+
+.. _v2.2.3:
+
+2.2.3 (2019-08-17)
+==================
+
+- Enabled client side compression
+
+.. _v2.2.2:
+
+2.2.2 (2019-08-17)
+==================
+
+- Fixed killed by players and players kill stats being inverted for ``KillStatistics``
+
+.. _v2.2.1:
+
+2.2.1 (2019-08-10)
+==================
+
+- Fixed bug with character parsing failing when the guild rank is ``(member)``.
+
+.. _v2.2.0:
+
+2.2.0 (2019-08-08)
+==================
+
+- Added support for account badges and character titles.
+
+.. _v2.1.0:
+
+2.1.0 (2019-06-17)
+==================
+
+- Added ways to sort and filter House list results like in Tibia.com.
+- Added support to get the Boosted Creature of the day.
+
+.. _v2.0.1:
+
+2.0.1 (2019-06-04)
+==================
+
+- Replaced references to ``secure.tibia.com`` with ``www.tibia.com`` as the former always redirects to the front page.
+
+.. _v2.0.0:
+
+2.0.0 (2019-06-03)
+==================
+
+- Added asynchronous client to fetch and parse Tibia.com sections.
+- Added news parsing.
+- Added kill statistics parsing.
+- Added support for tournament worlds.
+- Added support for house prices with 'k' suffixes.
+
+.. _v1.1.3:
+
+1.1.3 (2019-01-29)
+==================
+
+- Fixed incorrect parsing of deaths with summons involved when parsing characters from TibiaData.
+
+.. _v1.1.2:
+
+1.1.2 (2019-01-22)
+==================
+
+- Fixed TibiaData URLs of tibia characters with special characters in their names. (e.g Himmelhüpferin)
+
+.. _v1.1.1:
+
+1.1.1 (2019-01-09)
+==================
+
+- Fixed character houses having attributes mixed up.
+
+.. _v1.1.0:
+
+1.1.0 (2019-01-09)
+==================
+
+- Parsing Highscores from Tibia.com and TibiaData.
+- Some strings from TibiaData had unpredictable trailing whitespaces,
+  all leading and trailing whitespaces are removed.
+- Added type hints to many variables and methods.
+
+.. _v1.0.0:
+
+1.0.0 (2018-12-23)
+==================
+
+-  Added support for TibiaData JSON parsing. To have interoperability
+   between Tibia.com and TibiaData.
+-  Added support for parsing Houses, House lists, World and World list
+-  Added support for many missing attributes in Character and Guilds.
+-  All objects are now serializable to JSON strings.
+
+.. _v0.1.0:
+
+0.1.0 (2018-08-17)
+==================
+
+Initial release:
+
+-  Parses content from tibia.com
+
+   -  Character pages
+   -  Guild pages
+   -  Guild list pages
+
+-  Parses content into JSON format strings.
+-  Parses content into Python objects.
```

### Comparing `tibia.py-5.6.1/LICENSE` & `tibia.py-6.0.0a1/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2018 Allan Galarza
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2018 Allan Galarza
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `tibia.py-5.6.1/PKG-INFO` & `tibia.py-6.0.0a1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,111 @@
-Metadata-Version: 2.1
-Name: tibia.py
-Version: 5.6.1
-Summary: API that parses website content into python data.
-Home-page: https://github.com/Galarzaa90/tibia.py
-Author: Galarzaa90
-Author-email: allan.galarza@gmail.com
-License: Apache 2.0
-Project-URL: GitHub: Repo, https://github.com/Galarzaa90/tibia.py
-Project-URL: GitHub: Issues, https://github.com/Galarzaa90/tibia.py/issues
-Project-URL: Docs: RTD, https://tibiapy.readthedocs.io/en/stable/
-Project-URL: Docs: Changelog, https://tibiapy.readthedocs.io/en/stable/changelog.html
-Project-URL: Coverage: Codecov, https://app.codecov.io/gh/Galarzaa90/tibia.py
-Project-URL: Docker Hub: Repo, https://hub.docker.com/repository/docker/galarzaa90/tibia.py
-Project-URL: SonarCloud, https://sonarcloud.io/dashboard?id=Galarzaa90_tibia.py
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Games/Entertainment :: Role-Playing
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Text Processing :: Markup :: HTML
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: test
-License-File: LICENSE
-
-# Tibia.py
-An API to parse Tibia.com content into object oriented data.
-
-No fetching is done by this module, you must provide the html content.
-
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Galarzaa90/tibia.py/build.yml)
-[![codecov](https://codecov.io/gh/Galarzaa90/tibia.py/branch/master/graph/badge.svg?token=mS9Wxv6O2F)](https://codecov.io/gh/Galarzaa90/tibia.py)
-[![PyPI](https://img.shields.io/pypi/v/tibia.py.svg)](https://pypi.python.org/pypi/tibia.py/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tibia.py.svg)
-![PyPI - License](https://img.shields.io/pypi/l/tibia.py.svg)
-
-
-**Features:**
-
-- Converts data into well-structured Python objects.
-- Type consistent attributes.
-- All objects can be converted to JSON strings.
-- Can be used with any networking library.
-- Support for characters, guilds, houses and worlds, tournaments, forums, etc.
-
-## Installing
-Install and update using pip
-
-```commandline
-pip install tibia.py
-```
-
-Installing the latest version form GitHub
-
-```commandline
-pip install git+https://github.com/Galarzaa90/tibia.py.git -U
-```
-
-## Usage
-This library is composed of two parts, parsers and an asynchronous request client.
-
-The asynchronous client (`tibiapy.Client`) contains methods to obtain information from Tibia.com.
-
-The parsing methods allow you to get Python objects given the html content of a page.
-
-```python
-import tibiapy
-
-# Asynchronously
-import aiohttp
-
-async def get_character(name):
-    url = tibiapy.Character.get_url(name)
-
-    async with aiohttp.ClientSession() as session:
-        async with session.get(url) as resp:
-            content = await resp.text()
-    character = tibiapy.Character.from_content(content)
-    return character
-
-# Synchronously
-import requests
-
-def get_character_sync(name):
-    url = tibiapy.Character.get_url(name)
-    
-    r = requests.get(url)
-    content = r.text
-    character = tibiapy.Character.from_content(content)
-    return character
-
-```
-
-## Documentation
-https://tibiapy.readthedocs.io/
+Metadata-Version: 2.1
+Name: tibia.py
+Version: 6.0.0a1
+Summary: API that parses website content into python data.
+Home-page: https://github.com/Galarzaa90/tibia.py
+Author: Galarzaa90
+Author-email: allan.galarza@gmail.com
+License: Apache 2.0
+Project-URL: GitHub: Repo, https://github.com/Galarzaa90/tibia.py
+Project-URL: GitHub: Issues, https://github.com/Galarzaa90/tibia.py/issues
+Project-URL: Docs: RTD, https://tibiapy.readthedocs.io/en/stable/
+Project-URL: Docs: Changelog, https://tibiapy.readthedocs.io/en/stable/changelog.html
+Project-URL: Coverage: Codecov, https://app.codecov.io/gh/Galarzaa90/tibia.py
+Project-URL: Docker Hub: Repo, https://hub.docker.com/repository/docker/galarzaa90/tibia.py
+Project-URL: SonarCloud, https://sonarcloud.io/dashboard?id=Galarzaa90_tibia.py
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Games/Entertainment :: Role-Playing
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Text Processing :: Markup :: HTML
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: server
+License-File: LICENSE
+
+# Tibia.py
+An API to parse Tibia.com content into object oriented data.
+
+No fetching is done by this module, you must provide the html content.
+
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Galarzaa90/tibia.py/build.yml)
+[![codecov](https://codecov.io/gh/Galarzaa90/tibia.py/branch/master/graph/badge.svg?token=mS9Wxv6O2F)](https://codecov.io/gh/Galarzaa90/tibia.py)
+[![PyPI](https://img.shields.io/pypi/v/tibia.py.svg)](https://pypi.python.org/pypi/tibia.py/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tibia.py.svg)
+![PyPI - License](https://img.shields.io/pypi/l/tibia.py.svg)
+
+
+**Features:**
+
+- Converts data into well-structured Python objects.
+- Type consistent attributes.
+- All objects can be converted to JSON strings.
+- Can be used with any networking library.
+- Support for characters, guilds, houses and worlds, tournaments, forums, etc.
+
+## Installing
+Install and update using pip
+
+```commandline
+pip install tibia.py
+```
+
+Installing the latest version form GitHub
+
+```commandline
+pip install git+https://github.com/Galarzaa90/tibia.py.git -U
+```
+
+## Usage
+This library is composed of two parts, parsers and an asynchronous request client.
+
+The asynchronous client (`tibiapy.Client`) contains methods to obtain information from Tibia.com.
+
+The parsing methods allow you to get Python objects given the html content of a page.
+
+```python
+import tibiapy
+
+# Asynchronously
+import aiohttp
+
+async def get_character(name):
+    url = tibiapy.urls.get_character_url(name)
+
+    async with aiohttp.ClientSession() as session:
+        async with session.get(url) as resp:
+            content = await resp.text()
+    character = tibiapy.Character.from_content(content)
+    return character
+
+# Synchronously
+import requests
+
+def get_character_sync(name):
+    url = tibiapy.urls.get_character_url(name)
+    
+    r = requests.get(url)
+    content = r.text
+    character = tibiapy.Character.from_content(content)
+    return character
+
+```
+
+## Documentation
+https://tibiapy.readthedocs.io/
+
+
```

### Comparing `tibia.py-5.6.1/README.md` & `tibia.py-6.0.0a1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-# Tibia.py
-An API to parse Tibia.com content into object oriented data.
-
-No fetching is done by this module, you must provide the html content.
-
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Galarzaa90/tibia.py/build.yml)
-[![codecov](https://codecov.io/gh/Galarzaa90/tibia.py/branch/master/graph/badge.svg?token=mS9Wxv6O2F)](https://codecov.io/gh/Galarzaa90/tibia.py)
-[![PyPI](https://img.shields.io/pypi/v/tibia.py.svg)](https://pypi.python.org/pypi/tibia.py/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tibia.py.svg)
-![PyPI - License](https://img.shields.io/pypi/l/tibia.py.svg)
-
-
-**Features:**
-
-- Converts data into well-structured Python objects.
-- Type consistent attributes.
-- All objects can be converted to JSON strings.
-- Can be used with any networking library.
-- Support for characters, guilds, houses and worlds, tournaments, forums, etc.
-
-## Installing
-Install and update using pip
-
-```commandline
-pip install tibia.py
-```
-
-Installing the latest version form GitHub
-
-```commandline
-pip install git+https://github.com/Galarzaa90/tibia.py.git -U
-```
-
-## Usage
-This library is composed of two parts, parsers and an asynchronous request client.
-
-The asynchronous client (`tibiapy.Client`) contains methods to obtain information from Tibia.com.
-
-The parsing methods allow you to get Python objects given the html content of a page.
-
-```python
-import tibiapy
-
-# Asynchronously
-import aiohttp
-
-async def get_character(name):
-    url = tibiapy.Character.get_url(name)
-
-    async with aiohttp.ClientSession() as session:
-        async with session.get(url) as resp:
-            content = await resp.text()
-    character = tibiapy.Character.from_content(content)
-    return character
-
-# Synchronously
-import requests
-
-def get_character_sync(name):
-    url = tibiapy.Character.get_url(name)
-    
-    r = requests.get(url)
-    content = r.text
-    character = tibiapy.Character.from_content(content)
-    return character
-
-```
-
-## Documentation
-https://tibiapy.readthedocs.io/
+# Tibia.py
+An API to parse Tibia.com content into object oriented data.
+
+No fetching is done by this module, you must provide the html content.
+
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Galarzaa90/tibia.py/build.yml)
+[![codecov](https://codecov.io/gh/Galarzaa90/tibia.py/branch/master/graph/badge.svg?token=mS9Wxv6O2F)](https://codecov.io/gh/Galarzaa90/tibia.py)
+[![PyPI](https://img.shields.io/pypi/v/tibia.py.svg)](https://pypi.python.org/pypi/tibia.py/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tibia.py.svg)
+![PyPI - License](https://img.shields.io/pypi/l/tibia.py.svg)
+
+
+**Features:**
+
+- Converts data into well-structured Python objects.
+- Type consistent attributes.
+- All objects can be converted to JSON strings.
+- Can be used with any networking library.
+- Support for characters, guilds, houses and worlds, tournaments, forums, etc.
+
+## Installing
+Install and update using pip
+
+```commandline
+pip install tibia.py
+```
+
+Installing the latest version form GitHub
+
+```commandline
+pip install git+https://github.com/Galarzaa90/tibia.py.git -U
+```
+
+## Usage
+This library is composed of two parts, parsers and an asynchronous request client.
+
+The asynchronous client (`tibiapy.Client`) contains methods to obtain information from Tibia.com.
+
+The parsing methods allow you to get Python objects given the html content of a page.
+
+```python
+import tibiapy
+
+# Asynchronously
+import aiohttp
+
+async def get_character(name):
+    url = tibiapy.urls.get_character_url(name)
+
+    async with aiohttp.ClientSession() as session:
+        async with session.get(url) as resp:
+            content = await resp.text()
+    character = tibiapy.Character.from_content(content)
+    return character
+
+# Synchronously
+import requests
+
+def get_character_sync(name):
+    url = tibiapy.urls.get_character_url(name)
+    
+    r = requests.get(url)
+    content = r.text
+    character = tibiapy.Character.from_content(content)
+    return character
+
+```
+
+## Documentation
+https://tibiapy.readthedocs.io/
```

### Comparing `tibia.py-5.6.1/setup.py` & `tibia.py-6.0.0a1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,95 +1,98 @@
-import os
-import re
-import sys
-
-from setuptools import find_packages, setup
-
-if sys.version_info < (3, 7):
-    sys.exit('Sorry, Python < 3.7 is not supported')
-
-
-def get_version(package):
-    """Return package version as listed in `__version__` in `init.py`."""
-    init_py = open(os.path.join(package, '__init__.py')).read()
-    return re.search("__version__ = ['\"]([^'\"]+)['\"]", init_py).group(1)
-
-
-version = get_version("tibiapy")
-if version.endswith(('a', 'b', 'rc')):
-    # append version identifier based on commit count
-    try:
-        import subprocess
-        p = subprocess.Popen(['git', 'rev-list', '--count', 'HEAD'],
-                             stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-        out, err = p.communicate()
-        if out:
-            version += out.decode('utf-8').strip()
-        p = subprocess.Popen(['git', 'rev-parse', '--short', 'HEAD'],
-                             stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-        out, err = p.communicate()
-        if out:
-            version += '+g' + out.decode('utf-8').strip()
-    except Exception:
-        pass
-
-with open('requirements.txt') as f:
-    requirements = f.read().splitlines()
-
-with open('README.md') as f:
-    readme = f.read()
-
-extras_require = {
-    'docs': [
-        'sphinx',
-    ],
-    'test': [
-        'asynctest',
-        'aioresponses',
-        'coverage',
-    ],
-}
-
-setup(
-    name='tibia.py',
-    version=version,
-    author='Galarzaa90',
-    author_email="allan.galarza@gmail.com",
-    url='https://github.com/Galarzaa90/tibia.py',
-    license='Apache 2.0',
-    install_requires=requirements,
-    extras_require=extras_require,
-    description="API that parses website content into python data.",
-    long_description=readme,
-    long_description_content_type="text/markdown",
-    packages=find_packages(),
-    include_package_data=True,
-    project_urls={
-        "GitHub: Repo": "https://github.com/Galarzaa90/tibia.py",
-        "GitHub: Issues": "https://github.com/Galarzaa90/tibia.py/issues",
-        "Docs: RTD": "https://tibiapy.readthedocs.io/en/stable/",
-        "Docs: Changelog": "https://tibiapy.readthedocs.io/en/stable/changelog.html",
-        "Coverage: Codecov": "https://app.codecov.io/gh/Galarzaa90/tibia.py",
-        "Docker Hub: Repo": "https://hub.docker.com/repository/docker/galarzaa90/tibia.py",
-        "SonarCloud": "https://sonarcloud.io/dashboard?id=Galarzaa90_tibia.py",
-    },
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: Apache Software License',
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Topic :: Games/Entertainment :: Role-Playing',
-        'Topic :: Internet',
-        'Topic :: Software Development',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Text Processing :: Markup :: HTML',
-        'Topic :: Utilities',
-        'Typing :: Typed',
-    ],
-)
+import os
+import re
+import sys
+
+from setuptools import find_packages, setup
+
+if sys.version_info < (3, 8):
+    sys.exit('Sorry, Python < 3.8 is not supported')
+
+
+def get_version(package):
+    """Return package version as listed in `__version__` in `init.py`."""
+    init_py = open(os.path.join(package, '__init__.py')).read()
+    return re.search("__version__ = ['\"]([^'\"]+)['\"]", init_py).group(1)
+
+
+version = get_version("tibiapy")
+if version.endswith(('a', 'b', 'rc')):
+    # append version identifier based on commit count
+    try:
+        import subprocess
+        p = subprocess.Popen(['git', 'rev-list', '--count', 'HEAD'],
+                             stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        out, err = p.communicate()
+        if out:
+            version += out.decode('utf-8').strip()
+        p = subprocess.Popen(['git', 'rev-parse', '--short', 'HEAD'],
+                             stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        out, err = p.communicate()
+        if out:
+            version += '+g' + out.decode('utf-8').strip()
+    except Exception:
+        pass
+
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
+
+with open('README.md') as f:
+    readme = f.read()
+
+extras_require = {
+    'docs': [
+        'sphinx',
+        'autodoc-pydantic',
+    ],
+    'test': [
+        'asynctest',
+        'aioresponses',
+        'coverage',
+    ],
+    'server': [
+        'fastapi'
+    ]
+}
+
+setup(
+    name='tibia.py',
+    version=version,
+    author='Galarzaa90',
+    author_email="allan.galarza@gmail.com",
+    url='https://github.com/Galarzaa90/tibia.py',
+    license='Apache 2.0',
+    install_requires=requirements,
+    extras_require=extras_require,
+    description="API that parses website content into python data.",
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    packages=find_packages(),
+    include_package_data=True,
+    project_urls={
+        "GitHub: Repo": "https://github.com/Galarzaa90/tibia.py",
+        "GitHub: Issues": "https://github.com/Galarzaa90/tibia.py/issues",
+        "Docs: RTD": "https://tibiapy.readthedocs.io/en/stable/",
+        "Docs: Changelog": "https://tibiapy.readthedocs.io/en/stable/changelog.html",
+        "Coverage: Codecov": "https://app.codecov.io/gh/Galarzaa90/tibia.py",
+        "Docker Hub: Repo": "https://hub.docker.com/repository/docker/galarzaa90/tibia.py",
+        "SonarCloud": "https://sonarcloud.io/dashboard?id=Galarzaa90_tibia.py",
+    },
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: Apache Software License',
+        'Natural Language :: English',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3 :: Only',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Topic :: Games/Entertainment :: Role-Playing',
+        'Topic :: Internet',
+        'Topic :: Software Development',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Text Processing :: Markup :: HTML',
+        'Topic :: Utilities',
+        'Typing :: Typed',
+    ],
+)
```

### Comparing `tibia.py-5.6.1/tests/integration.py` & `tibia.py-6.0.0a1/tests/integration.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import asyncio
-import datetime
-import logging
-import random
-
-import tibiapy
-
-console_handler = logging.StreamHandler()
-console_handler.setFormatter(logging.Formatter('[%(asctime)s][%(levelname)s] %(message)s'))
-
-log = logging.getLogger("tibia.py")
-log.setLevel(logging.INFO)
-log.addHandler(console_handler)
-
-
-async def main():
-    log.info("Initializing client")
-    client = tibiapy.Client()
-    try:
-        log.info("Fetching world list...")
-        response = await client.fetch_world_list()
-        assert isinstance(response, tibiapy.TibiaResponse)
-        assert isinstance(response.data, tibiapy.WorldOverview)
-        log.info(f"{len(response.data.worlds)} worlds found.")
-        assert isinstance(response.data.record_count, int)
-        assert response.data.record_count > 0
-        assert isinstance(response.data.record_date, datetime.datetime)
-
-        selected = random.choice(response.data.regular_worlds)
-        assert isinstance(selected, tibiapy.WorldEntry)
-        log.info(f"World {selected.name} selected: {selected.online_count} online | {selected.pvp_type}"
-                 f" | {selected.location}")
-        assert isinstance(selected.pvp_type, tibiapy.PvpType)
-        assert isinstance(selected.location, tibiapy.WorldLocation)
-        log.info("Fetching world...")
-        response = await client.fetch_world(selected.name)
-        assert isinstance(response.data, tibiapy.World)
-
-    finally:
-        await client.session.close()
-
-if __name__ == '__main__':
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(main())
+import asyncio
+import datetime
+import logging
+import random
+
+import tibiapy
+
+console_handler = logging.StreamHandler()
+console_handler.setFormatter(logging.Formatter('[%(asctime)s][%(levelname)s] %(message)s'))
+
+log = logging.getLogger("tibia.py")
+log.setLevel(logging.INFO)
+log.addHandler(console_handler)
+
+
+async def main():
+    log.info("Initializing client")
+    client = tibiapy.Client()
+    try:
+        log.info("Fetching world list...")
+        response = await client.fetch_world_overview()
+        assert isinstance(response, tibiapy.TibiaResponse)
+        assert isinstance(response.data, tibiapy.WorldOverview)
+        log.info(f"{len(response.data.worlds)} worlds found.")
+        assert isinstance(response.data.record_count, int)
+        assert response.data.record_count > 0
+        assert isinstance(response.data.record_date, datetime.datetime)
+
+        selected = random.choice(response.data.regular_worlds)
+        assert isinstance(selected, tibiapy.WorldEntry)
+        log.info(f"World {selected.name} selected: {selected.online_count} online | {selected.pvp_type}"
+                 f" | {selected.location}")
+        assert isinstance(selected.pvp_type, tibiapy.PvpType)
+        assert isinstance(selected.location, tibiapy.WorldLocation)
+        log.info("Fetching world...")
+        response = await client.fetch_world(selected.name)
+        assert isinstance(response.data, tibiapy.World)
+
+    finally:
+        await client.session.close()
+
+if __name__ == '__main__':
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(main())
```

### Comparing `tibia.py-5.6.1/tests/tests_bazaar.py` & `tibia.py-6.0.0a1/tests/tests_bazaar.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,285 +1,284 @@
-import datetime
-import unittest
-
-from tests.tests_tibiapy import TestCommons
-from tibiapy import Auction, AuctionOrder, AuctionOrderBy, AuctionSearchType, AuctionStatus, BattlEyeTypeFilter, \
-    BidType, \
-    CharacterBazaar, \
-    InvalidContent, PvpTypeFilter, \
-    Sex, SkillFilter, \
-    Vocation, VocationAuctionFilter
-
-FILE_BAZAAR_CURRENT_EMPTY = "bazaar/tibiacom_history_empty.txt"
-FILE_BAZAAR_CURRENT = "bazaar/tibiacom_current.txt"
-FILE_BAZAAR_CURRENT_ALL_FILTERS = "bazaar/tibiacom_current_all_filters.txt"
-FILE_BAZAAR_HISTORY = "bazaar/tibiacom_history.txt"
-FILE_AUCTION_FINISHED = "bazaar/tibiacom_auction_finished.txt"
-FILE_AUCTION_UPGRADED_ITEMS = "bazaar/tibiacom_auction_upgraded_items.txt"
-FILE_AUCTION_NOT_FOUND = "bazaar/tibiacom_auction_not_found.txt"
-
-
-class TestBazaar(TestCommons, unittest.TestCase):
-    def test_character_bazaar_from_content_current_no_filters_selected(self):
-        bazaar = CharacterBazaar.from_content(self.load_resource(FILE_BAZAAR_CURRENT))
-
-        self.assertIsNotNone(bazaar)
-        self.assertEqual(300, bazaar.page)
-        self.assertEqual(482, bazaar.total_pages)
-        self.assertEqual(12031, bazaar.results_count)
-        self.assertEqual(25, len(bazaar.entries))
-        self.assertIsNotNone(bazaar.url)
-
-        auction = bazaar.entries[0]
-        self.assertEqual(30237, auction.auction_id)
-        self.assertEqual(800, auction.bid)
-        self.assertEqual(BidType.MINIMUM, auction.bid_type)
-        self.assertIsNotNone(auction.character_url)
-        self.assertEqual(0, len(auction.displayed_items))
-
-        self.assertIsNotNone(bazaar.filters)
-        self.assertIsNone(bazaar.filters.world)
-        self.assertIsNone(bazaar.filters.pvp_type)
-        self.assertIsNone(bazaar.filters.battleye)
-        self.assertIsNone(bazaar.filters.vocation)
-        self.assertIsNone(bazaar.filters.min_level)
-        self.assertIsNone(bazaar.filters.max_level)
-        self.assertIsNone(bazaar.filters.skill)
-        self.assertIsNone(bazaar.filters.min_skill_level)
-        self.assertIsNone(bazaar.filters.max_skill_level)
-        self.assertEqual(AuctionOrder.LOWEST_EARLIEST, bazaar.filters.order)
-
-    def test_character_bazaar_from_content_current_all_filters_selected(self):
-        bazaar = CharacterBazaar.from_content(self.load_resource(FILE_BAZAAR_CURRENT_ALL_FILTERS))
-
-        self.assertIsNotNone(bazaar)
-        self.assertEqual(1, bazaar.page)
-        self.assertEqual(4, bazaar.total_pages)
-        self.assertEqual(92, bazaar.results_count)
-        self.assertEqual(25, len(bazaar.entries))
-        self.assertIsNotNone(bazaar.url)
-
-        auction = bazaar.entries[0]
-        self.assertEqual(82526, auction.auction_id)
-        self.assertEqual(57000, auction.bid)
-        self.assertEqual(BidType.MINIMUM, auction.bid_type)
-        self.assertIsNotNone(auction.character_url)
-
-        self.assertIsNotNone(bazaar.filters)
-        self.assertEqual('Antica', bazaar.filters.world)
-        self.assertEqual(PvpTypeFilter.OPEN_PVP, bazaar.filters.pvp_type)
-        self.assertEqual(BattlEyeTypeFilter.PROTECTED, bazaar.filters.battleye)
-        self.assertEqual(VocationAuctionFilter.KNIGHT, bazaar.filters.vocation)
-        self.assertEqual(1, bazaar.filters.min_level)
-        self.assertEqual(1000, bazaar.filters.max_level)
-        self.assertEqual(SkillFilter.MAGIC_LEVEL, bazaar.filters.skill)
-        self.assertEqual(1, bazaar.filters.min_skill_level)
-        self.assertEqual(50, bazaar.filters.max_skill_level)
-        self.assertEqual(AuctionOrderBy.SHIELDING, bazaar.filters.order_by)
-        self.assertEqual(AuctionOrder.HIGHEST_LATEST, bazaar.filters.order)
-        self.assertEqual(AuctionSearchType.ITEM_WILDCARD, bazaar.filters.search_type)
-
-    def test_character_bazaar_from_content_empty(self):
-        bazaar = CharacterBazaar.from_content(self.load_resource(FILE_BAZAAR_CURRENT_EMPTY))
-        self.assertIsNotNone(bazaar)
-        self.assertFalse(bazaar.entries)
-
-    def test_character_bazaar_from_content_history(self):
-        bazaar = CharacterBazaar.from_content(self.load_resource(FILE_BAZAAR_HISTORY))
-
-        self.assertIsNotNone(bazaar)
-        self.assertEqual(1, bazaar.page)
-        self.assertEqual(1449, bazaar.total_pages)
-        self.assertEqual(36219, bazaar.results_count)
-        self.assertEqual(25, len(bazaar.entries))
-        self.assertIsNotNone(bazaar.url)
-
-        auction = bazaar.entries[0]
-        self.assertEqual(325058, auction.auction_id)
-        self.assertEqual(900, auction.bid)
-        self.assertEqual("Rcrazy Illuminati", auction.name)
-        self.assertEqual(255, auction.level)
-        self.assertEqual("Celebra", auction.world)
-        self.assertEqual(Vocation.MASTER_SORCERER, auction.vocation)
-        self.assertEqual(Sex.MALE, auction.sex)
-        self.assertEqual(BidType.WINNING, auction.bid_type)
-        self.assertIsNotNone(auction.character_url)
-        self.assertEqual(1, len(auction.displayed_items))
-        self.assertEqual(143, auction.outfit.outfit_id)
-
-        first_item = auction.displayed_items[0]
-        self.assertEqual(1, first_item.count)
-        self.assertEqual(25700, first_item.item_id)
-        self.assertEqual("dream blossom staff", first_item.name)
-        self.assertIsNotNone(first_item.image_url)
-
-        self.assertIsNone(bazaar.filters)
-
-    def test_character_bazaar_from_content_unrelated(self):
-        """Testing parsing an unrelated tibia.com section"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(InvalidContent):
-            CharacterBazaar.from_content(content)
-
-    def test_auction_details_from_content_finished(self):
-        auction = Auction.from_content(self.load_resource(FILE_AUCTION_FINISHED))
-
-        self.assertIsNotNone(auction)
-
-        # Listing box
-        self.assertEqual("Vireloz", auction.name)
-        self.assertIn(auction.name, auction.character_url)
-        self.assertIn(str(auction.auction_id), auction.url)
-        self.assertEqual(1161, auction.level)
-        self.assertEqual(Vocation.ROYAL_PALADIN, auction.vocation)
-        self.assertEqual(Sex.MALE, auction.sex)
-        self.assertEqual("Wintera", auction.world)
-        self.assertIsNotNone(auction.outfit)
-        self.assertEqual(1322, auction.outfit.outfit_id)
-        self.assertEqual(4, len(auction.displayed_items))
-        self.assertEqual("gnome armor", auction.displayed_items[0].name)
-        self.assertEqual("falcon coif", auction.displayed_items[1].name)
-        self.assertEqual("pair of soulstalkers", auction.displayed_items[2].name)
-        self.assertEqual("lion spangenhelm", auction.displayed_items[3].name)
-
-        self.assertEqual(330000, auction.bid)
-        self.assertEqual(BidType.MINIMUM, auction.bid_type)
-        self.assertEqual(AuctionStatus.FINISHED, auction.status)
-
-        self.assertEqual(11715, auction.hit_points)
-        self.assertEqual(17385, auction.mana)
-        self.assertEqual(23530, auction.capacity)
-        self.assertEqual(1270, auction.speed)
-        self.assertEqual(0, auction.blessings_count)
-        self.assertEqual(23, auction.mounts_count)
-        self.assertEqual(35, auction.outfits_count)
-        self.assertEqual(16, auction.titles_count)
-
-        self.assertEqual(8, len(auction.skills))
-        self.assertEqual(128, auction.skills_map["Distance Fighting"].level)
-        self.assertEqual(11.43, auction.skills_map["Distance Fighting"].progress)
-
-        self.assertIsInstance(auction.creation_date, datetime.datetime)
-        self.assertEqual(26006721711, auction.experience)
-        self.assertEqual(41893, auction.gold)
-        self.assertEqual(553, auction.achievement_points)
-        self.assertIsNone(auction.regular_world_transfer_available_date)
-        self.assertEqual(110, auction.available_charm_points)
-        self.assertEqual(5800, auction.spent_charm_points)
-
-        self.assertEqual(2, auction.daily_reward_streak)
-        self.assertEqual(1494, auction.hunting_task_points)
-        self.assertEqual(0, auction.permanent_hunting_task_slots)
-        self.assertEqual(1, auction.permanent_prey_slots)
-        self.assertEqual(1, auction.hirelings)
-        self.assertEqual(3, auction.hireling_jobs)
-        self.assertEqual(0, auction.hireling_outfits)
-
-        self.assertIsNotNone(auction.items)
-        self.assertEqual(76, len(auction.items.entries))
-        self.assertEqual(8, auction.items.total_pages)
-        self.assertEqual(567, auction.items.results)
-        self.assertEqual(141, auction.items.get_by_name("cigar").item_id)
-        self.assertEqual("cigar", auction.items.get_by_id(141).name)
-        self.assertEqual(7, len(auction.items.search('backpack')))
-
-        self.assertIsNotNone(auction.store_items)
-        self.assertEqual(16, len(auction.store_items.entries))
-        self.assertEqual(1, auction.store_items.total_pages)
-        self.assertEqual(16, auction.store_items.results)
-        self.assertEqual(23721, auction.store_items.get_by_name("gold pouch").item_id)
-        self.assertEqual("gold pouch", auction.store_items.get_by_id(23721).name)
-        self.assertEqual(2, len(auction.store_items.search('rune')))
-
-        self.assertIsNotNone(auction.mounts)
-        self.assertEqual(22, len(auction.mounts.entries))
-        self.assertEqual(1, auction.mounts.total_pages)
-        self.assertEqual(22, auction.mounts.results)
-        self.assertEqual(387, auction.mounts.get_by_name("donkey").mount_id)
-        self.assertEqual("Donkey", auction.mounts.get_by_id(387).name)
-        self.assertEqual(1, len(auction.mounts.search('drag')))
-
-        self.assertIsNotNone(auction.store_mounts)
-        self.assertEqual(1, len(auction.store_mounts.entries))
-        self.assertEqual(1, auction.store_mounts.total_pages)
-        self.assertEqual(1, auction.store_mounts.results)
-        self.assertEqual(906, auction.store_mounts.get_by_name("Wolpertinger").mount_id)
-        self.assertEqual("Wolpertinger", auction.store_mounts.get_by_id(906).name)
-        self.assertEqual(1, len(auction.store_mounts.search('Wolpertinger')))
-
-        self.assertIsNotNone(auction.outfits)
-        self.assertEqual(30, len(auction.outfits.entries))
-        self.assertEqual(2, auction.outfits.total_pages)
-        self.assertEqual(33, auction.outfits.results)
-        self.assertEqual(151, auction.outfits.get_by_name("pirate").outfit_id)
-        self.assertEqual('Glooth Engineer', auction.outfits.get_by_id(610).name)
-        self.assertEqual(2, len(auction.outfits.search('demon')))
-
-        self.assertIsNotNone(auction.store_outfits)
-        self.assertEqual(2, len(auction.store_outfits.entries))
-        self.assertEqual(1, auction.store_outfits.total_pages)
-        self.assertEqual(2, auction.store_outfits.results)
-        self.assertEqual(962, auction.store_outfits.get_by_name("retro warrior").outfit_id)
-        self.assertEqual('Retro Warrior', auction.store_outfits.get_by_id(962).name)
-        self.assertEqual(2, len(auction.store_outfits.search('retro')))
-
-        self.assertIsNotNone(auction.familiars)
-        self.assertEqual(1, len(auction.familiars.entries))
-        self.assertEqual(1, auction.familiars.total_pages)
-        self.assertEqual(1, auction.familiars.results)
-        self.assertEqual(992, auction.familiars.get_by_name("emberwing").familiar_id)
-        self.assertEqual('Emberwing', auction.familiars.get_by_id(992).name)
-        self.assertEqual(1, len(auction.familiars.search('ember')))
-
-        self.assertEqual(9, len(auction.blessings))
-        self.assertEqual(18, len(auction.imbuements))
-        self.assertEqual(8, len(auction.charms))
-        self.assertEqual(0, len(auction.completed_cyclopedia_map_areas))
-        self.assertEqual(16, len(auction.titles))
-        self.assertEqual(217, len(auction.achievements))
-        self.assertEqual(509, len(auction.bestiary_progress))
-        self.assertEqual(205, len(auction.completed_bestiary_entries))
-
-    def test_auction_details_from_content_finished_skip_details(self):
-        auction = Auction.from_content(self.load_resource(FILE_AUCTION_FINISHED), skip_details=True)
-
-        self.assertIsNotNone(auction)
-
-        # Listing box
-        self.assertEqual("Vireloz", auction.name)
-        self.assertIn(auction.name, auction.character_url)
-        self.assertIn(str(auction.auction_id), auction.url)
-        self.assertEqual(1161, auction.level)
-        self.assertEqual(Vocation.ROYAL_PALADIN, auction.vocation)
-        self.assertEqual(Sex.MALE, auction.sex)
-        self.assertEqual("Wintera", auction.world)
-        self.assertIsNotNone(auction.outfit)
-        self.assertEqual(1322, auction.outfit.outfit_id)
-        self.assertEqual(4, len(auction.displayed_items))
-        self.assertEqual("gnome armor", auction.displayed_items[0].name)
-        self.assertEqual("falcon coif", auction.displayed_items[1].name)
-        self.assertEqual("pair of soulstalkers", auction.displayed_items[2].name)
-        self.assertEqual("lion spangenhelm", auction.displayed_items[3].name)
-
-        self.assertEqual(330000, auction.bid)
-        self.assertEqual(BidType.MINIMUM, auction.bid_type)
-        self.assertEqual(AuctionStatus.FINISHED, auction.status)
-
-    def test_auction_details_from_content_with_upgraded_items(self):
-        auction = Auction.from_content(self.load_resource(FILE_AUCTION_UPGRADED_ITEMS))
-
-        self.assertIsNotNone(auction)
-
-        self.assertEqual(1, auction.displayed_items[0].tier)
-        self.assertEqual(1, auction.items.entries[1].tier)
-
-
-    def test_auction_details_from_content_not_found(self):
-        auction = Auction.from_content(self.load_resource(FILE_AUCTION_NOT_FOUND))
-
-        self.assertIsNone(auction)
-
-    def test_auction_details_from_content_unrelated(self):
-        """Testing parsing an unrelated tibia.com section"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(InvalidContent):
-            Auction.from_content(content)
+import datetime
+import unittest
+
+from tests.tests_tibiapy import TestCommons
+from tibiapy import AuctionOrderDirection, AuctionOrderBy, AuctionSearchType, AuctionStatus, AuctionBattlEyeFilter, \
+    BidType, \
+ \
+    InvalidContent, PvpTypeFilter, \
+    Sex, AuctionSkillFilter, \
+    Vocation, AuctionVocationFilter
+from tibiapy.parsers.bazaar import CharacterBazaarParser, AuctionParser
+
+FILE_BAZAAR_CURRENT_EMPTY = "bazaar/tibiacom_history_empty.txt"
+FILE_BAZAAR_CURRENT = "bazaar/tibiacom_current.txt"
+FILE_BAZAAR_CURRENT_ALL_FILTERS = "bazaar/tibiacom_current_all_filters.txt"
+FILE_BAZAAR_HISTORY = "bazaar/tibiacom_history.txt"
+FILE_AUCTION_FINISHED = "bazaar/tibiacom_auction_finished.txt"
+FILE_AUCTION_UPGRADED_ITEMS = "bazaar/tibiacom_auction_upgraded_items.txt"
+FILE_AUCTION_NOT_FOUND = "bazaar/tibiacom_auction_not_found.txt"
+
+
+class TestBazaar(TestCommons, unittest.TestCase):
+    def test_character_bazaar_from_content_current_no_filters_selected(self):
+        bazaar = CharacterBazaarParser.from_content(self.load_resource(FILE_BAZAAR_CURRENT))
+
+        self.assertIsNotNone(bazaar)
+        self.assertEqual(300, bazaar.current_page)
+        self.assertEqual(482, bazaar.total_pages)
+        self.assertEqual(12031, bazaar.results_count)
+        self.assertEqual(25, len(bazaar.entries))
+        self.assertIsNotNone(bazaar.url)
+
+        auction = bazaar.entries[0]
+        self.assertEqual(30237, auction.auction_id)
+        self.assertEqual(800, auction.bid)
+        self.assertEqual(BidType.MINIMUM, auction.bid_type)
+        self.assertIsNotNone(auction.character_url)
+        self.assertEqual(0, len(auction.displayed_items))
+
+        self.assertIsNotNone(bazaar.filters)
+        self.assertIsNone(bazaar.filters.world)
+        self.assertIsNone(bazaar.filters.pvp_type)
+        self.assertIsNone(bazaar.filters.battleye)
+        self.assertIsNone(bazaar.filters.vocation)
+        self.assertIsNone(bazaar.filters.min_level)
+        self.assertIsNone(bazaar.filters.max_level)
+        self.assertIsNone(bazaar.filters.skill)
+        self.assertIsNone(bazaar.filters.min_skill_level)
+        self.assertIsNone(bazaar.filters.max_skill_level)
+        self.assertEqual(AuctionOrderDirection.LOWEST_EARLIEST, bazaar.filters.order)
+
+    def test_character_bazaar_from_content_current_all_filters_selected(self):
+        bazaar = CharacterBazaarParser.from_content(self.load_resource(FILE_BAZAAR_CURRENT_ALL_FILTERS))
+
+        self.assertIsNotNone(bazaar)
+        self.assertEqual(1, bazaar.current_page)
+        self.assertEqual(4, bazaar.total_pages)
+        self.assertEqual(92, bazaar.results_count)
+        self.assertEqual(25, len(bazaar.entries))
+        self.assertIsNotNone(bazaar.url)
+
+        auction = bazaar.entries[0]
+        self.assertEqual(82526, auction.auction_id)
+        self.assertEqual(57000, auction.bid)
+        self.assertEqual(BidType.MINIMUM, auction.bid_type)
+        self.assertIsNotNone(auction.character_url)
+
+        self.assertIsNotNone(bazaar.filters)
+        self.assertEqual('Antica', bazaar.filters.world)
+        self.assertEqual(PvpTypeFilter.OPEN_PVP, bazaar.filters.pvp_type)
+        self.assertEqual(AuctionBattlEyeFilter.PROTECTED, bazaar.filters.battleye)
+        self.assertEqual(AuctionVocationFilter.KNIGHT, bazaar.filters.vocation)
+        self.assertEqual(1, bazaar.filters.min_level)
+        self.assertEqual(1000, bazaar.filters.max_level)
+        self.assertEqual(AuctionSkillFilter.MAGIC_LEVEL, bazaar.filters.skill)
+        self.assertEqual(1, bazaar.filters.min_skill_level)
+        self.assertEqual(50, bazaar.filters.max_skill_level)
+        self.assertEqual(AuctionOrderBy.SHIELDING, bazaar.filters.order_by)
+        self.assertEqual(AuctionOrderDirection.HIGHEST_LATEST, bazaar.filters.order)
+        self.assertEqual(AuctionSearchType.ITEM_WILDCARD, bazaar.filters.search_type)
+
+    def test_character_bazaar_from_content_empty(self):
+        bazaar = CharacterBazaarParser.from_content(self.load_resource(FILE_BAZAAR_CURRENT_EMPTY))
+        self.assertIsNotNone(bazaar)
+        self.assertFalse(bazaar.entries)
+
+    def test_character_bazaar_from_content_history(self):
+        bazaar = CharacterBazaarParser.from_content(self.load_resource(FILE_BAZAAR_HISTORY))
+
+        self.assertIsNotNone(bazaar)
+        self.assertEqual(1, bazaar.current_page)
+        self.assertEqual(1449, bazaar.total_pages)
+        self.assertEqual(36219, bazaar.results_count)
+        self.assertEqual(25, len(bazaar.entries))
+        self.assertIsNotNone(bazaar.url)
+
+        auction = bazaar.entries[0]
+        self.assertEqual(325058, auction.auction_id)
+        self.assertEqual(900, auction.bid)
+        self.assertEqual("Rcrazy Illuminati", auction.name)
+        self.assertEqual(255, auction.level)
+        self.assertEqual("Celebra", auction.world)
+        self.assertEqual(Vocation.MASTER_SORCERER, auction.vocation)
+        self.assertEqual(Sex.MALE, auction.sex)
+        self.assertEqual(BidType.WINNING, auction.bid_type)
+        self.assertIsNotNone(auction.character_url)
+        self.assertEqual(1, len(auction.displayed_items))
+        self.assertEqual(143, auction.outfit.outfit_id)
+
+        first_item = auction.displayed_items[0]
+        self.assertEqual(1, first_item.count)
+        self.assertEqual(25700, first_item.item_id)
+        self.assertEqual("dream blossom staff", first_item.name)
+        self.assertIsNotNone(first_item.image_url)
+
+        self.assertIsNone(bazaar.filters)
+
+    def test_character_bazaar_from_content_unrelated(self):
+        """Testing parsing an unrelated tibia.com section"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(InvalidContent):
+            CharacterBazaarParser.from_content(content)
+
+    def test_auction_details_from_content_finished(self):
+        auction = AuctionParser.from_content(self.load_resource(FILE_AUCTION_FINISHED))
+
+        self.assertIsNotNone(auction)
+
+        # Listing box
+        self.assertEqual("Hikeezor", auction.name)
+        self.assertIn(auction.name, auction.character_url)
+        self.assertIn(str(auction.auction_id), auction.url)
+        self.assertEqual(1496, auction.level)
+        self.assertEqual(Vocation.ELDER_DRUID, auction.vocation)
+        self.assertEqual(Sex.MALE, auction.sex)
+        self.assertEqual("Astera", auction.world)
+        self.assertIsNotNone(auction.outfit)
+        self.assertEqual(130, auction.outfit.outfit_id)
+        self.assertEqual(2, len(auction.displayed_items))
+        self.assertEqual("lasting exercise rod", auction.displayed_items[0].name)
+        self.assertEqual("lasting exercise wand", auction.displayed_items[1].name)
+
+        self.assertEqual(230000, auction.bid)
+        self.assertEqual(BidType.MINIMUM, auction.bid_type)
+        self.assertEqual(AuctionStatus.FINISHED, auction.status)
+
+        self.assertEqual(7625, auction.details.hit_points)
+        self.assertEqual(44730, auction.details.mana)
+        self.assertEqual(15350, auction.details.capacity)
+        self.assertEqual(1605, auction.details.speed)
+        self.assertEqual(0, auction.details.blessings_count)
+        self.assertEqual(65, auction.details.mounts_count)
+        self.assertEqual(51, auction.details.outfits_count)
+        self.assertEqual(36, auction.details.titles_count)
+
+        self.assertEqual(8, len(auction.details.skills))
+        self.assertEqual(21, auction.details.skills_map["Distance Fighting"].level)
+        self.assertEqual(16.37, auction.details.skills_map["Distance Fighting"].progress)
+
+        self.assertIsInstance(auction.details.creation_date, datetime.datetime)
+        self.assertEqual(55611897119, auction.details.experience)
+        self.assertEqual(1000, auction.details.gold)
+        self.assertEqual(1147, auction.details.achievement_points)
+        self.assertIsNone(auction.details.regular_world_transfer_available_date)
+        self.assertEqual(5110, auction.details.available_charm_points)
+        self.assertEqual(13600, auction.details.spent_charm_points)
+
+        self.assertEqual(935, auction.details.daily_reward_streak)
+        self.assertEqual(64304, auction.details.hunting_task_points)
+        self.assertEqual(1, auction.details.permanent_hunting_task_slots)
+        self.assertEqual(1, auction.details.permanent_prey_slots)
+        self.assertEqual(2, auction.details.hirelings)
+        self.assertEqual(4, auction.details.hireling_jobs)
+        self.assertEqual(1, auction.details.hireling_outfits)
+
+        self.assertIsNotNone(auction.details.items)
+        self.assertEqual(5, len(auction.details.items.entries))
+        self.assertEqual(1, auction.details.items.total_pages)
+        self.assertEqual(5, auction.details.items.results_count)
+        self.assertEqual(3507, auction.details.items.get_by_name("label").item_id)
+        self.assertEqual("brocade backpack", auction.details.items.get_by_id(8860).name)
+        self.assertEqual(1, len(auction.details.items.search('parcel')))
+
+        self.assertIsNotNone(auction.details.store_items)
+        self.assertEqual(30, len(auction.details.store_items.entries))
+        self.assertEqual(1, auction.details.store_items.total_pages)
+        self.assertEqual(30, auction.details.store_items.results_count)
+        self.assertEqual(32917, auction.details.store_items.get_by_name("gold deed").item_id)
+        self.assertEqual("podium of vigour", auction.details.store_items.get_by_id(38707).name)
+        self.assertEqual(5, len(auction.details.store_items.search('plushie')))
+
+        self.assertIsNotNone(auction.details.mounts)
+        self.assertEqual(30, len(auction.details.mounts.entries))
+        self.assertEqual(3, auction.details.mounts.total_pages)
+        self.assertEqual(61, auction.details.mounts.results_count)
+        self.assertEqual(387, auction.details.mounts.get_by_name("donkey").mount_id)
+        self.assertEqual("Donkey", auction.details.mounts.get_by_id(387).name)
+        self.assertEqual(1, len(auction.details.mounts.search('drag')))
+
+        self.assertIsNotNone(auction.details.store_mounts)
+        self.assertEqual(4, len(auction.details.store_mounts.entries))
+        self.assertEqual(1, auction.details.store_mounts.total_pages)
+        self.assertEqual(4, auction.details.store_mounts.results_count)
+        self.assertEqual(427, auction.details.store_mounts.get_by_name("shadow draptor").mount_id)
+        self.assertEqual("Shadow Draptor", auction.details.store_mounts.get_by_id(427).name)
+        self.assertEqual(1, len(auction.details.store_mounts.search('shadow')))
+
+        self.assertIsNotNone(auction.details.outfits)
+        self.assertEqual(30, len(auction.details.outfits.entries))
+        self.assertEqual(2, auction.details.outfits.total_pages)
+        self.assertEqual(50, auction.details.outfits.results_count)
+        self.assertEqual(153, auction.details.outfits.get_by_name("beggar").outfit_id)
+        self.assertEqual('Beggar', auction.details.outfits.get_by_id(153).name)
+        self.assertEqual(2, len(auction.details.outfits.search('demon')))
+
+        self.assertIsNotNone(auction.details.store_outfits)
+        self.assertEqual(1, len(auction.details.store_outfits.entries))
+        self.assertEqual(1, auction.details.store_outfits.total_pages)
+        self.assertEqual(1, auction.details.store_outfits.results_count)
+        self.assertEqual(1202, auction.details.store_outfits.get_by_name("void master").outfit_id)
+        self.assertEqual('Void Master', auction.details.store_outfits.get_by_id(1202).name)
+        self.assertEqual(1, len(auction.details.store_outfits.search('void')))
+
+        self.assertIsNotNone(auction.details.familiars)
+        self.assertEqual(2, len(auction.details.familiars.entries))
+        self.assertEqual(1, auction.details.familiars.total_pages)
+        self.assertEqual(2, auction.details.familiars.results_count)
+        self.assertEqual(993, auction.details.familiars.get_by_name("grovebeast").familiar_id)
+        self.assertEqual('Grovebeast', auction.details.familiars.get_by_id(993).name)
+        self.assertEqual(1, len(auction.details.familiars.search('grove')))
+
+        self.assertEqual(9, len(auction.details.blessings))
+        self.assertEqual(23, len(auction.details.imbuements))
+        self.assertEqual(15, len(auction.details.charms))
+        self.assertEqual(19, len(auction.details.completed_cyclopedia_map_areas))
+        self.assertEqual(36, len(auction.details.titles))
+        self.assertEqual(451, len(auction.details.achievements))
+        self.assertEqual(702, len(auction.details.bestiary_progress))
+        self.assertEqual(637, len(auction.details.completed_bestiary_entries))
+
+    def _test_auction_details_from_content_finished_skip_details(self):
+        auction = AuctionParser.from_content(self.load_resource(FILE_AUCTION_FINISHED), skip_details=True)
+
+        self.assertIsNotNone(auction)
+
+        # Listing box
+        self.assertEqual("Vireloz", auction.name)
+        self.assertIn(auction.name, auction.character_url)
+        self.assertIn(str(auction.auction_id), auction.url)
+        self.assertEqual(1161, auction.level)
+        self.assertEqual(Vocation.ROYAL_PALADIN, auction.vocation)
+        self.assertEqual(Sex.MALE, auction.sex)
+        self.assertEqual("Wintera", auction.world)
+        self.assertIsNotNone(auction.outfit)
+        self.assertEqual(1322, auction.outfit.outfit_id)
+        self.assertEqual(4, len(auction.displayed_items))
+        self.assertEqual("gnome armor", auction.displayed_items[0].name)
+        self.assertEqual("falcon coif", auction.displayed_items[1].name)
+        self.assertEqual("pair of soulstalkers", auction.displayed_items[2].name)
+        self.assertEqual("lion spangenhelm", auction.displayed_items[3].name)
+
+        self.assertEqual(330000, auction.bid)
+        self.assertEqual(BidType.MINIMUM, auction.bid_type)
+        self.assertEqual(AuctionStatus.FINISHED, auction.status)
+
+    def _test_auction_details_from_content_with_upgraded_items(self):
+        auction = AuctionParser.from_content(self.load_resource(FILE_AUCTION_UPGRADED_ITEMS))
+
+        self.assertIsNotNone(auction)
+
+        self.assertEqual(1, auction.displayed_items[0].tier)
+        self.assertEqual(1, auction.items.entries[1].tier)
+
+
+    def test_auction_details_from_content_not_found(self):
+        auction = AuctionParser.from_content(self.load_resource(FILE_AUCTION_NOT_FOUND))
+
+        self.assertIsNone(auction)
+
+    def test_auction_details_from_content_unrelated(self):
+        """Testing parsing an unrelated tibia.com section"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(InvalidContent):
+            AuctionParser.from_content(content)
```

### Comparing `tibia.py-5.6.1/tests/tests_character.py` & `tibia.py-6.0.0a1/tests/tests_character.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,192 +1,205 @@
-import datetime
-import unittest
-
-from tests.tests_tibiapy import TestCommons
-from tibiapy import AccountBadge, Character, CharacterHouse, Death, InvalidContent, Killer
-from tibiapy.enums import AccountStatus, Sex, Vocation
-from tibiapy.utils import parse_tibia_datetime
-
-FILE_CHARACTER_RESOURCE = "character/tibiacom_full.txt"
-FILE_CHARACTER_NOT_FOUND = "character/tibiacom_not_found.txt"
-FILE_CHARACTER_FORMER_NAMES = "character/tibiacom_former_names.txt"
-FILE_CHARACTER_SPECIAL_POSITION = "character/tibiacom_special_position.txt"
-FILE_CHARACTER_DELETION = "character/tibiacom_deletion.txt"
-FILE_CHARACTER_DEATHS_COMPLEX = "character/tibiacom_deaths_complex.txt"
-FILE_CHARACTER_TITLE_BADGES = "character/tibiacom_title_badges.txt"
-FILE_CHARACTER_NO_BADGES_SELECTED = "character/tibiacom_no_badges_selected.txt"
-FILE_CHARACTER_MULTIPLE_HOUSES = "character/tibiacom_multiple_houses.txt"
-FILE_CHARACTER_TRUNCATED_DEATHS = "character/tibiacom_truncated_deaths.txt"
-
-
-class TestCharacter(TestCommons, unittest.TestCase):
-    def _compare_character(self, mock_character, character):
-        self.assertEqual(mock_character.name, character.name)
-        self.assertEqual(mock_character.world, character.world)
-        self.assertEqual(mock_character.vocation, character.vocation)
-        self.assertEqual(mock_character.level, character.level)
-        self.assertEqual(mock_character.sex, character.sex)
-
-    # region Tibia.com Character Tests
-    def test_character_from_content(self):
-        """Testing parsing a character's HTML content"""
-        character = Character.from_content(self.load_resource(FILE_CHARACTER_RESOURCE))
-        self._compare_character(Character("Tschas", "Gladera", Vocation.ELDER_DRUID, 522, Sex.FEMALE), character)
-        self.assertIsNotNone(character.guild_membership)
-        self.assertEqual("Bald Dwarfs", character.guild_membership.name)
-        self.assertEqual("Emperor", character.guild_membership.rank)
-        self.assertIsNotNone(character.guild_url)
-        self.assertIsNone(character.married_to_url)
-        self.assertEqual(character.guild_name, character.guild_membership.name)
-        self.assertEqual(character.guild_rank, character.guild_membership.rank)
-        self.assertEqual(AccountStatus.PREMIUM_ACCOUNT, character.account_status)
-        self.assertEqual(304, character.achievement_points)
-        self.assertIsNone(character.deletion_date)
-        self.assertIsNotNone(character.deaths)
-        self.assertEqual(2, character.deaths.__len__())
-        self.assertEqual(parse_tibia_datetime("Aug 02 2021, 17:32:07 CEST"), character.last_login)
-        self.assertEqual(character.url, Character.get_url(character.name))
-        self.assertEqual(5, len(character.other_characters))
-        self.assertFalse(character.hidden)
-
-        # Badges
-        self.assertEqual(3, len(character.account_badges))
-        badge = character.account_badges[0]
-        self.assertEqual("Ancient Hero", badge.name)
-        self.assertEqual("The account is older than 15 years.", badge.description)
-
-    def test_character_from_content_not_found(self):
-        """Testing parsing a character not found page"""
-        content = self.load_resource(FILE_CHARACTER_NOT_FOUND)
-        char = Character.from_content(content)
-        self.assertIsNone(char)
-
-    def test_character_from_content_with_former_names(self):
-        """Testing parsing a character that has former names"""
-        content = self.load_resource(FILE_CHARACTER_FORMER_NAMES)
-        char = Character.from_content(content)
-        self.assertIsInstance(char.former_names, list)
-        self.assertTrue(char.former_names)
-        self.assertEqual(len(char.former_names), 2)
-
-        self.assertIsInstance(char.houses[0], CharacterHouse)
-        self.assertEqual(char.houses[0].owner, char.name)
-        self.assertEqual(char.houses[0].town, "Darashia")
-        self.assertEqual(char.houses[0].world, char.world)
-        self.assertIsInstance(char.houses[0].paid_until_date, datetime.date)
-
-    def test_character_from_content_with_position(self):
-        """Testing parsing a character with a position"""
-        content = self.load_resource(FILE_CHARACTER_SPECIAL_POSITION)
-
-        position = "CipSoft Member"
-
-        char = Character.from_content(content)
-        self.assertEqual("Steve", char.name)
-        self.assertEqual(position, char.position)
-        self.assertEqual(position, char.account_information.position)
-        steve_other = char.other_characters[2]
-        self.assertEqual("Steve", steve_other.name)
-        self.assertEqual("CipSoft Member", steve_other.position)
-
-    def test_character_from_content_deleted_character(self):
-        """Testing parsing a character scheduled for deletion"""
-        content = self.load_resource(FILE_CHARACTER_DELETION)
-        char = Character.from_content(content)
-        self.assertEqual("Expendable Dummy", char.name)
-        self.assertIsNotNone(char.deletion_date)
-        self.assertIsInstance(char.deletion_date, datetime.datetime)
-        self.assertEqual(parse_tibia_datetime("Oct 08 2018 22:17:00 CEST"), char.deletion_date)
-
-    def test_character_from_content_complex_deaths(self):
-        """Testing parsing a character with complex deaths (summons, assists, etc)"""
-        content = self.load_resource(FILE_CHARACTER_DEATHS_COMPLEX)
-        char = Character.from_content(content)
-        self.assertEqual(5, len(char.deaths))
-        death1, death2, death3, death4, death5 = char.deaths
-        self.assertIsInstance(death1, Death)
-        self.assertEqual(23, len(death1.killers))
-        self.assertEqual(1, len(death1.assists))
-
-        self.assertIsInstance(death2, Death)
-        self.assertEqual(1, len(death2.killers))
-        self.assertEqual(0, len(death2.assists))
-
-        self.assertIsInstance(death3, Death)
-        self.assertEqual(11, len(death3.killers))
-        self.assertEqual(0, len(death3.assists))
-        self.assertEqual("a paladin familiar", death3.killers[-1].summon)
-        self.assertEqual("Alloy Hat", death3.killers[-1].name)
-        self.assertTrue(death3.killers[-1].traded)
-
-        self.assertIsInstance(death4, Death)
-        self.assertEqual(12, len(death4.killers))
-        self.assertEqual(0, len(death4.assists))
-        self.assertEqual("Cliff Lee Burton", death4.killers[-1].name)
-        self.assertTrue(death4.killers[-1].traded)
-
-    def test_character_from_content_badges_and_title(self):
-        """Testing parsing a character with account badges and a title"""
-        content = self.load_resource(FILE_CHARACTER_TITLE_BADGES)
-        char = Character.from_content(content)
-        self.assertEqual("Galarzaa Fidera", char.name)
-        self.assertEqual(406, char.achievement_points)
-        self.assertEqual("Gold Hoarder", char.title)
-        self.assertEqual(8, char.unlocked_titles)
-        self.assertEqual(6, len(char.account_badges))
-        for badge in char.account_badges:
-            self.assertIsInstance(badge, AccountBadge)
-            self.assertIsInstance(badge.name, str)
-            self.assertIsInstance(badge.icon_url, str)
-            self.assertIsInstance(badge.description, str)
-
-    def test_character_from_content_no_selected_badges(self):
-        """Testing parsing a character with visible badges but none selected."""
-        content = self.load_resource(FILE_CHARACTER_NO_BADGES_SELECTED)
-        char = Character.from_content(content)
-        self.assertEqual("Cozzackirycerz", char.name)
-        self.assertEqual(25, char.achievement_points)
-        self.assertIsNone(char.title)
-        self.assertEqual(3, char.unlocked_titles)
-        self.assertEqual(0, len(char.account_badges))
-        self.assertEqual(0, len(char.former_names))
-
-    def test_character_from_content_multiple_houses(self):
-        """Testing parsing a character with multiple houses."""
-        content = self.load_resource(FILE_CHARACTER_MULTIPLE_HOUSES)
-        char = Character.from_content(content)
-        self.assertEqual("Sayuri Nowan", char.name)
-        self.assertEqual(2, len(char.houses))
-        first_house = char.houses[0]
-        second_house = char.houses[1]
-        self.assertEqual("Cormaya 10", first_house.name)
-        self.assertEqual("Old Heritage Estate", second_house.name)
-        self.assertEqual("Edron", first_house.town)
-        self.assertEqual("Rathleton", second_house.town)
-
-    def test_character_from_content_truncated_deaths(self):
-        """Testing parsing a character with truncated daths"""
-        content = self.load_resource(FILE_CHARACTER_TRUNCATED_DEATHS)
-        char = Character.from_content(content)
-        self.assertEqual("Godlike Terror", char.name)
-        self.assertEqual(51, len(char.deaths))
-        self.assertTrue(char.deaths_truncated)
-
-    def test_character_from_content_unrelated(self):
-        """Testing parsing an unrelated tibia.com section"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(InvalidContent):
-            Character.from_content(content)
-
-    # endregion
-
-    def test_death_types(self):
-        """Testing different death types"""
-        assisted_suicide = Death("Galarzaa", 280, killers=[Killer("Galarzaa", True), Killer("a pixy")],
-                                 time=datetime.datetime.now())
-        self.assertEqual(assisted_suicide.killer, assisted_suicide.killers[0])
-        self.assertFalse(assisted_suicide.by_player)
-
-        spawn_invasion = Death("Galarza", 270, killers=[Killer("a demon"), Killer("Nezune", True)])
-        self.assertEqual(spawn_invasion.killer, spawn_invasion.killers[0])
-        self.assertIsNone(spawn_invasion.killer.url)
-        self.assertTrue(spawn_invasion.by_player)
+import datetime
+import unittest
+
+from tests.tests_tibiapy import TestCommons
+from tibiapy import InvalidContent
+from tibiapy.models import Death, DeathParticipant, AccountBadge, CharacterHouse
+from tibiapy.parsers.character import CharacterParser
+from tibiapy.urls import get_character_url
+from tibiapy.utils import parse_tibia_datetime
+
+FILE_CHARACTER_RESOURCE = "character/tibiacom_full.txt"
+FILE_CHARACTER_NOT_FOUND = "character/tibiacom_not_found.txt"
+FILE_CHARACTER_FORMER_NAMES = "character/tibiacom_former_names.txt"
+FILE_CHARACTER_SPECIAL_POSITION = "character/tibiacom_special_position.txt"
+FILE_CHARACTER_DELETION = "character/tibiacom_deletion.txt"
+FILE_CHARACTER_DEATHS_COMPLEX = "character/tibiacom_deaths_complex.txt"
+FILE_CHARACTER_TITLE_BADGES = "character/tibiacom_title_badges.txt"
+FILE_CHARACTER_NO_BADGES_SELECTED = "character/tibiacom_no_badges_selected.txt"
+FILE_CHARACTER_MULTIPLE_HOUSES = "character/tibiacom_multiple_houses.txt"
+FILE_CHARACTER_TRUNCATED_DEATHS = "character/tibiacom_truncated_deaths.txt"
+
+
+class TestCharacter(TestCommons, unittest.TestCase):
+    def _compare_character(self, mock_character, character):
+        self.assertEqual(mock_character.name, character.name)
+        self.assertEqual(mock_character.world, character.world)
+        self.assertEqual(mock_character.vocation, character.vocation)
+        self.assertEqual(mock_character.level, character.level)
+        self.assertEqual(mock_character.sex, character.sex)
+
+    # region Tibia.com Character Tests
+    def test_character_from_content(self):
+        """Testing parsing a character's HTML content"""
+        character = CharacterParser.from_content(self.load_resource(FILE_CHARACTER_RESOURCE))
+        # TODO: Reenable
+        # self._compare_character(Character("Tschas", "Gladera", Vocation.ELDER_DRUID, 522, Sex.FEMALE), character)
+        self.assertIsNotNone(character.guild_membership)
+        self.assertEqual("Bald Dwarfs", character.guild_membership.name)
+        self.assertEqual("Exalted", character.guild_membership.rank)
+        self.assertIsNotNone(character.guild_url)
+        self.assertIsNone(character.married_to_url)
+        self.assertEqual(character.guild_name, character.guild_membership.name)
+        self.assertEqual(character.guild_rank, character.guild_membership.rank)
+        self.assertTrue(character.is_premium)
+        self.assertEqual(405, character.achievement_points)
+        self.assertIsNone(character.deletion_date)
+        self.assertIsNotNone(character.deaths)
+        self.assertEqual(0, character.deaths.__len__())
+        self.assertEqual(parse_tibia_datetime("Apr 16 2023, 00:43:29 CEST"), character.last_login)
+        self.assertEqual(character.url, get_character_url(character.name))
+        self.assertEqual(5, len(character.other_characters))
+        self.assertFalse(character.hidden)
+
+        # Badges
+        self.assertEqual(8, len(character.account_badges))
+        badge = character.account_badges[0]
+        self.assertEqual("Ancient Hero", badge.name)
+        self.assertEqual("The account is older than 15 years.", badge.description)
+
+    def test_character_from_content_not_found(self):
+        """Testing parsing a character not found page"""
+        content = self.load_resource(FILE_CHARACTER_NOT_FOUND)
+        char = CharacterParser.from_content(content)
+        self.assertIsNone(char)
+
+    def test_character_from_content_with_former_names(self):
+        """Testing parsing a character that has former names"""
+        content = self.load_resource(FILE_CHARACTER_FORMER_NAMES)
+        char = CharacterParser.from_content(content)
+        self.assertIsInstance(char.former_names, list)
+        self.assertTrue(char.former_names)
+        self.assertEqual(len(char.former_names), 2)
+
+        self.assertIsInstance(char.houses[0], CharacterHouse)
+        self.assertEqual(char.houses[0].town, "Darashia")
+        self.assertEqual(char.houses[0].world, char.world)
+        self.assertIsInstance(char.houses[0].paid_until_date, datetime.date)
+
+    def test_character_from_content_with_position(self):
+        """Testing parsing a character with a position"""
+        content = self.load_resource(FILE_CHARACTER_SPECIAL_POSITION)
+
+        position = "CipSoft Member"
+
+        char = CharacterParser.from_content(content)
+        self.assertEqual("Steve", char.name)
+        self.assertEqual(position, char.position)
+        self.assertEqual(position, char.account_information.position)
+        steve_other = char.other_characters[2]
+        self.assertEqual("Steve", steve_other.name)
+        self.assertEqual("CipSoft Member", steve_other.position)
+
+    def test_character_from_content_deleted_character(self):
+        """Testing parsing a character scheduled for deletion"""
+        content = self.load_resource(FILE_CHARACTER_DELETION)
+        char = CharacterParser.from_content(content)
+        self.assertEqual("Expendable Dummy", char.name)
+        self.assertIsNotNone(char.deletion_date)
+        self.assertIsInstance(char.deletion_date, datetime.datetime)
+        self.assertEqual(parse_tibia_datetime("Oct 08 2018 22:17:00 CEST"), char.deletion_date)
+
+    def test_character_from_content_complex_deaths(self):
+        """Testing parsing a character with complex deaths (summons, assists, etc)"""
+        content = self.load_resource(FILE_CHARACTER_DEATHS_COMPLEX)
+        char = CharacterParser.from_content(content)
+        self.assertEqual(5, len(char.deaths))
+        death1, death2, death3, death4, death5 = char.deaths
+        self.assertIsInstance(death1, Death)
+        self.assertEqual(23, len(death1.killers))
+        self.assertEqual(1, len(death1.assists))
+
+        self.assertIsInstance(death2, Death)
+        self.assertEqual(1, len(death2.killers))
+        self.assertEqual(0, len(death2.assists))
+
+        self.assertIsInstance(death3, Death)
+        self.assertEqual(11, len(death3.killers))
+        self.assertEqual(0, len(death3.assists))
+        self.assertEqual("a paladin familiar", death3.killers[-1].summon)
+        self.assertEqual("Alloy Hat", death3.killers[-1].name)
+        self.assertTrue(death3.killers[-1].traded)
+
+        self.assertIsInstance(death4, Death)
+        self.assertEqual(12, len(death4.killers))
+        self.assertEqual(0, len(death4.assists))
+        self.assertEqual("Cliff Lee Burton", death4.killers[-1].name)
+        self.assertTrue(death4.killers[-1].traded)
+
+    def test_character_from_content_badges_and_title(self):
+        """Testing parsing a character with account badges and a title"""
+        content = self.load_resource(FILE_CHARACTER_TITLE_BADGES)
+        char = CharacterParser.from_content(content)
+        self.assertEqual("Galarzaa Fidera", char.name)
+        self.assertEqual(410, char.achievement_points)
+        self.assertEqual("Gold Hoarder", char.title)
+        self.assertEqual(13, char.unlocked_titles)
+        self.assertEqual(8, len(char.account_badges))
+        for badge in char.account_badges:
+            self.assertIsInstance(badge, AccountBadge)
+            self.assertIsInstance(badge.name, str)
+            self.assertIsInstance(badge.icon_url, str)
+            self.assertIsInstance(badge.description, str)
+
+    def test_character_from_content_no_selected_badges(self):
+        """Testing parsing a character with visible badges but none selected."""
+        content = self.load_resource(FILE_CHARACTER_NO_BADGES_SELECTED)
+        char = CharacterParser.from_content(content)
+        self.assertEqual("Cozzackirycerz", char.name)
+        self.assertEqual(25, char.achievement_points)
+        self.assertIsNone(char.title)
+        self.assertEqual(3, char.unlocked_titles)
+        self.assertEqual(0, len(char.account_badges))
+        self.assertEqual(0, len(char.former_names))
+
+    def test_character_from_content_multiple_houses(self):
+        """Testing parsing a character with multiple houses."""
+        content = self.load_resource(FILE_CHARACTER_MULTIPLE_HOUSES)
+        char = CharacterParser.from_content(content)
+        self.assertEqual("Sayuri Nowan", char.name)
+        self.assertEqual(2, len(char.houses))
+        first_house = char.houses[0]
+        second_house = char.houses[1]
+        self.assertEqual("Cormaya 10", first_house.name)
+        self.assertEqual("Old Heritage Estate", second_house.name)
+        self.assertEqual("Edron", first_house.town)
+        self.assertEqual("Rathleton", second_house.town)
+
+    def test_character_from_content_truncated_deaths(self):
+        """Testing parsing a character with truncated daths"""
+        content = self.load_resource(FILE_CHARACTER_TRUNCATED_DEATHS)
+        char = CharacterParser.from_content(content)
+        self.assertEqual("Godlike Terror", char.name)
+        self.assertEqual(51, len(char.deaths))
+        self.assertTrue(char.deaths_truncated)
+
+    def test_character_from_content_unrelated(self):
+        """Testing parsing an unrelated tibia.com section"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(InvalidContent):
+            CharacterParser.from_content(content)
+
+    # endregion
+
+    def test_death_types(self):
+        """Testing different death types"""
+        assisted_suicide = Death(level=280,
+                                 killers=[
+                                     DeathParticipant(name="Galarzaa", player=True, summon=None, traded=False),
+                                     DeathParticipant(name="a pixy", player=False, summon=None, traded=False)
+                                 ],
+                                 assists=[],
+                                 time=datetime.datetime.now())
+        self.assertEqual(assisted_suicide.killer, assisted_suicide.killers[0])
+        self.assertTrue(assisted_suicide.by_player)
+
+        spawn_invasion = Death(level=270,
+                               killers=[
+                                   DeathParticipant(name="a demon", player=False, summon=None, traded=False),
+                                   DeathParticipant(name="Nezune", player=True, summon=None, traded=False)
+                               ],
+                               assists=[],
+                               time=datetime.datetime.now())
+        self.assertEqual(spawn_invasion.killer, spawn_invasion.killers[0])
+        self.assertIsNone(spawn_invasion.killer.url)
+        self.assertTrue(spawn_invasion.by_player)
```

### Comparing `tibia.py-5.6.1/tests/tests_client.py` & `tibia.py-6.0.0a1/tests/tests_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,350 +1,344 @@
-import datetime
-import sys
-import unittest.mock
-
-import aiohttp
-import asynctest
-from aioresponses import aioresponses
-
-import tibiapy
-from tests.tests_bazaar import FILE_BAZAAR_CURRENT, FILE_BAZAAR_HISTORY, FILE_AUCTION_FINISHED
-from tests.tests_character import FILE_CHARACTER_RESOURCE, FILE_CHARACTER_NOT_FOUND
-from tests.tests_events import FILE_EVENT_CALENDAR
-from tests.tests_forums import FILE_BOARD_THREAD_LIST, FILE_CM_POST_ARCHIVE_PAGES, FILE_WORLD_BOARDS
-from tests.tests_guild import FILE_GUILD_FULL, FILE_GUILD_LIST
-from tests.tests_highscores import FILE_HIGHSCORES_FULL
-from tests.tests_house import FILE_HOUSE_FULL, FILE_HOUSE_LIST
-from tests.tests_kill_statistics import FILE_KILL_STATISTICS_FULL
-from tests.tests_leaderboards import FILE_LEADERBOARD_CURRENT
-from tests.tests_news import FILE_NEWS_LIST, FILE_NEWS_ARTICLE
-from tests.tests_tibiapy import TestCommons
-from tests.tests_world import FILE_WORLD_FULL, FILE_WORLD_LIST
-from tibiapy import BoardEntry, CharacterBazaar, Client, Character, CMPostArchive, ForumBoard, Guild, GuildsSection, \
-    Highscores, \
-    HouseType, \
-    HousesSection, \
-    Leaderboard, NewsArchive, VocationFilter, \
-    Category, \
-    House, HouseEntry, \
-    GuildEntry, \
-    KillStatistics, NewsEntry, News, World, WorldOverview, Forbidden, NetworkError, CreatureEntry, Auction, \
-    EventSchedule
-
-
-class TestClient(asynctest.TestCase, TestCommons):
-    def setUp(self):
-        self.client = Client()
-
-    async def tearDown(self):
-        await self.client.session.close()
-
-    async def test_client_init_pass_session(self):
-        """Testing creating an instance passing a session"""
-        headers = {"User-Agent": "Python Unit Test"}
-        session = aiohttp.ClientSession(headers=headers)
-        client = Client(session=session)
-
-        self.assertEqual(client.session._default_headers, headers)
-
-        await client.session.close()
-
-    @aioresponses()
-    async def test_client_handle_errors(self, mock):
-        """Testing error handling"""
-        mock.get(WorldOverview.get_url(), status=403)
-        with self.assertRaises(Forbidden):
-            await self.client.fetch_world_list()
-
-        mock.get(WorldOverview.get_url(), status=404)
-        with self.assertRaises(NetworkError):
-            await self.client.fetch_world_list()
-
-        mock.get(NewsEntry.get_list_url(), exception=aiohttp.ClientError())
-        with self.assertRaises(NetworkError):
-            await self.client.fetch_world_list()
-
-        mock.post(NewsEntry.get_list_url(), exception=aiohttp.ClientOSError())
-        with self.assertRaises(NetworkError):
-            await self.client.fetch_recent_news(30)
-
-    @aioresponses()
-    async def test_client_fetch_character(self, mock):
-        """Testing fetching a character"""
-        name = "Tschas"
-        content = self.load_resource(FILE_CHARACTER_RESOURCE)
-        mock.get(Character.get_url(name), status=200, body=content)
-        character = await self.client.fetch_character(name)
-
-        self.assertIsInstance(character.data, Character)
-
-    @aioresponses()
-    async def test_client_fetch_character_not_found(self, mock):
-        """Testing fetching a non existent character"""
-        name = "Nezune"
-        content = self.load_resource(FILE_CHARACTER_NOT_FOUND)
-        mock.get(Character.get_url(name), status=200, body=content)
-        character = await self.client.fetch_character(name)
-
-        self.assertIsNone(character.data)
-
-    @aioresponses()
-    async def test_client_fetch_guild(self, mock):
-        """Testing fetching a guild"""
-        name = "Vitam et Mortem"
-        content = self.load_resource(FILE_GUILD_FULL)
-        mock.get(Guild.get_url(name), status=200, body=content)
-        guild = await self.client.fetch_guild(name)
-
-        self.assertIsInstance(guild.data, Guild)
-
-    @aioresponses()
-    async def test_client_fetch_world_guilds(self, mock):
-        """Testing fetching a world's guild list"""
-        world = "Zuna"
-        content = self.load_resource(FILE_GUILD_LIST)
-        mock.get(GuildsSection.get_url(world), status=200, body=content)
-        response = await self.client.fetch_world_guilds(world)
-        guilds = response.data.entries
-
-        self.assertIsInstance(guilds[0], GuildEntry)
-
-    @aioresponses()
-    async def test_client_fetch_highscores_page(self, mock):
-        """Testing fetching a highscores page"""
-        world = "Estela"
-        category = Category.MAGIC_LEVEL
-        vocations = VocationFilter.KNIGHTS
-        content = self.load_resource(FILE_HIGHSCORES_FULL)
-        mock.get(Highscores.get_url(world, category, vocations), status=200, body=content)
-        highscores = await self.client.fetch_highscores_page(world, category, vocations)
-
-        self.assertIsInstance(highscores.data, Highscores)
-
-    @aioresponses()
-    async def test_client_fetch_house(self, mock):
-        """Testing fetching a house"""
-        world = "Antica"
-        house_id = 5236
-        content = self.load_resource(FILE_HOUSE_FULL)
-        mock.get(House.get_url(house_id, world), status=200, body=content)
-        house = await self.client.fetch_house(house_id, world)
-
-        self.assertIsInstance(house.data, House)
-
-    @aioresponses()
-    async def test_client_fetch_world_houses(self, mock):
-        """Testing fetching a world's houses"""
-        world = "Antica"
-        city = "Edron"
-        content = self.load_resource(FILE_HOUSE_LIST)
-        mock.get(HousesSection.get_url(world=world, town=city, house_type=HouseType.HOUSE), status=200, body=content)
-        houses = await self.client.fetch_world_houses(world, city)
-
-        self.assertIsInstance(houses.data, HousesSection)
-        self.assertIsInstance(houses.data.entries[0], HouseEntry)
-
-    @aioresponses()
-    async def test_client_fetch_kill_statistics(self, mock):
-        """Testing fetching kill statistics"""
-        world = "Antica"
-        content = self.load_resource(FILE_KILL_STATISTICS_FULL)
-        mock.get(KillStatistics.get_url(world), status=200, body=content)
-        kill_statistics = await self.client.fetch_kill_statistics(world)
-
-        self.assertIsInstance(kill_statistics.data, KillStatistics)
-
-    @aioresponses()
-    async def test_client_fetch_recent_news(self, mock):
-        """Testing fetching recent nows"""
-        content = self.load_resource(FILE_NEWS_LIST)
-        mock.post(NewsArchive.get_url(), status=200, body=content)
-        recent_news = await self.client.fetch_recent_news(30)
-
-        self.assertIsInstance(recent_news.data, NewsArchive)
-        self.assertIsInstance(recent_news.data.entries[0], NewsEntry)
-
-    async def test_client_fetch_news_archive_invalid_dates(self):
-        """Testing fetching news archive with invalid dates"""
-        today = datetime.date.today()
-        yesterday = today - datetime.timedelta(days=1)
-        with self.assertRaises(ValueError):
-            await self.client.fetch_news_archive(today, yesterday)
-
-    @aioresponses()
-    async def test_client_fetch_news(self, mock):
-        """Testing fetch news"""
-        news_id = 6000
-        content = self.load_resource(FILE_NEWS_ARTICLE)
-        mock.get(News.get_url(news_id), status=200, body=content)
-        news = await self.client.fetch_news(news_id)
-
-        self.assertIsInstance(news.data, News)
-
-    @aioresponses()
-    async def test_client_fetch_world(self, mock):
-        """Testing fetching a world"""
-        name = "Antica"
-        content = self.load_resource(FILE_WORLD_FULL)
-        mock.get(World.get_url(name), status=200, body=content)
-        world = await self.client.fetch_world(name)
-
-        self.assertIsInstance(world.data, World)
-
-    @aioresponses()
-    async def test_client_fetch_world_list(self, mock):
-        """Testing fetching the world list"""
-        content = self.load_resource(FILE_WORLD_LIST)
-        mock.get(WorldOverview.get_url(), status=200, body=content)
-        worlds = await self.client.fetch_world_list()
-
-        self.assertIsInstance(worlds.data, WorldOverview)
-
-    @aioresponses()
-    async def test_client_fetch_boosted_creature(self, mock):
-        """Testing fetching the boosted creature"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        mock.get(News.get_list_url(), status=200, body=content)
-        creature = await self.client.fetch_boosted_creature()
-
-        self.assertIsInstance(creature.data, CreatureEntry)
-
-    @aioresponses()
-    async def test_client_fetch_cm_post_archive(self, mock):
-        """Testing fetching the CM Post Archive"""
-        content = self.load_resource(FILE_CM_POST_ARCHIVE_PAGES)
-        start_date = datetime.date.today()-datetime.timedelta(days=40)
-        end_date = datetime.date.today()
-        mock.get(CMPostArchive.get_url(start_date, end_date), status=200, body=content)
-        cm_post_archive = await self.client.fetch_cm_post_archive(start_date, end_date)
-
-        self.assertIsInstance(cm_post_archive.data, CMPostArchive)
-
-    async def test_client_fetch_cm_post_archive_invalid_dates(self):
-        """Testing fetching the CM Post Archive with invalid dates"""
-        end_date = datetime.date.today()-datetime.timedelta(days=40)
-        start_date = datetime.date.today()
-        with self.assertRaises(ValueError):
-            await self.client.fetch_cm_post_archive(start_date, end_date)
-
-    async def test_client_fetch_cm_post_archive_invalid_page(self):
-        """Testing fetching the CM Post Archive with invalid page number"""
-        start_date = datetime.date.today()-datetime.timedelta(days=40)
-        end_date = datetime.date.today()
-        with self.assertRaises(ValueError):
-            await self.client.fetch_cm_post_archive(start_date, end_date, -1)
-
-    @aioresponses()
-    async def test_client_fetch_current_auctions(self, mock):
-        """Testing fetching the current auctions"""
-        content = self.load_resource(FILE_BAZAAR_CURRENT)
-        mock.get(CharacterBazaar.get_current_auctions_url(), status=200, body=content)
-        response = await self.client.fetch_current_auctions()
-        self.assertIsInstance(response.data, CharacterBazaar)
-
-    async def test_client_fetch_current_auctions_invalid_page(self):
-        """Testing fetching the current auctions with an invalid page"""
-        with self.assertRaises(ValueError):
-            await self.client.fetch_current_auctions(-1)
-
-    @aioresponses()
-    async def test_client_fetch_auction_history(self, mock):
-        """Testing fetching the auction history"""
-        content = self.load_resource(FILE_BAZAAR_HISTORY)
-        mock.get(CharacterBazaar.get_auctions_history_url(), status=200, body=content)
-        response = await self.client.fetch_auction_history()
-        self.assertIsInstance(response.data, CharacterBazaar)
-
-    async def test_client_fetch_auction_history_invalid_page(self):
-        """Testing fetching the auction history with an incorrect page"""
-        with self.assertRaises(ValueError):
-            await self.client.fetch_auction_history(-1)
-
-    @aioresponses()
-    async def test_client_fetch_auction(self, mock):
-        """Testing fetching an auction"""
-        content = self.load_resource(FILE_AUCTION_FINISHED)
-        mock.get(Auction.get_url(134), status=200, body=content)
-        response = await self.client.fetch_auction(134)
-        self.assertIsInstance(response.data, Auction)
-
-    async def test_client_fetch_auction_invalid_id(self):
-        """Testing fetching an auction with an invalid id"""
-        with self.assertRaises(ValueError):
-            await self.client.fetch_auction(-1)
-
-    @aioresponses()
-    async def test_client_fetch_event_calendar(self, mock):
-        """Testing fetching the auction history"""
-        content = self.load_resource(FILE_EVENT_CALENDAR)
-        mock.get(EventSchedule.get_url(), status=200, body=content)
-        response = await self.client.fetch_event_schedule()
-        self.assertIsInstance(response.data, EventSchedule)
-
-    async def test_client_fetch_event_calendar_invalid_params(self):
-        """Testing fetching the auction history"""
-        with self.assertRaises(ValueError):
-            await self.client.fetch_event_schedule(3)
-
-    @aioresponses()
-    async def test_client_fetch_forum_community_boards(self, mock):
-        """Testing fetching the community boards"""
-        content = self.load_resource(FILE_WORLD_BOARDS)
-        mock.get(BoardEntry.get_community_boards_url(), status=200, body=content)
-        response = await self.client.fetch_forum_community_boards()
-        self.assertIsInstance(response.data[0], BoardEntry)
-
-    @aioresponses()
-    async def test_client_fetch_forum_trade_boards(self, mock):
-        """Testing fetching the trade boards"""
-        content = self.load_resource(FILE_WORLD_BOARDS)
-        mock.get(BoardEntry.get_trade_boards_url(), status=200, body=content)
-        response = await self.client.fetch_forum_trade_boards()
-        self.assertIsInstance(response.data[0], BoardEntry)
-
-    @aioresponses()
-    async def test_client_fetch_forum_support_boards(self, mock):
-        """Testing fetching the support boards"""
-        content = self.load_resource(FILE_WORLD_BOARDS)
-        mock.get(BoardEntry.get_support_boards_url(), status=200, body=content)
-        response = await self.client.fetch_forum_support_boards()
-        self.assertIsInstance(response.data[0], BoardEntry)
-
-    @aioresponses()
-    async def test_client_fetch_forum_world_boards(self, mock):
-        """Testing fetching the world boards"""
-        content = self.load_resource(FILE_WORLD_BOARDS)
-        mock.get(BoardEntry.get_world_boards_url(), status=200, body=content)
-        response = await self.client.fetch_forum_world_boards()
-        self.assertIsInstance(response.data[0], BoardEntry)
-
-    @aioresponses()
-    async def test_client_fetch_forum_board(self, mock):
-        """Testing fetching a forum board"""
-        content = self.load_resource(FILE_BOARD_THREAD_LIST)
-        mock.get(BoardEntry.get_url(1), status=200, body=content)
-        response = await self.client.fetch_forum_board(1)
-        self.assertIsInstance(response.data, ForumBoard)
-
-    @aioresponses()
-    async def test_client_fetch_leaderboards(self, mock):
-        """Testing fetching the leaderboards"""
-        content = self.load_resource(FILE_LEADERBOARD_CURRENT)
-        mock.get(Leaderboard.get_url("Antica"), status=200, body=content)
-        response = await self.client.fetch_leaderboard("Antica")
-        self.assertIsInstance(response.data, Leaderboard)
-
-    @unittest.mock.patch("tibiapy.bazaar.Auction._parse_page_items")
-    @unittest.skipIf(sys.version_info < (3, 8, 0), "AsyncMock was implemented in 3.8")
-    async def test_client__fetch_all_pages_success(self, parse_page_items):
-        """Testing internal method to fetch all pages of an auction item collection."""
-        paginator = tibiapy.ItemSummary(page=1, total_pages=5)
-        self.client._fetch_ajax_page = unittest.mock.AsyncMock()
-
-        await self.client._fetch_all_pages(1, paginator, 1)
-
-        self.assertEqual(4, self.client._fetch_ajax_page.await_count)
-        self.assertEqual(4, parse_page_items.call_count)
-
-    async def test_client__fetch_all_pages_none_input(self):
-        """Testing internal method to fetch all pages of an auction item collection."""
-        self.assertIsNone(await self.client._fetch_all_pages(1, None, 1))
+import datetime
+import sys
+import unittest.mock
+
+import aiohttp
+from aioresponses import aioresponses
+
+from tests.tests_bazaar import FILE_BAZAAR_CURRENT, FILE_BAZAAR_HISTORY, FILE_AUCTION_FINISHED
+from tests.tests_character import FILE_CHARACTER_RESOURCE, FILE_CHARACTER_NOT_FOUND
+from tests.tests_events import FILE_EVENT_CALENDAR
+from tests.tests_forums import FILE_BOARD_THREAD_LIST, FILE_CM_POST_ARCHIVE_PAGES, FILE_WORLD_BOARDS
+from tests.tests_guild import FILE_GUILD_FULL, FILE_GUILD_LIST
+from tests.tests_highscores import FILE_HIGHSCORES_FULL
+from tests.tests_house import FILE_HOUSE_FULL, FILE_HOUSE_LIST
+from tests.tests_kill_statistics import FILE_KILL_STATISTICS_FULL
+from tests.tests_leaderboards import FILE_LEADERBOARD_CURRENT
+from tests.tests_news import FILE_NEWS_ARCHIVE_RESULTS, FILE_NEWS_ARTICLE
+from tests.tests_tibiapy import TestCommons
+from tests.tests_world import FILE_WORLD_FULL, FILE_WORLD_LIST
+from tibiapy import Client, Forbidden, NetworkError, HouseType, BazaarType
+from tibiapy.models import BoardEntry, CharacterBazaar, Character, CMPostArchive, ForumBoard, Guild, Highscores, \
+    HousesSection, Leaderboard, HighscoresProfession, HighscoresCategory, House, HouseEntry, GuildEntry, KillStatistics, \
+    World, WorldOverview, Auction, NewsArchive, NewsEntry, News, ItemSummary, ForumSection
+from tibiapy.models.creature import CreatureEntry
+from tibiapy.models.event import EventSchedule
+from tibiapy.urls import get_character_url, get_world_guilds_url, get_guild_url, get_house_url, get_world_overview_url, \
+    get_news_archive_url, get_news_url, get_forum_board_url, get_highscores_url, get_kill_statistics_url, \
+    get_event_schedule_url, get_houses_section_url, get_auction_url, get_bazaar_url, get_cm_post_archive_url, \
+    get_leaderboards_url, get_world_url
+
+
+class TestClient(unittest.IsolatedAsyncioTestCase, TestCommons):
+    def setUp(self):
+        self.client = Client()
+
+    async def asyncTearDown(self):
+        await self.client.session.close()
+
+    async def test_client_init_pass_session(self):
+        """Testing creating an instance passing a session"""
+        headers = {"User-Agent": "Python Unit Test"}
+        session = aiohttp.ClientSession(headers=headers)
+        client = Client(session=session)
+
+        self.assertEqual(client.session._default_headers, headers)
+
+        await client.session.close()
+
+    @aioresponses()
+    async def test_client_handle_errors(self, mock):
+        """Testing error handling"""
+        mock.get(get_world_overview_url(), status=403)
+        with self.assertRaises(Forbidden):
+            await self.client.fetch_world_overview()
+
+        mock.get(get_world_overview_url(), status=404)
+        with self.assertRaises(NetworkError):
+            await self.client.fetch_world_overview()
+
+        mock.get(get_news_archive_url(), exception=aiohttp.ClientError())
+        with self.assertRaises(NetworkError):
+            await self.client.fetch_world_overview()
+
+        mock.post(get_news_archive_url(), exception=aiohttp.ClientOSError())
+        with self.assertRaises(NetworkError):
+            await self.client.fetch_news_archive_by_days(30)
+
+    @aioresponses()
+    async def test_client_fetch_character(self, mock):
+        """Testing fetching a character"""
+        name = "Tschas"
+        content = self.load_resource(FILE_CHARACTER_RESOURCE)
+        mock.get(get_character_url(name), status=200, body=content)
+        character = await self.client.fetch_character(name)
+
+        self.assertIsInstance(character.data, Character)
+
+    @aioresponses()
+    async def test_client_fetch_character_not_found(self, mock):
+        """Testing fetching a non existent character"""
+        name = "Nezune"
+        content = self.load_resource(FILE_CHARACTER_NOT_FOUND)
+        mock.get(get_character_url(name), status=200, body=content)
+        character = await self.client.fetch_character(name)
+
+        self.assertIsNone(character.data)
+
+    @aioresponses()
+    async def test_client_fetch_guild(self, mock):
+        """Testing fetching a guild"""
+        name = "Vitam et Mortem"
+        content = self.load_resource(FILE_GUILD_FULL)
+        mock.get(get_guild_url(name), status=200, body=content)
+        guild = await self.client.fetch_guild(name)
+
+        self.assertIsInstance(guild.data, Guild)
+
+    @aioresponses()
+    async def test_client_fetch_world_guilds(self, mock):
+        """Testing fetching a world's guild list"""
+        world = "Zuna"
+        content = self.load_resource(FILE_GUILD_LIST)
+        mock.get(get_world_guilds_url(world), status=200, body=content)
+        response = await self.client.fetch_world_guilds(world)
+        guilds = response.data.entries
+
+        self.assertIsInstance(guilds[0], GuildEntry)
+
+    @aioresponses()
+    async def test_client_fetch_highscores_page(self, mock):
+        """Testing fetching a highscores page"""
+        world = "Estela"
+        category = HighscoresCategory.MAGIC_LEVEL
+        vocations = HighscoresProfession.KNIGHTS
+        content = self.load_resource(FILE_HIGHSCORES_FULL)
+        mock.get(get_highscores_url(world, category, vocations), status=200, body=content)
+        highscores = await self.client.fetch_highscores_page(world, category, vocations)
+
+        self.assertIsInstance(highscores.data, Highscores)
+
+    @aioresponses()
+    async def test_client_fetch_house(self, mock):
+        """Testing fetching a house"""
+        world = "Antica"
+        house_id = 5236
+        content = self.load_resource(FILE_HOUSE_FULL)
+        mock.get(get_house_url(world, house_id), status=200, body=content)
+        house = await self.client.fetch_house(house_id, world)
+
+        self.assertIsInstance(house.data, House)
+
+    @aioresponses()
+    async def test_client_fetch_world_houses(self, mock):
+        """Testing fetching a world's houses"""
+        world = "Antica"
+        city = "Edron"
+        content = self.load_resource(FILE_HOUSE_LIST)
+        mock.get(get_houses_section_url(world=world, town=city, house_type=HouseType.HOUSE), status=200, body=content)
+        houses = await self.client.fetch_houses_section(world, city)
+
+        self.assertIsInstance(houses.data, HousesSection)
+        self.assertIsInstance(houses.data.entries[0], HouseEntry)
+
+    @aioresponses()
+    async def test_client_fetch_kill_statistics(self, mock):
+        """Testing fetching kill statistics"""
+        world = "Antica"
+        content = self.load_resource(FILE_KILL_STATISTICS_FULL)
+        mock.get(get_kill_statistics_url(world), status=200, body=content)
+        kill_statistics = await self.client.fetch_kill_statistics(world)
+
+        self.assertIsInstance(kill_statistics.data, KillStatistics)
+
+    @aioresponses()
+    async def test_client_fetch_recent_news(self, mock):
+        """Testing fetching recent nows"""
+        content = self.load_resource(FILE_NEWS_ARCHIVE_RESULTS)
+        mock.post(get_news_archive_url(), status=200, body=content)
+        recent_news = await self.client.fetch_news_archive_by_days(30)
+
+        self.assertIsInstance(recent_news.data, NewsArchive)
+        self.assertIsInstance(recent_news.data.entries[0], NewsEntry)
+
+    async def test_client_fetch_news_archive_invalid_dates(self):
+        """Testing fetching news archive with invalid dates"""
+        today = datetime.date.today()
+        yesterday = today - datetime.timedelta(days=1)
+        with self.assertRaises(ValueError):
+            await self.client.fetch_news_archive(today, yesterday)
+
+    @aioresponses()
+    async def test_client_fetch_news(self, mock):
+        """Testing fetch news"""
+        news_id = 6000
+        content = self.load_resource(FILE_NEWS_ARTICLE)
+        mock.get(get_news_url(news_id), status=200, body=content)
+        news = await self.client.fetch_news(news_id)
+
+        self.assertIsInstance(news.data, News)
+
+    @aioresponses()
+    async def test_client_fetch_world(self, mock):
+        """Testing fetching a world"""
+        name = "Antica"
+        content = self.load_resource(FILE_WORLD_FULL)
+        mock.get(get_world_url(name), status=200, body=content)
+        world = await self.client.fetch_world(name)
+
+        self.assertIsInstance(world.data, World)
+
+    @aioresponses()
+    async def test_client_fetch_world_list(self, mock):
+        """Testing fetching the world list"""
+        content = self.load_resource(FILE_WORLD_LIST)
+        mock.get(get_world_overview_url(), status=200, body=content)
+        worlds = await self.client.fetch_world_overview()
+
+        self.assertIsInstance(worlds.data, WorldOverview)
+
+    @aioresponses()
+    async def test_client_fetch_boosted_creature(self, mock):
+        """Testing fetching the boosted creature"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        mock.get(get_news_archive_url(), status=200, body=content)
+        creature = await self.client.fetch_boosted_creature()
+
+        self.assertIsInstance(creature.data, CreatureEntry)
+
+    @aioresponses()
+    async def test_client_fetch_cm_post_archive(self, mock):
+        """Testing fetching the CM Post Archive"""
+        content = self.load_resource(FILE_CM_POST_ARCHIVE_PAGES)
+        start_date = datetime.date.today()-datetime.timedelta(days=40)
+        end_date = datetime.date.today()
+        mock.get(get_cm_post_archive_url(start_date, end_date), status=200, body=content)
+        cm_post_archive = await self.client.fetch_cm_post_archive(start_date, end_date)
+
+        self.assertIsInstance(cm_post_archive.data, CMPostArchive)
+
+    async def test_client_fetch_cm_post_archive_invalid_dates(self):
+        """Testing fetching the CM Post Archive with invalid dates"""
+        end_date = datetime.date.today()-datetime.timedelta(days=40)
+        start_date = datetime.date.today()
+        with self.assertRaises(ValueError):
+            await self.client.fetch_cm_post_archive(start_date, end_date)
+
+    async def test_client_fetch_cm_post_archive_invalid_page(self):
+        """Testing fetching the CM Post Archive with invalid page number"""
+        start_date = datetime.date.today()-datetime.timedelta(days=40)
+        end_date = datetime.date.today()
+        with self.assertRaises(ValueError):
+            await self.client.fetch_cm_post_archive(start_date, end_date, -1)
+
+    @aioresponses()
+    async def test_client_fetch_current_auctions(self, mock):
+        """Testing fetching the current auctions"""
+        content = self.load_resource(FILE_BAZAAR_CURRENT)
+        mock.get(get_bazaar_url(BazaarType.CURRENT), status=200, body=content)
+        response = await self.client.fetch_current_auctions()
+        self.assertIsInstance(response.data, CharacterBazaar)
+
+    async def test_client_fetch_current_auctions_invalid_page(self):
+        """Testing fetching the current auctions with an invalid page"""
+        with self.assertRaises(ValueError):
+            await self.client.fetch_current_auctions(-1)
+
+    @aioresponses()
+    async def test_client_fetch_auction_history(self, mock):
+        """Testing fetching the auction history"""
+        content = self.load_resource(FILE_BAZAAR_HISTORY)
+        mock.get(get_bazaar_url(BazaarType.HISTORY), status=200, body=content)
+        response = await self.client.fetch_auction_history()
+        self.assertIsInstance(response.data, CharacterBazaar)
+
+    async def test_client_fetch_auction_history_invalid_page(self):
+        """Testing fetching the auction history with an incorrect page"""
+        with self.assertRaises(ValueError):
+            await self.client.fetch_auction_history(-1)
+
+    @aioresponses()
+    async def test_client_fetch_auction(self, mock):
+        """Testing fetching an auction"""
+        content = self.load_resource(FILE_AUCTION_FINISHED)
+        mock.get(get_auction_url(134), status=200, body=content)
+        response = await self.client.fetch_auction(134)
+        self.assertIsInstance(response.data, Auction)
+
+    async def test_client_fetch_auction_invalid_id(self):
+        """Testing fetching an auction with an invalid id"""
+        with self.assertRaises(ValueError):
+            await self.client.fetch_auction(-1)
+
+    @aioresponses()
+    async def test_client_fetch_event_calendar(self, mock):
+        """Testing fetching the auction history"""
+        content = self.load_resource(FILE_EVENT_CALENDAR)
+        mock.get(get_event_schedule_url(), status=200, body=content)
+        response = await self.client.fetch_event_schedule()
+        self.assertIsInstance(response.data, EventSchedule)
+
+    async def test_client_fetch_event_calendar_invalid_params(self):
+        """Testing fetching the auction history"""
+        with self.assertRaises(ValueError):
+            await self.client.fetch_event_schedule(3)
+
+    @aioresponses()
+    async def test_client_fetch_forum_community_boards(self, mock):
+        """Testing fetching the community boards"""
+        content = self.load_resource(FILE_WORLD_BOARDS)
+        mock.get(BoardEntry.get_community_boards_url(), status=200, body=content)
+        response = await self.client.fetch_forum_community_boards()
+        self.assertIsInstance(response.data, ForumSection)
+
+    @aioresponses()
+    async def test_client_fetch_forum_trade_boards(self, mock):
+        """Testing fetching the trade boards"""
+        content = self.load_resource(FILE_WORLD_BOARDS)
+        mock.get(BoardEntry.get_trade_boards_url(), status=200, body=content)
+        response = await self.client.fetch_forum_trade_boards()
+        self.assertIsInstance(response.data, ForumSection)
+
+    @aioresponses()
+    async def test_client_fetch_forum_support_boards(self, mock):
+        """Testing fetching the support boards"""
+        content = self.load_resource(FILE_WORLD_BOARDS)
+        mock.get(BoardEntry.get_support_boards_url(), status=200, body=content)
+        response = await self.client.fetch_forum_support_boards()
+        self.assertIsInstance(response.data, ForumSection)
+
+    @aioresponses()
+    async def test_client_fetch_forum_world_boards(self, mock):
+        """Testing fetching the world boards"""
+        content = self.load_resource(FILE_WORLD_BOARDS)
+        mock.get(BoardEntry.get_world_boards_url(), status=200, body=content)
+        response = await self.client.fetch_forum_world_boards()
+        self.assertIsInstance(response.data, ForumSection)
+
+    @aioresponses()
+    async def test_client_fetch_forum_board(self, mock):
+        """Testing fetching a forum board"""
+        content = self.load_resource(FILE_BOARD_THREAD_LIST)
+        mock.get(get_forum_board_url(1), status=200, body=content)
+        response = await self.client.fetch_forum_board(1)
+        self.assertIsInstance(response.data, ForumBoard)
+
+    @aioresponses()
+    async def test_client_fetch_leaderboards(self, mock):
+        """Testing fetching the leaderboards"""
+        content = self.load_resource(FILE_LEADERBOARD_CURRENT)
+        mock.get(get_leaderboards_url("Antica"), status=200, body=content)
+        response = await self.client.fetch_leaderboard("Antica")
+        self.assertIsInstance(response.data, Leaderboard)
+
+    @unittest.mock.patch("tibiapy.parsers.bazaar.AuctionParser._parse_page_items")
+    @unittest.skipIf(sys.version_info < (3, 8, 0), "AsyncMock was implemented in 3.8")
+    async def test_client__fetch_all_pages_success(self, parse_page_items):
+        """Testing internal method to fetch all pages of an auction item collection."""
+        paginator = ItemSummary(page=1, total_pages=5)
+        self.client._fetch_ajax_page = unittest.mock.AsyncMock()
+
+        await self.client._fetch_all_pages(1, paginator, 1)
+
+        self.assertEqual(4, self.client._fetch_ajax_page.await_count)
+        self.assertEqual(4, parse_page_items.call_count)
```

### Comparing `tibia.py-5.6.1/tests/tests_creature.py` & `tibia.py-6.0.0a1/tests/tests_creature.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,111 +1,113 @@
-import unittest
-
-from tests.tests_tibiapy import TestCommons
-from tibiapy import BoostableBosses, InvalidContent, CreaturesSection, Creature, CreatureEntry
-
-FILE_CREATURE_SECTION = "library/creature_list.txt"
-FILE_CREATURE_CONVINCEABLE = "library/creature_convinceable.txt"
-FILE_CREATURE_ELEMENTAL_RESISTANCES = "library/creature_elemental_resistances.txt"
-FILE_BOOSTABLE_BOSSES = "library/boss_list.txt"
-
-
-class TestCreature(TestCommons, unittest.TestCase):
-    def test_creatures_section_from_boosted_creature_header_content(self):
-        """Testing parsing the boosted creture from any tibia.com page."""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        creature = CreaturesSection.boosted_creature_from_header(content)
-
-        self.assertIsInstance(creature, CreatureEntry)
-        self.assertEqual("Menacing Carnivor", creature.name)
-
-    def test_creatures_section_from_boosted_creature_header_content_not_tibiacom(self):
-        """Testing parsing the boosted creature from a page that is not Tibia.com"""
-        with self.assertRaises(InvalidContent):
-            CreaturesSection.boosted_creature_from_header("<html><div><p>Nothing</p></div></html>")
-
-    def test_creature_section_from_content(self):
-        """Test parsing the creatures section"""
-        content = self.load_resource(FILE_CREATURE_SECTION)
-        creatures = CreaturesSection.from_content(content)
-
-        self.assertIsNotNone(creatures)
-        self.assertIsNotNone(creatures.boosted_creature)
-        self.assertEqual("Blood Crab", creatures.boosted_creature.name)
-        self.assertEqual("bloodcrab", creatures.boosted_creature.identifier)
-        self.assertIsNotNone(creatures.boosted_creature.image_url)
-        self.assertIsNotNone(creatures.boosted_creature.url)
-        self.assertEqual(536, len(creatures.creatures))
-        for creature in creatures.creatures:
-            with self.subTest(name=creature.name):
-                self.assertIsInstance(creature.name, str)
-                self.assertIsInstance(creature.identifier, str)
-
-    def test_creatures_section_from_content_invalid_content(self):
-        """Testing parsing the creatures section from an invalid section"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(InvalidContent):
-            CreaturesSection.from_content(content)
-
-    def test_creature_from_content(self):
-        content = self.load_resource(FILE_CREATURE_CONVINCEABLE)
-        creature = Creature.from_content(content)
-
-        self.assertIsNotNone(creature)
-        self.assertEqual("Fish", creature.name)
-        self.assertEqual("fish", creature.identifier)
-        self.assertEqual(25, creature.hitpoints)
-        self.assertEqual(0, creature.experience)
-        self.assertEqual(0, creature.mana_cost)
-        self.assertFalse(creature.summonable)
-        self.assertTrue(creature.convinceable)
-        self.assertEqual("nothing", creature.loot)
-
-    def test_creature_from_content_elemental_resistances(self):
-        content = self.load_resource(FILE_CREATURE_ELEMENTAL_RESISTANCES)
-        creature = Creature.from_content(content)
-
-        self.assertIsNotNone(creature)
-        self.assertEqual("Dragons", creature.name)
-        self.assertEqual("dragon", creature.identifier)
-        self.assertEqual(1000, creature.hitpoints)
-        self.assertEqual(700, creature.experience)
-        self.assertIsNone(creature.mana_cost)
-        self.assertFalse(creature.summonable)
-        self.assertFalse(creature.convinceable)
-        self.assertIsNotNone(creature.description)
-        self.assertIn("energy", creature.strong_against)
-        self.assertIn("fire", creature.immune_to)
-        self.assertIn("ice", creature.weak_against)
-
-    def test_creature_from_content_invalid_content(self):
-        """Testing parsing the creatures section from an invalid section"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-
-        creature = Creature.from_content(content)
-
-        self.assertIsNone(creature)
-
-    def test_boostable_bosses_from_content(self):
-        """Test parsing the boostable bosses section"""
-        content = self.load_resource(FILE_BOOSTABLE_BOSSES)
-        bosses = BoostableBosses.from_content(content)
-
-        self.assertIsNotNone(bosses)
-        self.assertIsNotNone(bosses.boosted_boss)
-        self.assertEqual("Tentugly", bosses.boosted_boss.name)
-        self.assertEqual("fakeseamonster", bosses.boosted_boss.identifier)
-        self.assertIsNotNone(bosses.boosted_boss.image_url)
-        self.assertEqual(88, len(bosses.bosses))
-        for boss in bosses.bosses:
-            with self.subTest(name=boss.name):
-                self.assertIsInstance(boss.name, str)
-                self.assertIsInstance(boss.identifier, str)
-
-    def test_boostable_bosses_from_content_invalid_content(self):
-        """Testing parsing the creatures section from an invalid section"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-
-        with self.assertRaises(InvalidContent):
-            BoostableBosses.from_content(content)
-
-
+import unittest
+
+from tests.tests_tibiapy import TestCommons
+from tibiapy import InvalidContent
+from tibiapy.models.creature import CreatureEntry
+from tibiapy.parsers.creature import CreaturesSectionParser, CreatureParser, BoostableBossesParser
+
+FILE_CREATURE_SECTION = "library/creature_list.txt"
+FILE_CREATURE_CONVINCEABLE = "library/creature_convinceable.txt"
+FILE_CREATURE_ELEMENTAL_RESISTANCES = "library/creature_elemental_resistances.txt"
+FILE_BOOSTABLE_BOSSES = "library/boss_list.txt"
+
+
+class TestCreature(TestCommons, unittest.TestCase):
+    def test_creatures_section_from_boosted_creature_header_content(self):
+        """Testing parsing the boosted creture from any tibia.com page."""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        creature = CreaturesSectionParser.boosted_creature_from_header(content)
+
+        self.assertIsInstance(creature, CreatureEntry)
+        self.assertEqual("Menacing Carnivor", creature.name)
+
+    def test_creatures_section_from_boosted_creature_header_content_not_tibiacom(self):
+        """Testing parsing the boosted creature from a page that is not Tibia.com"""
+        with self.assertRaises(InvalidContent):
+            CreaturesSectionParser.boosted_creature_from_header("<html><div><p>Nothing</p></div></html>")
+
+    def test_creature_section_from_content(self):
+        """Test parsing the creatures section"""
+        content = self.load_resource(FILE_CREATURE_SECTION)
+        creatures = CreaturesSectionParser.from_content(content)
+
+        self.assertIsNotNone(creatures)
+        self.assertIsNotNone(creatures.boosted_creature)
+        self.assertEqual("Blood Crab", creatures.boosted_creature.name)
+        self.assertEqual("bloodcrab", creatures.boosted_creature.identifier)
+        self.assertIsNotNone(creatures.boosted_creature.image_url)
+        self.assertIsNotNone(creatures.boosted_creature.url)
+        self.assertEqual(536, len(creatures.creatures))
+        for creature in creatures.creatures:
+            with self.subTest(name=creature.name):
+                self.assertIsInstance(creature.name, str)
+                self.assertIsInstance(creature.identifier, str)
+
+    def test_creatures_section_from_content_invalid_content(self):
+        """Testing parsing the creatures section from an invalid section"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(InvalidContent):
+            CreaturesSectionParser.from_content(content)
+
+    def test_creature_from_content(self):
+        content = self.load_resource(FILE_CREATURE_CONVINCEABLE)
+        creature = CreatureParser.from_content(content)
+
+        self.assertIsNotNone(creature)
+        self.assertEqual("Fish", creature.name)
+        self.assertEqual("fish", creature.identifier)
+        self.assertEqual(25, creature.hitpoints)
+        self.assertEqual(0, creature.experience)
+        self.assertEqual(0, creature.mana_cost)
+        self.assertFalse(creature.summonable)
+        self.assertTrue(creature.convinceable)
+        self.assertEqual("nothing", creature.loot)
+
+    def test_creature_from_content_elemental_resistances(self):
+        content = self.load_resource(FILE_CREATURE_ELEMENTAL_RESISTANCES)
+        creature = CreatureParser.from_content(content)
+
+        self.assertIsNotNone(creature)
+        self.assertEqual("Dragons", creature.name)
+        self.assertEqual("dragon", creature.identifier)
+        self.assertEqual(1000, creature.hitpoints)
+        self.assertEqual(700, creature.experience)
+        self.assertIsNone(creature.mana_cost)
+        self.assertFalse(creature.summonable)
+        self.assertFalse(creature.convinceable)
+        self.assertIsNotNone(creature.description)
+        self.assertIn("energy", creature.strong_against)
+        self.assertIn("fire", creature.immune_to)
+        self.assertIn("ice", creature.weak_against)
+
+    def test_creature_from_content_invalid_content(self):
+        """Testing parsing the creatures section from an invalid section"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+
+        creature = CreatureParser.from_content(content)
+
+        self.assertIsNone(creature)
+
+    def test_boostable_bosses_from_content(self):
+        """Test parsing the boostable bosses section"""
+        content = self.load_resource(FILE_BOOSTABLE_BOSSES)
+        bosses = BoostableBossesParser.from_content(content)
+
+        self.assertIsNotNone(bosses)
+        self.assertIsNotNone(bosses.boosted_boss)
+        self.assertEqual("Tentugly", bosses.boosted_boss.name)
+        self.assertEqual("fakeseamonster", bosses.boosted_boss.identifier)
+        self.assertIsNotNone(bosses.boosted_boss.image_url)
+        self.assertEqual(88, len(bosses.bosses))
+        for boss in bosses.bosses:
+            with self.subTest(name=boss.name):
+                self.assertIsInstance(boss.name, str)
+                self.assertIsInstance(boss.identifier, str)
+
+    def test_boostable_bosses_from_content_invalid_content(self):
+        """Testing parsing the creatures section from an invalid section"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+
+        with self.assertRaises(InvalidContent):
+            BoostableBossesParser.from_content(content)
+
+
```

### Comparing `tibia.py-5.6.1/tests/tests_forums.py` & `tibia.py-6.0.0a1/tests/tests_forums.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,321 +1,328 @@
-import datetime
-import unittest
-
-import tibiapy
-from tests.tests_tibiapy import TestCommons
-from tibiapy import CMPostArchive, ForumAnnouncement, ForumBoard, ForumThread, InvalidContent, LastPost, BoardEntry, \
-    ThreadEntry, ThreadStatus
-
-FILE_WORLD_BOARDS = "forums/tibiacom_section.txt"
-FILE_SECTION_EMPTY_BOARD = "forums/tibiacom_section_empty_board.txt"
-FILE_SECTION_EMPTY = "forums/tibiacom_section_empty.txt"
-FILE_BOARD_THREAD_LIST = "forums/tibiacom_board.txt"
-FILE_BOARD_EMPTY_THREAD_LIST = "forums/tibiacom_board_empty.txt"
-FILE_BOARD_INVALID_PAGE = "forums/tibiacom_board_invalid_page.txt"
-FILE_BOARD_GOLDEN_FRAMES = "forums/tibiacom_board_golden_frame.txt"
-FILE_ANNOUNCEMENT = "forums/tibiacom_announcement.txt"
-FILE_ANNOUNCEMENT_NOT_FOUND = "forums/tibiacom_announcement_not_found.txt"
-FILE_THREAD = "forums/tibiacom_thread.txt"
-FILE_THREAD_NOT_FOUND = "forums/tibiacom_thread_not_found.txt"
-FILE_THREAD_INVALID_PAGE = "forums/tibiacom_thread_invalid_page.txt"
-FILE_CM_POST_ARCHIVE_INITIAL = "forums/tibiacom_cmpostarchive_initial.txt"
-FILE_CM_POST_ARCHIVE_NO_PAGES = "forums/tibiacom_cmpostarchive_no_pages.txt"
-FILE_CM_POST_ARCHIVE_NO_RESULTS = "forums/tibiacom_cmpostarchive_no_results.txt"
-FILE_CM_POST_ARCHIVE_PAGES = "forums/tibiacom_cmpostarchive_pages.txt"
-
-
-class TestForum(TestCommons, unittest.TestCase):
-    def test_listed_board_list_from_content_world_boards(self):
-        content = self.load_resource(FILE_WORLD_BOARDS)
-
-        boards = BoardEntry.list_from_content(content)
-
-        self.assertEqual(82, len(boards))
-        for i, board in enumerate(boards):
-            with self.subTest(i=i):
-                self.assertIsInstance(board, BoardEntry)
-                self.assertIsNotNone(board.name)
-                self.assertGreater(board.board_id, 0)
-                self.assertGreater(board.posts, 0)
-                self.assertGreater(board.threads, 0)
-                self.assertIsInstance(board.last_post, LastPost)
-
-    def test_listed_board_list_from_content_empty_board(self):
-        content = self.load_resource(FILE_SECTION_EMPTY_BOARD)
-
-        boards = BoardEntry.list_from_content(content)
-
-        self.assertEqual(84, len(boards))
-        for i, board in enumerate(boards):
-            with self.subTest(i=i):
-                self.assertIsInstance(board, BoardEntry)
-                self.assertIsNotNone(board.name)
-                self.assertGreater(board.board_id, 0)
-                self.assertGreaterEqual(board.posts, 0)
-                self.assertGreaterEqual(board.threads, 0)
-                self.assertIsNotNone(board.url)
-
-    def test_listed_board_list_from_content_empty_section(self):
-        content = self.load_resource(FILE_SECTION_EMPTY)
-
-        boards = BoardEntry.list_from_content(content)
-
-        self.assertIsInstance(boards, list)
-
-    def test_listed_board_list_from_content_unrelated_section(self):
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-
-        with self.assertRaises(InvalidContent):
-            BoardEntry.list_from_content(content)
-
-    def test_forum_board_from_content(self):
-        content = self.load_resource(FILE_BOARD_THREAD_LIST)
-
-        board = ForumBoard.from_content(content)
-
-        self.assertIsNotNone(board)
-        self.assertEqual("Antica", board.name)
-        self.assertEqual("World Boards", board.section)
-        self.assertEqual(1, board.page)
-        self.assertEqual(2, board.total_pages)
-        self.assertEqual(25, board.board_id)
-        self.assertEqual(30, len(board.threads))
-        self.assertIsNotNone(board.url)
-        self.assertIsNotNone(board.next_page_url)
-        self.assertEqual(board.next_page_url, BoardEntry.get_url(board.board_id, board.page + 1, board.age))
-        for i, thread in enumerate(board.threads):
-            with self.subTest(i=i):
-                self.assertIsInstance(thread, ThreadEntry)
-                self.assertIsNotNone(thread.title)
-                self.assertGreater(thread.thread_id, 0)
-                self.assertGreaterEqual(thread.views, 0)
-                self.assertGreaterEqual(thread.replies, 0)
-                self.assertIsInstance(thread.last_post, LastPost)
-                self.assertIsNotNone(thread.last_post.author_url)
-
-        with self.assertRaises(ValueError):
-            board.get_page_url(-1)
-
-    def test_board_section_urls(self):
-        self.assertIsNotNone(BoardEntry.get_community_boards_url())
-        self.assertIsNotNone(BoardEntry.get_support_boards_url())
-        self.assertIsNotNone(BoardEntry.get_world_boards_url())
-        self.assertIsNotNone(BoardEntry.get_trade_boards_url())
-
-    def test_forum_board_from_content_empty_threads(self):
-        content = self.load_resource(FILE_BOARD_EMPTY_THREAD_LIST)
-
-        board = ForumBoard.from_content(content)
-
-        self.assertIsNotNone(board)
-        self.assertEqual("Role Playing", board.name)
-        self.assertEqual("Community Boards", board.section)
-        self.assertEqual(1, board.page)
-        self.assertEqual(1, board.total_pages)
-        self.assertEqual(11, board.board_id)
-        self.assertEqual(0, len(board.threads))
-        self.assertIsNone(board.next_page_url)
-        self.assertIsNone(board.previous_page_url)
-
-    def test_forum_board_from_content_unrelated_section(self):
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-
-        with self.assertRaises(InvalidContent):
-            ForumBoard.from_content(content)
-
-    def test_forum_board_from_content_invalid_page(self):
-        content = self.load_resource(FILE_BOARD_INVALID_PAGE)
-
-        board = ForumBoard.from_content(content)
-
-        self.assertEqual("Antica", board.name)
-        self.assertEqual("World Boards", board.section)
-        self.assertEqual([], board.threads)
-        self.assertEqual(0, board.board_id)
-
-    def test_forum_board_from_content_golden_frame(self):
-        content = self.load_resource(FILE_BOARD_GOLDEN_FRAMES)
-
-        board = ForumBoard.from_content(content)
-
-        self.assertEqual("Proposals (English Only)", board.name)
-        self.assertEqual("Community Boards", board.section)
-        self.assertEqual(30, len(board.threads))
-        self.assertEqual(5, len(board.announcements))
-        self.assertEqual(1893, board.total_pages)
-        for i, thread in enumerate(board.threads):
-            with self.subTest(i=i):
-                self.assertTrue(thread.golden_frame)
-                self.assertTrue(thread.status & ThreadStatus.HOT)
-                self.assertTrue(thread.status & ThreadStatus.CLOSED)
-                self.assertIsNotNone(thread.url)
-
-    def test_forum_announcement_from_content(self):
-        content = self.load_resource(FILE_ANNOUNCEMENT)
-
-        announcement = ForumAnnouncement.from_content(content, 33)
-
-        self.assertIsNotNone(announcement)
-        self.assertEqual("Legal Disclaimer", announcement.title)
-        self.assertEqual(33, announcement.announcement_id)
-        self.assertEqual("Proposals (English Only)", announcement.board)
-        self.assertEqual(10, announcement.board_id)
-        self.assertEqual("Community Boards", announcement.section)
-        self.assertEqual(12, announcement.section_id)
-        self.assertIsNotNone(announcement.author)
-        self.assertEqual("CM Mirade", announcement.author.name)
-        self.assertEqual(2, announcement.author.level)
-        self.assertEqual(159, announcement.author.posts)
-        self.assertEqual("Vunira", announcement.author.world)
-        self.assertEqual("Community Manager", announcement.author.position)
-        self.assertIsNotNone(announcement.url)
-
-    def test_forum_announcement_from_content_not_found(self):
-        content = self.load_resource(FILE_ANNOUNCEMENT_NOT_FOUND)
-
-        announcement = ForumAnnouncement.from_content(content, 34)
-
-        self.assertIsNone(announcement)
-
-    def test_forum_announcement_from_content_unrelated_section(self):
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-
-        with self.assertRaises(InvalidContent):
-            ForumAnnouncement.from_content(content, 34)
-
-    def test_forum_thread_from_content(self):
-        content = self.load_resource(FILE_THREAD)
-
-        thread = ForumThread.from_content(content)
-
-        self.assertEqual("News: Team Finder, Visualisation of Loot Lists", thread.title)
-        self.assertEqual(4797985, thread.thread_id)
-        self.assertEqual('Auditorium (English Only)', thread.board)
-        self.assertEqual('Community Boards', thread.section)
-        self.assertEqual(4796826, thread.previous_topic_number)
-        self.assertEqual(4797838, thread.next_topic_number)
-        self.assertEqual(1, thread.page)
-        self.assertEqual(9, thread.total_pages)
-        self.assertEqual(20, len(thread.posts))
-        self.assertIsNotNone(thread.url)
-        self.assertIsNone(thread.previous_page_url)
-        self.assertIsNotNone(thread.next_page_url)
-        self.assertIsNotNone(thread.previous_thread_url)
-        self.assertIsNotNone(thread.next_thread_url)
-
-        post = thread.posts[0]
-        self.assertEqual("Skerio", post.author.name)
-        self.assertEqual("Olima", post.author.world)
-        self.assertEqual("Community Manager", post.author.position)
-        self.assertEqual(872, post.author.posts)
-        self.assertEqual("Mirade", post.edited_by)
-        self.assertTrue(post.golden_frame)
-        self.assertEqual(38969385, post.post_id)
-        self.assertIsNotNone(post.url)
-
-        with self.assertRaises(ValueError):
-            thread.get_page_url(-1)
-
-    def test_forum_thread_from_content_invalid_page(self):
-        content = self.load_resource(FILE_THREAD_INVALID_PAGE)
-
-        thread = ForumThread.from_content(content)
-
-        self.assertEqual("News: Te...", thread.title)
-        self.assertEqual(0, thread.thread_id)
-        self.assertEqual('Auditorium (English Only)', thread.board)
-        self.assertEqual('Community Boards', thread.section)
-        self.assertEqual(0, thread.previous_topic_number)
-        self.assertEqual(0, thread.next_topic_number)
-        self.assertEqual(1, thread.page)
-        self.assertEqual(1, thread.total_pages)
-        self.assertEqual(0, len(thread.posts))
-
-    def test_forum_thread_from_content_not_found(self):
-        content = self.load_resource(FILE_THREAD_NOT_FOUND)
-
-        thread = ForumThread.from_content(content)
-
-        self.assertIsNone(thread)
-
-    def test_forum_thread_from_content_unrelated_section(self):
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-
-        with self.assertRaises(InvalidContent):
-            ForumThread.from_content(content)
-
-    def test_cm_post_archive_from_content_initial(self):
-        content = self.load_resource(FILE_CM_POST_ARCHIVE_INITIAL)
-
-        cm_post_archive = CMPostArchive.from_content(content)
-
-        self.assertIsNotNone(cm_post_archive)
-        self.assertEqual(0, cm_post_archive.results_count)
-        self.assertEqual(1, cm_post_archive.page)
-        self.assertEqual(1, cm_post_archive.total_pages)
-
-    def test_cm_post_archive_from_content_no_pages(self):
-        content = self.load_resource(FILE_CM_POST_ARCHIVE_NO_PAGES)
-
-        cm_post_archive = CMPostArchive.from_content(content)
-
-        self.assertIsNotNone(cm_post_archive)
-        self.assertEqual(5, cm_post_archive.results_count)
-        self.assertEqual(1, cm_post_archive.page)
-        self.assertEqual(1, cm_post_archive.total_pages)
-        self.assertEqual(cm_post_archive.results_count, len(cm_post_archive.posts))
-
-        post = cm_post_archive.posts[0]
-        self.assertIsInstance(post, tibiapy.abc.BasePost)
-        self.assertEqual('Auditorium (English Only)', post.board)
-        self.assertEqual(38974254, post.post_id)
-        self.assertEqual('Ticker Messages June 2020', post.thread_title)
-
-    def test_cm_post_archive_from_content_no_results(self):
-        content = self.load_resource(FILE_CM_POST_ARCHIVE_NO_RESULTS)
-
-        cm_post_archive = CMPostArchive.from_content(content)
-
-        self.assertIsNotNone(cm_post_archive)
-        self.assertEqual(0, cm_post_archive.results_count)
-        self.assertEqual(1, cm_post_archive.page)
-        self.assertEqual(1, cm_post_archive.total_pages)
-        self.assertEqual(cm_post_archive.results_count, len(cm_post_archive.posts))
-
-    def test_cm_post_archive_from_content_pages(self):
-        content = self.load_resource(FILE_CM_POST_ARCHIVE_PAGES)
-
-        cm_post_archive = CMPostArchive.from_content(content)
-
-        self.assertIsNotNone(cm_post_archive)
-        self.assertIsNotNone(cm_post_archive.url)
-        self.assertIsNotNone(cm_post_archive.previous_page_url)
-        self.assertIsNone(cm_post_archive.next_page_url)
-        self.assertEqual(8370, cm_post_archive.results_count)
-        self.assertEqual(168, cm_post_archive.page)
-        self.assertEqual(168, cm_post_archive.total_pages)
-        self.assertEqual(20, len(cm_post_archive.posts))
-
-    def test_cm_post_archive_from_content_unrelated_section(self):
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(InvalidContent):
-            CMPostArchive.from_content(content)
-
-    def test_cm_post_archive_get_page_url_negative_page(self):
-        with self.assertRaises(ValueError):
-            cmpost_archive = CMPostArchive()
-            cmpost_archive.get_page_url(-1)
-
-    def test_cm_post_archive_get_url_missing_parameter(self):
-        with self.assertRaises(TypeError):
-            CMPostArchive.get_url(None, datetime.date.today())
-        with self.assertRaises(TypeError):
-            CMPostArchive.get_url(datetime.date.today(), None)
-
-    def test_cm_post_archive_get_url_invalid_dates(self):
-        with self.assertRaises(ValueError):
-            CMPostArchive.get_url(datetime.date.today(), datetime.date.today()-datetime.timedelta(days=20))
-
-    def test_cm_post_archive_get_url_invalid_page(self):
-        with self.assertRaises(ValueError):
-            CMPostArchive.get_url(datetime.date.today()-datetime.timedelta(days=20), datetime.date.today(), -2)
+import datetime
+import unittest
+
+from tests.tests_tibiapy import TestCommons
+from tibiapy import InvalidContent, ThreadStatus
+from tibiapy.models import BoardEntry, LastPost, ThreadEntry, CMPostArchive
+from tibiapy.models.forum import BasePost, ForumSection
+from tibiapy.parsers.forum import ForumBoardParser, ForumAnnouncementParser, ForumThreadParser, \
+    CMPostArchiveParser, ForumSectionParser
+from tibiapy.urls import get_forum_board_url, get_cm_post_archive_url
+
+FILE_WORLD_BOARDS = "forums/tibiacom_section.txt"
+FILE_SECTION_EMPTY_BOARD = "forums/tibiacom_section_empty_board.txt"
+FILE_SECTION_EMPTY = "forums/tibiacom_section_empty.txt"
+FILE_BOARD_THREAD_LIST = "forums/tibiacom_board.txt"
+FILE_BOARD_EMPTY_THREAD_LIST = "forums/tibiacom_board_empty.txt"
+FILE_BOARD_INVALID_PAGE = "forums/tibiacom_board_invalid_page.txt"
+FILE_BOARD_GOLDEN_FRAMES = "forums/tibiacom_board_golden_frame.txt"
+FILE_ANNOUNCEMENT = "forums/tibiacom_announcement.txt"
+FILE_ANNOUNCEMENT_NOT_FOUND = "forums/tibiacom_announcement_not_found.txt"
+FILE_THREAD = "forums/tibiacom_thread.txt"
+FILE_THREAD_NOT_FOUND = "forums/tibiacom_thread_not_found.txt"
+FILE_THREAD_INVALID_PAGE = "forums/tibiacom_thread_invalid_page.txt"
+FILE_CM_POST_ARCHIVE_INITIAL = "forums/tibiacom_cmpostarchive_initial.txt"
+FILE_CM_POST_ARCHIVE_NO_PAGES = "forums/tibiacom_cmpostarchive_no_pages.txt"
+FILE_CM_POST_ARCHIVE_NO_RESULTS = "forums/tibiacom_cmpostarchive_no_results.txt"
+FILE_CM_POST_ARCHIVE_PAGES = "forums/tibiacom_cmpostarchive_pages.txt"
+
+
+class TestForum(TestCommons, unittest.TestCase):
+    def test_forum_section_parser_from_content_world_boards(self):
+        content = self.load_resource(FILE_WORLD_BOARDS)
+
+        forum_section = ForumSectionParser.from_content(content)
+
+        self.assertEqual(2, forum_section.section_id)
+        self.assertEqual(82, len(forum_section.entries))
+        for i, board in enumerate(forum_section.entries):
+            with self.subTest(i=i):
+                self.assertIsInstance(board, BoardEntry)
+                self.assertIsNotNone(board.name)
+                self.assertGreater(board.board_id, 0)
+                self.assertGreater(board.posts, 0)
+                self.assertGreater(board.threads, 0)
+                self.assertIsInstance(board.last_post, LastPost)
+
+    def test_forum_section_parser_from_content_empty_board(self):
+        content = self.load_resource(FILE_SECTION_EMPTY_BOARD)
+
+        forum_section = ForumSectionParser.from_content(content)
+
+        self.assertEqual(3, forum_section.section_id)
+        self.assertEqual(84, len(forum_section.entries))
+        for i, board in enumerate(forum_section.entries):
+            with self.subTest(i=i):
+                self.assertIsInstance(board, BoardEntry)
+                self.assertIsNotNone(board.name)
+                self.assertGreater(board.board_id, 0)
+                self.assertGreaterEqual(board.posts, 0)
+                self.assertGreaterEqual(board.threads, 0)
+                self.assertIsNotNone(board.url)
+
+    def test_forum_section_parser_from_content_empty_section(self):
+        content = self.load_resource(FILE_SECTION_EMPTY)
+
+        forum_section = ForumSectionParser.from_content(content)
+
+        self.assertEqual(10, forum_section.section_id)
+        self.assertIsInstance(forum_section, ForumSection)
+        self.assertEqual(0, len(forum_section.entries))
+
+    def test_forum_section_parser_from_content_unrelated_section(self):
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+
+        with self.assertRaises(InvalidContent):
+            ForumSectionParser.from_content(content)
+
+    def test_forum_board_from_content(self):
+        content = self.load_resource(FILE_BOARD_THREAD_LIST)
+
+        board = ForumBoardParser.from_content(content)
+
+        self.assertIsNotNone(board)
+        self.assertEqual("Antica", board.name)
+        self.assertEqual("World Boards", board.section)
+        self.assertEqual(1, board.current_page)
+        self.assertEqual(2, board.total_pages)
+        self.assertEqual(25, board.board_id)
+        self.assertEqual(30, len(board.entries))
+        self.assertIsNotNone(board.url)
+        self.assertIsNotNone(board.next_page_url)
+        self.assertEqual(board.next_page_url, get_forum_board_url(board.board_id, board.current_page + 1, board.age))
+        for i, thread in enumerate(board.entries):
+            with self.subTest(i=i):
+                self.assertIsInstance(thread, ThreadEntry)
+                self.assertIsNotNone(thread.title)
+                self.assertGreater(thread.thread_id, 0)
+                self.assertGreaterEqual(thread.views, 0)
+                self.assertGreaterEqual(thread.replies, 0)
+                self.assertIsInstance(thread.last_post, LastPost)
+                self.assertIsNotNone(thread.last_post.author_url)
+
+        with self.assertRaises(ValueError):
+            board.get_page_url(-1)
+
+    def test_board_section_urls(self):
+        self.assertIsNotNone(BoardEntry.get_community_boards_url())
+        self.assertIsNotNone(BoardEntry.get_support_boards_url())
+        self.assertIsNotNone(BoardEntry.get_world_boards_url())
+        self.assertIsNotNone(BoardEntry.get_trade_boards_url())
+
+    def test_forum_board_from_content_empty_threads(self):
+        content = self.load_resource(FILE_BOARD_EMPTY_THREAD_LIST)
+
+        board = ForumBoardParser.from_content(content)
+
+        self.assertIsNotNone(board)
+        self.assertEqual("Role Playing", board.name)
+        self.assertEqual("Community Boards", board.section)
+        self.assertEqual(1, board.current_page)
+        self.assertEqual(1, board.total_pages)
+        self.assertEqual(11, board.board_id)
+        self.assertEqual(0, len(board.entries))
+        self.assertIsNone(board.next_page_url)
+        self.assertIsNone(board.previous_page_url)
+
+    def test_forum_board_from_content_unrelated_section(self):
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+
+        with self.assertRaises(InvalidContent):
+            ForumBoardParser.from_content(content)
+
+    def test_forum_board_from_content_invalid_page(self):
+        content = self.load_resource(FILE_BOARD_INVALID_PAGE)
+
+        board = ForumBoardParser.from_content(content)
+
+        self.assertEqual("Antica", board.name)
+        self.assertEqual("World Boards", board.section)
+        self.assertEqual([], board.entries)
+        self.assertEqual(0, board.board_id)
+
+    def test_forum_board_from_content_golden_frame(self):
+        content = self.load_resource(FILE_BOARD_GOLDEN_FRAMES)
+
+        board = ForumBoardParser.from_content(content)
+
+        self.assertEqual("Proposals (English Only)", board.name)
+        self.assertEqual("Community Boards", board.section)
+        self.assertEqual(30, len(board.entries))
+        self.assertEqual(5, len(board.announcements))
+        self.assertEqual(1893, board.total_pages)
+        for i, thread in enumerate(board.entries):
+            with self.subTest(i=i):
+                self.assertTrue(thread.golden_frame)
+                self.assertTrue(thread.status & ThreadStatus.HOT)
+                self.assertTrue(thread.status & ThreadStatus.CLOSED)
+                self.assertIsNotNone(thread.url)
+
+    def test_forum_announcement_from_content(self):
+        content = self.load_resource(FILE_ANNOUNCEMENT)
+
+        announcement = ForumAnnouncementParser.from_content(content, 33)
+
+        self.assertIsNotNone(announcement)
+        self.assertEqual("Legal Disclaimer", announcement.title)
+        self.assertEqual(33, announcement.announcement_id)
+        self.assertEqual("Proposals (English Only)", announcement.board)
+        self.assertEqual(10, announcement.board_id)
+        self.assertEqual("Community Boards", announcement.section)
+        self.assertEqual(12, announcement.section_id)
+        self.assertIsNotNone(announcement.author)
+        self.assertEqual("CM Mirade", announcement.author.name)
+        self.assertEqual(2, announcement.author.level)
+        self.assertEqual(159, announcement.author.posts)
+        self.assertEqual("Vunira", announcement.author.world)
+        self.assertEqual("Community Manager", announcement.author.position)
+        self.assertIsNotNone(announcement.url)
+
+    def test_forum_announcement_from_content_not_found(self):
+        content = self.load_resource(FILE_ANNOUNCEMENT_NOT_FOUND)
+
+        announcement = ForumAnnouncementParser.from_content(content, 34)
+
+        self.assertIsNone(announcement)
+
+    def test_forum_announcement_from_content_unrelated_section(self):
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+
+        with self.assertRaises(InvalidContent):
+            ForumAnnouncementParser.from_content(content, 34)
+
+    def test_forum_thread_from_content(self):
+        content = self.load_resource(FILE_THREAD)
+
+        thread = ForumThreadParser.from_content(content)
+
+        self.assertEqual("News: Team Finder, Visualisation of Loot Lists", thread.title)
+        self.assertEqual(4797985, thread.thread_id)
+        self.assertEqual('Auditorium (English Only)', thread.board)
+        self.assertEqual('Community Boards', thread.section)
+        self.assertEqual(4796826, thread.previous_topic_number)
+        self.assertEqual(4797838, thread.next_topic_number)
+        self.assertEqual(1, thread.current_page)
+        self.assertEqual(9, thread.total_pages)
+        self.assertEqual(20, len(thread.entries))
+        self.assertIsNotNone(thread.url)
+        self.assertIsNone(thread.previous_page_url)
+        self.assertIsNotNone(thread.next_page_url)
+        self.assertIsNotNone(thread.previous_thread_url)
+        self.assertIsNotNone(thread.next_thread_url)
+
+        post = thread.entries[0]
+        self.assertEqual("Skerio", post.author.name)
+        self.assertEqual("Olima", post.author.world)
+        self.assertEqual("Community Manager", post.author.position)
+        self.assertEqual(872, post.author.posts)
+        self.assertEqual("Mirade", post.edited_by)
+        self.assertTrue(post.golden_frame)
+        self.assertEqual(38969385, post.post_id)
+        self.assertIsNotNone(post.url)
+
+        with self.assertRaises(ValueError):
+            thread.get_page_url(-1)
+
+    def test_forum_thread_from_content_invalid_page(self):
+        content = self.load_resource(FILE_THREAD_INVALID_PAGE)
+
+        thread = ForumThreadParser.from_content(content)
+
+        self.assertEqual("News: Te...", thread.title)
+        self.assertEqual(0, thread.thread_id)
+        self.assertEqual('Auditorium (English Only)', thread.board)
+        self.assertEqual('Community Boards', thread.section)
+        self.assertIsNone(thread.previous_topic_number)
+        self.assertIsNone(thread.next_topic_number)
+        self.assertEqual(1, thread.current_page)
+        self.assertEqual(1, thread.total_pages)
+        self.assertEqual(0, len(thread.entries))
+
+    def test_forum_thread_from_content_not_found(self):
+        content = self.load_resource(FILE_THREAD_NOT_FOUND)
+
+        thread = ForumThreadParser.from_content(content)
+
+        self.assertIsNone(thread)
+
+    def test_forum_thread_from_content_unrelated_section(self):
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+
+        with self.assertRaises(InvalidContent):
+            ForumThreadParser.from_content(content)
+
+    def test_cm_post_archive_from_content_initial(self):
+        content = self.load_resource(FILE_CM_POST_ARCHIVE_INITIAL)
+
+        cm_post_archive = CMPostArchiveParser.from_content(content)
+
+        self.assertIsNotNone(cm_post_archive)
+        self.assertEqual(0, cm_post_archive.results_count)
+        self.assertEqual(1, cm_post_archive.current_page)
+        self.assertEqual(1, cm_post_archive.total_pages)
+
+    def test_cm_post_archive_from_content_no_pages(self):
+        content = self.load_resource(FILE_CM_POST_ARCHIVE_NO_PAGES)
+
+        cm_post_archive = CMPostArchiveParser.from_content(content)
+
+        self.assertIsNotNone(cm_post_archive)
+        self.assertEqual(5, cm_post_archive.results_count)
+        self.assertEqual(1, cm_post_archive.current_page)
+        self.assertEqual(1, cm_post_archive.total_pages)
+        self.assertEqual(cm_post_archive.results_count, len(cm_post_archive.entries))
+
+        post = cm_post_archive.entries[0]
+        self.assertIsInstance(post, BasePost)
+        self.assertEqual('Auditorium (English Only)', post.board)
+        self.assertEqual(38974254, post.post_id)
+        self.assertEqual('Ticker Messages June 2020', post.thread_title)
+
+    def test_cm_post_archive_from_content_no_results(self):
+        content = self.load_resource(FILE_CM_POST_ARCHIVE_NO_RESULTS)
+
+        cm_post_archive = CMPostArchiveParser.from_content(content)
+
+        self.assertIsNotNone(cm_post_archive)
+        self.assertEqual(0, cm_post_archive.results_count)
+        self.assertEqual(1, cm_post_archive.current_page)
+        self.assertEqual(1, cm_post_archive.total_pages)
+        self.assertEqual(cm_post_archive.results_count, len(cm_post_archive.entries))
+
+    def test_cm_post_archive_from_content_pages(self):
+        content = self.load_resource(FILE_CM_POST_ARCHIVE_PAGES)
+
+        cm_post_archive = CMPostArchiveParser.from_content(content)
+
+        self.assertIsNotNone(cm_post_archive)
+        self.assertIsNotNone(cm_post_archive.url)
+        self.assertIsNotNone(cm_post_archive.previous_page_url)
+        self.assertIsNone(cm_post_archive.next_page_url)
+        self.assertEqual(8370, cm_post_archive.results_count)
+        self.assertEqual(168, cm_post_archive.current_page)
+        self.assertEqual(168, cm_post_archive.total_pages)
+        self.assertEqual(20, len(cm_post_archive.entries))
+
+    def test_cm_post_archive_from_content_unrelated_section(self):
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(InvalidContent):
+            CMPostArchiveParser.from_content(content)
+
+    def test_cm_post_archive_get_page_url_negative_page(self):
+        with self.assertRaises(ValueError):
+            cmpost_archive = CMPostArchive()
+            cmpost_archive.get_page_url(-1)
+
+    def test_cm_post_archive_get_url_missing_parameter(self):
+        with self.assertRaises(TypeError):
+            get_cm_post_archive_url(None, datetime.date.today())
+        with self.assertRaises(TypeError):
+            get_cm_post_archive_url(datetime.date.today(), None)
+
+    def test_cm_post_archive_get_url_invalid_dates(self):
+        with self.assertRaises(ValueError):
+            get_cm_post_archive_url(datetime.date.today(), datetime.date.today()-datetime.timedelta(days=20))
+
+    def test_cm_post_archive_get_url_invalid_page(self):
+        with self.assertRaises(ValueError):
+            get_cm_post_archive_url(datetime.date.today()-datetime.timedelta(days=20), datetime.date.today(), -2)
```

### Comparing `tibia.py-5.6.1/tests/tests_guild.py` & `tibia.py-6.0.0a1/tests/tests_guild.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,271 +1,231 @@
-import datetime
-import unittest
-
-from tests.tests_tibiapy import TestCommons
-from tibiapy import Guild, GuildHouse, GuildInvite, GuildMember, GuildWars, GuildsSection, InvalidContent, GuildEntry
-
-FILE_GUILD_FULL = "guild/tibiacom_full.txt"
-FILE_GUILD_NOT_FOUND = "guild/tibiacom_not_found.txt"
-FILE_GUILD_INFO_COMPLETE = "guild/tibiacom_info_complete.txt"
-FILE_GUILD_INFO_MINIMUM = "guild/tibiacom_info_minimum.txt"
-FILE_GUILD_INFO_DISBANDING = "guild/tibiacom_info_disbanding.txt"
-FILE_GUILD_INFO_FORMATION = "guild/tibiacom_info_formation.txt"
-FILE_GUILD_LIST = "guild/tibiacom_list.txt"
-FILE_GUILD_LIST_NOT_FOUND = "guild/tibiacom_list_not_found.txt"
-FILE_GUILD_IN_WAR = "guild/tibiacom_war.txt"
-
-FILE_GUILD_WAR_ACTIVE_HISTORY = "guild/wars/tibiacom_active_history.txt"
-FILE_GUILD_WAR_EMPTY = "guild/wars/tibiacom_empty.txt"
-FILE_GUILD_WAR_UNACTIVE_HISTORY = "guild/wars/tibiacom_unactive_history.txt"
-
-
-class TestsGuild(TestCommons, unittest.TestCase):
-    def setUp(self):
-        self.guild = Guild()
-
-    def test_guild_from_content(self):
-        """Testing parsing a guild"""
-        content = self.load_resource(FILE_GUILD_FULL)
-        guild = Guild.from_content(content)
-        self.assertIsInstance(guild, Guild, "Guild should be a Guild object.")
-        self.assertEqual(guild.url, Guild.get_url(guild.name))
-        self.assertEqual(guild.url_wars, Guild.get_url_wars(guild.name))
-        self.assertTrue(guild.active, "Guild should be active")
-        self.assertIsInstance(guild.founded, datetime.date, "Guild founded date should be an instance of datetime.date")
-        self.assertTrue(guild.open_applications, "Guild applications should be open")
-        self.assertIsNotNone(guild.description, "Guild should have a description")
-        self.assertTrue(guild.members, "Guild should have members")
-        self.assertEqual(guild.member_count, len(guild.members))
-        self.assertTrue(guild.invites, "Guild should have invites")
-        self.assertIsInstance(guild.online_members, list, "Guild online members should be a list.")
-        self.assertEqual(len(guild.online_members), guild.online_count, "Length of online_members should be equal "
-                                                                        "to online_count")
-        self.assertTrue(guild.ranks, "Guild ranks should not be empty.")
-        for member in guild.members:
-            self.assertIsInstance(member.level, int, "Member level should be an integer.")
-            self.assertIsInstance(member.joined, datetime.date, "Member's joined date should be datetime.date.")
-        for invited in guild.invites:
-            self.assertIsNotNone(invited.name, "Invited character's name should not be None.")
-            self.assertIsInstance(invited.date, datetime.date, "Invited character's date should be datetime.date.")
-
-        self.assertEqual(8, len(guild.members_by_rank['Vice Leader']))
-
-        self.assertIsInstance(guild.guildhall, GuildHouse)
-        self.assertEqual(guild.guildhall.owner, guild.members[0].name)
-        self.assertEqual(guild.guildhall.world, guild.world)
-        self.assertIsInstance(guild.guildhall.paid_until_date, datetime.date)
-
-    def test_guild_from_content_not_found(self):
-        """Testing parsing a non existent guild"""
-        content = self.load_resource(FILE_GUILD_NOT_FOUND)
-        guild = Guild.from_content(content)
-        self.assertIsNone(guild)
-
-    def test_guild_from_content_unrelated(self):
-        """Testing parsing an unrelated tibiacom section"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(InvalidContent):
-            Guild.from_content(content)
-
-    def test_guild_from_content_complete_info(self):
-        """Testing parsing a guild with all information possible"""
-        content = self.load_parsed_resource(FILE_GUILD_INFO_COMPLETE)
-        self.guild._parse_guild_disband_info(content)
-        self.assertIsNone(self.guild.disband_condition, "Guild should not be under disband warning")
-        self.assertIsNone(self.guild.disband_date, "Guild should not have disband date")
-
-        self.guild._parse_guild_guildhall(content)
-        self.assertIsNotNone(self.guild.guildhall, "Guild should have guildhall")
-        self.assertEqual(self.guild.guildhall.name, "Sky Lane, Guild 1")
-        self.assertEqual(self.guild.guildhall.paid_until_date, datetime.date(2018, 8, 26))
-
-        self.guild._parse_guild_homepage(content)
-        self.assertIsNotNone(self.guild.homepage, "Guild homepage must exist")
-        self.assertEqual("tibiammo.reddit.com", self.guild.homepage)
-
-        self.guild._parse_application_info(content)
-        self.assertTrue(self.guild.open_applications, "Guild should be open to applications")
-
-        self.guild._parse_guild_info(content)
-        self.assertIsNotNone(self.guild.description, "Guild description must exist")
-        self.assertEqual("Gladera", self.guild.world)
-        self.assertEqual(datetime.date(2015, 7, 23), self.guild.founded)
-        self.assertTrue(self.guild.active, "Guild should be active")
-
-    def test_guild_from_content_minimum_info(self):
-        """Testing parsing a guild with the minimum information possible"""
-        content = self.load_parsed_resource(FILE_GUILD_INFO_MINIMUM)
-        self.guild._parse_guild_disband_info(content)
-        self.assertIsNone(self.guild.disband_condition, "Guild should not be under disband warning")
-        self.assertIsNone(self.guild.disband_date, "Guild should not have disband date")
-
-        self.guild._parse_guild_guildhall(content)
-        self.assertIsNone(self.guild.guildhall, "Guild should not have a guildhall")
-
-        self.guild._parse_guild_homepage(content)
-        self.assertIsNone(self.guild.homepage, "Guild should not have a guildhall")
-
-        self.guild._parse_guild_info(content)
-        self.assertIsNone(self.guild.description, "Guild description must not exist")
-        self.assertEqual("Gladera", self.guild.world)
-        self.assertEqual(datetime.date(year=2018, month=5, day=18), self.guild.founded)
-
-    def test_guild_from_content_in_war(self):
-        content = self.load_resource(FILE_GUILD_IN_WAR)
-        guild = Guild.from_content(content)
-
-        self.assertIsInstance(guild, Guild)
-        self.assertFalse(guild.open_applications)
-        self.assertTrue(guild.active_war)
-
-    def test_guild_from_content_disbanding(self):
-        """Testing parsing a guild that is disbanding"""
-        content = self.load_parsed_resource(FILE_GUILD_INFO_DISBANDING)
-        self.guild._parse_guild_info(content)
-        self.assertTrue(self.guild.active, "Guild should be active")
-
-        self.guild._parse_guild_disband_info(content)
-        self.assertIsNotNone(self.guild.disband_condition, "Guild should have a disband warning")
-        self.assertEqual(self.guild.disband_date, datetime.date(2018, 8, 17), "Guild should have disband date")
-
-    def test_guild_from_content_formation(self):
-        """Testing parsing a guild that is in formation"""
-        content = self.load_parsed_resource(FILE_GUILD_INFO_FORMATION)
-        Guild._parse_guild_info(self.guild, content)
-        self.assertFalse(self.guild["active"], "Guild should not be active")
-
-        Guild._parse_guild_disband_info(self.guild, content)
-        self.assertIsNotNone(self.guild.disband_condition, "Guild should have a disband warning")
-        self.assertEqual(self.guild.disband_date, datetime.date(2018, 8, 16), "Guild should have disband date")
-
-    def test_listed_guild_from_content(self):
-        """Testing parsing the list of guilds of a world"""
-        content = self.load_resource(FILE_GUILD_LIST)
-        guilds_section = GuildsSection.from_content(content)
-        guilds = guilds_section.entries
-
-        self.assertEqual(7, len(guilds_section.active_guilds))
-        self.assertEqual(1, len(guilds_section.in_formation_guilds))
-        self.assertEqual(55, len(guilds_section.available_worlds))
-        self.assertEqual(GuildsSection.get_url(guilds_section.world),guilds_section.url)
-        self.assertEqual("Zuna", guilds[0].world)
-        self.assertTrue(guilds[0].active)
-        self.assertFalse(guilds[-1].active)
-
-    def test_listed_guild_from_content_not_found(self):
-        """Testing parsing the guild list of a world that doesn't exist"""
-        content = self.load_resource(FILE_GUILD_LIST_NOT_FOUND)
-        guilds_section = GuildsSection.from_content(content)
-        self.assertIsNotNone(guilds_section)
-        self.assertIsNone(guilds_section.world)
-        self.assertEqual(0, len(guilds_section.entries))
-
-    def test_listed_guild_from_content_unrelated(self):
-        """Testing parsing and unrelated section"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(InvalidContent):
-            GuildsSection.from_content(content)
-
-    def test_parse_invited_member_date(self):
-        """Testing the invitation date of a invited member"""
-        name = "Tschas"
-        date = "Invitation Date"
-        values = name, date
-        self.guild._parse_invited_member(values)
-        self.assertIsNotNone(self.guild.invites)
-        self.assertListEqual(self.guild.invites, [])
-
-    def test_parse_invited_member(self):
-        """Testing parsing an invited member"""
-        name = "Tschas"
-        date = "Jun 20 2018"
-        values = name, date
-        Guild._parse_invited_member(self.guild, values)
-        self.assertIsNotNone(self.guild.invites)
-        self.assertIsNotNone(self.guild.invites[0])
-        self.assertEqual(self.guild.invites[0].name, name)
-        self.assertEqual(self.guild.invites[0].date, datetime.date(2018, 6, 20))
-
-    def test_guild_member_init_join_date(self):
-        """Testing different combinations of join dates for instance creation"""
-        self.assertIsInstance(GuildMember(joined="Jul 20 2018").joined, datetime.date)
-        self.assertIsInstance(GuildMember(joined=datetime.date.today()).joined, datetime.date)
-        self.assertIsInstance(GuildMember(joined=datetime.datetime.now()).joined, datetime.date)
-        self.assertIsNone(GuildMember(joined=None).joined)
-        self.assertIsNone(GuildMember(joined="Jul 20").joined)
-
-    def test_guild_invite_init_invite_date(self):
-        """Testing different combinations of invite dates for instance creation"""
-        self.assertIsInstance(GuildInvite(date="Jul 20 2018").date, datetime.date)
-        self.assertIsInstance(GuildInvite(date=datetime.date.today()).date, datetime.date)
-        self.assertIsInstance(GuildInvite(date=datetime.datetime.now()).date, datetime.date)
-        self.assertIsNone(GuildInvite(date=None).date)
-        self.assertIsNone(GuildInvite(date="Jul 20").date)
-
-    def test_guild_init_founded(self):
-        """Testing different founded date inputs for instance creation"""
-        self.assertIsInstance(Guild(founded="Jul 20 2018").founded, datetime.date)
-        self.assertIsInstance(Guild(founded=datetime.date.today()).founded, datetime.date)
-        self.assertIsInstance(Guild(founded=datetime.datetime.now()).founded, datetime.date)
-        self.assertIsNone(Guild(founded=None).founded)
-        self.assertIsNone(Guild(founded="Jul 20").founded)
-
-    # region Guild War Tests
-    def test_guild_wars_from_content_active_history(self):
-        """Testing parsing the guild wars of a guild currently in war and with war history."""
-        content = self.load_resource(FILE_GUILD_WAR_ACTIVE_HISTORY)
-        guild_wars = GuildWars.from_content(content)
-
-        self.assertIsInstance(guild_wars, GuildWars)
-        self.assertEqual("Army Geddon", guild_wars.name)
-        self.assertIsNotNone(guild_wars.current)
-        self.assertEqual(guild_wars.name, guild_wars.current.guild_name)
-        self.assertEqual(178, guild_wars.current.guild_score)
-        self.assertEqual("Willyboiis Boys", guild_wars.current.opponent_name)
-        self.assertEqual(218, guild_wars.current.opponent_score)
-        self.assertEqual(1000, guild_wars.current.score_limit)
-
-        self.assertEqual(2, len(guild_wars.history))
-
-        self.assertEqual(guild_wars.name, guild_wars.history[0].guild_name)
-        self.assertEqual(0, guild_wars.history[0].guild_score)
-        self.assertEqual(None, guild_wars.history[0].opponent_name)
-        self.assertEqual(0, guild_wars.history[0].opponent_score)
-        self.assertEqual(420, guild_wars.history[0].score_limit)
-        self.assertTrue(guild_wars.history[0].surrender)
-
-        self.assertEqual(guild_wars.name, guild_wars.history[1].guild_name)
-        self.assertEqual(500, guild_wars.history[1].guild_score)
-        self.assertEqual(None, guild_wars.history[1].opponent_name)
-        self.assertEqual(491, guild_wars.history[1].opponent_score)
-        self.assertEqual(500, guild_wars.history[1].score_limit)
-        self.assertEqual(guild_wars.name, guild_wars.history[1].winner)
-
-    def test_guild_wars_from_content_empty(self):
-        """Testing parsing the guild wars of a guild that has never been in a war"""
-        content = self.load_resource(FILE_GUILD_WAR_EMPTY)
-        guild_wars = GuildWars.from_content(content)
-
-        self.assertEqual("Redd Alliance", guild_wars.name)
-        self.assertIsNone(guild_wars.current)
-        self.assertFalse(guild_wars.history)
-
-    def test_guild_wars_from_content_unactive_history(self):
-        """Testing parsing the guild wars of a war currently not in war and with war history."""
-        content = self.load_resource(FILE_GUILD_WAR_UNACTIVE_HISTORY)
-        guild_wars = GuildWars.from_content(content)
-
-        self.assertIsInstance(guild_wars, GuildWars)
-        self.assertEqual("Dinastia de Perrones", guild_wars.name)
-        self.assertIsNone(guild_wars.current)
-
-        self.assertEqual(1, len(guild_wars.history))
-
-        self.assertEqual(guild_wars.name, guild_wars.history[0].guild_name)
-        self.assertEqual(0, guild_wars.history[0].guild_score)
-        self.assertEqual(None, guild_wars.history[0].opponent_name)
-        self.assertEqual(0, guild_wars.history[0].opponent_score)
-        self.assertEqual(1000, guild_wars.history[0].score_limit)
-        self.assertTrue(guild_wars.history[0].surrender)
-
-    # endregion
+import datetime
+import unittest
+
+from tests.tests_tibiapy import TestCommons
+from tibiapy import InvalidContent
+from tibiapy.builders.guild import GuildBuilder
+from tibiapy.models import Guild, GuildWars
+from tibiapy.models.guild import GuildHouse
+from tibiapy.parsers.guild import GuildParser, GuildWarsParser, GuildsSectionParser
+from tibiapy.urls import get_world_guilds_url, get_guild_url, get_guild_wars_url
+
+FILE_GUILD_FULL = "guild/tibiacom_full.txt"
+FILE_GUILD_NOT_FOUND = "guild/tibiacom_not_found.txt"
+FILE_GUILD_INFO_COMPLETE = "guild/tibiacom_info_complete.txt"
+FILE_GUILD_INFO_MINIMUM = "guild/tibiacom_info_minimum.txt"
+FILE_GUILD_INFO_DISBANDING = "guild/tibiacom_info_disbanding.txt"
+FILE_GUILD_INFO_FORMATION = "guild/tibiacom_info_formation.txt"
+FILE_GUILD_LIST = "guild/tibiacom_list.txt"
+FILE_GUILD_LIST_NOT_FOUND = "guild/tibiacom_list_not_found.txt"
+FILE_GUILD_IN_WAR = "guild/tibiacom_war.txt"
+
+FILE_GUILD_WAR_ACTIVE_HISTORY = "guild/wars/tibiacom_active_history.txt"
+FILE_GUILD_WAR_EMPTY = "guild/wars/tibiacom_empty.txt"
+FILE_GUILD_WAR_UNACTIVE_HISTORY = "guild/wars/tibiacom_unactive_history.txt"
+
+
+class TestsGuild(TestCommons, unittest.TestCase):
+    def setUp(self):
+        self.guild = GuildBuilder()
+
+    def test_guild_from_content(self):
+        """Testing parsing a guild"""
+        content = self.load_resource(FILE_GUILD_FULL)
+        guild = GuildParser.from_content(content)
+        self.assertIsInstance(guild, Guild, "Guild should be a Guild object.")
+        self.assertEqual(guild.url, get_guild_url(guild.name))
+        self.assertEqual(guild.url_wars, get_guild_wars_url(guild.name))
+        self.assertTrue(guild.active, "Guild should be active")
+        self.assertIsInstance(guild.founded, datetime.date, "Guild founded date should be an instance of datetime.date")
+        self.assertTrue(guild.open_applications, "Guild applications should be open")
+        self.assertIsNotNone(guild.description, "Guild should have a description")
+        self.assertTrue(guild.members, "Guild should have members")
+        self.assertEqual(guild.member_count, len(guild.members))
+        self.assertTrue(guild.invites, "Guild should have invites")
+        self.assertIsInstance(guild.online_members, list, "Guild online members should be a list.")
+        self.assertEqual(len(guild.online_members), guild.online_count, "Length of online_members should be equal "
+                                                                        "to online_count")
+        self.assertTrue(guild.ranks, "Guild ranks should not be empty.")
+        for member in guild.members:
+            self.assertIsInstance(member.level, int, "Member level should be an integer.")
+            self.assertIsInstance(member.joined, datetime.date, "Member's joined date should be datetime.date.")
+        for invited in guild.invites:
+            self.assertIsNotNone(invited.name, "Invited character's name should not be None.")
+            self.assertIsInstance(invited.date, datetime.date, "Invited character's date should be datetime.date.")
+
+        self.assertEqual(8, len(guild.members_by_rank['Vice Leader']))
+
+        self.assertIsInstance(guild.guildhall, GuildHouse)
+        self.assertIsInstance(guild.guildhall.paid_until_date, datetime.date)
+
+    def test_guild_from_content_not_found(self):
+        """Testing parsing a non existent guild"""
+        content = self.load_resource(FILE_GUILD_NOT_FOUND)
+        guild = GuildParser.from_content(content)
+        self.assertIsNone(guild)
+
+    def test_guild_from_content_unrelated(self):
+        """Testing parsing an unrelated tibiacom section"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(InvalidContent):
+            GuildParser.from_content(content)
+
+    def test_guild_from_content_complete_info(self):
+        """Testing parsing a guild with all information possible"""
+        content = self.load_parsed_resource(FILE_GUILD_INFO_COMPLETE)
+        GuildParser._parse_guild_disband_info(self.guild, content)
+        self.assertIsNone(self.guild._disband_condition, "Guild should not be under disband warning")
+        self.assertIsNone(self.guild._disband_date, "Guild should not have disband date")
+
+        GuildParser._parse_guild_guildhall(self.guild, content)
+        self.assertIsNotNone(self.guild._guildhall, "Guild should have guildhall")
+        self.assertEqual(self.guild._guildhall.name, "Sky Lane, Guild 1")
+        self.assertEqual(self.guild._guildhall.paid_until_date, datetime.date(2018, 8, 26))
+
+        GuildParser._parse_guild_homepage(self.guild, content)
+        self.assertIsNotNone(self.guild.homepage, "Guild homepage must exist")
+        self.assertEqual("tibiammo.reddit.com", self.guild._homepage)
+
+        GuildParser._parse_application_info(self.guild, content)
+        self.assertTrue(self.guild._open_applications, "Guild should be open to applications")
+
+        GuildParser._parse_guild_info(self.guild, content)
+        self.assertIsNotNone(self.guild._description, "Guild description must exist")
+        self.assertEqual("Gladera", self.guild._world)
+        self.assertEqual(datetime.date(2015, 7, 23), self.guild._founded)
+        self.assertTrue(self.guild._active, "Guild should be active")
+
+    def test_guild_from_content_minimum_info(self):
+        """Testing parsing a guild with the minimum information possible"""
+        content = self.load_parsed_resource(FILE_GUILD_INFO_MINIMUM)
+        GuildParser._parse_guild_disband_info(self.guild, content)
+        self.assertIsNone(self.guild._disband_condition, "Guild should not be under disband warning")
+        self.assertIsNone(self.guild._disband_date, "Guild should not have disband date")
+
+        GuildParser._parse_guild_guildhall(self.guild, content)
+        self.assertIsNone(self.guild._guildhall, "Guild should not have a guildhall")
+
+        GuildParser._parse_guild_homepage(self.guild, content)
+        self.assertIsNone(self.guild._homepage, "Guild should not have a guildhall")
+
+        GuildParser._parse_guild_info(self.guild, content)
+        self.assertIsNone(self.guild._description, "Guild description must not exist")
+        self.assertEqual("Gladera", self.guild._world)
+        self.assertEqual(datetime.date(year=2018, month=5, day=18), self.guild._founded)
+
+    def test_guild_from_content_in_war(self):
+        content = self.load_resource(FILE_GUILD_IN_WAR)
+        guild = GuildParser.from_content(content)
+
+        self.assertIsInstance(guild, Guild)
+        self.assertFalse(guild.open_applications)
+        self.assertTrue(guild.active_war)
+
+    def test_guild_from_content_disbanding(self):
+        """Testing parsing a guild that is disbanding"""
+        content = self.load_parsed_resource(FILE_GUILD_INFO_DISBANDING)
+        GuildParser._parse_guild_info(self.guild, content)
+        self.assertTrue(self.guild._active, "Guild should be active")
+
+        GuildParser._parse_guild_disband_info(self.guild, content)
+        self.assertIsNotNone(self.guild._disband_condition, "Guild should have a disband warning")
+        self.assertEqual(self.guild._disband_date, datetime.date(2018, 8, 17), "Guild should have disband date")
+
+    def test_guild_from_content_formation(self):
+        """Testing parsing a guild that is in formation"""
+        content = self.load_parsed_resource(FILE_GUILD_INFO_FORMATION)
+        GuildParser._parse_guild_info(self.guild, content)
+        self.assertFalse(self.guild._active, "Guild should not be active")
+
+        GuildParser._parse_guild_disband_info(self.guild, content)
+        self.assertIsNotNone(self.guild._disband_condition, "Guild should have a disband warning")
+        self.assertEqual(self.guild._disband_date, datetime.date(2018, 8, 16), "Guild should have disband date")
+
+    def test_listed_guild_from_content(self):
+        """Testing parsing the list of guilds of a world"""
+        content = self.load_resource(FILE_GUILD_LIST)
+        guilds_section = GuildsSectionParser.from_content(content)
+        guilds = guilds_section.entries
+
+        self.assertEqual(7, len(guilds_section.active_guilds))
+        self.assertEqual(1, len(guilds_section.in_formation_guilds))
+        self.assertEqual(55, len(guilds_section.available_worlds))
+        self.assertEqual(get_world_guilds_url(guilds_section.world), guilds_section.url)
+        self.assertEqual("Zuna", guilds[0].world)
+        self.assertTrue(guilds[0].active)
+        self.assertFalse(guilds[-1].active)
+
+    def test_listed_guild_from_content_not_found(self):
+        """Testing parsing the guild list of a world that doesn't exist"""
+        content = self.load_resource(FILE_GUILD_LIST_NOT_FOUND)
+        guilds_section = GuildsSectionParser.from_content(content)
+        self.assertIsNotNone(guilds_section)
+        self.assertIsNone(guilds_section.world)
+        self.assertEqual(0, len(guilds_section.entries))
+
+    def test_listed_guild_from_content_unrelated(self):
+        """Testing parsing and unrelated section"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(InvalidContent):
+            GuildsSectionParser.from_content(content)
+
+
+    # region Guild War Tests
+    def test_guild_wars_from_content_active_history(self):
+        """Testing parsing the guild wars of a guild currently in war and with war history."""
+        content = self.load_resource(FILE_GUILD_WAR_ACTIVE_HISTORY)
+        guild_wars = GuildWarsParser.from_content(content)
+
+        self.assertIsInstance(guild_wars, GuildWars)
+        self.assertEqual("Army Geddon", guild_wars.name)
+        self.assertIsNotNone(guild_wars.current)
+        self.assertEqual(guild_wars.name, guild_wars.current.guild_name)
+        self.assertEqual(178, guild_wars.current.guild_score)
+        self.assertEqual("Willyboiis Boys", guild_wars.current.opponent_name)
+        self.assertEqual(218, guild_wars.current.opponent_score)
+        self.assertEqual(1000, guild_wars.current.score_limit)
+
+        self.assertEqual(2, len(guild_wars.history))
+
+        self.assertEqual(guild_wars.name, guild_wars.history[0].guild_name)
+        self.assertEqual(0, guild_wars.history[0].guild_score)
+        self.assertEqual(None, guild_wars.history[0].opponent_name)
+        self.assertEqual(0, guild_wars.history[0].opponent_score)
+        self.assertEqual(420, guild_wars.history[0].score_limit)
+        self.assertTrue(guild_wars.history[0].surrender)
+
+        self.assertEqual(guild_wars.name, guild_wars.history[1].guild_name)
+        self.assertEqual(500, guild_wars.history[1].guild_score)
+        self.assertEqual(None, guild_wars.history[1].opponent_name)
+        self.assertEqual(491, guild_wars.history[1].opponent_score)
+        self.assertEqual(500, guild_wars.history[1].score_limit)
+        self.assertEqual(guild_wars.name, guild_wars.history[1].winner)
+
+    def test_guild_wars_from_content_empty(self):
+        """Testing parsing the guild wars of a guild that has never been in a war"""
+        content = self.load_resource(FILE_GUILD_WAR_EMPTY)
+        guild_wars = GuildWarsParser.from_content(content)
+
+        self.assertEqual("Redd Alliance", guild_wars.name)
+        self.assertIsNone(guild_wars.current)
+        self.assertFalse(guild_wars.history)
+
+    def test_guild_wars_from_content_unactive_history(self):
+        """Testing parsing the guild wars of a war currently not in war and with war history."""
+        content = self.load_resource(FILE_GUILD_WAR_UNACTIVE_HISTORY)
+        guild_wars = GuildWarsParser.from_content(content)
+
+        self.assertIsInstance(guild_wars, GuildWars)
+        self.assertEqual("Dinastia de Perrones", guild_wars.name)
+        self.assertIsNone(guild_wars.current)
+
+        self.assertEqual(1, len(guild_wars.history))
+
+        self.assertEqual(guild_wars.name, guild_wars.history[0].guild_name)
+        self.assertEqual(0, guild_wars.history[0].guild_score)
+        self.assertEqual(None, guild_wars.history[0].opponent_name)
+        self.assertEqual(0, guild_wars.history[0].opponent_score)
+        self.assertEqual(1000, guild_wars.history[0].score_limit)
+        self.assertTrue(guild_wars.history[0].surrender)
+
+    # endregion
```

### Comparing `tibia.py-5.6.1/tests/tests_highscores.py` & `tibia.py-6.0.0a1/tests/tests_highscores.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,138 +1,140 @@
-import datetime
-import unittest
-
-from tests.tests_tibiapy import TestCommons
-from tibiapy import Category, Highscores, HighscoresEntry, InvalidContent, LoyaltyHighscoresEntry, \
-    Vocation, VocationFilter, BattlEyeHighscoresFilter
-
-FILE_HIGHSCORES_FULL = "highscores/tibiacom_full.txt"
-FILE_HIGHSCORES_EXPERIENCE = "highscores/tibiacom_experience.txt"
-FILE_HIGHSCORES_LOYALTY = "highscores/tibiacom_loyalty.txt"
-FILE_HIGHSCORES_BATTLEYE_PVP_FILTER = "highscores/tibiacom_battleye_pvp_filters.txt"
-FILE_HIGHSCORES_EMPTY = "highscores/tibiacom_empty.txt"
-FILE_HIGHSCORES_NO_RESULTS = "highscores/tibiacom_no_results.txt"
-
-
-class TestHighscores(unittest.TestCase, TestCommons):
-    # region Tibia.com Tests
-    def test_highscores_from_content(self):
-        """Testing parsing Highscores"""
-        content = self.load_resource(FILE_HIGHSCORES_FULL)
-        highscores = Highscores.from_content(content)
-
-        self.assertEqual("Estela", highscores.world)
-        self.assertEqual(VocationFilter.KNIGHTS, highscores.vocation)
-        self.assertEqual(Category.MAGIC_LEVEL, highscores.category)
-        self.assertEqual(BattlEyeHighscoresFilter.ANY_WORLD, highscores.battleye_filter)
-        self.assertEqual(1983, highscores.results_count)
-        self.assertEqual(38, highscores.from_rank)
-        self.assertEqual(38, highscores.to_rank)
-        self.assertEqual(4, highscores.page)
-        self.assertEqual(40, highscores.total_pages)
-        self.assertIsNotNone(highscores.get_page_url(1))
-        self.assertIsNotNone(highscores.url)
-        self.assertIsNotNone(highscores.next_page_url)
-        self.assertIsNotNone(highscores.previous_page_url)
-        self.assertEqual(datetime.timedelta(minutes=6), highscores.last_updated)
-
-        for entry in highscores.entries:
-            self.assertIsInstance(entry, HighscoresEntry)
-            self.assertIsInstance(entry.name, str)
-            self.assertIsInstance(entry.vocation, Vocation)
-            self.assertIsInstance(entry.rank, int)
-            self.assertIsInstance(entry.value, int)
-            self.assertIsInstance(entry.level, int)
-            self.assertEqual("Estela", entry.world)
-
-    def test_highscores_from_content_highscores(self):
-        """Testing parsing experience highscores"""
-        content = self.load_resource(FILE_HIGHSCORES_EXPERIENCE)
-        highscores = Highscores.from_content(content)
-
-        self.assertEqual(highscores.world, "Gladera")
-        self.assertEqual(highscores.vocation, VocationFilter.PALADINS)
-        self.assertEqual(highscores.category, Category.EXPERIENCE)
-        self.assertEqual(highscores.results_count, 1000)
-        self.assertEqual(highscores.total_pages, 20)
-
-        for entry in highscores.entries:
-            self.assertIsInstance(entry, HighscoresEntry)
-            self.assertIsInstance(entry.name, str)
-            self.assertIsInstance(entry.vocation, Vocation)
-            self.assertIsInstance(entry.rank, int)
-            self.assertIsInstance(entry.value, int)
-            self.assertIsInstance(entry.level, int)
-            self.assertEqual(entry.world, "Gladera")
-
-    def test_highscores_from_content_loyalty(self):
-        """Testing parsing experience loyalty"""
-        content = self.load_resource(FILE_HIGHSCORES_LOYALTY)
-        highscores = Highscores.from_content(content)
-
-        self.assertEqual("Calmera", highscores.world)
-        self.assertEqual(VocationFilter.PALADINS, highscores.vocation)
-        self.assertEqual(Category.LOYALTY_POINTS, highscores.category)
-        self.assertEqual(1007, highscores.results_count)
-        self.assertEqual(21, highscores.total_pages)
-
-        for entry in highscores.entries:
-            self.assertIsInstance(entry, LoyaltyHighscoresEntry)
-            self.assertIsInstance(entry.name, str)
-            self.assertIsInstance(entry.vocation, Vocation)
-            self.assertIsInstance(entry.rank, int)
-            self.assertIsInstance(entry.value, int)
-            self.assertIsInstance(entry.level, int)
-            self.assertIsInstance(entry.title, str)
-
-    def test_highscores_from_content_battleye_and_pvp_filters(self):
-        """Testing parsing Highscores"""
-        content = self.load_resource(FILE_HIGHSCORES_BATTLEYE_PVP_FILTER)
-        highscores = Highscores.from_content(content)
-
-        self.assertEqual(None, highscores.world)
-        self.assertEqual(VocationFilter.ALL, highscores.vocation)
-        self.assertEqual(Category.EXPERIENCE, highscores.category)
-        self.assertEqual(BattlEyeHighscoresFilter.INITIALLY_PROTECTED, highscores.battleye_filter)
-        self.assertEqual(1000, highscores.results_count)
-        self.assertEqual(1, highscores.from_rank)
-        self.assertEqual(50, highscores.to_rank)
-        self.assertEqual(1, highscores.page)
-        self.assertEqual(20, highscores.total_pages)
-        self.assertEqual(3, len(highscores.pvp_types_filter))
-        self.assertIsNotNone(highscores.url)
-        self.assertEqual(datetime.timedelta(minutes=27), highscores.last_updated)
-
-        for entry in highscores.entries:
-            self.assertIsInstance(entry, HighscoresEntry)
-            self.assertIsInstance(entry.name, str)
-            self.assertIsInstance(entry.vocation, Vocation)
-            self.assertIsInstance(entry.rank, int)
-            self.assertIsInstance(entry.value, int)
-            self.assertIsInstance(entry.level, int)
-
-    def test_highscores_from_content_empty(self):
-        """Testing parsing highscores when empty (world doesn't exist)"""
-        content = self.load_resource(FILE_HIGHSCORES_EMPTY)
-        highscores = Highscores.from_content(content)
-
-        self.assertIsNone(highscores)
-
-    def _test_highscores_from_content_no_results(self):
-        """Testing parsing highscores with no results (first day of a new world)"""
-        content = self.load_resource(FILE_HIGHSCORES_NO_RESULTS)
-        highscores = Highscores.from_content(content)
-
-        self.assertIsInstance(highscores, Highscores)
-        self.assertEqual(highscores.world, "Unica")
-        self.assertEqual(highscores.category, Category.EXPERIENCE)
-        self.assertEqual(highscores.vocation, VocationFilter.ALL)
-        self.assertEqual(highscores.total_pages, 0)
-        self.assertEqual(len(highscores.entries), 0)
-
-    def test_highscores_from_content_unrelated_section(self):
-        """Testing parsing an unrelated section"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(InvalidContent):
-            Highscores.from_content(content)
-
-    # endregion
+import datetime
+import unittest
+
+from tests.tests_tibiapy import TestCommons
+from tibiapy import HighscoresCategory, InvalidContent, \
+    Vocation, HighscoresProfession, HighscoresBattlEyeType
+from tibiapy.models import Highscores, HighscoresEntry, LoyaltyHighscoresEntry
+from tibiapy.parsers.highscores import HighscoresParser
+
+FILE_HIGHSCORES_FULL = "highscores/tibiacom_full.txt"
+FILE_HIGHSCORES_EXPERIENCE = "highscores/tibiacom_experience.txt"
+FILE_HIGHSCORES_LOYALTY = "highscores/tibiacom_loyalty.txt"
+FILE_HIGHSCORES_BATTLEYE_PVP_FILTER = "highscores/tibiacom_battleye_pvp_filters.txt"
+FILE_HIGHSCORES_EMPTY = "highscores/tibiacom_empty.txt"
+FILE_HIGHSCORES_NO_RESULTS = "highscores/tibiacom_no_results.txt"
+
+
+class TestHighscores(unittest.TestCase, TestCommons):
+    # region Tibia.com Tests
+    def test_highscores_from_content(self):
+        """Testing parsing Highscores"""
+        content = self.load_resource(FILE_HIGHSCORES_FULL)
+        highscores = HighscoresParser.from_content(content)
+
+        self.assertEqual("Estela", highscores.world)
+        self.assertEqual(HighscoresProfession.KNIGHTS, highscores.vocation)
+        self.assertEqual(HighscoresCategory.MAGIC_LEVEL, highscores.category)
+        self.assertEqual(HighscoresBattlEyeType.ANY_WORLD, highscores.battleye_filter)
+        self.assertEqual(1983, highscores.results_count)
+        self.assertEqual(38, highscores.from_rank)
+        self.assertEqual(38, highscores.to_rank)
+        self.assertEqual(4, highscores.current_page)
+        self.assertEqual(40, highscores.total_pages)
+        self.assertIsNotNone(highscores.get_page_url(1))
+        self.assertIsNotNone(highscores.url)
+        self.assertIsNotNone(highscores.next_page_url)
+        self.assertIsNotNone(highscores.previous_page_url)
+        self.assertEqual(datetime.timedelta(minutes=6), highscores.last_updated)
+
+        for entry in highscores.entries:
+            self.assertIsInstance(entry, HighscoresEntry)
+            self.assertIsInstance(entry.name, str)
+            self.assertIsInstance(entry.vocation, Vocation)
+            self.assertIsInstance(entry.rank, int)
+            self.assertIsInstance(entry.value, int)
+            self.assertIsInstance(entry.level, int)
+            self.assertEqual("Estela", entry.world)
+
+    def test_highscores_from_content_highscores(self):
+        """Testing parsing experience highscores"""
+        content = self.load_resource(FILE_HIGHSCORES_EXPERIENCE)
+        highscores = HighscoresParser.from_content(content)
+
+        self.assertEqual(highscores.world, "Gladera")
+        self.assertEqual(highscores.vocation, HighscoresProfession.PALADINS)
+        self.assertEqual(highscores.category, HighscoresCategory.EXPERIENCE)
+        self.assertEqual(highscores.results_count, 1000)
+        self.assertEqual(highscores.total_pages, 20)
+
+        for entry in highscores.entries:
+            self.assertIsInstance(entry, HighscoresEntry)
+            self.assertIsInstance(entry.name, str)
+            self.assertIsInstance(entry.vocation, Vocation)
+            self.assertIsInstance(entry.rank, int)
+            self.assertIsInstance(entry.value, int)
+            self.assertIsInstance(entry.level, int)
+            self.assertEqual(entry.world, "Gladera")
+
+    def test_highscores_from_content_loyalty(self):
+        """Testing parsing experience loyalty"""
+        content = self.load_resource(FILE_HIGHSCORES_LOYALTY)
+        highscores = HighscoresParser.from_content(content)
+
+        self.assertEqual("Calmera", highscores.world)
+        self.assertEqual(HighscoresProfession.PALADINS, highscores.vocation)
+        self.assertEqual(HighscoresCategory.LOYALTY_POINTS, highscores.category)
+        self.assertEqual(1007, highscores.results_count)
+        self.assertEqual(21, highscores.total_pages)
+
+        for entry in highscores.entries:
+            self.assertIsInstance(entry, LoyaltyHighscoresEntry)
+            self.assertIsInstance(entry.name, str)
+            self.assertIsInstance(entry.vocation, Vocation)
+            self.assertIsInstance(entry.rank, int)
+            self.assertIsInstance(entry.value, int)
+            self.assertIsInstance(entry.level, int)
+            self.assertIsInstance(entry.title, str)
+
+    def test_highscores_from_content_battleye_and_pvp_filters(self):
+        """Testing parsing Highscores"""
+        content = self.load_resource(FILE_HIGHSCORES_BATTLEYE_PVP_FILTER)
+        highscores = HighscoresParser.from_content(content)
+
+        self.assertEqual(None, highscores.world)
+        self.assertEqual(HighscoresProfession.ALL, highscores.vocation)
+        self.assertEqual(HighscoresCategory.EXPERIENCE, highscores.category)
+        self.assertEqual(HighscoresBattlEyeType.INITIALLY_PROTECTED, highscores.battleye_filter)
+        self.assertEqual(1000, highscores.results_count)
+        self.assertEqual(1, highscores.from_rank)
+        self.assertEqual(50, highscores.to_rank)
+        self.assertEqual(1, highscores.current_page)
+        self.assertEqual(20, highscores.total_pages)
+        self.assertEqual(3, len(highscores.pvp_types_filter))
+        self.assertIsNotNone(highscores.url)
+        self.assertEqual(datetime.timedelta(minutes=27), highscores.last_updated)
+
+        for entry in highscores.entries:
+            self.assertIsInstance(entry, HighscoresEntry)
+            self.assertIsInstance(entry.name, str)
+            self.assertIsInstance(entry.vocation, Vocation)
+            self.assertIsInstance(entry.rank, int)
+            self.assertIsInstance(entry.value, int)
+            self.assertIsInstance(entry.level, int)
+
+    def test_highscores_from_content_empty(self):
+        """Testing parsing highscores when empty (world doesn't exist)"""
+        content = self.load_resource(FILE_HIGHSCORES_EMPTY)
+        highscores = HighscoresParser.from_content(content)
+
+        self.assertIsNone(highscores)
+
+    def _test_highscores_from_content_no_results(self):
+        """Testing parsing highscores with no results (first day of a new world)"""
+        content = self.load_resource(FILE_HIGHSCORES_NO_RESULTS)
+        highscores = HighscoresParser.from_content(content)
+
+        self.assertIsInstance(highscores, Highscores)
+        self.assertEqual(highscores.world, "Unica")
+        self.assertEqual(highscores.category, HighscoresCategory.EXPERIENCE)
+        self.assertEqual(highscores.vocation, HighscoresProfession.ALL)
+        self.assertEqual(highscores.total_pages, 0)
+        self.assertEqual(len(highscores.entries), 0)
+
+    def test_highscores_from_content_unrelated_section(self):
+        """Testing parsing an unrelated section"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(InvalidContent):
+            HighscoresParser.from_content(content)
+
+    # endregion
```

### Comparing `tibia.py-5.6.1/tests/tests_house.py` & `tibia.py-6.0.0a1/tests/tests_house.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,143 +1,146 @@
-import datetime
-import json
-import unittest
-
-from tests.tests_tibiapy import TestCommons
-from tibiapy import House, HousesSection, InvalidContent, HouseEntry
-from tibiapy.enums import HouseOrder, HouseStatus, HouseType
-
-FILE_HOUSE_FULL = "house/tibiacom_full.txt"
-FILE_HOUSE_STATUS_TRANSFER = "house/tibiacom_status_transfer.txt"
-FILE_HOUSE_STATUS_NO_BIDS = "house/tibiacom_status_no_bids.txt"
-FILE_HOUSE_STATUS_WITH_BIDS = "house/tibiacom_status_with_bids.txt"
-FILE_HOUSE_STATUS_RENTED = "house/tibiacom_status_rented.txt"
-FILE_HOUSE_NOT_FOUND = "house/tibiacom_not_found.txt"
-FILE_HOUSE_LIST = "house/tibiacom_list.txt"
-FILE_HOUSE_LIST_NOT_FOUND = "house/tibiacom_list_not_found.txt"
-FILE_HOUSE_LIST_EMPTY = "house/tibiacom_list_empty.txt"
-
-
-class TestsHouse(TestCommons, unittest.TestCase):
-    def test_house_from_content(self):
-        """Testing parsing a house"""
-        content = self.load_resource(FILE_HOUSE_FULL)
-        house = House.from_content(content)
-
-        self.assertIsInstance(house, House)
-        self.assertEqual(house.name, "Sorcerer's Avenue Labs 2e")
-        self.assertEqual(house.beds, 1)
-        self.assertTrue(house.rent, 715)
-        self.assertEqual(house.status, HouseStatus.AUCTIONED)
-        self.assertEqual(house.url, House.get_url(house.id, house.world))
-        self.assertIsNone(house.owner)
-        self.assertIsNone(house.owner_url)
-        self.assertIsNotNone(house.highest_bidder)
-        self.assertIsNotNone(house.highest_bidder_url)
-        self.assertEqual(house.highest_bid, 0)
-
-        house_json_raw = house.to_json()
-        house_json = json.loads(house_json_raw)
-        self.assertEqual(house.image_url, house_json["image_url"])
-
-    def test_house_from_content_transferred(self):
-        """Testing parsing a house being transferred"""
-        house = House("Name")
-        content = self.load_resource(FILE_HOUSE_STATUS_TRANSFER)
-        house._parse_status(content)
-        self.assertEqual(house.status, HouseStatus.RENTED)
-        self.assertEqual(house.owner, "Xenaris mag")
-        self.assertEqual(house.transferee, "Ivarr Bezkosci")
-        self.assertIsNotNone(house.transferee_url)
-        self.assertTrue(house.transfer_accepted)
-        self.assertEqual(house.transfer_price, 850000)
-
-    def test_house_parse_status_rented(self):
-        """Testing parsing a rented status"""
-        house = House("Name")
-        content = self.load_resource(FILE_HOUSE_STATUS_RENTED)
-        house._parse_status(content)
-        self.assertEqual(house.status, HouseStatus.RENTED)
-        self.assertEqual(house.owner, "Thorcen")
-        self.assertIsInstance(house.paid_until, datetime.datetime)
-
-    def test_house_parse_status_with_bids(self):
-        """Testing parsing a house status with bids"""
-        house = House("Name")
-        content = self.load_resource(FILE_HOUSE_STATUS_WITH_BIDS)
-        house._parse_status(content)
-        self.assertEqual(house.status, HouseStatus.AUCTIONED)
-        self.assertIsNone(house.owner)
-        self.assertEqual(house.highest_bid, 15000)
-        self.assertEqual(house.highest_bidder, "King of Bosnia")
-        self.assertIsInstance(house.auction_end, datetime.datetime)
-
-    def test_house_parse_status_without_bids(self):
-        """Testing parsing the status of a house with no bids"""
-        house = House("Name")
-        content = self.load_resource(FILE_HOUSE_STATUS_NO_BIDS)
-        house._parse_status(content)
-        self.assertEqual(house.status, HouseStatus.AUCTIONED)
-        self.assertIsNone(house.auction_end)
-
-    def test_house_from_content_not_found(self):
-        """Testing parsing a house that doesn't exist"""
-        content = self.load_resource(FILE_HOUSE_NOT_FOUND)
-        house = House.from_content(content)
-
-        self.assertIsNone(house)
-
-    def test_house_from_content_unrelated(self):
-        """Testing parsing an unrelated section"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(InvalidContent):
-            House.from_content(content)
-
-    def test_house_section_from_content(self):
-        """Testing parsing the house list of a world and city"""
-        content = self.load_resource(FILE_HOUSE_LIST)
-        house_results = HousesSection.from_content(content)
-
-        self.assertIsInstance(house_results, HousesSection)
-        self.assertEqual("Carlin", house_results.town)
-        self.assertEqual("Alumbra", house_results.world)
-        self.assertEqual(HouseStatus.RENTED, house_results.status)
-        self.assertEqual(HouseType.HOUSE, house_results.house_type)
-        self.assertEqual(HouseOrder.RENT, house_results.order)
-
-        houses = house_results.entries
-        self.assertIsInstance(houses, list)
-        self.assertGreater(len(houses), 0)
-        self.assertIsInstance(houses[0], HouseEntry)
-        self.assertEqual(houses[0].town, "Carlin")
-        self.assertEqual(houses[0].type, HouseType.HOUSE)
-        self.assertEqual(houses[0].status, HouseStatus.RENTED)
-        self.assertIsInstance(houses[0].id, int)
-
-        self.assertEqual(houses[25].status, HouseStatus.RENTED)
-
-    def test_house_section_from_content_empty(self):
-        """Testing parsing an empty house list"""
-        content = self.load_resource(FILE_HOUSE_LIST_EMPTY)
-        house_results = HousesSection.from_content(content)
-
-        self.assertIsInstance(house_results, HousesSection)
-        self.assertEqual("Edron", house_results.town)
-        self.assertEqual("Antica", house_results.world)
-        self.assertEqual(HouseStatus.AUCTIONED, house_results.status)
-        self.assertEqual(HouseType.GUILDHALL, house_results.house_type)
-        self.assertEqual(HouseOrder.RENT, house_results.order)
-        self.assertEqual(len(house_results.entries), 0)
-
-    def test_house_section_from_content_not_found(self):
-        """Testing parsing an empty house list"""
-        content = self.load_resource(FILE_HOUSE_LIST_NOT_FOUND)
-        results = HousesSection.from_content(content)
-        self.assertIsInstance(results, HousesSection)
-        self.assertEqual(0, len(results.entries))
-
-    def test_house_section_from_content_unrelated(self):
-        """Testing parsing an unrelated section"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(InvalidContent):
-            HousesSection.from_content(content)
-
+import datetime
+import json
+import unittest
+
+from tests.tests_tibiapy import TestCommons
+from tibiapy import InvalidContent
+from tibiapy.builders.house import HouseBuilder
+from tibiapy.enums import HouseOrder, HouseStatus, HouseType
+from tibiapy.models import House, HousesSection, HouseEntry
+from tibiapy.parsers.house import HouseParser, HousesSectionParser
+from tibiapy.urls import get_house_url
+
+FILE_HOUSE_FULL = "house/tibiacom_full.txt"
+FILE_HOUSE_STATUS_TRANSFER = "house/tibiacom_status_transfer.txt"
+FILE_HOUSE_STATUS_NO_BIDS = "house/tibiacom_status_no_bids.txt"
+FILE_HOUSE_STATUS_WITH_BIDS = "house/tibiacom_status_with_bids.txt"
+FILE_HOUSE_STATUS_RENTED = "house/tibiacom_status_rented.txt"
+FILE_HOUSE_NOT_FOUND = "house/tibiacom_not_found.txt"
+FILE_HOUSE_LIST = "house/tibiacom_list.txt"
+FILE_HOUSE_LIST_NOT_FOUND = "house/tibiacom_list_not_found.txt"
+FILE_HOUSE_LIST_EMPTY = "house/tibiacom_list_empty.txt"
+
+
+class TestsHouse(TestCommons, unittest.TestCase):
+    def test_house_from_content(self):
+        """Testing parsing a house"""
+        content = self.load_resource(FILE_HOUSE_FULL)
+        house = HouseParser.from_content(content)
+
+        self.assertIsInstance(house, House)
+        self.assertEqual(house.name, "Sorcerer's Avenue Labs 2e")
+        self.assertEqual(house.beds, 1)
+        self.assertTrue(house.rent, 715)
+        self.assertEqual(house.status, HouseStatus.AUCTIONED)
+        self.assertEqual(house.url, get_house_url(house.world, house.id))
+        self.assertIsNone(house.owner)
+        self.assertIsNone(house.owner_url)
+        self.assertIsNotNone(house.highest_bidder)
+        self.assertIsNotNone(house.highest_bidder_url)
+        self.assertEqual(house.highest_bid, 0)
+
+        house_json_raw = house.json()
+        house_json = json.loads(house_json_raw)
+        self.assertEqual(house.image_url, house_json["image_url"])
+
+    def test_house_from_content_transferred(self):
+        """Testing parsing a house being transferred"""
+        house = HouseBuilder().name("Name")
+        content = self.load_resource(FILE_HOUSE_STATUS_TRANSFER)
+        HouseParser._parse_status(house, content)
+        self.assertEqual(house._status, HouseStatus.RENTED)
+        self.assertEqual(house._owner, "Xenaris mag")
+        self.assertEqual(house._transferee, "Ivarr Bezkosci")
+        self.assertTrue(house._transfer_accepted)
+        self.assertEqual(house._transfer_price, 850000)
+
+    def test_house_parse_status_rented(self):
+        """Testing parsing a rented status"""
+        house = HouseBuilder().name("Name")
+        content = self.load_resource(FILE_HOUSE_STATUS_RENTED)
+        HouseParser._parse_status(house, content)
+        self.assertEqual(house._status, HouseStatus.RENTED)
+        self.assertEqual(house._owner, "Thorcen")
+        self.assertIsInstance(house._paid_until, datetime.datetime)
+
+    def test_house_parse_status_with_bids(self):
+        """Testing parsing a house status with bids"""
+        house = HouseBuilder().name("Name")
+        content = self.load_resource(FILE_HOUSE_STATUS_WITH_BIDS)
+        HouseParser._parse_status(house, content)
+        self.assertEqual(house._status, HouseStatus.AUCTIONED)
+        self.assertIsNone(house._owner)
+        self.assertEqual(house._highest_bid, 15000)
+        self.assertEqual(house._highest_bidder, "King of Bosnia")
+        self.assertIsInstance(house._auction_end, datetime.datetime)
+
+    def test_house_parse_status_without_bids(self):
+        """Testing parsing the status of a house with no bids"""
+        house = HouseBuilder().name("Name")
+        content = self.load_resource(FILE_HOUSE_STATUS_NO_BIDS)
+        HouseParser._parse_status(house, content)
+        self.assertEqual(house._status, HouseStatus.AUCTIONED)
+        self.assertIsNone(house._auction_end)
+
+    def test_house_from_content_not_found(self):
+        """Testing parsing a house that doesn't exist"""
+        content = self.load_resource(FILE_HOUSE_NOT_FOUND)
+        house = HouseParser.from_content(content)
+
+        self.assertIsNone(house)
+
+    def test_house_from_content_unrelated(self):
+        """Testing parsing an unrelated section"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(InvalidContent):
+            HouseParser.from_content(content)
+
+    def test_house_section_from_content(self):
+        """Testing parsing the house list of a world and city"""
+        content = self.load_resource(FILE_HOUSE_LIST)
+        house_results = HousesSectionParser.from_content(content)
+
+        self.assertIsInstance(house_results, HousesSection)
+        self.assertEqual("Carlin", house_results.town)
+        self.assertEqual("Alumbra", house_results.world)
+        self.assertEqual(HouseStatus.RENTED, house_results.status)
+        self.assertEqual(HouseType.HOUSE, house_results.house_type)
+        self.assertEqual(HouseOrder.RENT, house_results.order)
+
+        houses = house_results.entries
+        self.assertIsInstance(houses, list)
+        self.assertGreater(len(houses), 0)
+        self.assertIsInstance(houses[0], HouseEntry)
+        self.assertEqual(houses[0].town, "Carlin")
+        self.assertEqual(houses[0].type, HouseType.HOUSE)
+        self.assertEqual(houses[0].status, HouseStatus.RENTED)
+        self.assertIsInstance(houses[0].id, int)
+
+        self.assertEqual(houses[25].status, HouseStatus.RENTED)
+
+    def test_house_section_from_content_empty(self):
+        """Testing parsing an empty house list"""
+        content = self.load_resource(FILE_HOUSE_LIST_EMPTY)
+        house_results = HousesSectionParser.from_content(content)
+
+        self.assertIsInstance(house_results, HousesSection)
+        self.assertEqual("Edron", house_results.town)
+        self.assertEqual("Antica", house_results.world)
+        self.assertEqual(HouseStatus.AUCTIONED, house_results.status)
+        self.assertEqual(HouseType.GUILDHALL, house_results.house_type)
+        self.assertEqual(HouseOrder.RENT, house_results.order)
+        self.assertEqual(len(house_results.entries), 0)
+
+    def test_house_section_from_content_not_found(self):
+        """Testing parsing an empty house list"""
+        content = self.load_resource(FILE_HOUSE_LIST_NOT_FOUND)
+        results = HousesSectionParser.from_content(content)
+        self.assertIsInstance(results, HousesSection)
+        self.assertEqual(0, len(results.entries))
+
+    def test_house_section_from_content_unrelated(self):
+        """Testing parsing an unrelated section"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(InvalidContent):
+            HousesSectionParser.from_content(content)
+
```

### Comparing `tibia.py-5.6.1/tests/tests_kill_statistics.py` & `tibia.py-6.0.0a1/tests/tests_kill_statistics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-import unittest
-
-from tests.tests_tibiapy import TestCommons
-from tibiapy import KillStatistics, InvalidContent
-
-FILE_KILL_STATISTICS_FULL = "kill_statistics/tibiacom_full.txt"
-FILE_KILL_STATISTICS_EMPTY = "kill_statistics/tibiacom_empty.txt"
-
-
-class TestHighscores(TestCommons, unittest.TestCase):
-    # region Tibia.com Tests
-    def test_kill_statistics_from_content(self):
-        """Testing parsing kill statistics"""
-        content = self.load_resource(FILE_KILL_STATISTICS_FULL)
-        kill_statistics = KillStatistics.from_content(content)
-
-        self.assertEqual(kill_statistics.world, "Gladera")
-        self.assertEqual(len(kill_statistics.entries), 920)
-        self.assertIsNotNone(kill_statistics.total)
-        self.assertIsNotNone(kill_statistics.url)
-
-        # players shortcurt property
-        self.assertEqual(kill_statistics.players, kill_statistics.entries["players"])
-        self.assertEqual(kill_statistics.players.last_day_killed, 2)
-        self.assertEqual(kill_statistics.players.last_day_killed, kill_statistics.players.last_day_players_killed)
-        self.assertEqual(kill_statistics.players.last_week_killed, 7)
-        self.assertEqual(kill_statistics.players.last_week_killed, kill_statistics.players.last_week_players_killed)
-
-        # demons
-        demons_entry = kill_statistics.entries["demons"]
-        self.assertEqual(2071, demons_entry.last_day_killed)
-        self.assertEqual(1, demons_entry.last_day_players_killed)
-        self.assertEqual(18484, demons_entry.last_week_killed)
-        self.assertEqual(8, demons_entry.last_week_players_killed)
-
-    def test_kill_statistics_from_content_empty(self):
-        """Testing parsing empty kill statistics"""
-        content = self.load_resource(FILE_KILL_STATISTICS_EMPTY)
-        kill_statistics = KillStatistics.from_content(content)
-
-        self.assertIsNone(kill_statistics)
-
-    def test_kill_statistics_from_content_unrelated_section(self):
-        """Testing parsing an unrelated section"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(InvalidContent):
-            KillStatistics.from_content(content)
-
-    # endregion
+import unittest
+
+from tests.tests_tibiapy import TestCommons
+from tibiapy import InvalidContent
+from tibiapy.parsers.kill_statistics import KillStatisticsParser
+
+FILE_KILL_STATISTICS_FULL = "kill_statistics/tibiacom_full.txt"
+FILE_KILL_STATISTICS_EMPTY = "kill_statistics/tibiacom_empty.txt"
+
+
+class TestHighscores(TestCommons, unittest.TestCase):
+    # region Tibia.com Tests
+    def test_kill_statistics_from_content(self):
+        """Testing parsing kill statistics"""
+        content = self.load_resource(FILE_KILL_STATISTICS_FULL)
+        kill_statistics = KillStatisticsParser.from_content(content)
+
+        self.assertEqual(kill_statistics.world, "Gladera")
+        self.assertEqual(len(kill_statistics.entries), 920)
+        self.assertIsNotNone(kill_statistics.total)
+        self.assertIsNotNone(kill_statistics.url)
+
+        # players shortcurt property
+        self.assertEqual(kill_statistics.players, kill_statistics.entries["players"])
+        self.assertEqual(kill_statistics.players.last_day_killed, 2)
+        self.assertEqual(kill_statistics.players.last_day_killed, kill_statistics.players.last_day_players_killed)
+        self.assertEqual(kill_statistics.players.last_week_killed, 7)
+        self.assertEqual(kill_statistics.players.last_week_killed, kill_statistics.players.last_week_players_killed)
+
+        # demons
+        demons_entry = kill_statistics.entries["demons"]
+        self.assertEqual(2071, demons_entry.last_day_killed)
+        self.assertEqual(1, demons_entry.last_day_players_killed)
+        self.assertEqual(18484, demons_entry.last_week_killed)
+        self.assertEqual(8, demons_entry.last_week_players_killed)
+
+    def test_kill_statistics_from_content_empty(self):
+        """Testing parsing empty kill statistics"""
+        content = self.load_resource(FILE_KILL_STATISTICS_EMPTY)
+        kill_statistics = KillStatisticsParser.from_content(content)
+
+        self.assertIsNone(kill_statistics)
+
+    def test_kill_statistics_from_content_unrelated_section(self):
+        """Testing parsing an unrelated section"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(InvalidContent):
+            KillStatisticsParser.from_content(content)
+
+    # endregion
```

### Comparing `tibia.py-5.6.1/tests/tests_news.py` & `tibia.py-6.0.0a1/tests/tests_news.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,119 @@
-import datetime
-import unittest
-
-from tests.tests_tibiapy import TestCommons
-from tibiapy import NewsEntry, News, InvalidContent, NewsArchive
-from tibiapy.enums import NewsCategory, NewsType
-
-FILE_NEWS_LIST = "news/tibiacom_list.txt"
-FILE_NEWS_LIST_EMPTY = "news/tibiacom_list_empty.txt"
-FILE_NEWS_EMPTY = "news/tibiacom_empty.txt"
-FILE_NEWS_ARTICLE = "news/tibiacom_news.txt"
-FILE_NEWS_TICKER = "news/tibiacom_news_ticker.txt"
-
-
-class TestNews(TestCommons, unittest.TestCase):
-    # region Tibia.com Tests
-    def test_news_archive_from_content(self):
-        """Testing parsing news"""
-        content = self.load_resource(FILE_NEWS_LIST)
-        news_archive = NewsArchive.from_content(content)
-
-        self.assertEqual(datetime.date(2019, 3, 25), news_archive.start_date)
-        self.assertEqual(datetime.date(2019, 5, 25), news_archive.end_date)
-        self.assertEqual(3, len(news_archive.types))
-        self.assertEqual(5, len(news_archive.categories))
-
-        news_list = news_archive.entries
-        self.assertGreater(len(news_list), 0)
-        latest_news = news_list[0]
-        self.assertIsInstance(latest_news, NewsEntry)
-        self.assertIsInstance(latest_news.id, int)
-        self.assertIsInstance(latest_news.category, NewsCategory)
-        self.assertIsInstance(latest_news.type, NewsType)
-        self.assertIsInstance(latest_news.date, datetime.date)
-        self.assertIsNotNone(latest_news.url)
-        self.assertEqual(latest_news.url, NewsEntry.get_url(latest_news.id))
-
-    def test_news_archive_from_content_empty(self):
-        """Testing parsing a news article that doesn't exist"""
-        content = self.load_resource(FILE_NEWS_LIST_EMPTY)
-        news_archive = NewsArchive.from_content(content)
-
-        self.assertEqual(datetime.date(2019, 5, 23), news_archive.start_date)
-        self.assertEqual(datetime.date(2019, 5, 25), news_archive.end_date)
-        self.assertEqual(1, len(news_archive.types))
-        self.assertEqual(5, len(news_archive.categories))
-
-        self.assertEqual(0, len(news_archive.entries))
-
-    def test_news_archive_from_content_unrelated(self):
-        """Testing parsing an unrelated section"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(InvalidContent):
-            NewsArchive.from_content(content)
-
-    def test_news_from_content_empty(self):
-        """Testing parsing an empty news article"""
-        content = self.load_resource(FILE_NEWS_EMPTY)
-        news = News.from_content(content)
-        self.assertIsNone(news)
-
-    def test_news_from_content_unrelated(self):
-        """Testing parsing an unrelated section"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(InvalidContent):
-            News.from_content(content)
-
-    def test_news_from_content_ticker(self):
-        """Testing parsing a news ticker"""
-        content = self.load_resource(FILE_NEWS_TICKER)
-        news = News.from_content(content)
-
-        self.assertIsInstance(news, News)
-        self.assertEqual(news.category, NewsCategory.TECHNICAL_ISSUES)
-        self.assertIsInstance(news.date, datetime.date)
-        self.assertEqual(news.title, "News Ticker")
-        self.assertIsNone(news.thread_id)
-
-    def test_news_from_content_article(self):
-        """Testing parsing an article"""
-        content = self.load_resource(FILE_NEWS_ARTICLE)
-        news = News.from_content(content)
-
-        self.assertIsInstance(news, News)
-        self.assertEqual(news.category, NewsCategory.DEVELOPMENT)
-        self.assertIsInstance(news.date, datetime.date)
-        self.assertEqual(news.title, "Sign Up for the VANGUARD Tournament")
-        self.assertEqual(news.thread_id, 4725194)
-
-    # endregion
+import datetime
+import unittest
+
+from tests.tests_tibiapy import TestCommons
+from tibiapy import InvalidContent
+from tibiapy.enums import NewsCategory, NewsType
+from tibiapy.models.news import NewsEntry, NewsArchive, News
+from tibiapy.parsers.news import NewsArchiveParser, NewsParser
+from tibiapy.urls import get_news_url
+
+FILE_NEWS_ARCHIVE_INITIAL = "news/news_archive_initial.txt"
+FILE_NEWS_ARCHIVE_RESULTS = "news/news_archive_results.txt"
+FILE_NEWS_ARCHIVE_EMPTY = "news/news_archive_empty.txt"
+FILE_NEWS_ARCHIVE_ERROR = "news/news_archive_error.txt"
+FILE_NEWS_NOT_FOUND = "news/news_not_found.txt"
+FILE_NEWS_ARTICLE = "news/news_article.txt"
+FILE_NEWS_TICKER = "news/news_ticker.txt"
+
+
+class TestNews(TestCommons, unittest.TestCase):
+    def test_news_archive_parser_from_content_initial(self):
+        """Test parsing the news archive initial page."""
+        content = self.load_resource(FILE_NEWS_ARCHIVE_INITIAL)
+
+        news_archive = NewsArchiveParser.from_content(content)
+
+        self.assertIsInstance(news_archive, NewsArchive)
+        self.assertEqual(datetime.date(2023, 3, 16), news_archive.start_date)
+        self.assertEqual(datetime.date(2023, 4, 15), news_archive.end_date)
+        self.assertEqual(3, len(news_archive.types))
+        self.assertEqual(5, len(news_archive.categories))
+
+    def test_news_archive_parser_from_content_with_results(self):
+        """Testing parsing the news archive with results."""
+        content = self.load_resource(FILE_NEWS_ARCHIVE_RESULTS)
+
+        news_archive = NewsArchiveParser.from_content(content)
+
+        self.assertEqual(datetime.date(2019, 3, 25), news_archive.start_date)
+        self.assertEqual(datetime.date(2019, 5, 25), news_archive.end_date)
+        self.assertEqual(3, len(news_archive.types))
+        self.assertEqual(5, len(news_archive.categories))
+        news_list = news_archive.entries
+        self.assertGreater(len(news_list), 0)
+        latest_news = news_list[0]
+        self.assertIsInstance(latest_news, NewsEntry)
+        self.assertIsInstance(latest_news.id, int)
+        self.assertIsInstance(latest_news.category, NewsCategory)
+        self.assertIsInstance(latest_news.type, NewsType)
+        self.assertIsInstance(latest_news.date, datetime.date)
+        self.assertIsNotNone(latest_news.url)
+        self.assertEqual(latest_news.url, get_news_url(latest_news.id))
+
+    def test_news_archive_parser_from_content_empty(self):
+        """Testing parsing a news article that doesn't exist"""
+        content = self.load_resource(FILE_NEWS_ARCHIVE_EMPTY)
+
+        news_archive = NewsArchiveParser.from_content(content)
+
+        self.assertEqual(datetime.date(2023, 4, 13), news_archive.start_date)
+        self.assertEqual(datetime.date(2023, 4, 15), news_archive.end_date)
+        self.assertEqual(1, len(news_archive.types))
+        self.assertEqual(5, len(news_archive.categories))
+        self.assertEqual(0, len(news_archive.entries))
+
+    def test_news_archive_parser_from_content_error(self):
+        """Testing parsing the news archive resulting in an error message."""
+        content = self.load_resource(FILE_NEWS_ARCHIVE_ERROR)
+
+        news_archive = NewsArchiveParser.from_content(content)
+
+        self.assertIsInstance(news_archive, NewsArchive)
+        self.assertEqual(datetime.date(2019, 3, 25), news_archive.start_date)
+        self.assertEqual(datetime.date(2018, 5, 25), news_archive.end_date)
+        self.assertEqual(3, len(news_archive.types))
+        self.assertEqual(5, len(news_archive.categories))
+        self.assertEqual(0, len(news_archive.entries))
+
+    def test_news_archive_parser_from_content_unrelated(self):
+        """Testing parsing an unrelated section"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(InvalidContent):
+            NewsArchiveParser.from_content(content)
+
+    def test_news_parser_from_content_empty(self):
+        """Testing parsing an empty news article"""
+        content = self.load_resource(FILE_NEWS_NOT_FOUND)
+        news = NewsParser.from_content(content)
+        self.assertIsNone(news)
+
+    def test_news_parser_from_content_unrelated(self):
+        """Testing parsing an unrelated section"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(InvalidContent):
+            NewsParser.from_content(content)
+
+    def test_news_parser_from_content_ticker(self):
+        """Testing parsing a news ticker"""
+        content = self.load_resource(FILE_NEWS_TICKER)
+        news = NewsParser.from_content(content)
+
+        self.assertIsInstance(news, News)
+        self.assertEqual(news.category, NewsCategory.TECHNICAL_ISSUES)
+        self.assertIsInstance(news.date, datetime.date)
+        self.assertEqual(news.title, "News Ticker")
+        self.assertIsNone(news.thread_id)
+
+    def test_news_parser_from_content_article(self):
+        """Testing parsing an article"""
+        content = self.load_resource(FILE_NEWS_ARTICLE)
+        news = NewsParser.from_content(content)
+
+        self.assertIsInstance(news, News)
+        self.assertEqual(news.category, NewsCategory.DEVELOPMENT)
+        self.assertIsInstance(news.date, datetime.date)
+        self.assertEqual(news.title, "Sign Up for the VANGUARD Tournament")
+        self.assertEqual(news.thread_id, 4725194)
+
+
```

### Comparing `tibia.py-5.6.1/tests/tests_spell.py` & `tibia.py-6.0.0a1/tests/tests_spell.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-import unittest
-
-import tibiapy
-from tests.tests_tibiapy import TestCommons
-from tibiapy import Spell, SpellsSection
-
-FILE_SPELLS_SECTION = "library/spell_list_default.txt"
-FILE_SPELL_RUNE = "library/spell_rune.txt"
-FILE_SPELL_SECONDARY_GROUP = "library/spell_secondary_group.txt"
-
-
-class TestSpell(TestCommons, unittest.TestCase):
-    # region Tibia.com Tests
-    def test_spells_section_from_content(self):
-        """Testing parsing a boosted creature"""
-        content = self.load_resource(FILE_SPELLS_SECTION)
-        spells_section = SpellsSection.from_content(content)
-
-        self.assertIsNotNone(spells_section)
-        self.assertEqual(141, len(spells_section.entries))
-
-    def test_spells_section_from_content_unrelated_section(self):
-        """Testing parsing a boosted creature"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(tibiapy.InvalidContent):
-            spells_section = SpellsSection.from_content(content)
-
-    def test_spell_from_content_rune(self):
-        """Testing parsing a rune spell."""
-        content = self.load_resource(FILE_SPELL_RUNE)
-        spell = Spell.from_content(content)
-
-        self.assertIsNotNone(spell)
-        self.assertEqual("Chameleon Rune", spell.name)
-        self.assertEqual("adevo ina", spell.words)
-        self.assertIn("Druid", spell.vocations)
-        self.assertEqual("Support", spell.group.value)
-        self.assertEqual("Rune", spell.spell_type.value)
-        self.assertEqual(2, spell.cooldown)
-        self.assertEqual(2, spell.cooldown_group)
-        self.assertEqual(2, spell.soul_points)
-        self.assertEqual(1, spell.amount)
-        self.assertEqual(27, spell.exp_level)
-        self.assertEqual(600, spell.mana)
-        self.assertEqual(1300, spell.price)
-        self.assertIn("Thais", spell.cities)
-        self.assertIn("Yalahar", spell.cities)
-        self.assertIn("Edron", spell.cities)
-        self.assertFalse(spell.premium)
-        self.assertEqual("Chameleon Rune", spell.rune.name)
-        self.assertIn("Knight", spell.rune.vocations)
-        self.assertEqual("Support", spell.rune.group.value)
-        self.assertEqual(27, spell.rune.exp_level)
-        self.assertEqual(4, spell.rune.magic_level)
-
-    def test_spell_from_content_secondary_group(self):
-        """Testing parsing a spell with a secondary group."""
-        content = self.load_resource(FILE_SPELL_SECONDARY_GROUP)
-        spell = Spell.from_content(content)
-
-        self.assertIsNotNone(spell)
-        self.assertEqual("Protector", spell.name)
-        self.assertEqual("utamo tempo", spell.words)
-        self.assertIn("Knight", spell.vocations)
-        self.assertEqual("Support", spell.group.value)
-        self.assertEqual("Focus", spell.group_secondary)
-        self.assertEqual("Instant", spell.spell_type.value)
-        self.assertEqual(2, spell.cooldown)
-        self.assertEqual(2, spell.cooldown_group)
-        self.assertEqual(2, spell.cooldown_group_secondary)
-        self.assertIsNone(spell.soul_points)
-        self.assertIsNone(spell.amount)
-        self.assertEqual(55, spell.exp_level)
-        self.assertEqual(200, spell.mana)
-        self.assertEqual(6000, spell.price)
-        self.assertIn("Edron", spell.cities)
-        self.assertTrue(spell.premium)
-
-    def test_spells_from_content_unknown_spell(self):
-        """Testing parsing an unknown spell
-
-        When trying to fetch a spell that doesn't exist, the website will just show the spells section."""
-        content = self.load_resource(FILE_SPELLS_SECTION)
-        spell = Spell.from_content(content)
-
-        self.assertIsNone(spell)
-
-    def test_spells_from_content_unrelated_section(self):
-        """Testing parsing a boosted creature"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(tibiapy.InvalidContent):
-            spell = Spell.from_content(content)
-
-    # endregion
+import unittest
+
+import tibiapy
+from tests.tests_tibiapy import TestCommons
+from tibiapy.parsers.spell import SpellsSectionParser, SpellParser
+
+FILE_SPELLS_SECTION = "library/spell_list_default.txt"
+FILE_SPELL_RUNE = "library/spell_rune.txt"
+FILE_SPELL_SECONDARY_GROUP = "library/spell_secondary_group.txt"
+
+
+class TestSpell(TestCommons, unittest.TestCase):
+    # region Tibia.com Tests
+    def test_spells_section_from_content(self):
+        """Testing parsing a boosted creature"""
+        content = self.load_resource(FILE_SPELLS_SECTION)
+        spells_section = SpellsSectionParser.from_content(content)
+
+        self.assertIsNotNone(spells_section)
+        self.assertEqual(141, len(spells_section.entries))
+
+    def test_spells_section_from_content_unrelated_section(self):
+        """Testing parsing a boosted creature"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(tibiapy.InvalidContent):
+            spells_section = SpellsSectionParser.from_content(content)
+
+    def test_spell_from_content_rune(self):
+        """Testing parsing a rune spell."""
+        content = self.load_resource(FILE_SPELL_RUNE)
+        spell = SpellParser.from_content(content)
+
+        self.assertIsNotNone(spell)
+        self.assertEqual("Chameleon Rune", spell.name)
+        self.assertEqual("adevo ina", spell.words)
+        self.assertIn("Druid", spell.vocations)
+        self.assertEqual("Support", spell.group.value)
+        self.assertEqual("Rune", spell.spell_type.value)
+        self.assertEqual(2, spell.cooldown)
+        self.assertEqual(2, spell.cooldown_group)
+        self.assertEqual(2, spell.soul_points)
+        self.assertEqual(1, spell.amount)
+        self.assertEqual(27, spell.exp_level)
+        self.assertEqual(600, spell.mana)
+        self.assertEqual(1300, spell.price)
+        self.assertIn("Thais", spell.cities)
+        self.assertIn("Yalahar", spell.cities)
+        self.assertIn("Edron", spell.cities)
+        self.assertFalse(spell.premium)
+        self.assertEqual("Chameleon Rune", spell.rune.name)
+        self.assertIn("Knight", spell.rune.vocations)
+        self.assertEqual("Support", spell.rune.group.value)
+        self.assertEqual(27, spell.rune.exp_level)
+        self.assertEqual(4, spell.rune.magic_level)
+
+    def test_spell_from_content_secondary_group(self):
+        """Testing parsing a spell with a secondary group."""
+        content = self.load_resource(FILE_SPELL_SECONDARY_GROUP)
+        spell = SpellParser.from_content(content)
+
+        self.assertIsNotNone(spell)
+        self.assertEqual("Protector", spell.name)
+        self.assertEqual("utamo tempo", spell.words)
+        self.assertIn("Knight", spell.vocations)
+        self.assertEqual("Support", spell.group.value)
+        self.assertEqual("Focus", spell.group_secondary)
+        self.assertEqual("Instant", spell.spell_type.value)
+        self.assertEqual(2, spell.cooldown)
+        self.assertEqual(2, spell.cooldown_group)
+        self.assertEqual(2, spell.cooldown_group_secondary)
+        self.assertIsNone(spell.soul_points)
+        self.assertIsNone(spell.amount)
+        self.assertEqual(55, spell.exp_level)
+        self.assertEqual(200, spell.mana)
+        self.assertEqual(6000, spell.price)
+        self.assertIn("Edron", spell.cities)
+        self.assertTrue(spell.premium)
+
+    def test_spells_from_content_unknown_spell(self):
+        """Testing parsing an unknown spell
+
+        When trying to fetch a spell that doesn't exist, the website will just show the spells section."""
+        content = self.load_resource(FILE_SPELLS_SECTION)
+        spell = SpellParser.from_content(content)
+
+        self.assertIsNone(spell)
+
+    def test_spells_from_content_unrelated_section(self):
+        """Testing parsing a boosted creature"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(tibiapy.InvalidContent):
+            spell = SpellParser.from_content(content)
+
+    # endregion
```

### Comparing `tibia.py-5.6.1/tests/tests_utils.py` & `tibia.py-6.0.0a1/tests/tests_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,262 +1,238 @@
-import datetime
-import unittest
-
-import tibiapy
-from tests.tests_tibiapy import TestCommons
-from tibiapy import enums, utils
-from tibiapy.utils import get_tibia_url, parse_integer, parse_tibia_money
-
-TIBIA_DATETIME_CEST = "Jul 10 2018, 07:13:32 CEST"
-TIBIA_DATETIME_CET = "Jan 10 2018, 07:13:32 CET"
-TIBIA_DATETIME_PST = "Aug 10 2015, 23:13:32 PST"
-TIBIA_DATETIME_INVALID = "13:37:00 10 Feb 2003"
-
-TIBIA_DATE = "Jun 20 2018"
-TIBIA_FULL_DATE = "July 23, 2015"
-TIBIA_DATE_INVALID = "8 Nov 2018"
-
-
-class TestUtils(TestCommons, unittest.TestCase):
-    def test_serializable_get_item(self):
-        """Testing the muliple ways to use __get__ for Serializable"""
-        # Class inherits from Serializable
-        world = tibiapy.World("Calmera")
-
-        # Serializable allows accessing attributes like a dictionary
-        self.assertEqual(world.name, world["name"])
-        # And setting values too
-        world["location"] = tibiapy.enums.WorldLocation.NORTH_AMERICA
-        self.assertEqual(world.location, tibiapy.enums.WorldLocation.NORTH_AMERICA)
-
-        # Accessing via __get__ returns KeyError instead of AttributeError to follow dictionary behaviour
-        with self.assertRaises(KeyError):
-            _level = world["level"]  # NOSONAR
-
-        # Accessing an undefined attribute that is defined in __slots__ returns `None` instead of raising an exception.
-        del world.location
-        self.assertIsNone(world["location"])
-
-        # New attributes can't be created by assignation
-        with self.assertRaises(KeyError):
-            world["custom"] = "custom value"
-
-    def test_parse_tibia_datetime(self):
-        time = utils.parse_tibia_datetime(TIBIA_DATETIME_CEST)
-        self.assertIsInstance(time, datetime.datetime)
-        self.assertEqual(time.month, 7)
-        self.assertEqual(time.day, 10)
-        self.assertEqual(time.year, 2018)
-        self.assertEqual(time.hour, 5)
-        self.assertEqual(time.minute, 13)
-        self.assertEqual(time.second, 32)
-
-        time = utils.parse_tibia_datetime(TIBIA_DATETIME_CET)
-        self.assertIsInstance(time, datetime.datetime)
-        self.assertEqual(time.month, 1)
-        self.assertEqual(time.day, 10)
-        self.assertEqual(time.year, 2018)
-        self.assertEqual(time.hour, 6)
-        self.assertEqual(time.minute, 13)
-        self.assertEqual(time.second, 32)
-
-    def test_parse_tibia_datetime_invalid_timezone(self):
-        time = utils.parse_tibia_datetime(TIBIA_DATETIME_PST)
-        self.assertIsNone(time)
-
-    def test_parse_tibia_datetime_invalid_datetime(self):
-        time = utils.parse_tibia_datetime(TIBIA_DATETIME_INVALID)
-        self.assertIsNone(time)
-
-    def test_parse_tibia_date(self):
-        date = utils.parse_tibia_date(TIBIA_DATE)
-        self.assertIsInstance(date, datetime.date)
-        self.assertEqual(date.month, 6)
-        self.assertEqual(date.day, 20)
-        self.assertEqual(date.year, 2018)
-
-    def test_parse_tibia_date_full(self):
-        date = utils.parse_tibia_full_date(TIBIA_FULL_DATE)
-        self.assertIsInstance(date, datetime.date)
-        self.assertEqual(date.month, 7)
-        self.assertEqual(date.day, 23)
-        self.assertEqual(date.year, 2015)
-
-    def test_parse_tibia_date_invalid(self):
-        date = utils.parse_tibia_date(TIBIA_DATETIME_INVALID)
-        self.assertIsNone(date)
-
-    def test_try_date(self):
-        date = utils.try_date(datetime.datetime.now())
-        self.assertIsInstance(date, datetime.date)
-
-        date = utils.try_date(datetime.date.today())
-        self.assertIsInstance(date, datetime.date)
-        self.assertEqual(date, datetime.date.today())
-
-        date = utils.try_date(TIBIA_DATE)
-        self.assertIsInstance(date, datetime.date)
-
-        date = utils.try_date(TIBIA_FULL_DATE)
-        self.assertIsInstance(date, datetime.date)
-
-    def test_try_date_time(self):
-        date_time = utils.try_datetime(datetime.datetime.now())
-        self.assertIsInstance(date_time, datetime.datetime)
-
-        date_time = utils.try_datetime(TIBIA_DATETIME_CEST)
-        self.assertIsInstance(date_time, datetime.datetime)
-
-    def test_parse_number_words(self):
-        self.assertEqual(utils.parse_number_words("one"), 1)
-        self.assertEqual(utils.parse_number_words("no"), 0)
-        self.assertEqual(utils.parse_number_words("..."), 0)
-        self.assertEqual(utils.parse_number_words("twenty-one"), 21)
-        self.assertEqual(utils.parse_number_words("one hundred two"), 102)
-        self.assertEqual(utils.parse_number_words("two thousand forty five"), 2045)
-
-    def test_try_enum(self):
-        self.assertEqual(utils.try_enum(enums.Sex, "male"), enums.Sex.MALE)
-        self.assertEqual(utils.try_enum(enums.TransferType, "", enums.TransferType.REGULAR), enums.TransferType.REGULAR)
-        self.assertEqual(utils.try_enum(enums.WorldLocation, enums.WorldLocation.EUROPE), enums.WorldLocation.EUROPE)
-        self.assertEqual(utils.try_enum(enums.VocationFilter, 4), enums.VocationFilter.SORCERERS)
-        self.assertEqual(utils.try_enum(enums.Category, "FISHING"), enums.Category.FISHING)
-
-    def test_enum_str(self):
-        self.assertEqual(str(enums.Sex.MALE), enums.Sex.MALE.value)
-        self.assertEqual(enums.VocationFilter.from_name("royal paladin"), enums.VocationFilter.PALADINS)
-        self.assertEqual(enums.VocationFilter.from_name("unknown"), enums.VocationFilter.ALL)
-        self.assertIsNone(enums.VocationFilter.from_name("unknown", False))
-
-    def test_parse_tibia_money(self):
-        self.assertEqual(1000, parse_tibia_money("1k"))
-        self.assertEqual(5000000, parse_tibia_money("5kk"))
-        self.assertEqual(2500, parse_tibia_money("2.5k"))
-        self.assertEqual(50, parse_tibia_money("50"))
-        with self.assertRaises(ValueError):
-            parse_tibia_money("abc")
-
-    def test_parse_integer(self):
-        self.assertEqual(1450, parse_integer("1.450"))
-        self.assertEqual(1110, parse_integer("1,110"))
-        self.assertEqual(15, parse_integer("15"))
-        self.assertEqual(0, parse_integer("abc"))
-        self.assertEqual(-1, parse_integer("abc", -1))
-
-    def test_get_tibia_url(self):
-        self.assertEqual("https://www.tibia.com/community/?subtopic=character&name=Galarzaa+Fidera",
-                         get_tibia_url("community", "character", name="Galarzaa Fidera"))
-        self.assertEqual("https://www.tibia.com/community/?subtopic=character&name=Fn%F6",
-                         get_tibia_url("community", "character", name="Fnö"))
-
-    def test_parse_pagination_collapsed_first_page(self):
-        """Parsing with current page 1 out of 915"""
-        content = """<td class="PageNavigation"><small><div style="float: left;"><b>» <span class="PageLink 
-        FirstOrLastElement"><span class="CurrentPageLink">First Page</span></span> <span class="PageLink "><a 
-        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=2">2</a></span> 
-        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
-        ;currentpage=3">3</a></span> <span class="PageLink "><a 
-        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=4">4</a></span> 
-        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
-        ;currentpage=5">5</a></span> <span class="PageLink "><a 
-        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=6">6</a></span> 
-        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
-        ;currentpage=7">7</a></span> ... <span class="PageLink FirstOrLastElement"><a 
-        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=915">Last 
-        Page</a></span></b></div><div style="float: right;"><b>» Results: 22874</b></div></small></td>"""
-        parsed_content = utils.parse_tibiacom_content(content, builder="html5lib")
-        page, total_pages, results_count = utils.parse_pagination(parsed_content)
-        self.assertEqual(1, page)
-        self.assertEqual(915, total_pages)
-        self.assertEqual(22874, results_count)
-
-    def test_parse_pagination_collapse_second_page(self):
-        """Parsing with current page 2 out of 928"""
-        content = """<td class="PageNavigation"><small><div style="float: left;"><b>» <span class="PageLink 
-        FirstOrLastElement"><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
-        ;currentpage=1">First Page</a></span> <span class="PageLink "><span class="CurrentPageLink">2</span></span> 
-        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
-        ;currentpage=3">3</a></span> <span class="PageLink "><a 
-        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=4">4</a></span> 
-        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
-        ;currentpage=5">5</a></span> <span class="PageLink "><a 
-        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=6">6</a></span> 
-        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
-        ;currentpage=7">7</a></span> <span class="PageLink "><a 
-        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=8">8</a></span> ... 
-        <span class="PageLink FirstOrLastElement"><a 
-        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=928">Last 
-        Page</a></span></b></div><div style="float: right;"><b>» Results: 23197</b></div></small></td> """
-        parsed_content = utils.parse_tibiacom_content(content, builder="html5lib")
-        page, total_pages, results_count = utils.parse_pagination(parsed_content)
-        self.assertEqual(2, page)
-        self.assertEqual(928, total_pages)
-        self.assertEqual(23197, results_count)
-
-    def test_parse_pagination_collapse_last_page(self):
-        """Parsing the last page out of 928"""
-        content = """<td class="PageNavigation"><small><div style="float: left;"><b>» <span class="PageLink 
-        FirstOrLastElement"><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
-        ;currentpage=1">First Page</a></span> ... <span class="PageLink "><a 
-        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=925">925</a></span> 
-        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
-        ;currentpage=926">926</a></span> <span class="PageLink "><a 
-        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=927">927</a></span> 
-        <span class="PageLink FirstOrLastElement"><span class="CurrentPageLink">Last Page</span></span></b></div><div 
-        style="float: right;"><b>» Results: 23197</b></div></small></td> """
-        parsed_content = utils.parse_tibiacom_content(content, builder="html5lib")
-        page, total_pages, results_count = utils.parse_pagination(parsed_content)
-        self.assertEqual(928, page)
-        self.assertEqual(928, total_pages)
-        self.assertEqual(23197, results_count)
-
-    def test_parse_pagination_collapsed_middle(self):
-        """Parsing page 300 out of 503"""
-        content = """<td class="PageNavigation"><small><div style="float: left;"><b>» <span class="PageLink 
-        FirstOrLastElement"><a href="https://www.tibia.com/charactertrade/?subtopic=currentcharactertrades&amp
-        ;currentpage=1">First Page</a></span> ... <span class="PageLink "><a 
-        href="https://www.tibia.com/charactertrade/?subtopic=currentcharactertrades&currentpage=297">297</a></span> 
-        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=currentcharactertrades
-        &currentpage=298">298</a></span> <span class="PageLink "><a 
-        href="https://www.tibia.com/charactertrade/?subtopic=currentcharactertrades&currentpage=299">299</a></span> 
-        <span class="PageLink "><span class="CurrentPageLink">300</span></span> <span class="PageLink "><a 
-        href="https://www.tibia.com/charactertrade/?subtopic=currentcharactertrades&currentpage=301">301</a></span> 
-        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=currentcharactertrades
-        &currentpage=302">302</a></span> <span class="PageLink "><a 
-        href="https://www.tibia.com/charactertrade/?subtopic=currentcharactertrades&currentpage=303">303</a></span> 
-        ... <span class="PageLink FirstOrLastElement"><a 
-        href="https://www.tibia.com/charactertrade/?subtopic=currentcharactertrades&currentpage=503">Last 
-        Page</a></span></b></div><div style="float: right;"><b>» Results: 12568</b></div></small></td> """
-        parsed_content = utils.parse_tibiacom_content(content, builder="html5lib")
-        page, total_pages, results_count = utils.parse_pagination(parsed_content)
-        self.assertEqual(300, page)
-        self.assertEqual(503, total_pages)
-        self.assertEqual(12568, results_count)
-
-    def parse_parse_pagination_not_collapsed_first_page(self):
-        """Parsing first page with page numbers not collapsed"""
-        content = """<small><div style="float: left;"><b>» Pages: <span 
-        class="PageLink "><span class="CurrentPageLink">1</span></span> <span class="PageLink "><a 
-        class="CipAjaxLink" ajaxcip="true" ajaxcip_datatype="Container" 
-        href="https://www.tibia.com/charactertrade/ajax_getcharacterdata.php?auctionid=29122&amp;type=0&amp
-        ;currentpage=2">2</a></span> <span class="PageLink "><a class="CipAjaxLink" ajaxcip="true" 
-        ajaxcip_datatype="Container" href="https://www.tibia.com/charactertrade/ajax_getcharacterdata.php?auctionid
-        =29122&amp;type=0&amp;currentpage=3">3</a></span> <span class="PageLink "><a class="CipAjaxLink" 
-        ajaxcip="true" ajaxcip_datatype="Container" 
-        href="https://www.tibia.com/charactertrade/ajax_getcharacterdata.php?auctionid=29122&amp;type=0&amp
-        ;currentpage=4">4</a></span> <span class="PageLink "><a class="CipAjaxLink" ajaxcip="true" 
-        ajaxcip_datatype="Container" href="https://www.tibia.com/charactertrade/ajax_getcharacterdata.php?auctionid
-        =29122&amp;type=0&amp;currentpage=5">5</a></span> <span class="PageLink "><a class="CipAjaxLink" 
-        ajaxcip="true" ajaxcip_datatype="Container" 
-        href="https://www.tibia.com/charactertrade/ajax_getcharacterdata.php?auctionid=29122&amp;type=0&amp
-        ;currentpage=6">6</a></span> <span class="PageLink "><a class="CipAjaxLink" ajaxcip="true" 
-        ajaxcip_datatype="Container" href="https://www.tibia.com/charactertrade/ajax_getcharacterdata.php?auctionid
-        =29122&amp;type=0&amp;currentpage=7">7</a></span> <span class="PageLink "><a class="CipAjaxLink" 
-        ajaxcip="true" ajaxcip_datatype="Container" 
-        href="https://www.tibia.com/charactertrade/ajax_getcharacterdata.php?auctionid=29122&amp;type=0&amp
-        ;currentpage=8">8</a></span></b></div><div style="float: right;"><b>» Results: 567</b></div></small>"""
-        parsed_content = utils.parse_tibiacom_content(content, builder="html5lib")
-        page, total_pages, results_count = utils.parse_pagination(parsed_content)
-        self.assertEqual(1, page)
-        self.assertEqual(8, total_pages)
-        self.assertEqual(567, results_count)
-
+import datetime
+import unittest
+
+from tests.tests_tibiapy import TestCommons
+from tibiapy import enums, utils
+from tibiapy.utils import get_tibia_url, parse_integer, parse_tibia_money
+
+TIBIA_DATETIME_CEST = "Jul 10 2018, 07:13:32 CEST"
+TIBIA_DATETIME_CET = "Jan 10 2018, 07:13:32 CET"
+TIBIA_DATETIME_PST = "Aug 10 2015, 23:13:32 PST"
+TIBIA_DATETIME_INVALID = "13:37:00 10 Feb 2003"
+
+TIBIA_DATE = "Jun 20 2018"
+TIBIA_FULL_DATE = "July 23, 2015"
+TIBIA_DATE_INVALID = "8 Nov 2018"
+
+
+class TestUtils(TestCommons, unittest.TestCase):
+
+    def test_parse_tibia_datetime(self):
+        time = utils.parse_tibia_datetime(TIBIA_DATETIME_CEST)
+        self.assertIsInstance(time, datetime.datetime)
+        self.assertEqual(time.month, 7)
+        self.assertEqual(time.day, 10)
+        self.assertEqual(time.year, 2018)
+        self.assertEqual(time.hour, 5)
+        self.assertEqual(time.minute, 13)
+        self.assertEqual(time.second, 32)
+
+        time = utils.parse_tibia_datetime(TIBIA_DATETIME_CET)
+        self.assertIsInstance(time, datetime.datetime)
+        self.assertEqual(time.month, 1)
+        self.assertEqual(time.day, 10)
+        self.assertEqual(time.year, 2018)
+        self.assertEqual(time.hour, 6)
+        self.assertEqual(time.minute, 13)
+        self.assertEqual(time.second, 32)
+
+    def test_parse_tibia_datetime_invalid_timezone(self):
+        time = utils.parse_tibia_datetime(TIBIA_DATETIME_PST)
+        self.assertIsNone(time)
+
+    def test_parse_tibia_datetime_invalid_datetime(self):
+        time = utils.parse_tibia_datetime(TIBIA_DATETIME_INVALID)
+        self.assertIsNone(time)
+
+    def test_parse_tibia_date(self):
+        date = utils.parse_tibia_date(TIBIA_DATE)
+        self.assertIsInstance(date, datetime.date)
+        self.assertEqual(date.month, 6)
+        self.assertEqual(date.day, 20)
+        self.assertEqual(date.year, 2018)
+
+    def test_parse_tibia_date_full(self):
+        date = utils.parse_tibia_full_date(TIBIA_FULL_DATE)
+        self.assertIsInstance(date, datetime.date)
+        self.assertEqual(date.month, 7)
+        self.assertEqual(date.day, 23)
+        self.assertEqual(date.year, 2015)
+
+    def test_parse_tibia_date_invalid(self):
+        date = utils.parse_tibia_date(TIBIA_DATETIME_INVALID)
+        self.assertIsNone(date)
+
+    def test_try_date(self):
+        date = utils.try_date(datetime.datetime.now())
+        self.assertIsInstance(date, datetime.date)
+
+        date = utils.try_date(datetime.date.today())
+        self.assertIsInstance(date, datetime.date)
+        self.assertEqual(date, datetime.date.today())
+
+        date = utils.try_date(TIBIA_DATE)
+        self.assertIsInstance(date, datetime.date)
+
+        date = utils.try_date(TIBIA_FULL_DATE)
+        self.assertIsInstance(date, datetime.date)
+
+    def test_try_date_time(self):
+        date_time = utils.try_datetime(datetime.datetime.now())
+        self.assertIsInstance(date_time, datetime.datetime)
+
+        date_time = utils.try_datetime(TIBIA_DATETIME_CEST)
+        self.assertIsInstance(date_time, datetime.datetime)
+
+    def test_parse_number_words(self):
+        self.assertEqual(utils.parse_number_words("one"), 1)
+        self.assertEqual(utils.parse_number_words("no"), 0)
+        self.assertEqual(utils.parse_number_words("..."), 0)
+        self.assertEqual(utils.parse_number_words("twenty-one"), 21)
+        self.assertEqual(utils.parse_number_words("one hundred two"), 102)
+        self.assertEqual(utils.parse_number_words("two thousand forty five"), 2045)
+
+    def test_try_enum(self):
+        self.assertEqual(utils.try_enum(enums.Sex, "male"), enums.Sex.MALE)
+        self.assertEqual(utils.try_enum(enums.TransferType, "", enums.TransferType.REGULAR), enums.TransferType.REGULAR)
+        self.assertEqual(utils.try_enum(enums.WorldLocation, enums.WorldLocation.EUROPE), enums.WorldLocation.EUROPE)
+        self.assertEqual(utils.try_enum(enums.HighscoresProfession, 4), enums.HighscoresProfession.SORCERERS)
+        self.assertEqual(utils.try_enum(enums.HighscoresCategory, "FISHING"), enums.HighscoresCategory.FISHING)
+
+    def test_enum_str(self):
+        self.assertEqual(enums.HighscoresProfession.from_name("royal paladin"), enums.HighscoresProfession.PALADINS)
+        self.assertEqual(enums.HighscoresProfession.from_name("unknown"), enums.HighscoresProfession.ALL)
+        self.assertIsNone(enums.HighscoresProfession.from_name("unknown", False))
+
+    def test_parse_tibia_money(self):
+        self.assertEqual(1000, parse_tibia_money("1k"))
+        self.assertEqual(5000000, parse_tibia_money("5kk"))
+        self.assertEqual(2500, parse_tibia_money("2.5k"))
+        self.assertEqual(50, parse_tibia_money("50"))
+        with self.assertRaises(ValueError):
+            parse_tibia_money("abc")
+
+    def test_parse_integer(self):
+        self.assertEqual(1450, parse_integer("1.450"))
+        self.assertEqual(1110, parse_integer("1,110"))
+        self.assertEqual(15, parse_integer("15"))
+        self.assertEqual(0, parse_integer("abc"))
+        self.assertEqual(-1, parse_integer("abc", -1))
+
+    def test_get_tibia_url(self):
+        self.assertEqual("https://www.tibia.com/community/?subtopic=character&name=Galarzaa+Fidera",
+                         get_tibia_url("community", "character", name="Galarzaa Fidera"))
+        self.assertEqual("https://www.tibia.com/community/?subtopic=character&name=Fn%F6",
+                         get_tibia_url("community", "character", name="Fnö"))
+
+    def test_parse_pagination_collapsed_first_page(self):
+        """Parsing with current page 1 out of 915"""
+        content = """<td class="PageNavigation"><small><div style="float: left;"><b>» <span class="PageLink 
+        FirstOrLastElement"><span class="CurrentPageLink">First Page</span></span> <span class="PageLink "><a 
+        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=2">2</a></span> 
+        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
+        ;currentpage=3">3</a></span> <span class="PageLink "><a 
+        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=4">4</a></span> 
+        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
+        ;currentpage=5">5</a></span> <span class="PageLink "><a 
+        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=6">6</a></span> 
+        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
+        ;currentpage=7">7</a></span> ... <span class="PageLink FirstOrLastElement"><a 
+        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=915">Last 
+        Page</a></span></b></div><div style="float: right;"><b>» Results: 22874</b></div></small></td>"""
+        parsed_content = utils.parse_tibiacom_content(content, builder="html5lib")
+        page, total_pages, results_count = utils.parse_pagination(parsed_content)
+        self.assertEqual(1, page)
+        self.assertEqual(915, total_pages)
+        self.assertEqual(22874, results_count)
+
+    def test_parse_pagination_collapse_second_page(self):
+        """Parsing with current page 2 out of 928"""
+        content = """<td class="PageNavigation"><small><div style="float: left;"><b>» <span class="PageLink 
+        FirstOrLastElement"><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
+        ;currentpage=1">First Page</a></span> <span class="PageLink "><span class="CurrentPageLink">2</span></span> 
+        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
+        ;currentpage=3">3</a></span> <span class="PageLink "><a 
+        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=4">4</a></span> 
+        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
+        ;currentpage=5">5</a></span> <span class="PageLink "><a 
+        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=6">6</a></span> 
+        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
+        ;currentpage=7">7</a></span> <span class="PageLink "><a 
+        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=8">8</a></span> ... 
+        <span class="PageLink FirstOrLastElement"><a 
+        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=928">Last 
+        Page</a></span></b></div><div style="float: right;"><b>» Results: 23197</b></div></small></td> """
+        parsed_content = utils.parse_tibiacom_content(content, builder="html5lib")
+        page, total_pages, results_count = utils.parse_pagination(parsed_content)
+        self.assertEqual(2, page)
+        self.assertEqual(928, total_pages)
+        self.assertEqual(23197, results_count)
+
+    def test_parse_pagination_collapse_last_page(self):
+        """Parsing the last page out of 928"""
+        content = """<td class="PageNavigation"><small><div style="float: left;"><b>» <span class="PageLink 
+        FirstOrLastElement"><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
+        ;currentpage=1">First Page</a></span> ... <span class="PageLink "><a 
+        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=925">925</a></span> 
+        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp
+        ;currentpage=926">926</a></span> <span class="PageLink "><a 
+        href="https://www.tibia.com/charactertrade/?subtopic=pastcharactertrades&amp;currentpage=927">927</a></span> 
+        <span class="PageLink FirstOrLastElement"><span class="CurrentPageLink">Last Page</span></span></b></div><div 
+        style="float: right;"><b>» Results: 23197</b></div></small></td> """
+        parsed_content = utils.parse_tibiacom_content(content, builder="html5lib")
+        page, total_pages, results_count = utils.parse_pagination(parsed_content)
+        self.assertEqual(928, page)
+        self.assertEqual(928, total_pages)
+        self.assertEqual(23197, results_count)
+
+    def test_parse_pagination_collapsed_middle(self):
+        """Parsing page 300 out of 503"""
+        content = """<td class="PageNavigation"><small><div style="float: left;"><b>» <span class="PageLink 
+        FirstOrLastElement"><a href="https://www.tibia.com/charactertrade/?subtopic=currentcharactertrades&amp
+        ;currentpage=1">First Page</a></span> ... <span class="PageLink "><a 
+        href="https://www.tibia.com/charactertrade/?subtopic=currentcharactertrades&currentpage=297">297</a></span> 
+        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=currentcharactertrades
+        &currentpage=298">298</a></span> <span class="PageLink "><a 
+        href="https://www.tibia.com/charactertrade/?subtopic=currentcharactertrades&currentpage=299">299</a></span> 
+        <span class="PageLink "><span class="CurrentPageLink">300</span></span> <span class="PageLink "><a 
+        href="https://www.tibia.com/charactertrade/?subtopic=currentcharactertrades&currentpage=301">301</a></span> 
+        <span class="PageLink "><a href="https://www.tibia.com/charactertrade/?subtopic=currentcharactertrades
+        &currentpage=302">302</a></span> <span class="PageLink "><a 
+        href="https://www.tibia.com/charactertrade/?subtopic=currentcharactertrades&currentpage=303">303</a></span> 
+        ... <span class="PageLink FirstOrLastElement"><a 
+        href="https://www.tibia.com/charactertrade/?subtopic=currentcharactertrades&currentpage=503">Last 
+        Page</a></span></b></div><div style="float: right;"><b>» Results: 12568</b></div></small></td> """
+        parsed_content = utils.parse_tibiacom_content(content, builder="html5lib")
+        page, total_pages, results_count = utils.parse_pagination(parsed_content)
+        self.assertEqual(300, page)
+        self.assertEqual(503, total_pages)
+        self.assertEqual(12568, results_count)
+
+    def parse_parse_pagination_not_collapsed_first_page(self):
+        """Parsing first page with page numbers not collapsed"""
+        content = """<small><div style="float: left;"><b>» Pages: <span 
+        class="PageLink "><span class="CurrentPageLink">1</span></span> <span class="PageLink "><a 
+        class="CipAjaxLink" ajaxcip="true" ajaxcip_datatype="Container" 
+        href="https://www.tibia.com/charactertrade/ajax_getcharacterdata.php?auctionid=29122&amp;type=0&amp
+        ;currentpage=2">2</a></span> <span class="PageLink "><a class="CipAjaxLink" ajaxcip="true" 
+        ajaxcip_datatype="Container" href="https://www.tibia.com/charactertrade/ajax_getcharacterdata.php?auctionid
+        =29122&amp;type=0&amp;currentpage=3">3</a></span> <span class="PageLink "><a class="CipAjaxLink" 
+        ajaxcip="true" ajaxcip_datatype="Container" 
+        href="https://www.tibia.com/charactertrade/ajax_getcharacterdata.php?auctionid=29122&amp;type=0&amp
+        ;currentpage=4">4</a></span> <span class="PageLink "><a class="CipAjaxLink" ajaxcip="true" 
+        ajaxcip_datatype="Container" href="https://www.tibia.com/charactertrade/ajax_getcharacterdata.php?auctionid
+        =29122&amp;type=0&amp;currentpage=5">5</a></span> <span class="PageLink "><a class="CipAjaxLink" 
+        ajaxcip="true" ajaxcip_datatype="Container" 
+        href="https://www.tibia.com/charactertrade/ajax_getcharacterdata.php?auctionid=29122&amp;type=0&amp
+        ;currentpage=6">6</a></span> <span class="PageLink "><a class="CipAjaxLink" ajaxcip="true" 
+        ajaxcip_datatype="Container" href="https://www.tibia.com/charactertrade/ajax_getcharacterdata.php?auctionid
+        =29122&amp;type=0&amp;currentpage=7">7</a></span> <span class="PageLink "><a class="CipAjaxLink" 
+        ajaxcip="true" ajaxcip_datatype="Container" 
+        href="https://www.tibia.com/charactertrade/ajax_getcharacterdata.php?auctionid=29122&amp;type=0&amp
+        ;currentpage=8">8</a></span></b></div><div style="float: right;"><b>» Results: 567</b></div></small>"""
+        parsed_content = utils.parse_tibiacom_content(content, builder="html5lib")
+        page, total_pages, results_count = utils.parse_pagination(parsed_content)
+        self.assertEqual(1, page)
+        self.assertEqual(8, total_pages)
+        self.assertEqual(567, results_count)
+
```

### Comparing `tibia.py-5.6.1/tests/tests_world.py` & `tibia.py-6.0.0a1/tests/tests_world.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,138 +1,122 @@
-import datetime
-import json
-import unittest
-
-from tests.tests_tibiapy import TestCommons
-from tibiapy import InvalidContent, TournamentWorldType, World, WorldOverview
-from tibiapy.enums import PvpType, TransferType, WorldLocation
-from tibiapy.world import WorldEntry
-
-FILE_WORLD_FULL = "world/tibiacom_online.txt"
-FILE_WORLD_FULL_OFFLINE = "world/tibiacom_offline.txt"
-FILE_WORLD_TOURNAMENT = "world/tibiacom_tournament.txt"
-FILE_WORLD_NOT_FOUND = "world/tibiacom_not_found.txt"
-FILE_WORLD_LIST = "world/tibiacom_list_online.txt"
-FILE_WORLD_LIST_OFFLINE = "world/tibiacom_list_offline.txt"
-
-
-class TestWorld(TestCommons, unittest.TestCase):
-
-    # region Tibia.com Tests
-    def test_world_from_content_full(self):
-        """Testing parsing a world with full information"""
-        content = self.load_resource(FILE_WORLD_FULL)
-        world = World.from_content(content)
-
-        self.assertIsInstance(world, World)
-        self.assertEqual(world.name, "Premia")
-        self.assertEqual(world.status, "Online")
-        self.assertEqual(world.record_count, 531)
-        self.assertIsInstance(world.record_date, datetime.datetime)
-        self.assertEqual(world.creation_date, "2002-04")
-        self.assertEqual(world.creation_year, 2002)
-        self.assertEqual(world.creation_month, 4)
-        self.assertEqual(world.location, WorldLocation.EUROPE)
-        self.assertEqual(world.pvp_type, PvpType.OPEN_PVP)
-        self.assertEqual(world.transfer_type, TransferType.REGULAR)
-        self.assertEqual(len(world.world_quest_titles), 4)
-        self.assertTrue(world.premium_only)
-        self.assertTrue(world.battleye_protected)
-        self.assertEqual(world.battleye_date, datetime.date(2017, 9, 5))
-        self.assertFalse(world.experimental)
-        self.assertEqual(len(world.online_players), world.online_count)
-        self.assertEqual(World.get_url(world.name), world.url)
-
-        world_json_raw = world.to_json()
-        world_json = json.loads(world_json_raw)
-        self.assertEqual(len(world.online_players), len(world_json["online_players"]))
-
-    def test_world_from_content_offline(self):
-        """Testing parsing an offline world"""
-        content = self.load_resource(FILE_WORLD_FULL_OFFLINE, )
-        world = World.from_content(content)
-
-        self.assertIsInstance(world, World)
-        self.assertEqual(world.name, "Antica")
-        self.assertEqual(world.status, "Offline")
-        self.assertEqual(world.record_count, 1052)
-        self.assertIsInstance(world.record_date, datetime.datetime)
-        self.assertEqual(world.creation_date, "1997-01")
-        self.assertEqual(world.creation_year, 1997)
-        self.assertEqual(world.creation_month, 1)
-        self.assertEqual(world.location, WorldLocation.EUROPE)
-        self.assertEqual(world.pvp_type, PvpType.OPEN_PVP)
-        self.assertEqual(world.transfer_type, TransferType.REGULAR)
-        self.assertEqual(len(world.world_quest_titles), 5)
-        self.assertFalse(world.premium_only)
-        self.assertTrue(world.battleye_protected)
-        self.assertEqual(world.battleye_date, datetime.date(2017, 8, 29))
-        self.assertFalse(world.experimental)
-        self.assertEqual(len(world.online_players), world.online_count)
-        self.assertEqual(World.get_url(world.name), world.url)
-
-    def test_world_from_content_not_found(self):
-        """Testing parsing a world that doesn't exist"""
-        content = self.load_resource(FILE_WORLD_NOT_FOUND)
-        world = World.from_content(content)
-
-        self.assertIsNone(world)
-
-    def test_world_from_content_unrelated_section(self):
-        """Testing parsing a world using an unrelated section"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(InvalidContent):
-            World.from_content(content)
-
-    def test_world_from_content_tournament(self):
-        """Testing parsing a tournament world"""
-        content = self.load_resource(FILE_WORLD_TOURNAMENT)
-        world = World.from_content(content)
-
-        self.assertIsInstance(world, World)
-        self.assertIsInstance(world.tournament_world_type, TournamentWorldType)
-        self.assertEqual(world.tournament_world_type, TournamentWorldType.REGULAR)
-        self.assertEqual(world.record_count, 21)
-        self.assertTrue(world.premium_only)
-        self.assertFalse(world.world_quest_titles)
-
-    # endregion
-
-    # region Tibia.com WorldOverview Tests
-    def _test_world_overview_from_content(self):
-        """Testing parsing world overview"""
-        content = self.load_resource(FILE_WORLD_LIST)
-        world_overview = WorldOverview.from_content(content)
-
-        self.assertIsInstance(world_overview, WorldOverview)
-        self.assertEqual(WorldOverview.get_url(), WorldEntry.get_list_url())
-        self.assertGreater(len(world_overview.worlds), 0)
-        self.assertGreater(world_overview.total_online, 0)
-        self.assertIsNotNone(world_overview.record_date)
-        self.assertIsNotNone(world_overview.record_count)
-        self.assertEqual(82, len(world_overview.regular_worlds))
-        self.assertEqual(6, len(world_overview.tournament_worlds))
-
-        worlds = WorldEntry.list_from_content(content)
-        self.assertEqual(len(world_overview.worlds), len(worlds))
-
-    # TODO: Enable when we have a sample again
-    def _test_world_overview_from_content_offline(self):
-        """Testing parsing world overview with offline worlds"""
-        content = self.load_resource(FILE_WORLD_LIST_OFFLINE)
-        world_overview = WorldOverview.from_content(content)
-
-        self.assertEqual(world_overview.record_count, 64028)
-        self.assertIsInstance(world_overview.record_date, datetime.datetime)
-        self.assertGreater(len(world_overview.worlds), 0)
-        self.assertIsInstance(world_overview.worlds[0], WorldEntry)
-        self.assertIsInstance(world_overview.worlds[0].pvp_type, PvpType)
-        self.assertIsInstance(world_overview.worlds[0].transfer_type, TransferType)
-        self.assertIsInstance(world_overview.worlds[0].location, WorldLocation)
-        self.assertIsInstance(world_overview.worlds[0].online_count, int)
-
-    def test_world_overview_from_content_unrelated(self):
-        """Testing parsing an unrealted tibia section"""
-        content = self.load_resource(self.FILE_UNRELATED_SECTION)
-        with self.assertRaises(InvalidContent):
-            WorldEntry.list_from_content(content)
-    # endregion
+import datetime
+import json
+import unittest
+
+from tests.tests_tibiapy import TestCommons
+from tibiapy import InvalidContent
+from tibiapy.enums import PvpType, TransferType, WorldLocation
+from tibiapy.models.world import WorldOverview, WorldEntry, World
+from tibiapy.parsers.world import WorldOverviewParser, WorldParser
+from tibiapy.urls import get_world_url
+
+FILE_WORLD_FULL = "world/tibiacom_online.txt"
+FILE_WORLD_FULL_OFFLINE = "world/tibiacom_offline.txt"
+FILE_WORLD_TOURNAMENT = "world/tibiacom_tournament.txt"
+FILE_WORLD_NOT_FOUND = "world/tibiacom_not_found.txt"
+FILE_WORLD_LIST = "world/tibiacom_list_online.txt"
+FILE_WORLD_LIST_OFFLINE = "world/tibiacom_list_offline.txt"
+
+
+class TestWorld(TestCommons, unittest.TestCase):
+
+    # region Tibia.com Tests
+    def test_world_from_content_full(self):
+        """Testing parsing a world with full information"""
+        content = self.load_resource(FILE_WORLD_FULL)
+        world = WorldParser.from_content(content)
+
+        self.assertIsInstance(world, World)
+        self.assertEqual(world.name, "Premia")
+        self.assertTrue(world.online)
+        self.assertEqual(world.record_count, 531)
+        self.assertIsInstance(world.record_date, datetime.datetime)
+        self.assertEqual(world.creation_date, "2002-04")
+        self.assertEqual(world.creation_year, 2002)
+        self.assertEqual(world.creation_month, 4)
+        self.assertEqual(world.location, WorldLocation.EUROPE)
+        self.assertEqual(world.pvp_type, PvpType.OPEN_PVP)
+        self.assertEqual(world.transfer_type, TransferType.REGULAR)
+        self.assertEqual(len(world.world_quest_titles), 4)
+        self.assertTrue(world.premium_only)
+        self.assertTrue(world.battleye_protected)
+        self.assertEqual(world.battleye_date, datetime.date(2017, 9, 5))
+        self.assertFalse(world.experimental)
+        self.assertEqual(len(world.online_players), world.online_count)
+        self.assertEqual(get_world_url(world.name), world.url)
+
+        world_json_raw = world.json()
+        world_json = json.loads(world_json_raw)
+        self.assertEqual(len(world.online_players), len(world_json["online_players"]))
+
+    def test_world_from_content_offline(self):
+        """Testing parsing an offline world"""
+        content = self.load_resource(FILE_WORLD_FULL_OFFLINE)
+        world = WorldParser.from_content(content)
+
+        self.assertIsInstance(world, World)
+        self.assertEqual(world.name, "Antica")
+        self.assertFalse(world.online)
+        self.assertEqual(world.record_count, 1052)
+        self.assertIsInstance(world.record_date, datetime.datetime)
+        self.assertEqual(world.creation_date, "1997-01")
+        self.assertEqual(world.creation_year, 1997)
+        self.assertEqual(world.creation_month, 1)
+        self.assertEqual(world.location, WorldLocation.EUROPE)
+        self.assertEqual(world.pvp_type, PvpType.OPEN_PVP)
+        self.assertEqual(world.transfer_type, TransferType.REGULAR)
+        self.assertEqual(len(world.world_quest_titles), 5)
+        self.assertFalse(world.premium_only)
+        self.assertTrue(world.battleye_protected)
+        self.assertEqual(world.battleye_date, datetime.date(2017, 8, 29))
+        self.assertFalse(world.experimental)
+        self.assertEqual(len(world.online_players), world.online_count)
+        self.assertEqual(get_world_url(world.name), world.url)
+
+    def test_world_from_content_not_found(self):
+        """Testing parsing a world that doesn't exist"""
+        content = self.load_resource(FILE_WORLD_NOT_FOUND)
+        world = WorldParser.from_content(content)
+
+        self.assertIsNone(world)
+
+    def test_world_from_content_unrelated_section(self):
+        """Testing parsing a world using an unrelated section"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(InvalidContent):
+            WorldParser.from_content(content)
+
+
+    # endregion
+
+    # region Tibia.com WorldOverview Tests
+    def test_world_overview_from_content(self):
+        """Testing parsing world overview"""
+        content = self.load_resource(FILE_WORLD_LIST)
+        world_overview = WorldOverviewParser.from_content(content)
+
+        self.assertIsInstance(world_overview, WorldOverview)
+        self.assertGreater(len(world_overview.worlds), 0)
+        self.assertGreater(world_overview.total_online, 0)
+        self.assertIsNotNone(world_overview.record_date)
+        self.assertIsNotNone(world_overview.record_count)
+
+    def test_world_overview_from_content_offline(self):
+        """Testing parsing world overview with offline worlds"""
+        content = self.load_resource(FILE_WORLD_LIST_OFFLINE)
+        world_overview = WorldOverviewParser.from_content(content)
+
+        self.assertEqual(world_overview.record_count, 64028)
+        self.assertIsInstance(world_overview.record_date, datetime.datetime)
+        self.assertGreater(len(world_overview.worlds), 0)
+        self.assertIsInstance(world_overview.worlds[0], WorldEntry)
+        self.assertIsInstance(world_overview.worlds[0].pvp_type, PvpType)
+        self.assertIsInstance(world_overview.worlds[0].transfer_type, TransferType)
+        self.assertIsInstance(world_overview.worlds[0].location, WorldLocation)
+        self.assertIsInstance(world_overview.worlds[0].online_count, int)
+
+    def test_world_overview_from_content_unrelated(self):
+        """Testing parsing an unrealted tibia section"""
+        content = self.load_resource(self.FILE_UNRELATED_SECTION)
+        with self.assertRaises(InvalidContent):
+            WorldOverviewParser.from_content(content)
+    # endregion
```

### Comparing `tibia.py-5.6.1/tibia.py.egg-info/PKG-INFO` & `tibia.py-6.0.0a1/tibia.py.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,111 @@
-Metadata-Version: 2.1
-Name: tibia.py
-Version: 5.6.1
-Summary: API that parses website content into python data.
-Home-page: https://github.com/Galarzaa90/tibia.py
-Author: Galarzaa90
-Author-email: allan.galarza@gmail.com
-License: Apache 2.0
-Project-URL: GitHub: Repo, https://github.com/Galarzaa90/tibia.py
-Project-URL: GitHub: Issues, https://github.com/Galarzaa90/tibia.py/issues
-Project-URL: Docs: RTD, https://tibiapy.readthedocs.io/en/stable/
-Project-URL: Docs: Changelog, https://tibiapy.readthedocs.io/en/stable/changelog.html
-Project-URL: Coverage: Codecov, https://app.codecov.io/gh/Galarzaa90/tibia.py
-Project-URL: Docker Hub: Repo, https://hub.docker.com/repository/docker/galarzaa90/tibia.py
-Project-URL: SonarCloud, https://sonarcloud.io/dashboard?id=Galarzaa90_tibia.py
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Games/Entertainment :: Role-Playing
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Text Processing :: Markup :: HTML
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: test
-License-File: LICENSE
-
-# Tibia.py
-An API to parse Tibia.com content into object oriented data.
-
-No fetching is done by this module, you must provide the html content.
-
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Galarzaa90/tibia.py/build.yml)
-[![codecov](https://codecov.io/gh/Galarzaa90/tibia.py/branch/master/graph/badge.svg?token=mS9Wxv6O2F)](https://codecov.io/gh/Galarzaa90/tibia.py)
-[![PyPI](https://img.shields.io/pypi/v/tibia.py.svg)](https://pypi.python.org/pypi/tibia.py/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tibia.py.svg)
-![PyPI - License](https://img.shields.io/pypi/l/tibia.py.svg)
-
-
-**Features:**
-
-- Converts data into well-structured Python objects.
-- Type consistent attributes.
-- All objects can be converted to JSON strings.
-- Can be used with any networking library.
-- Support for characters, guilds, houses and worlds, tournaments, forums, etc.
-
-## Installing
-Install and update using pip
-
-```commandline
-pip install tibia.py
-```
-
-Installing the latest version form GitHub
-
-```commandline
-pip install git+https://github.com/Galarzaa90/tibia.py.git -U
-```
-
-## Usage
-This library is composed of two parts, parsers and an asynchronous request client.
-
-The asynchronous client (`tibiapy.Client`) contains methods to obtain information from Tibia.com.
-
-The parsing methods allow you to get Python objects given the html content of a page.
-
-```python
-import tibiapy
-
-# Asynchronously
-import aiohttp
-
-async def get_character(name):
-    url = tibiapy.Character.get_url(name)
-
-    async with aiohttp.ClientSession() as session:
-        async with session.get(url) as resp:
-            content = await resp.text()
-    character = tibiapy.Character.from_content(content)
-    return character
-
-# Synchronously
-import requests
-
-def get_character_sync(name):
-    url = tibiapy.Character.get_url(name)
-    
-    r = requests.get(url)
-    content = r.text
-    character = tibiapy.Character.from_content(content)
-    return character
-
-```
-
-## Documentation
-https://tibiapy.readthedocs.io/
+Metadata-Version: 2.1
+Name: tibia.py
+Version: 6.0.0a1
+Summary: API that parses website content into python data.
+Home-page: https://github.com/Galarzaa90/tibia.py
+Author: Galarzaa90
+Author-email: allan.galarza@gmail.com
+License: Apache 2.0
+Project-URL: GitHub: Repo, https://github.com/Galarzaa90/tibia.py
+Project-URL: GitHub: Issues, https://github.com/Galarzaa90/tibia.py/issues
+Project-URL: Docs: RTD, https://tibiapy.readthedocs.io/en/stable/
+Project-URL: Docs: Changelog, https://tibiapy.readthedocs.io/en/stable/changelog.html
+Project-URL: Coverage: Codecov, https://app.codecov.io/gh/Galarzaa90/tibia.py
+Project-URL: Docker Hub: Repo, https://hub.docker.com/repository/docker/galarzaa90/tibia.py
+Project-URL: SonarCloud, https://sonarcloud.io/dashboard?id=Galarzaa90_tibia.py
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Games/Entertainment :: Role-Playing
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Text Processing :: Markup :: HTML
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: server
+License-File: LICENSE
+
+# Tibia.py
+An API to parse Tibia.com content into object oriented data.
+
+No fetching is done by this module, you must provide the html content.
+
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Galarzaa90/tibia.py/build.yml)
+[![codecov](https://codecov.io/gh/Galarzaa90/tibia.py/branch/master/graph/badge.svg?token=mS9Wxv6O2F)](https://codecov.io/gh/Galarzaa90/tibia.py)
+[![PyPI](https://img.shields.io/pypi/v/tibia.py.svg)](https://pypi.python.org/pypi/tibia.py/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tibia.py.svg)
+![PyPI - License](https://img.shields.io/pypi/l/tibia.py.svg)
+
+
+**Features:**
+
+- Converts data into well-structured Python objects.
+- Type consistent attributes.
+- All objects can be converted to JSON strings.
+- Can be used with any networking library.
+- Support for characters, guilds, houses and worlds, tournaments, forums, etc.
+
+## Installing
+Install and update using pip
+
+```commandline
+pip install tibia.py
+```
+
+Installing the latest version form GitHub
+
+```commandline
+pip install git+https://github.com/Galarzaa90/tibia.py.git -U
+```
+
+## Usage
+This library is composed of two parts, parsers and an asynchronous request client.
+
+The asynchronous client (`tibiapy.Client`) contains methods to obtain information from Tibia.com.
+
+The parsing methods allow you to get Python objects given the html content of a page.
+
+```python
+import tibiapy
+
+# Asynchronously
+import aiohttp
+
+async def get_character(name):
+    url = tibiapy.urls.get_character_url(name)
+
+    async with aiohttp.ClientSession() as session:
+        async with session.get(url) as resp:
+            content = await resp.text()
+    character = tibiapy.Character.from_content(content)
+    return character
+
+# Synchronously
+import requests
+
+def get_character_sync(name):
+    url = tibiapy.urls.get_character_url(name)
+    
+    r = requests.get(url)
+    content = r.text
+    character = tibiapy.Character.from_content(content)
+    return character
+
+```
+
+## Documentation
+https://tibiapy.readthedocs.io/
+
+
```

### Comparing `tibia.py-5.6.1/tibiapy/errors.py` & `tibia.py-6.0.0a1/tibiapy/errors.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-"""Exceptions thrown by tibia.py."""
-
-
-class TibiapyException(Exception):
-    """Base exception for the tibiapy module.
-
-    All exceptions thrown by the module are inherited from this.
-    """
-
-    pass
-
-
-class InvalidContent(TibiapyException):
-    """Exception thrown when the provided content is unrelated for the calling function.
-
-    This usually means that the content provided belongs to a different website or section of the website.
-    This serves as a way to differentiate those cases from a parsing that returned no results (e.g. Character not found)
-
-    In some cases this can mean that Tibia.com's format has changed and the library needs updating.
-
-    Attributes
-    ----------
-    original: :class:`Exception`
-        The original exception that caused this exception.
-    """
-
-    def __init__(self, message, original=None):
-        super().__init__(message)
-        self.original = original
-
-
-class NetworkError(TibiapyException):
-    """Exception thrown when there was a network error trying to fetch a resource from the web.
-
-    Attributes
-    ----------
-    original: :class:`Exception`
-        The original exception that caused this exception.
-    fetching_time: :class:`float`
-        The time between the request and the response.
-    """
-
-    def __init__(self, message, original=None, fetching_time=0):
-        super().__init__(message)
-        self.original = original
-        self.fetching_time = fetching_time
-
-
-class Forbidden(NetworkError):
-    """A subclass of :class:`NetworkError` thrown when Tibia.com returns a 403 status code.
-
-    Tibia.com returns a 403 status code when it detects that too many requests are being done.
-    This has its own subclass to let the user decide to treat this differently than other network errors.
-    """
-
-
-class SiteMaintenanceError(NetworkError):
-    """A subclass of :class:`NetworkError` thrown when Tibia.com is down for maintenance.
-
-    When Tibia.com is under maintenance, all sections of the website redirect to maintenance.tibia.com.
-    """
+"""Exceptions thrown by tibia.py."""
+
+
+class TibiapyException(Exception):
+    """Base exception for the tibiapy module.
+
+    All exceptions thrown by the module are inherited from this.
+    """
+
+    pass
+
+
+class InvalidContent(TibiapyException):
+    """Exception thrown when the provided content is unrelated for the calling function.
+
+    This usually means that the content provided belongs to a different website or section of the website.
+    This serves as a way to differentiate those cases from a parsing that returned no results (e.g. Character not found)
+
+    In some cases this can mean that Tibia.com's format has changed and the library needs updating.
+
+    Attributes
+    ----------
+    original: :class:`Exception`
+        The original exception that caused this exception.
+    """
+
+    def __init__(self, message, original=None):
+        super().__init__(message)
+        self.original = original
+
+
+class NetworkError(TibiapyException):
+    """Exception thrown when there was a network error trying to fetch a resource from the web.
+
+    Attributes
+    ----------
+    original: :class:`Exception`
+        The original exception that caused this exception.
+    fetching_time: :class:`float`
+        The time between the request and the response.
+    """
+
+    def __init__(self, message, original=None, fetching_time=0):
+        super().__init__(message)
+        self.original = original
+        self.fetching_time = fetching_time
+
+
+class Forbidden(NetworkError):
+    """A subclass of :class:`NetworkError` thrown when Tibia.com returns a 403 status code.
+
+    Tibia.com returns a 403 status code when it detects that too many requests are being done.
+    This has its own subclass to let the user decide to treat this differently than other network errors.
+    """
+
+
+class SiteMaintenanceError(NetworkError):
+    """A subclass of :class:`NetworkError` thrown when Tibia.com is down for maintenance.
+
+    When Tibia.com is under maintenance, all sections of the website redirect to maintenance.tibia.com.
+    """
```

### Comparing `tibia.py-5.6.1/tibiapy/utils.py` & `tibia.py-6.0.0a1/tibiapy/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,665 +1,749 @@
-"""These are functions used thorough the module that may not be intended for public use."""
-import datetime
-import functools
-import itertools
-import re
-import urllib.parse
-import warnings
-from collections import OrderedDict
-from typing import Dict, Optional, Tuple, Type, TypeVar, Union
-
-import bs4
-
-TIBIA_CASH_PATTERN = re.compile(r'(\d*\.?\d*)\s?k*$')
-
-
-def convert_line_breaks(element):
-    """Convert the <br> tags in a HTML elements to actual line breaks.
-
-    Parameters
-    ----------
-    element: :class:`bs4.Tag`
-        A BeautifulSoup object.
-    """
-    for br in element.find_all("br"):
-        br.replace_with("\n")
-
-
-def get_tibia_url(section, subtopic=None, *args, anchor=None, test=False, **kwargs):
-    """Build a URL to Tibia.com with the given parameters.
-
-    Parameters
-    ----------
-    section: :class:`str`
-        The desired section (e.g. community, abouttibia, manual, library)
-    subtopic: :class:`str`, optional
-        The desired subtopic (e.g. characters, guilds, houses, etc)
-    anchor: :class:`str`
-        A link anchor to add to the link.
-    args:
-        A list of key-value pairs to add as query parameters.
-        This allows passing multiple parameters with the same name.
-    kwargs:
-        Additional parameters to pass to the url as query parameters (e.g name, world, houseid, etc)
-    test: :class:`bool`
-        Whether to use the test website or not.
-
-    Returns
-    -------
-    :class:`str`
-        The generated Tibia.com URL.
-
-    Examples
-    --------
-    >>> get_tibia_url("community", "houses", page="view", houseid=55302, world="Gladera")
-    https://www.tibia.com/community/?subtopic=houses&page=view&houseid=55302&world=Gladera
-
-    You can also build a dictionary and pass it like:
-
-    >>> params = {'world': "Gladera"}
-    >>> get_tibia_url("community", "worlds", **params)
-    https://www.tibia.com/community/?subtopic=worlds&world=Gladera
-    """
-    base_url = "www.tibia.com" if not test else "www.test.tibia.com"
-    url = f"https://{base_url}/{section}/?"
-    params = OrderedDict(subtopic=subtopic) if subtopic else OrderedDict()
-    if kwargs:
-        for key, value in kwargs.items():
-            if isinstance(value, str):
-                value = value.encode('iso-8859-1')
-            if value is None:
-                continue
-            params[key] = value
-    url += urllib.parse.urlencode(params)
-    if args:
-        url += "&"
-        url += urllib.parse.urlencode(args)
-    if anchor:
-        url += f"#{anchor}"
-    return url
-
-
-def parse_form_data(form: bs4.Tag, include_options=True):
-    """Parse the currently selected values in a form.
-
-    This should correspond to all the data the form would send if submitted.
-
-    Parameters
-    ----------
-    form: :class:`bs4.Tag`
-        A form tag.
-    include_options: :class:`bool`
-        Whether to also include listings of all the possible options.
-        These will be nested inside the __options__ parameter of the resulting dictionary.
-
-    Returns
-    -------
-    :class:`dict`
-        A dictionary containing all the data.
-    """
-    data = {}
-    if "action" in form.attrs:
-        data["__action__"] = form.attrs["action"]
-    if "method" in form.attrs:
-        data["__method__"] = form.attrs["method"]
-    text_inputs = form.find_all("input", {"type": "text"})
-    data.update({field.attrs.get("name"): field.attrs.get("value") for field in text_inputs})
-    selects = form.find_all("select")
-    if include_options:
-        data["__options__"] = {}
-    for select in selects:
-        name = select.attrs.get("name")
-        selected_option = select.find("option", {"selected": True})
-        if include_options:
-            options = select.find_all("option")
-            data["__options__"][name] = {opt.text: opt.attrs.get("value") for opt in options}
-        data[name] = selected_option.attrs.get("value") if selected_option else None
-    checkboxes = form.find_all("input", {"type": "checkbox", "checked": True})
-    data.update({field.attrs.get("name"): field.attrs.get("value") for field in checkboxes})
-    # Parse Radios
-    all_radios = form.find_all("input", {"type": "radio"})
-    for name, _radios in itertools.groupby(all_radios, key=lambda t: t.attrs["name"]):
-        radios = list(_radios)
-        selected_radio = next((r for r in radios if r.attrs.get("checked") is not None), None)
-        if include_options:
-            data["__options__"][name] = {str(r.next_sibling).strip(): r.attrs["value"] for r in radios}
-        data[name] = selected_radio.attrs["value"] if selected_radio else None
-    return data
-
-
-def parse_integer(number: str, default: Optional[int] = 0):
-    """Parse a string representing an integer, ignoring commas or periods.
-
-    Parameters
-    ----------
-    number: :class:`str`
-        A string representing a number.
-    default: :class:`int`
-        The default value to use if the string is not numeric.
-        By default, 0 is used.
-
-    Returns
-    -------
-    :class:`int`
-        The represented integer, or the default value if invalid.
-    """
-    if number is None:
-        return default
-    try:
-        number = re.sub(r'[,.]', '', number.strip())
-        return int(number)
-    except ValueError:
-        return default
-
-
-def parse_link_info(link_tag):
-    """Parse the information of a link tag.
-
-    It will parse the link's content, target URL as well as the query parameters where applicable.
-
-    Parameters
-    ----------
-    link_tag: :class:`bs4.Tag`
-        The link tag object.
-
-    Returns
-    -------
-    :class:`dict`:
-        A dictionary containing the link's data.
-
-    Examples
-    --------
-    >>> # <a href="https://www.tibia.com/community/?subtopic=houses&page=view&houseid=55302&world=Gladera">House</>
-    >>> parse_link_info(link_tag)
-    {
-        "text": "House",
-        "url": "https://www.tibia.com/community/?subtopic=houses&page=view&houseid=55302&world=Gladera"
-        "query": {
-            "subtopic": "houses",
-            "page": "view",
-            "houseid": "55302",
-            "world": "Gladera"
-        }
-    }
-
-    When parsing links that have multiple query parameters, they are displayed as a list.
-    Empty parameters are omitted.
-
-    >>> # <a href="https://example.com/?world=&beprotection=-1&worldtypes[]=0&worldtypes[]=3">Link</a>
-    >>> parse_link_info(link_tag)
-    {
-        "text": "Link",
-        "url": "https://example.com/?world=&beprotection=-1&worldtypes[]=0&worldtypes[]=3"
-        "query": {
-            "beprotection": "-1",
-            "worldtypes": ["0", "3"]
-        }
-    }
-    """
-    url = link_tag["href"]
-    info = {"text": link_tag.text.strip(), "url": url, "query": {}}
-    parsed_url = urllib.parse.urlparse(url)
-    if parsed_url.query:
-        query_params = urllib.parse.parse_qs(parsed_url.query)
-        for param, value in query_params.items():
-            if len(value) == 1:
-                info["query"][param] = value[0]
-            else:
-                info["query"][param] = value
-    return info
-
-
-def parse_tibia_datetime(datetime_str) -> Optional[datetime.datetime]:
-    """Parse date and time from the format used in Tibia.com.
-
-    Accepted format:
-
-    - ``MMM DD YYYY, HH:mm:ss ZZZ``, e.g. ``Dec 10 2018, 21:53:37 CET``.
-    - ``MMM DD YYYY, HH:mm ZZZ``, e.g. ``Dec 10 2018, 21:53 CET``.
-
-    Parameters
-    -------------
-    datetime_str: :class:`str`
-        The date and time as represented in Tibia.com
-
-    Returns
-    -----------
-    :class:`datetime.datetime`, optional
-        The represented datetime, in UTC (timezone aware).
-    """
-    try:
-        datetime_str = datetime_str.replace(",", "").replace("&#160;", " ").strip()
-        # Extracting timezone
-        tz = datetime_str[-4:].strip()
-
-        # Convert time string to time object
-        # Removing timezone cause CEST and CET are not supported
-        try:
-            t = datetime.datetime.strptime(datetime_str[:-4].strip(), "%b %d %Y %H:%M:%S")
-        except ValueError:
-            t = datetime.datetime.strptime(datetime_str[:-4].strip(), "%b %d %Y %H:%M")
-
-        # Getting the offset
-        if tz == "CET":
-            utc_offset = 1
-        elif tz == "CEST":
-            utc_offset = 2
-        else:
-            return None
-        # Add/subtract hours to get the real time
-        t = t - datetime.timedelta(hours=utc_offset)
-        return t.replace(tzinfo=datetime.timezone.utc)
-    except (ValueError, AttributeError):
-        return None
-
-
-def parse_tibia_date(date_str) -> Optional[datetime.date]:
-    """Parse a date from the format used in Tibia.com.
-
-    Accepted format:
-
-    - ``MMM DD YYYY``, e.g. ``Jul 23 2015``
-
-    Parameters
-    -----------
-    date_str: :class:`str`
-        The date as represented in Tibia.com
-
-    Returns
-    -----------
-    :class:`datetime.date`, optional
-        The represented date, in UTC (timezone aware).
-    """
-    try:
-        t = datetime.datetime.strptime(date_str.strip(), "%b %d %Y")
-        return t.date()
-    except (ValueError, AttributeError):
-        return None
-
-
-def parse_tibia_forum_datetime(datetime_str, utc_offset=1):
-    """Parse a date in the format used in the Tibia.com forums.
-
-    Accepted format:
-
-    - ``DD.MM.YY HH:mm:ss``, e.g. ``23.07.2015 21:30:30``
-
-    Parameters
-    ----------
-    datetime_str: :class:`str`
-        The string containing the date and time.
-    utc_offset: :class:`int`
-        The UTC offset to apply to the parsed datetime.
-
-        Since the timestamps contain no timezone information, it can be passed as an additional parameter.
-
-        By default CET (+1) is considered.
-
-    Returns
-    -------
-    :class:`datetime`
-        The represented datetime, in UTC (timezone aware).
-    """
-    t = datetime.datetime.strptime(datetime_str.strip(), "%d.%m.%Y %H:%M:%S")
-    # Add/subtract hours to get the real time
-    t = t - datetime.timedelta(hours=utc_offset)
-    return t.replace(tzinfo=datetime.timezone.utc)
-
-
-def parse_tibia_full_date(date_str) -> Optional[datetime.date]:
-    """Parse a date in the fuller format used in Tibia.com.
-
-    Accepted format:
-
-    - ``MMMM DD, YYYY``, e.g. ``July 23, 2015``
-
-    Parameters
-    -----------
-    date_str: :class:`str`
-        The date as represented in Tibia.com
-
-    Returns
-    -----------
-    :class:`datetime.date`, optional
-        The represented date, in UTC (timezone aware).
-    """
-    try:
-        t = datetime.datetime.strptime(date_str.strip(), "%B %d, %Y")
-        return t.date()
-    except (ValueError, AttributeError):
-        return None
-
-
-def parse_number_words(text_num):
-    """Parse the word representation of a number to a integer.
-
-    Parameters
-    ----------
-    text_num: :class:`str`
-        The text representation of a number.
-
-    Returns
-    -------
-    :class:`int`
-        The number represented by the string.
-    """
-    numwords = {}
-    units = [
-        "zero", "one", "two", "three", "four", "five", "six", "seven", "eight",
-        "nine", "ten", "eleven", "twelve", "thirteen", "fourteen", "fifteen",
-        "sixteen", "seventeen", "eighteen", "nineteen",
-    ]
-
-    tens = ["", "", "twenty", "thirty", "forty", "fifty", "sixty", "seventy", "eighty", "ninety"]
-
-    scales = ["hundred", "thousand", "million", "billion", "trillion"]
-
-    numwords["and"] = (1, 0)
-    for idx, word in enumerate(units):
-        numwords[word] = (1, idx)
-    for idx, word in enumerate(tens):
-        numwords[word] = (1, idx * 10)
-    for idx, word in enumerate(scales):
-        numwords[word] = (10 ** (idx * 3 or 2), 0)
-
-    current = result = 0
-    text_num = text_num.replace("-", " ")
-    for word in text_num.split():
-        if word not in numwords:
-            return 0
-
-        scale, increment = numwords[word]
-        current = current * scale + increment
-        if scale > 100:
-            result += current
-            current = 0
-
-    return result + current
-
-
-def try_datetime(obj) -> Optional[datetime.datetime]:
-    """Attempt to convert an object into a datetime.
-
-    If the date format is known, it's recommended to use the corresponding function
-    This is meant to be used in constructors.
-
-    Parameters
-    ----------
-    obj: :class:`str`, :class:`dict`, :class:`datetime.datetime`
-        The object to convert.
-
-    Returns
-    -------
-    :class:`datetime.datetime`, optional
-        The represented datetime, in UTC (timezone aware), or :obj:`None` if conversion wasn't possible.
-    """
-    if obj is None:
-        return None
-    if isinstance(obj, datetime.datetime):
-        return obj
-    return parse_tibia_datetime(obj)
-
-
-def try_date(obj) -> Optional[datetime.date]:
-    """Attempt to convert an object into a date.
-
-    If the date format is known, it's recommended to use the corresponding function
-    This is meant to be used in constructors.
-
-    Parameters
-    ----------
-    obj: :class:`str`, :class:`datetime.datetime`, :class:`datetime.date`
-        The object to convert.
-
-    Returns
-    -------
-    :class:`datetime.date`, optional
-        The represented date, in UTC (timezone aware).
-    """
-    if obj is None:
-        return None
-    if isinstance(obj, datetime.datetime):
-        return obj.date()
-    if isinstance(obj, datetime.date):
-        return obj
-    res = parse_tibia_date(obj)
-    if res is not None:
-        return res
-    return parse_tibia_full_date(obj)
-
-
-def parse_tibiacom_content(content, *, html_class="BoxContent", tag="div", builder="lxml"):
-    """Parse HTML content from Tibia.com into a BeautifulSoup object.
-
-    Parameters
-    ----------
-    content: :class:`str`
-        The raw HTML content from Tibia.com
-    html_class: :class:`str`
-        The HTML class of the parsed element. The default value is ``BoxContent``.
-    tag: :class:`str`
-        The HTML tag select. The default value is ``div``.
-    builder: :class:`str`
-        The builder to use. The default value is ``lxml``.
-
-    Returns
-    -------
-    :class:`bs4.BeautifulSoup`, optional
-        The parsed content.
-    """
-    strainer = bs4.SoupStrainer(tag, class_=html_class) if builder != "html5lib" else None
-    return bs4.BeautifulSoup(content.replace('ISO-8859-1', 'utf-8', 1), builder, parse_only=strainer)
-
-
-def parse_tibiacom_tables(parsed_content) -> Dict[str, bs4.Tag]:
-    """Parse tables from Tibia.com into a mapping by the tables title.
-
-    This is used for the table style used in Tibia.com, where a table is wrapped in a container with a title.
-
-    Parameters
-    ----------
-    parsed_content: :class:`bs4.BeautifulSoup`
-        The content to find the tables in.
-
-    Returns
-    -------
-    :class:`dict`
-        A dictionary mapping the container titles and the contained table.
-    """
-    table_containers = parsed_content.find_all("div", attrs={"class": "TableContainer"})
-    tables = {}
-    for table_container in table_containers:
-        text_tag = table_container.find("div", attrs={"class": "Text"})
-        table = table_container.find("table", attrs={"class": "TableContent"})
-        if not table:
-            continue
-        tables[text_tag.text.strip()] = table
-    return tables
-
-
-T = TypeVar('T')
-D = TypeVar('D')
-
-
-def try_enum(cls: Type[T], val, default: D = None) -> Union[T, D]:
-    """Attempt to convert a value into their enum value.
-
-    Parameters
-    ----------
-    cls: :class:`Enum`
-        The enum to convert to.
-    val:
-        The value to try to convert to Enum
-    default: optional
-        The value to return if no enum value is found.
-
-    Returns
-    -------
-    obj:
-        The enum value if found, otherwise None.
-    """
-    if isinstance(val, cls):
-        return val
-    try:
-        return cls(val)
-    except ValueError:
-        try:
-            if isinstance(val, str):
-                val = val.upper()
-            return cls._member_map_[val]
-        except KeyError:
-            return default
-
-
-def parse_tibia_money(argument):
-    """Parse a string that may contain 'k' as thousand suffix.
-
-    Parameters
-    ----------
-    argument: :class:`str`
-        A numeric string using k as a prefix for thousands.
-
-    Returns
-    -------
-    :class:`int`:
-        The value represented by the string.
-    """
-    try:
-        return int(argument)
-    except ValueError:
-        argument = argument.replace(",", "").strip().lower()
-        m = TIBIA_CASH_PATTERN.match(argument)
-        if not m or not m.group(1):
-            raise ValueError("not a numeric value")
-        num = float(m.group(1))
-        k_count = argument.count("k")
-        num *= pow(1000, k_count)
-        return int(num)
-
-
-def split_list(items, separator=",", last_separator=" and "):
-    """Split a string listing elements into an actual list.
-
-    Parameters
-    ----------
-    items: :class:`str`
-        A string listing elements.
-    separator: :class:`str`
-        The separator between each item. A comma by default.
-    last_separator: :class:`str`
-        The separator used for the last item. ' and ' by default.
-
-    Returns
-    -------
-    :class:`list` of :class:`str`
-        A list containing each one of the items.
-    """
-    if items is None:
-        return None
-    items = items.split(separator)
-    last_item = items[-1]
-    last_split = last_item.split(last_separator)
-    if len(last_split) > 1:
-        items[-1] = last_separator.join(last_split[:-1])
-        items.append(last_split[-1])
-    return [e.strip() for e in items]
-
-
-def _recursive_strip(value):  # pragma: no cover
-    if isinstance(value, dict):
-        return {k: _recursive_strip(v) for k, v in value.items()}
-    if isinstance(value, list):
-        return [_recursive_strip(i) for i in value]
-    if isinstance(value, str):
-        return value.strip()
-    return value
-
-
-def deprecated(instead=None):  # pragma: no cover
-    def actual_decorator(func):
-        @functools.wraps(func)
-        def decorated(*args, **kwargs):
-            warnings.simplefilter('always', DeprecationWarning)
-            if instead:
-                fmt = "{0.__name__} is deprecated, use {1} instead."
-            else:
-                fmt = '{0.__name__} is deprecated.'
-
-            warnings.warn(fmt.format(func, instead), stacklevel=3, category=DeprecationWarning)
-            warnings.simplefilter('default', DeprecationWarning)
-            return func(*args, **kwargs)
-        return decorated
-    return actual_decorator
-
-
-def parse_popup(popup_content) -> Tuple[str, bs4.BeautifulSoup]:
-    """Parse the information popups used through Tibia.com.
-
-    Parameters
-    ----------
-    popup_content: :class:`str`
-        The raw content of the javascript function that creates the popup.
-
-    Returns
-    -------
-    :class:`str`
-        The popup's title.
-    :class:`bs4.BeautifulSoup`
-        The parsed HTML content of the popup.
-    """
-    parts = popup_content.split(",", 2)
-    title = parts[1].replace(r"'", "").strip()
-    html = parts[-1].replace(r"\'", '"').replace(r"'", "").replace(",);", "").replace(", );", "").strip()
-    parsed_html = bs4.BeautifulSoup(html, 'lxml')
-    return title, parsed_html
-
-
-results_pattern = re.compile(r'Results: ([\d,]+)')
-page_pattern = re.compile(r'page=(\d+)')
-
-
-def parse_pagination(pagination_block) -> Tuple[int, int, int]:
-    """Parse a pagination section in Tibia.com and extracts its information.
-
-    Parameters
-    ----------
-    pagination_block: :class:`bs4.Tag`
-        The HTML containing the pagination information.
-
-    Returns
-    -------
-    page : :class:`int`
-        The current page.
-    total_pages : :class:`int`
-        The total number of pages.
-    results_count : :class:`int`
-        The total number of results.
-    """
-    pages_div, results_div = pagination_block.find_all("div")
-    current_page_link = pages_div.find("span", {"class": "CurrentPageLink"})
-    page_links = pages_div.find_all("span", {"class": "PageLink"})
-    # pages_with_links = pages_div.select(#)
-    first_or_last_pages = pages_div.find_all("span", {"class": "FirstOrLastElement"})
-    page = -1
-    total_pages = -1
-    if first_or_last_pages:
-        last_page_link = first_or_last_pages[-1].find("a")
-        if last_page_link:
-            m = page_pattern.search(last_page_link["href"])
-            if m:
-                total_pages = int(m.group(1))
-        else:
-            last_page_link = page_links[-2].find("a")
-            total_pages = int(last_page_link.text) + 1
-    else:
-        last_page_link = page_links[-1]
-        total_pages = int(last_page_link.text)
-    try:
-        page = int(current_page_link.text)
-    except ValueError:
-        if "First" in current_page_link.text:
-            page = 1
-        else:
-            page = total_pages
-    results_count = parse_integer(results_pattern.search(results_div.text).group(1))
-    return page, total_pages, results_count
+"""These are functions used thorough the module that may not be intended for public use."""
+import datetime
+import functools
+import itertools
+import re
+import urllib.parse
+import warnings
+from collections import OrderedDict, defaultdict
+from typing import Dict, Optional, Tuple, Type, TypeVar, Union, List
+
+import bs4
+from pydantic import BaseModel
+
+from tibiapy.errors import InvalidContent
+
+TIBIA_CASH_PATTERN = re.compile(r'(\d*\.?\d*)\s?k*$')
+
+
+def clean_text(tag: Union[bs4.Tag, str]):
+    if isinstance(tag, bs4.Tag):
+        text = tag.text
+    else:
+        text = tag
+    return text.replace("\xa0", " ").strip()
+
+
+def convert_line_breaks(element):
+    """Convert the <br> tags in a HTML elements to actual line breaks.
+
+    Parameters
+    ----------
+    element: :class:`bs4.Tag`
+        A BeautifulSoup object.
+    """
+    for br in element.find_all("br"):
+        br.replace_with("\n")
+
+
+def get_rows(table_tag: bs4.Tag):
+    return table_tag.select("tr")
+
+
+def get_tibia_url(section, subtopic=None, *args, anchor=None, test=False, **kwargs):
+    """Build a URL to Tibia.com with the given parameters.
+
+    Parameters
+    ----------
+    section: :class:`str`
+        The desired section (e.g. community, abouttibia, manual, library)
+    subtopic: :class:`str`, optional
+        The desired subtopic (e.g. characters, guilds, houses, etc)
+    anchor: :class:`str`
+        A link anchor to add to the link.
+    args:
+        A list of key-value pairs to add as query parameters.
+        This allows passing multiple parameters with the same name.
+    kwargs:
+        Additional parameters to pass to the url as query parameters (e.g name, world, houseid, etc)
+    test: :class:`bool`
+        Whether to use the test website or not.
+
+    Returns
+    -------
+    :class:`str`
+        The generated Tibia.com URL.
+
+    Examples
+    --------
+    >>> get_tibia_url("community", "houses", page="view", houseid=55302, world="Gladera")
+    https://www.tibia.com/community/?subtopic=houses&page=view&houseid=55302&world=Gladera
+
+    You can also build a dictionary and pass it like:
+
+    >>> params = {'world': "Gladera"}
+    >>> get_tibia_url("community", "worlds", **params)
+    https://www.tibia.com/community/?subtopic=worlds&world=Gladera
+    """
+    base_url = "www.tibia.com" if not test else "www.test.tibia.com"
+    url = f"https://{base_url}/{section}/?"
+    params = OrderedDict(subtopic=subtopic) if subtopic else OrderedDict()
+    if kwargs:
+        for key, value in kwargs.items():
+            if isinstance(value, str):
+                value = value.encode('iso-8859-1')
+            if value is None:
+                continue
+            params[key] = value
+    url += urllib.parse.urlencode(params)
+    if args:
+        url += "&"
+        url += urllib.parse.urlencode(args)
+    if anchor:
+        url += f"#{anchor}"
+    return url
+
+
+def parse_form_data(form: bs4.Tag, include_options=True):
+    """Parse the currently selected values in a form.
+
+    This should correspond to all the data the form would send if submitted.
+
+    Parameters
+    ----------
+    form: :class:`bs4.Tag`
+        A form tag.
+    include_options: :class:`bool`
+        Whether to also include listings of all the possible options.
+        These will be nested inside the __options__ parameter of the resulting dictionary.
+
+    Returns
+    -------
+    :class:`dict`
+        A dictionary containing all the data.
+    """
+    data = {}
+    if "action" in form.attrs:
+        data["__action__"] = form.attrs["action"]
+    if "method" in form.attrs:
+        data["__method__"] = form.attrs["method"]
+    text_inputs = form.find_all("input", {"type": "text"})
+    data.update({field.attrs.get("name"): field.attrs.get("value") for field in text_inputs})
+    selects = form.find_all("select")
+    if include_options:
+        data["__options__"] = {}
+    for select in selects:
+        name = select.attrs.get("name")
+        selected_option = select.find("option", {"selected": True})
+        if include_options:
+            options = select.find_all("option")
+            data["__options__"][name] = {opt.text: opt.attrs.get("value") for opt in options}
+        data[name] = selected_option.attrs.get("value") if selected_option else None
+    checkboxes = form.find_all("input", {"type": "checkbox", "checked": True})
+    data.update({field.attrs.get("name"): field.attrs.get("value") for field in checkboxes})
+    # Parse Radios
+    all_radios = form.find_all("input", {"type": "radio"})
+    for name, _radios in itertools.groupby(all_radios, key=lambda t: t.attrs["name"]):
+        radios = list(_radios)
+        selected_radio = next((r for r in radios if r.attrs.get("checked") is not None), None)
+        if include_options:
+            data["__options__"][name] = {str(r.next_sibling).strip(): r.attrs["value"] for r in radios}
+        data[name] = selected_radio.attrs["value"] if selected_radio else None
+    return data
+
+
+class FormData(BaseModel):
+    values: Dict[str, str] = {}
+    values_multiple: Dict[str, List[str]] = defaultdict(list)
+    available_options: Dict[str, Dict[str, str]] = defaultdict(dict)
+    action: Optional[str] = None
+    method: Optional[str] = None
+
+
+def parse_form_data_new(form: bs4.Tag):
+    """Parse the currently selected values in a form.
+
+    This should correspond to all the data the form would send if submitted.
+
+    Parameters
+    ----------
+    form: :class:`bs4.Tag`
+        A form tag.
+    include_options: :class:`bool`
+        Whether to also include listings of all the possible options.
+        These will be nested inside the __options__ parameter of the resulting dictionary.
+
+    Returns
+    -------
+    :class:`FormData`
+        A dictionary containing all the data.
+    """
+    form_data = FormData()
+    if "action" in form.attrs:
+        form_data.action = form.attrs["action"]
+    if "method" in form.attrs:
+        form_data.method = form.attrs["method"]
+    for field in form.select("input[type=text], input[type=hidden]"):
+        form_data.values[field.attrs.get("name")] = field.attrs.get("value")
+    for select in form.select("select"):
+        name = select.attrs.get("name")
+        selected_option = select.select_one("option[selected]")
+        options = select.select("option")
+        form_data.available_options[name].update({clean_text(opt): opt.attrs.get("value") for opt in options})
+        form_data.values[name] = selected_option.attrs.get("value") if selected_option else None
+    for checkbox in form.select("input[type=checkbox]"):
+        name = checkbox.attrs.get("name")
+        label = checkbox.parent.text
+        value = checkbox.attrs.get("value")
+        form_data.available_options[name][label] = value
+        if checkbox.has_attr("checked"):
+            form_data.values_multiple[name].append(value)
+    for radio in form.select("input[type=radio]"):
+        name = radio.attrs.get("name")
+        value = radio.attrs.get("value")
+        label = radio.next_sibling.text.strip()
+        form_data.available_options[name][label] = value
+        if radio.has_attr("checked"):
+            form_data.values[name] = value
+    return form_data
+
+
+def parse_integer(number: str, default: Optional[int] = 0):
+    """Parse a string representing an integer, ignoring commas or periods.
+
+    Parameters
+    ----------
+    number: :class:`str`
+        A string representing a number.
+    default: :class:`int`
+        The default value to use if the string is not numeric.
+        By default, 0 is used.
+
+    Returns
+    -------
+    :class:`int`
+        The represented integer, or the default value if invalid.
+    """
+    if number is None:
+        return default
+    try:
+        number = re.sub(r'[,.]', '', number.strip())
+        return int(number)
+    except ValueError:
+        return default
+
+
+def parse_link_info(link_tag):
+    """Parse the information of a link tag.
+
+    It will parse the link's content, target URL as well as the query parameters where applicable.
+
+    Parameters
+    ----------
+    link_tag: :class:`bs4.Tag`
+        The link tag object.
+
+    Returns
+    -------
+    :class:`dict`:
+        A dictionary containing the link's data.
+
+    Examples
+    --------
+    >>> # <a href="https://www.tibia.com/community/?subtopic=houses&page=view&houseid=55302&world=Gladera">House</>
+    >>> parse_link_info(link_tag)
+    {
+        "text": "House",
+        "url": "https://www.tibia.com/community/?subtopic=houses&page=view&houseid=55302&world=Gladera"
+        "query": {
+            "subtopic": "houses",
+            "page": "view",
+            "houseid": "55302",
+            "world": "Gladera"
+        }
+    }
+
+    When parsing links that have multiple query parameters, they are displayed as a list.
+    Empty parameters are omitted.
+
+    >>> # <a href="https://example.com/?world=&beprotection=-1&worldtypes[]=0&worldtypes[]=3">Link</a>
+    >>> parse_link_info(link_tag)
+    {
+        "text": "Link",
+        "url": "https://example.com/?world=&beprotection=-1&worldtypes[]=0&worldtypes[]=3"
+        "query": {
+            "beprotection": "-1",
+            "worldtypes": ["0", "3"]
+        }
+    }
+    """
+    url = link_tag["href"]
+    info = {"text": link_tag.text.strip(), "url": url, "query": {}}
+    parsed_url = urllib.parse.urlparse(url)
+    if parsed_url.query:
+        query_params = urllib.parse.parse_qs(parsed_url.query)
+        for param, value in query_params.items():
+            if len(value) == 1:
+                info["query"][param] = value[0]
+            else:
+                info["query"][param] = value
+    return info
+
+
+def parse_tibia_datetime(datetime_str) -> Optional[datetime.datetime]:
+    """Parse date and time from the format used in Tibia.com.
+
+    Accepted format:
+
+    - ``MMM DD YYYY, HH:mm:ss ZZZ``, e.g. ``Dec 10 2018, 21:53:37 CET``.
+    - ``MMM DD YYYY, HH:mm ZZZ``, e.g. ``Dec 10 2018, 21:53 CET``.
+
+    Parameters
+    -------------
+    datetime_str: :class:`str`
+        The date and time as represented in Tibia.com
+
+    Returns
+    -----------
+    :class:`datetime.datetime`, optional
+        The represented datetime, in UTC (timezone aware).
+    """
+    try:
+        datetime_str = datetime_str.replace(",", "").replace("&#160;", " ").replace("\xa0", " ").strip()
+        # Extracting timezone
+        tz = datetime_str[-4:].strip()
+
+        # Convert time string to time object
+        # Removing timezone cause CEST and CET are not supported
+        try:
+            t = datetime.datetime.strptime(datetime_str[:-4].strip(), "%b %d %Y %H:%M:%S")
+        except ValueError:
+            t = datetime.datetime.strptime(datetime_str[:-4].strip(), "%b %d %Y %H:%M")
+
+        # Getting the offset
+        if tz == "CET":
+            utc_offset = 1
+        elif tz == "CEST":
+            utc_offset = 2
+        else:
+            return None
+        # Add/subtract hours to get the real time
+        t = t - datetime.timedelta(hours=utc_offset)
+        return t.replace(tzinfo=datetime.timezone.utc)
+    except (ValueError, AttributeError):
+        return None
+
+
+def parse_tibia_date(date_str) -> Optional[datetime.date]:
+    """Parse a date from the format used in Tibia.com.
+
+    Accepted format:
+
+    - ``MMM DD YYYY``, e.g. ``Jul 23 2015``
+
+    Parameters
+    -----------
+    date_str: :class:`str`
+        The date as represented in Tibia.com
+
+    Returns
+    -----------
+    :class:`datetime.date`, optional
+        The represented date, in UTC (timezone aware).
+    """
+    try:
+        t = datetime.datetime.strptime(date_str.strip(), "%b %d %Y")
+        return t.date()
+    except (ValueError, AttributeError):
+        return None
+
+
+def parse_tibia_forum_datetime(datetime_str, utc_offset=1):
+    """Parse a date in the format used in the Tibia.com forums.
+
+    Accepted format:
+
+    - ``DD.MM.YY HH:mm:ss``, e.g. ``23.07.2015 21:30:30``
+
+    Parameters
+    ----------
+    datetime_str: :class:`str`
+        The string containing the date and time.
+    utc_offset: :class:`int`
+        The UTC offset to apply to the parsed datetime.
+
+        Since the timestamps contain no timezone information, it can be passed as an additional parameter.
+
+        By default CET (+1) is considered.
+
+    Returns
+    -------
+    :class:`datetime.datetime`
+        The represented datetime, in UTC (timezone aware).
+    """
+    t = datetime.datetime.strptime(datetime_str.strip(), "%d.%m.%Y %H:%M:%S")
+    # Add/subtract hours to get the real time
+    t = t - datetime.timedelta(hours=utc_offset)
+    return t.replace(tzinfo=datetime.timezone.utc)
+
+
+def parse_tibia_full_date(date_str) -> Optional[datetime.date]:
+    """Parse a date in the fuller format used in Tibia.com.
+
+    Accepted format:
+
+    - ``MMMM DD, YYYY``, e.g. ``July 23, 2015``
+
+    Parameters
+    -----------
+    date_str: :class:`str`
+        The date as represented in Tibia.com
+
+    Returns
+    -----------
+    :class:`datetime.date`, optional
+        The represented date, in UTC (timezone aware).
+    """
+    try:
+        t = datetime.datetime.strptime(date_str.strip(), "%B %d, %Y")
+        return t.date()
+    except (ValueError, AttributeError):
+        return None
+
+
+def parse_number_words(text_num):
+    """Parse the word representation of a number to a integer.
+
+    Parameters
+    ----------
+    text_num: :class:`str`
+        The text representation of a number.
+
+    Returns
+    -------
+    :class:`int`
+        The number represented by the string.
+    """
+    numwords = {}
+    units = [
+        "zero", "one", "two", "three", "four", "five", "six", "seven", "eight",
+        "nine", "ten", "eleven", "twelve", "thirteen", "fourteen", "fifteen",
+        "sixteen", "seventeen", "eighteen", "nineteen",
+    ]
+
+    tens = ["", "", "twenty", "thirty", "forty", "fifty", "sixty", "seventy", "eighty", "ninety"]
+
+    scales = ["hundred", "thousand", "million", "billion", "trillion"]
+
+    numwords["and"] = (1, 0)
+    for idx, word in enumerate(units):
+        numwords[word] = (1, idx)
+    for idx, word in enumerate(tens):
+        numwords[word] = (1, idx * 10)
+    for idx, word in enumerate(scales):
+        numwords[word] = (10 ** (idx * 3 or 2), 0)
+
+    current = result = 0
+    text_num = text_num.replace("-", " ")
+    for word in text_num.split():
+        if word not in numwords:
+            return 0
+
+        scale, increment = numwords[word]
+        current = current * scale + increment
+        if scale > 100:
+            result += current
+            current = 0
+
+    return result + current
+
+
+def try_datetime(obj) -> Optional[datetime.datetime]:
+    """Attempt to convert an object into a datetime.
+
+    If the date format is known, it's recommended to use the corresponding function
+    This is meant to be used in constructors.
+
+    Parameters
+    ----------
+    obj: :class:`str`, :class:`dict`, :class:`datetime.datetime`
+        The object to convert.
+
+    Returns
+    -------
+    :class:`datetime.datetime`, optional
+        The represented datetime, in UTC (timezone aware), or :obj:`None` if conversion wasn't possible.
+    """
+    if obj is None:
+        return None
+    if isinstance(obj, datetime.datetime):
+        return obj
+    return parse_tibia_datetime(obj)
+
+
+def try_date(obj) -> Optional[datetime.date]:
+    """Attempt to convert an object into a date.
+
+    If the date format is known, it's recommended to use the corresponding function
+    This is meant to be used in constructors.
+
+    Parameters
+    ----------
+    obj: :class:`str`, :class:`datetime.datetime`, :class:`datetime.date`
+        The object to convert.
+
+    Returns
+    -------
+    :class:`datetime.date`, optional
+        The represented date, in UTC (timezone aware).
+    """
+    if obj is None:
+        return None
+    if isinstance(obj, datetime.datetime):
+        return obj.date()
+    if isinstance(obj, datetime.date):
+        return obj
+    res = parse_tibia_date(obj)
+    if res is not None:
+        return res
+    return parse_tibia_full_date(obj)
+
+
+def parse_tables_map(parsed_content: bs4.BeautifulSoup, selector = "div.TableContentContainer") -> Dict[str, bs4.Tag]:
+    tables = parsed_content.select("div.TableContainer")
+    output = {}
+    for table in tables:
+        caption = table.select_one("div.Text")
+        if not caption:
+            raise InvalidContent("table has no caption")
+        if content_table := table.select_one(selector):
+            output[clean_text(caption)] = content_table
+    return output
+
+
+def parse_tibiacom_content(content, *, html_class="BoxContent", tag="div", builder="lxml") -> bs4.BeautifulSoup:
+    """Parse HTML content from Tibia.com into a BeautifulSoup object.
+
+    Parameters
+    ----------
+    content: :class:`str`
+        The raw HTML content from Tibia.com
+    html_class: :class:`str`
+        The HTML class of the parsed element. The default value is ``BoxContent``.
+    tag: :class:`str`
+        The HTML tag select. The default value is ``div``.
+    builder: :class:`str`
+        The builder to use. The default value is ``lxml``.
+
+    Returns
+    -------
+    :class:`bs4.BeautifulSoup`, optional
+        The parsed content.
+    """
+    strainer = bs4.SoupStrainer(tag, class_=html_class) if builder != "html5lib" else None
+    return bs4.BeautifulSoup(content.replace('ISO-8859-1', 'utf-8', 1), builder, parse_only=strainer)
+
+
+
+def parse_tibiacom_tables(parsed_content) -> Dict[str, bs4.Tag]:
+    """Parse tables from Tibia.com into a mapping by the tables title.
+
+    This is used for the table style used in Tibia.com, where a table is wrapped in a container with a title.
+
+    Parameters
+    ----------
+    parsed_content: :class:`bs4.BeautifulSoup`
+        The content to find the tables in.
+
+    Returns
+    -------
+    :class:`dict`
+        A dictionary mapping the container titles and the contained table.
+    """
+    table_containers = parsed_content.find_all("div", attrs={"class": "TableContainer"})
+    tables = {}
+    for table_container in table_containers:
+        text_tag = table_container.find("div", attrs={"class": "Text"})
+        table = table_container.find("table", attrs={"class": "TableContent"})
+        if not table:
+            continue
+        tables[text_tag.text.strip()] = table
+    return tables
+
+
+T = TypeVar('T')
+D = TypeVar('D')
+
+
+def try_enum(cls: Type[T], val, default: D = None) -> Union[T, D]:
+    """Attempt to convert a value into their enum value.
+
+    Parameters
+    ----------
+    cls: :class:`Enum`
+        The enum to convert to.
+    val:
+        The value to try to convert to Enum
+    default: optional
+        The value to return if no enum value is found.
+
+    Returns
+    -------
+    obj:
+        The enum value if found, otherwise None.
+    """
+    if isinstance(val, cls):
+        return val
+    try:
+        return cls(val)
+    except ValueError:
+        try:
+            if isinstance(val, str):
+                val = val.upper()
+            return cls._member_map_[val]
+        except KeyError:
+            return default
+
+
+def parse_tibia_money(argument):
+    """Parse a string that may contain 'k' as thousand suffix.
+
+    Parameters
+    ----------
+    argument: :class:`str`
+        A numeric string using k as a prefix for thousands.
+
+    Returns
+    -------
+    :class:`int`:
+        The value represented by the string.
+    """
+    try:
+        return int(argument)
+    except ValueError:
+        argument = argument.replace(",", "").strip().lower()
+        m = TIBIA_CASH_PATTERN.match(argument)
+        if not m or not m.group(1):
+            raise ValueError("not a numeric value")
+        num = float(m.group(1))
+        k_count = argument.count("k")
+        num *= pow(1000, k_count)
+        return int(num)
+
+
+def split_list(items, separator=",", last_separator=" and "):
+    """Split a string listing elements into an actual list.
+
+    Parameters
+    ----------
+    items: :class:`str`
+        A string listing elements.
+    separator: :class:`str`
+        The separator between each item. A comma by default.
+    last_separator: :class:`str`
+        The separator used for the last item. ' and ' by default.
+
+    Returns
+    -------
+    :class:`list` of :class:`str`
+        A list containing each one of the items.
+    """
+    if items is None:
+        return None
+    items = items.split(separator)
+    last_item = items[-1]
+    last_split = last_item.split(last_separator)
+    if len(last_split) > 1:
+        items[-1] = last_separator.join(last_split[:-1])
+        items.append(last_split[-1])
+    return [e.strip() for e in items]
+
+
+def _recursive_strip(value):  # pragma: no cover
+    if isinstance(value, dict):
+        return {k: _recursive_strip(v) for k, v in value.items()}
+    if isinstance(value, list):
+        return [_recursive_strip(i) for i in value]
+    if isinstance(value, str):
+        return value.strip()
+    return value
+
+
+def deprecated(instead=None):  # pragma: no cover
+    def actual_decorator(func):
+        @functools.wraps(func)
+        def decorated(*args, **kwargs):
+            warnings.simplefilter('always', DeprecationWarning)
+            if instead:
+                fmt = "{0.__name__} is deprecated, use {1} instead."
+            else:
+                fmt = '{0.__name__} is deprecated.'
+
+            warnings.warn(fmt.format(func, instead), stacklevel=3, category=DeprecationWarning)
+            warnings.simplefilter('default', DeprecationWarning)
+            return func(*args, **kwargs)
+        return decorated
+    return actual_decorator
+
+
+def parse_popup(popup_content) -> Tuple[str, bs4.BeautifulSoup]:
+    """Parse the information popups used through Tibia.com.
+
+    Parameters
+    ----------
+    popup_content: :class:`str`
+        The raw content of the javascript function that creates the popup.
+
+    Returns
+    -------
+    :class:`str`
+        The popup's title.
+    :class:`bs4.BeautifulSoup`
+        The parsed HTML content of the popup.
+    """
+    parts = popup_content.split(",", 2)
+    title = parts[1].replace(r"'", "").strip()
+    html = parts[-1].replace(r"\'", '"').replace(r"'", "").replace(",);", "").replace(", );", "").strip()
+    parsed_html = bs4.BeautifulSoup(html, 'lxml')
+    return title, parsed_html
+
+
+results_pattern = re.compile(r'Results: ([\d,]+)')
+page_pattern = re.compile(r'page=(\d+)')
+
+
+def parse_pagination(pagination_block) -> Tuple[int, int, int]:
+    """Parse a pagination section in Tibia.com and extracts its information.
+
+    Parameters
+    ----------
+    pagination_block: :class:`bs4.Tag`
+        The HTML containing the pagination information.
+
+    Returns
+    -------
+    page : :class:`int`
+        The current page.
+    total_pages : :class:`int`
+        The total number of pages.
+    results_count : :class:`int`
+        The total number of results.
+    """
+    pages_div, results_div = pagination_block.select("small > div")
+    current_page_link = pages_div.find("span", {"class": "CurrentPageLink"})
+    page_links = pages_div.find_all("span", {"class": "PageLink"})
+    # pages_with_links = pages_div.select(#)
+    first_or_last_pages = pages_div.find_all("span", {"class": "FirstOrLastElement"})
+    page = -1
+    total_pages = -1
+    if first_or_last_pages:
+        last_page_link = first_or_last_pages[-1].find("a")
+        if last_page_link:
+            m = page_pattern.search(last_page_link["href"])
+            if m:
+                total_pages = int(m.group(1))
+        else:
+            last_page_link = page_links[-2].find("a")
+            total_pages = int(last_page_link.text) + 1
+    else:
+        last_page_link = page_links[-1]
+        total_pages = int(last_page_link.text)
+    try:
+        page = int(current_page_link.text)
+    except ValueError:
+        if "First" in current_page_link.text:
+            page = 1
+        else:
+            page = total_pages
+    results_count = parse_integer(results_pattern.search(results_div.text).group(1))
+    return page, total_pages, results_count
```

