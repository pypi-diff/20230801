# Comparing `tmp/APKMirror_Search-1.0.0-py3-none-any.whl.zip` & `tmp/APKMirror_Search-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 20897 bytes, number of entries: 12
--rwxrwxrwx  2.0 unx      371 b- defN 22-Jul-26 02:42 apksearch/__init__.py
--rwxrwxrwx  2.0 unx     1875 b- defN 22-Jul-26 01:26 apksearch/entities.py
--rwxrwxrwx  2.0 unx     5936 b- defN 22-Jul-26 10:15 apksearch/parsing.py
--rwxrwxrwx  2.0 unx     7212 b- defN 22-Jul-26 19:45 apksearch/search.py
--rwxrwxrwx  2.0 unx      229 b- defN 22-Jul-26 01:44 tests/__init__.py
--rwxrwxrwx  2.0 unx     6864 b- defN 22-Jul-26 10:19 tests/test_parsing.py
--rwxrwxrwx  2.0 unx     5266 b- defN 22-Jul-26 19:47 tests/test_search.py
--rwxrwxrwx  2.0 unx    35149 b- defN 22-Jul-26 19:48 APKMirror_Search-1.0.0.dist-info/LICENSE
--rwxrwxrwx  2.0 unx      300 b- defN 22-Jul-26 19:48 APKMirror_Search-1.0.0.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 22-Jul-26 19:48 APKMirror_Search-1.0.0.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       16 b- defN 22-Jul-26 19:48 APKMirror_Search-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      967 b- defN 22-Jul-26 19:48 APKMirror_Search-1.0.0.dist-info/RECORD
-12 files, 64277 bytes uncompressed, 19277 bytes compressed:  70.0%
+Zip file size: 20920 bytes, number of entries: 12
+-rwxrwxrwx  2.0 unx      371 b- defN 23-Aug-01 11:07 apksearch/__init__.py
+-rwxrwxrwx  2.0 unx     1875 b- defN 23-Aug-01 11:07 apksearch/entities.py
+-rwxrwxrwx  2.0 unx     5936 b- defN 23-Aug-01 11:07 apksearch/parsing.py
+-rwxrwxrwx  2.0 unx     6983 b- defN 23-Aug-01 11:07 apksearch/search.py
+-rwxrwxrwx  2.0 unx      229 b- defN 23-Aug-01 11:07 tests/__init__.py
+-rwxrwxrwx  2.0 unx     7401 b- defN 23-Aug-01 11:07 tests/test_parsing.py
+-rwxrwxrwx  2.0 unx     5727 b- defN 23-Aug-01 11:07 tests/test_search.py
+-rwxrwxrwx  2.0 unx    35149 b- defN 23-Aug-01 11:07 APKMirror_Search-1.0.1.dist-info/LICENSE
+-rwxrwxrwx  2.0 unx      237 b- defN 23-Aug-01 11:07 APKMirror_Search-1.0.1.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Aug-01 11:07 APKMirror_Search-1.0.1.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       16 b- defN 23-Aug-01 11:07 APKMirror_Search-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      967 b- defN 23-Aug-01 11:07 APKMirror_Search-1.0.1.dist-info/RECORD
+12 files, 64983 bytes uncompressed, 19300 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tests/test_parsing.py
 Comment: 
 
 Filename: tests/test_search.py
 Comment: 
 
-Filename: APKMirror_Search-1.0.0.dist-info/LICENSE
+Filename: APKMirror_Search-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: APKMirror_Search-1.0.0.dist-info/METADATA
+Filename: APKMirror_Search-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: APKMirror_Search-1.0.0.dist-info/WHEEL
+Filename: APKMirror_Search-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: APKMirror_Search-1.0.0.dist-info/top_level.txt
+Filename: APKMirror_Search-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: APKMirror_Search-1.0.0.dist-info/RECORD
+Filename: APKMirror_Search-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## apksearch/__init__.py

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from .search import package_search_match, generate_download_url
+from .search import generate_download_url, package_search_match
 
 __all__ = ["package_search_match", "generate_download_url"]
 
 
 logger = logging.getLogger(__name__)
 ch = logging.StreamHandler()
 ch.setLevel(logging.DEBUG)
```

## apksearch/parsing.py

 * *Ordering differences only*

```diff
@@ -1,12 +1,12 @@
 import logging
 import re
 import unicodedata
-from typing import Dict, List
 import urllib
+from typing import Dict, List
 
 from bs4 import BeautifulSoup
 
 from .entities import PackageBase, PackageVariant, PackageVersion
 
 logger = logging.getLogger(__name__)
```

## apksearch/search.py

```diff
@@ -22,16 +22,16 @@
 HEADERS = {
     "user-agent": "apksearch APKMirrorSearcher/1.0.0",
 }
 
 logger = logging.getLogger(__name__)
 
 
-async def gather_from_dict(tasks: Dict[Hashable, Awaitable], loop=None, return_exceptions=False):
-    results = await asyncio.gather(*tasks.values(), loop=loop, return_exceptions=return_exceptions)
+async def gather_from_dict(tasks: Dict[Hashable, Awaitable], return_exceptions=False):
+    results = await asyncio.gather(*tasks.values(), return_exceptions=return_exceptions)
     return dict(zip(tasks.keys(), results))
 
 
 def _generate_params_list(packages: List[str]) -> List[str]:
     param_list = []
     for package in packages:
         params = copy.copy(QUERY_PARAMS)
@@ -82,119 +82,112 @@
 
 
 async def generate_download_url(variant: PackageVariant) -> str:
     """Generates a packages temporary download URL
 
     :param variant: Variant to determine URL
     """
-    loop = asyncio.get_running_loop()
-    results = await _perform_basic_query(loop, [variant.variant_info])
-    variant_defs = {
-        variant: results[0]
-    }
+    results = await _perform_basic_query([variant.variant_info])
+    variant_defs = {variant: results[0]}
     parsing.process_variant_result(variant_defs)
-    results = await _perform_basic_query(loop, [variant.variant_download_page])
-    download_results = {
-        variant: results[0]
-    }
+    results = await _perform_basic_query([variant.variant_download_page])
+    download_results = {variant: results[0]}
     parsing.process_variant_download_result(download_results)
     return variant.download_url
 
 
 async def execute_package_search(packages: List[str]) -> List[str]:
     """Perform aiohttp requests to APKMirror
 
     :param list packages: Packages that will be searched for. Each package will generate a new
         request
 
     :return: A list of results containing the first page of each package search
     :rtype: list
     """
     param_list: List[str] = _generate_params_list(packages)
-    loop = asyncio.get_running_loop()
-    return await _perform_search(loop, param_list)
+    return await _perform_search(param_list)
 
 
 async def execute_package_page(packages: List[str]) -> Dict[str, PackageBase]:
     """Query all root package pages
 
     :param packages: List of root package pages to query
     """
-    loop = asyncio.get_running_loop()
-    results = await _perform_basic_query(loop, packages)
+    results = await _perform_basic_query(packages)
     return parsing.process_package_page(results)
 
 
 async def execute_release_info(packages: Dict[str, PackageBase]) -> Dict[PackageVersion, str]:
     """Execute all requests related to the package versions
 
     :param dict package_defs: Current found information from the initial search. It will be updated
         in place with the release information found during the step
     """
     releases = []
     for info in packages.values():
         for package_version in info.versions.values():
             releases.append(package_version)
-    loop = asyncio.get_running_loop()
-    return await _perform_dict_lookup(loop, releases)
+    return await _perform_dict_lookup(releases)
 
 
 async def execute_variant_info(packages: Dict[str, PackageBase]) -> Dict[PackageVersion, str]:
     variants = []
     for info in packages.values():
         for package_version in info.versions.values():
             for arch in package_version.arch.values():
                 variants.extend(arch)
-    loop = asyncio.get_running_loop()
-    return await _perform_dict_lookup(loop, variants)
+    return await _perform_dict_lookup(variants)
 
 
 async def gather_release_info(releases: List[PackageBase]) -> Tuple[PackageVersion, PackageVariant, str]:
     loop = asyncio.get_running_loop()
-    results = loop.run_until_complete(_perform_dict_lookup(loop, releases))
+    results = loop.run_until_complete(_perform_dict_lookup(releases))
     return results
 
 
 async def _fetch_one(session, url, params):
     async with session.get(url, ssl=ssl.SSLContext(), params=params, headers=HEADERS) as response:
         logger.debug("About to query %s", response.request_info)
         return await response.text()
 
 
-async def _perform_search(loop, query_params: List[str]):
+async def _perform_search(query_params: List[str]):
+    loop = asyncio.get_running_loop()
     async with aiohttp.ClientSession(loop=loop) as session:
         required_urls = [_fetch_one(session, QUERY_URL, param) for param in query_params]
         logger.info("About to query %s packages", len(required_urls))
         results = await asyncio.gather(
             *required_urls,
             return_exceptions=True,
         )
         return results
 
 
-async def _perform_basic_query(loop, urls: List[str]):
-    async with aiohttp.ClientSession(loop=loop) as session:
+async def _perform_basic_query(urls: List[str]):
+    async with aiohttp.ClientSession() as session:
         required_urls = [_fetch_one(session, url, {}) for url in urls]
         logger.info("About to query %s packages", len(required_urls))
         results = await asyncio.gather(
             *required_urls,
             return_exceptions=True,
         )
         return results
 
 
-async def _perform_dict_lookup(loop, requests: List[Union[PackageVersion, PackageVariant]]):
+async def _perform_dict_lookup(requests: List[Union[PackageVersion, PackageVariant]]):
     if len(requests) == 0:
         return []
-    if type(requests[0]) == PackageVersion:
+    if isinstance(requests[0], PackageVersion):
         identifier = "releases"
         url_attr = "link"
     else:
         identifier = "variants"
         url_attr = "variant_download_page"
+    loop = asyncio.get_running_loop()
     async with aiohttp.ClientSession(loop=loop) as session:
         tasks = {}
         logger.info("About to query %s %s", len(requests), identifier)
         for request in requests:
             tasks[request] = _fetch_one(session, getattr(request, url_attr), {})
         results = await gather_from_dict(tasks)
         return results
```

## tests/test_parsing.py

```diff
@@ -1,47 +1,52 @@
-import os
+# flake8: noqa E501
+
 import pytest
+
 from apksearch import entities, parsing
+
 from . import get_test_contents
 
 
 def build_test(filename, base_entity):
     return {base_entity: get_test_contents(filename)}
 
 
 @pytest.mark.parametrize(
-    "filename,expected", [
+    "filename,expected",
+    [
         (
             "pogo_0.243.0_32_apk_download.html",
-            "https://apkmirror.com/wp-content/themes/APKMirror/download.php?id=3692376&key=1893849fcf0eaeb278bb3d53c9425a96f190c243&forcebaseapk=true"
+            "https://apkmirror.com/wp-content/themes/APKMirror/download.php?id=3692376&key=1893849fcf0eaeb278bb3d53c9425a96f190c243&forcebaseapk=true",
         ),
         (
             "pogo_0.243.0_32_bundle_download.html",
-            "https://apkmirror.com/wp-content/themes/APKMirror/download.php?id=3694845&key=82896f35e2a70709ab00137be28fc968624a661c"
+            "https://apkmirror.com/wp-content/themes/APKMirror/download.php?id=3694845&key=82896f35e2a70709ab00137be28fc968624a661c",
         ),
-    ]
+    ],
 )
 def test_generate_download_link(filename, expected):
     content = get_test_contents(filename)
     assert parsing.generate_download_link(content) == expected
 
 
 @pytest.mark.parametrize(
-    "variant,filename,expected", [
+    "variant,filename,expected",
+    [
         (
             entities.PackageVariant(
                 "APK",
                 "nodpi",
                 2022070700,
                 variant_info=(
                     "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/pokemon-go-0-243-0-android-apk-download/"
                 ),
             ),
             "pogo_0.243.0_32_apk_download.html",
-            "https://apkmirror.com/wp-content/themes/APKMirror/download.php?id=3692376&key=1893849fcf0eaeb278bb3d53c9425a96f190c243&forcebaseapk=true"
+            "https://apkmirror.com/wp-content/themes/APKMirror/download.php?id=3692376&key=1893849fcf0eaeb278bb3d53c9425a96f190c243&forcebaseapk=true",
         ),
         (
             entities.PackageVariant(
                 "BUNDLE",
                 "nodpi",
                 2022070700,
                 variant_info=(
@@ -58,38 +63,37 @@
                 2022070701,
                 variant_info=(
                     "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/pokemon-go-0-243-0-4-android-apk-download/"
                 ),
             ),
             "pogo_0.243.0_64_bundle_download.html",
             "https://apkmirror.com/wp-content/themes/APKMirror/download.php?id=3694846&key=1ba4afa3a8584742f2fcc2ac09dfc6376fb20a07",
-        )
-    ]
+        ),
+    ],
 )
 def test_process_variant_download_result(variant, filename, expected):
-    results = {
-        variant: get_test_contents(filename)
-    }
+    results = {variant: get_test_contents(filename)}
     parsing.process_variant_download_result(results)
     assert variant.download_url == expected
 
 
 @pytest.mark.parametrize(
-    "variant,filename,expected", [
+    "variant,filename,expected",
+    [
         (
             entities.PackageVariant(
                 "APK",
                 "nodpi",
                 2022070700,
                 variant_info=(
                     "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/pokemon-go-0-243-0-android-apk-download/"
                 ),
             ),
             "pogo_0.243.0_32_apk.html",
-            "https://apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/pokemon-go-0-243-0-android-apk-download/download/?key=74cda5696fa78d83b50da3f4fa5c9885d17076a1&forcebaseapk=true"
+            "https://apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/pokemon-go-0-243-0-android-apk-download/download/?key=74cda5696fa78d83b50da3f4fa5c9885d17076a1&forcebaseapk=true",
         ),
         (
             entities.PackageVariant(
                 "BUNDLE",
                 "nodpi",
                 2022070700,
                 variant_info=(
@@ -106,53 +110,71 @@
                 2022070701,
                 variant_info=(
                     "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/pokemon-go-0-243-0-4-android-apk-download/"
                 ),
             ),
             "pogo_0.243.0_64_bundle.html",
             "https://apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/pokemon-go-0-243-0-4-android-apk-download/download/?key=5a99f61e71380269ef0e71e33715ddbc073f966c",
-        )
-    ]
+        ),
+    ],
 )
 def test_process_variant(variant, filename, expected):
-    results = {
-        variant: get_test_contents(filename)
-    }
+    results = {variant: get_test_contents(filename)}
     parsing.process_variant_result(results)
     assert variant.variant_download_page == expected
 
 
 # @TODO
 def test_process_release_result():
     pass
 
 
 @pytest.mark.parametrize(
-    "filename,expected", [
+    "filename,expected",
+    [
         (
             "pogo.html",
             {
-                "Pokemon GO":
-                entities.PackageBase(
+                "Pokemon GO": entities.PackageBase(
                     "Pokemon GO",
                     "com.nianticlabs.pokemongo",
                     info_page="https://www.apkmirror.com/apk/niantic-inc/pokemon-go/",
                     versions={
-                        "0.243.0": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/"),
-                        "0.241.1": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-241-1-release/"),
-                        "0.241.0": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-241-0-release/"),
-                        "0.239.2": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-239-2-release/"),
-                        "0.239.1": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-239-1-release/"),
-                        "0.239.0": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-239-0-release/"),
-                        "0.237.0": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-237-0-release/"),
-                        "0.235.0": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-235-0-release/"),
-                        "0.233.1": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-233-1-release/"),
-                        "0.233.0": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-233-0-release/"),
-                    }
+                        "0.243.0": entities.PackageVersion(
+                            "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/"
+                        ),
+                        "0.241.1": entities.PackageVersion(
+                            "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-241-1-release/"
+                        ),
+                        "0.241.0": entities.PackageVersion(
+                            "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-241-0-release/"
+                        ),
+                        "0.239.2": entities.PackageVersion(
+                            "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-239-2-release/"
+                        ),
+                        "0.239.1": entities.PackageVersion(
+                            "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-239-1-release/"
+                        ),
+                        "0.239.0": entities.PackageVersion(
+                            "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-239-0-release/"
+                        ),
+                        "0.237.0": entities.PackageVersion(
+                            "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-237-0-release/"
+                        ),
+                        "0.235.0": entities.PackageVersion(
+                            "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-235-0-release/"
+                        ),
+                        "0.233.1": entities.PackageVersion(
+                            "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-233-1-release/"
+                        ),
+                        "0.233.0": entities.PackageVersion(
+                            "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-233-0-release/"
+                        ),
+                    },
                 )
-            }
+            },
         ),
-    ]
+    ],
 )
 def test_parse_package_page(filename, expected):
     data = get_test_contents(filename)
     assert parsing.process_package_page([data]) == expected
```

## tests/test_search.py

```diff
@@ -1,103 +1,129 @@
+# flake8: noqa E501
+
 import pytest
+from aioresponses import aioresponses
+
+from apksearch import entities, search
 
-from apksearch import search, entities
 from . import get_test_contents
-from aioresponses import aioresponses
 
 
 @pytest.mark.asyncio
 async def test_execute_package_page():
     with aioresponses() as mocked:
         mocked.get(
-            "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/",
-            status=200,
-            body=get_test_contents("pogo.html")
+            "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/", status=200, body=get_test_contents("pogo.html")
         )
         results = await search.execute_package_page(["https://www.apkmirror.com/apk/niantic-inc/pokemon-go/"])
     expected = {
-        "Pokemon GO":
-        entities.PackageBase(
+        "Pokemon GO": entities.PackageBase(
             "Pokemon GO",
             "com.nianticlabs.pokemongo",
             info_page="https://www.apkmirror.com/apk/niantic-inc/pokemon-go/",
             versions={
-                "0.243.0": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/"),
-                "0.241.1": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-241-1-release/"),
-                "0.241.0": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-241-0-release/"),
-                "0.239.2": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-239-2-release/"),
-                "0.239.1": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-239-1-release/"),
-                "0.239.0": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-239-0-release/"),
-                "0.237.0": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-237-0-release/"),
-                "0.235.0": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-235-0-release/"),
-                "0.233.1": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-233-1-release/"),
-                "0.233.0": entities.PackageVersion("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-233-0-release/"),
-            }
+                "0.243.0": entities.PackageVersion(
+                    "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/"
+                ),
+                "0.241.1": entities.PackageVersion(
+                    "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-241-1-release/"
+                ),
+                "0.241.0": entities.PackageVersion(
+                    "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-241-0-release/"
+                ),
+                "0.239.2": entities.PackageVersion(
+                    "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-239-2-release/"
+                ),
+                "0.239.1": entities.PackageVersion(
+                    "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-239-1-release/"
+                ),
+                "0.239.0": entities.PackageVersion(
+                    "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-239-0-release/"
+                ),
+                "0.237.0": entities.PackageVersion(
+                    "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-237-0-release/"
+                ),
+                "0.235.0": entities.PackageVersion(
+                    "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-235-0-release/"
+                ),
+                "0.233.1": entities.PackageVersion(
+                    "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-233-1-release/"
+                ),
+                "0.233.0": entities.PackageVersion(
+                    "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-233-0-release/"
+                ),
+            },
         )
     }
     assert results == expected
 
 
 @pytest.mark.asyncio
 async def test_package_search_match():
     versions = ["0.243.0", "0.241.0"]
     with aioresponses() as mocked:
         mocked.get(
-            "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/",
-            status=200,
-            body=get_test_contents("pogo.html")
+            "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/", status=200, body=get_test_contents("pogo.html")
         )
         mocked.get(
             "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/",
             status=200,
-            body=get_test_contents("pogo_0.243.0.html")
+            body=get_test_contents("pogo_0.243.0.html"),
         )
         mocked.get(
             "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-241-0-release/",
             status=200,
-            body=get_test_contents("pogo_0.243.0.html")
+            body=get_test_contents("pogo_0.243.0.html"),
+        )
+        results = await search.package_search_match(
+            "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/", versions=versions
         )
-        results = await search.package_search_match("https://www.apkmirror.com/apk/niantic-inc/pokemon-go/", versions=versions)
     assert len(versions) == len(results.versions)
     for version in versions:
         assert version in results.versions
         assert "armeabi-v7a" in results.versions[version].arch
         assert "arm64-v8a" in results.versions[version].arch
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
-    "variant,expected_download_url", [
+    "variant,expected_download_url",
+    [
         (
-            entities.PackageVariant("APK", "nodpi", 2022070700, variant_info="https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/pokemon-go-0-243-0-android-apk-download/"),
-            "https://apkmirror.com/wp-content/themes/APKMirror/download.php?id=3692376&key=1893849fcf0eaeb278bb3d53c9425a96f190c243&forcebaseapk=true"
+            entities.PackageVariant(
+                "APK",
+                "nodpi",
+                2022070700,
+                variant_info="https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/pokemon-go-0-243-0-android-apk-download/",
+            ),
+            "https://apkmirror.com/wp-content/themes/APKMirror/download.php?id=3692376&key=1893849fcf0eaeb278bb3d53c9425a96f190c243&forcebaseapk=true",
         )
-    ]
+    ],
 )
 async def test_generate_download_url(variant, expected_download_url):
     with aioresponses() as mocked:
         mocked.get(
             "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/pokemon-go-0-243-0-android-apk-download/",
             status=200,
-            body=get_test_contents("pogo_0.243.0_32_apk.html")
+            body=get_test_contents("pogo_0.243.0_32_apk.html"),
         )
         mocked.get(
             "https://apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/pokemon-go-0-243-0-android-apk-download/download/?key=74cda5696fa78d83b50da3f4fa5c9885d17076a1&forcebaseapk=true",
             status=200,
-            body=get_test_contents("pogo_0.243.0_32_apk_download.html")
+            body=get_test_contents("pogo_0.243.0_32_apk_download.html"),
         )
         mocked.get(
             "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/pokemon-go-0-243-0-3-android-apk-download/",
             status=200,
-            body=get_test_contents("pogo_0.243.0_32_bundle.html")
+            body=get_test_contents("pogo_0.243.0_32_bundle.html"),
         )
         mocked.get(
             "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/pokemon-go-0-243-0-4-android-apk-download/",
             status=200,
-            body=get_test_contents("pogo_0.243.0_64_bundle.html")
+            body=get_test_contents("pogo_0.243.0_64_bundle.html"),
         )
         mocked.get(
             "https://www.apkmirror.com/apk/niantic-inc/pokemon-go/pokemon-go-0-243-0-release/pokemon-go-0-243-0-2-android-apk-download/",
             status=200,
-            body=get_test_contents("pogo_0.243.0_64_apk.html")
+            body=get_test_contents("pogo_0.243.0_64_apk.html"),
         )
         assert await search.generate_download_url(variant) == expected_download_url
```

## Comparing `APKMirror_Search-1.0.0.dist-info/LICENSE` & `APKMirror_Search-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

