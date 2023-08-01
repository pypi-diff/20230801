# Comparing `tmp/weboptout-0.2.2.tar.gz` & `tmp/weboptout-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weboptout-0.2.2.tar", max compression
+gzip compressed data, was "weboptout-0.3.tar", max compression
```

## Comparing `weboptout-0.2.2.tar` & `weboptout-0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     5003 2023-07-27 10:15:30.579513 weboptout-0.2.2/LICENSE
--rw-r--r--   0        0        0     7766 2023-07-27 10:15:31.339551 weboptout-0.2.2/data/tos.jsonl
--rw-r--r--   0        0        0      900 2023-07-27 10:15:31.355552 weboptout-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      191 2023-07-27 10:15:31.355552 weboptout-0.2.2/src/weboptout/__init__.py
--rw-r--r--   0        0        0     1228 2023-07-27 10:15:30.579513 weboptout-0.2.2/src/weboptout/client.py
--rw-r--r--   0        0        0     1742 2023-07-27 10:15:30.579513 weboptout-0.2.2/src/weboptout/config.py
--rw-r--r--   0        0        0     4092 2023-07-27 10:15:30.579513 weboptout-0.2.2/src/weboptout/html.py
--rw-r--r--   0        0        0     8030 2023-07-27 10:15:30.579513 weboptout-0.2.2/src/weboptout/http.py
--rw-r--r--   0        0        0     1637 2023-07-27 10:15:30.579513 weboptout-0.2.2/src/weboptout/types.py
--rw-r--r--   0        0        0     7003 2023-07-27 10:15:30.579513 weboptout-0.2.2/src/weboptout/utils.py
--rw-r--r--   0        0        0     1690 2023-07-27 10:15:30.579513 weboptout-0.2.2/src/weboptout/web.py
--rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 weboptout-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     5003 2023-08-01 16:39:50.822271 weboptout-0.3/LICENSE
+-rw-r--r--   0        0        0     8820 2023-08-01 16:39:51.746272 weboptout-0.3/data/tos.jsonl
+-rw-r--r--   0        0        0      896 2023-08-01 16:39:51.766273 weboptout-0.3/pyproject.toml
+-rw-r--r--   0        0        0      189 2023-08-01 16:39:51.770273 weboptout-0.3/src/weboptout/__init__.py
+-rw-r--r--   0        0        0     3710 2023-08-01 16:39:50.822271 weboptout-0.3/src/weboptout/client.py
+-rw-r--r--   0        0        0     1820 2023-08-01 16:39:50.822271 weboptout-0.3/src/weboptout/config.py
+-rw-r--r--   0        0        0     4137 2023-08-01 16:39:50.822271 weboptout-0.3/src/weboptout/html.py
+-rw-r--r--   0        0        0     7374 2023-08-01 16:39:50.822271 weboptout-0.3/src/weboptout/http.py
+-rw-r--r--   0        0        0     1650 2023-08-01 16:39:50.822271 weboptout-0.3/src/weboptout/steps.py
+-rw-r--r--   0        0        0     1604 2023-08-01 16:39:50.822271 weboptout-0.3/src/weboptout/types.py
+-rw-r--r--   0        0        0     7178 2023-08-01 16:39:50.822271 weboptout-0.3/src/weboptout/utils.py
+-rw-r--r--   0        0        0     1625 2023-08-01 16:39:50.822271 weboptout-0.3/src/weboptout/web.py
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 weboptout-0.3/PKG-INFO
```

### Comparing `weboptout-0.2.2/LICENSE` & `weboptout-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `weboptout-0.2.2/data/tos.jsonl` & `weboptout-0.3/data/tos.jsonl`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ## Copyright © 2023, Alex J. Champandard. All rights reserved; see LICENSE! ⚘
 ["*cnn.com", "https://edition.cnn.com/terms0"]
 ["deviantart.com", "https://www.deviantart.com/about/policy/service"]
 ["pinterest.com", "https://policy.pinterest.com/en-gb/community-guidelines"]
 ["instagram.com", "https://help.instagram.com/581066165581870/"]
 ["facebook.com", "https://www.facebook.com/legal/terms"]
 ["twitter.com", "https://twitter.com/en/tos"]
+["*.twimg.com", "https://twitter.com/en/tos"]
 ["behance.net", "https://www.adobe.com/legal/terms.html"]
 ["wordpress.com", "https://wordpress.com/tos/"]
 ["*shopify.com", "https://www.shopify.com/legal/terms"]
 ["thumbs.dreamstime.com", "https://www.dreamstime.com/terms"]
 ["i.pinimg.com", "https://policy.pinterest.com/en-gb/community-guidelines"]
 ["i.ebayimg.com", "https://www.ebay.com/help/policies/member-behaviour-policies/user-agreement?id=4259"]
 ["*ebay.com", "https://www.ebay.com/help/policies/member-behaviour-policies/user-agreement?id=4259"]
@@ -20,15 +21,14 @@
 ["*.zcache.*", "https://www.zazzle.com/mk/policy/user_agreement"]
 ["i.ytimg.com", "https://www.youtube.com/t/terms"]
 ["*.yimg.com", "https://legal.yahoo.com/us/en/yahoo/terms/otos/index.html"]
 ["*amazon.com", "https://www.amazon.com/gp/help/customer/display.html%3FnodeId%3DGLSBYFE9MGKKQXXM"]
 ["static.wixstatic.com", "https://www.wix.com/about/terms-of-use"]
 ["i?.wp.com", "https://wordpress.com/tos/"]
 ["images.squarespace-cdn.com", "https://www.squarespace.com/acceptable-use-policy/"]
-["images.slideplayer.com", "https://slideplayer.com/support/terms/"]
 ["photos.smugmug.com", "https://www.smugmug.com/about/terms"]
 ["i?.cpcache.com", "https://www.cafepress.com/p/terms-conditions"]
 ["*aliexpress.*", "https://rulechannel.alibaba.com/icbu?spm=a1zaa.8161610.0.0.23eb61ecCCJxWd&type=detail&ruleId=2041&cId=1307#/rule/detail?cId=1307&ruleId=2041"]
 ["*.alicdn.com", "https://rulechannel.alibaba.com/icbu?spm=a1zaa.8161610.0.0.23eb61ecCCJxWd&type=detail&ruleId=2041&cId=1307#/rule/detail?cId=1307&ruleId=2041"]                
 ["*.i.aliimg.com", "https://rulechannel.alibaba.com/icbu?type=detail&ruleId=2041&cId=1307#/rule/detail?cId=1307&ruleId=2041"]
 ["*gettyimages.com", "https://www.gettyimages.com/company/terms?language=en-us"]
 ["cdn*.bigcommerce.com", "https://www.bigcommerce.com/terms/acceptable-use-policy/"]
@@ -42,31 +42,31 @@
 ["ssl.c.photoshelter.com", "https://company.photoshelter.com/terms/"]
 ["?.bp.blogspot.com", "https://policies.google.com/u/0/terms"]
 ["*.scribdassets.com", "https://support.scribd.com/hc/en-us/articles/210129326-General-Terms-of-Use"]
 ["ctl.s6img.com", "https://society6.com/terms"]
 ["*.bing.net", "https://www.microsoft.com/en-us/legal/terms-of-use"]
 ["upload.wikimedia.org", "https://foundation.wikimedia.org/wiki/Policy:Terms_of_Use"]
 ["img.shopstyle-cdn.com", "https://www.shopstyle.com/tos"]
-["cdn.webshopapp.com", "https://www.lightspeedhq.com/legal/lightspeed-service-agreement/"]
+["cdn.webshopapp.com", "https://www.lightspeedhq.com/legal/acceptable-use-policy/"]
 ["?.keepcalms.com", "https://keepcalms.com/privacy/"]
-["slideplayer.com", "https://slideplayer.com/support/terms/"]
+["*slideplayer.*", "https://slideplayer.com/support/terms/"]
 ["http?.mlstatic.com", "https://www.mercadolibre.com.mx/ayuda/terminos-y-condiciones-uso-del-sitio_2090"]
 ["res.cloudinary.com", "https://cloudinary.com/tou"]
 ["ecdn.teacherspayteachers.com", "https://www.teacherspayteachers.com/Terms-of-Service"]
-["www.dhresource.com", "https://www.dhgate.com/helpbuyer/11111111111111111111111111111111-en-0/444c48545da84a0e9ad179106ca19d09.html"]
+["*.dhresource.com", "https://www.dhgate.com/helpbuyer/11111111111111111111111111111111-en-0/444c48545da84a0e9ad179106ca19d09.html"]
 ["?.*.photoshelter.com", "https://www.photoshelter.com/support/terms"]
 ["*shutterstock.com", "https://www.shutterstock.com/terms?language=en-US"]
 ["data.whicdn.com", "https://prezi.com/legal/terms-of-service/"]
 ["cdn.vectorstock.com", "https://www.vectorstock.com/faq/members/terms-of-use"]
 ["img.youtube.com", "https://www.youtube.com/t/terms"]
 ["image.slidesharecdn.com", "https://support.scribd.com/hc/en-us/articles/210129326-General-Terms-of-Use"]
 ["*istockphoto.com", "https://www.istockphoto.com/en/legal/terms-of-use"]
 ["*.etsystatic.com", "https://www.etsy.com/legal/terms-of-use?ref=ftr"]
 ["*etsy.com", "https://www.etsy.com/legal/terms-of-use?ref=ftr"]
-["cdn.shoplightspeed.com", "https://www.lightspeedhq.com/legal/lightspeed-service-agreement/"]
+["*.shoplightspeed.com", "https://www.lightspeedhq.com/legal/acceptable-use-policy/"]
 ["image.jimcdn.com", "https://www.jimdo.com/info/terms-of-service/"]
 ["i.dailymail.co.uk", "https://www.dailymail.co.uk/home/article-1388146/Terms.html"]
 ["pictures.abebooks.com", "https://www.abebooks.com/docs/legal/termsandconditions.shtml?cm_sp=Ftr-_-Home-_-legal"]
 ["images-wixmp-*.wixmp.com", "https://www.wix.com/about/terms-of-use"]
 ["books.google.com", "https://books.google.com/intl/en/googlebooks/tos.html"]
 ["*.bigstockphoto.com", "https://www.bigstockphoto.com/usage.html"]
 ["ak?.ostkcdn.com", "https://help.overstock.com/help/s/article/TERMS-AND-CONDITIONS"]
@@ -83,20 +83,37 @@
 ["*.redbubble.net", "https://help.redbubble.com/hc/en-us/articles/202270929-Community-and-Content-Guidelines"]
 ["cdp.azureedge.net", "https://kenssports.com/Terms"]
 ["i.bosscdn.com", "https://www.bossgoo.com/rule/term.html"]
 ["lid.zoocdn.com", "https://www.zoopla.co.uk/terms/"]
 ["www.cowcow.com", "https://www.cowcow.com/useragreement.html"]
 ["i.oodleimg.com", "https://www.oodle.com/info/terms/"]
 ["cdn?.volusion.com", "https://volusion.com/terms-of-service/"]
-["thumbs.slideserve.com", "https://www.slideserve.com/terms"]
+["*.slideserve.com", "https://www.slideserve.com/terms"]
 ["*.akamaihd.net", "https://authorize.kobo.com/terms/termsofuse"]
 ["s.ecrater.com", "https://www.ecrater.com/terms.php"]
 ["*deviantart.*", "https://www.deviantart.com/about/policy/service"]
-["image.slideserve.com", "https://www.slideserve.com/terms"]
-["img.evbuc.com", "https://www.eventbrite.com/help/en-us/articles/251210/eventbrite-terms-of-service/"]
+["*.evbuc.com", "https://www.eventbrite.com/help/en-us/articles/251210/eventbrite-terms-of-service/"]
 ["*.hdnux.com", "https://www.hearst.com/-/hearst-com-terms-of-use"]
 ["*.vectorstock.com", "https://vectorstock.com/faq/members/terms-of-use"]
 ["*.wikia.*", "https://www.fandom.com/terms-of-use"]
 ["cdn-*.threadless.com", "https://www.threadless.com/info/terms"]
 ["cdn*.bigcommerce.com", "https://www.bigcommerce.com/terms/acceptable-use-policy/"]
 ["*.tradesy.com", "https://faq.vestiairecollective.com/hc/en-us/articles/8996751206929-Website-Terms-of-Use"]
-["*.static.flickr.com", "https://flickr.com/help/terms"]
+["*.static.flickr.com", "https://flickr.com/help/terms"]
+["*.rediff.com", "https://imshopping.rediff.com/shopping/shpterms.htm"]
+["images?.bonhams.com", "https://www.bonhams.com/legals/9944/"]
+["*reviewjournal.com", "https://www.reviewjournal.com/terms-of-service/"]
+["*itv.com", "https://www.itv.com/terms/articles/itvxtermsofuse"]
+["*.scene7.com", "https://www.adobe.com/legal/terms.html"]
+["*.ftcdn.net", "https://www.fastly.com/acceptable-use/"]
+["*.zstat.net", "https://www.zalando.de/zalando-agb/"]
+["*.bonanzastatic.com", "https://www.bonanza.com/site_help/user_agreement"]
+["*.gr-assets.com", "https://www.goodreads.com/about/terms"]
+["*.macyassets.com", "https://customerservice-macys.com/articles/legal-notice"]
+["*flickr.com", "https://flickr.com/help/terms"]
+["*.sndcdn.com", "https://soundcloud.com/terms-of-use"]
+["*.motor1.com", "https://www.motorsport.com/info/terms-of-use/"]
+["*.motorsport.com", "https://www.motorsport.com/info/terms-of-use/"]
+["*immo.vlan.be", "https://immo.vlan.be/en/general-conditions"]
+["*mixcloud.com", "https://www.mixcloud.com/terms/"]
+["*homify.com", "https://www.homify.com/terms_for_users"]
+["*mzstatic.com", "https://www.apple.com/legal/internet-services/terms/site.html"]
```

### Comparing `weboptout-0.2.2/pyproject.toml` & `weboptout-0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "weboptout"
 description = "Checks the Copyright information of online works and their conditions of use."
-version = "0.2.2"
+version = "0.3"
 authors = ["Alex J. Champandard <445208+alexjc@users.noreply.github.com>"]
 repository = "https://github.com/alexjc/weboptout"
 license = "MIT and UNLICENSED"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
 ]
@@ -17,15 +17,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 aiohttp = ">=3.8"
 langdetect = ">=1.0.9"
 beautifulsoup4 = ">=4.12"
-selenium = { version = "0.2.2", optional = true }
+selenium = { version = "0.3", optional = true }
 
 [tool.poetry.extras]
 webdriver = ["selenium"]
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.0.0"
 hypothesis = ">=6.0.0"
```

### Comparing `weboptout-0.2.2/src/weboptout/config.py` & `weboptout-0.3/src/weboptout/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     ]
 ]
 
 # Parts of words that indicate non-commercial or personal use only.
 RE_NFP_CONCEPTS = [
     re.compile(p, re.I) for p in [
         "(non-commercial|non commercial) (use|purpose)",
+        "(any )?commercial use [\w\s]+is (strictly )?(prohibited|forbidden)",
         "not\s*(meant|intended)?\s*for commercial (use|usage)",
         "not-for-profit",
         "(personal|private) (use|purpose)",
     ]
 ]
 
 # Bag-of-words that represent legal concepts to detect legal documents.
```

### Comparing `weboptout-0.2.2/src/weboptout/html.py` & `weboptout-0.3/src/weboptout/html.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 ## Copyright © 2023, Alex J. Champandard.  Licensed under MIT; see LICENSE! ⚘
 
 import re
+import warnings
 import langdetect
 from bs4 import BeautifulSoup
 
 from .types import Status
 from .config import RE_TDM_CONCEPTS, RE_LEGAL_WORDS, RE_NFP_CONCEPTS
+from .steps import Steps as S
 
 
 __all__ = ["check_tos_reservation"]
 
 
 def _find_matching_paragraphs(patterns: list, text: str) -> list[tuple]:
     """
@@ -34,83 +36,80 @@
             reasons.append((rank, explain, line))
             break
 
     return sorted(reasons, key=lambda x: x[0] * 1000 - len(x[1]))
 
 
 def check_tos_reservation(client, url: str, html: str) -> Status:
-    soup = BeautifulSoup(html, "html.parser")
-    text = "\n".join(_extract_paragraphs(soup))
+    with warnings.catch_warnings(record=True) as w:
+        soup = BeautifulSoup(html, "html.parser")
 
-    para_count = text.count("\n") + 1
+    with client.setup_log() as report:
+        report(S.ParsePage, fail=len(w) > 0, url=url, **{'html': html, 'warnings': w} if len(w) > 0 else {})
 
-    # Only english language is currently supported.
-    if len(text) > 1_000 and (lang := langdetect.detect(text)) != "en":
-        client.log(
-            Status.FAILURE,
-            f"Found a possible ToS page but language is '{lang.upper()}' at {url}",
-        )
-        return Status.ABORT
+        text = "\n".join(_extract_paragraphs(soup))
 
-    # Words that match data-mining concepts.
-    if len(reasons := _find_matching_paragraphs(RE_TDM_CONCEPTS, text)):
-        client.log(
-            Status.SUCCESS,
-            f"Found a total of {len(reasons)} matching paragraphs out of "
-            f"{para_count} in Terms Of Service.",
-            highlight=reasons[0][1],
-            paragraph=reasons[0][2],
+        report(S.ExtractText, fail=len(text) < 500, bytes=len(text), paragraphs=text.count("\n")+1)
+
+        # Only English language is currently supported.
+        lang = langdetect.detect(text)
+        report(S.ValidateTextLanguage, fail=bool(lang != "en"), lang=lang)
+        assert lang == 'en'
+
+        # Words that match data-mining concepts.
+        reasons = _find_matching_paragraphs(RE_TDM_CONCEPTS, text)
+        if len(reasons) > 0:
+            client._output.append((1234, reasons[0][1], reasons[0][2]))
+
+        report(
+            S.ExtractParagraphs,
+            succeed=len(reasons) > 0,
+            type="Text- and Data-Mining",
+            paragraphs=len(reasons),
         )
-        return Status.SUCCESS
 
-    # Words that match not-for-profit reservations.
-    if len(reasons := _find_matching_paragraphs(RE_NFP_CONCEPTS, text)):
-        client.log(
-            Status.SUCCESS,
-            f"Found total of {len(reasons)} paragraphs matching "
-            f"non-commercial activities in Terms Of Service.",
-            highlight=reasons[0][1],
+        # Words that match not-for-profit reservations.
+        reasons = _find_matching_paragraphs(RE_NFP_CONCEPTS, text)
+        if len(reasons) > 0:
+            client._output.append((5678, reasons[0][1], reasons[0][2]))
+
+        report(
+            S.ExtractParagraphs,
+            succeed=len(reasons) > 0,
+            type="Not-For-Profit",
+            paragraphs=len(reasons),
         )
-        return Status.SUCCESS
 
-    if (size := len(text)) < 2_000:
-        client.log(
-            Status.FAILURE,
-            f"Too little information extracted, only {size:,} bytes from "
-            f"the ToS page at {url}",
-        )
+        report(S.ExtractText, fail=len(text) < 2_000)
 
-        # Suggest fetching page again via HTTP with Selenium.
-        return Status.RETRY
+        legal_words = RE_LEGAL_WORDS.findall(text)
+        report(S.ValidateLegalText, fail=len(legal_words) < 36)
 
-    if len(RE_LEGAL_WORDS.findall(text)) < 36:
-        client.log(
-            Status.FAILURE,
-            f"The ToS page does not appear to contain a legal text at {url}",
-        )
-        return Status.FAILURE
+    if tuple(client._steps[-1][0:2]) == (Status.FAILURE, S.ValidateTextLanguage):
+        return Status.ABORT
+
+    if tuple(client._steps[-1][0:2]) == (Status.FAILURE, S.ExtractText):
+        return Status.RETRY
 
-    client.log(
-        Status.FAILURE,
-        f"No direct matches found in {para_count} paragraphs found at {url}",
-    )
-    return Status.ABORT
+    assert len(client._steps) > 0
+    assert report.status is not None
+    return report.status
 
 
 def _extract_paragraphs(soup):
     """
     Iterator that returns a cleaned up list of paragraphs, lists items, from
     (ideally) the main body of HTML that are most likely to be legal text.
     """
     re_cleanup = re.compile("(\s+|\n|\t)")
 
     for para in soup.find_all(["p", "li", "ol", "ul", "span"]):
         if para.find_parent("a") or para.find_parent(["header", "footer"]):
             continue
-        if para.name == "span" and para.find_parent('p'):
+        if para.name == "span" and para.find_parent("p"):
             continue
         if para.name in ("ol", "ul") and len(para.find_all()) > 0:
             continue
 
         children = [
             p for p in para.contents
             if not isinstance(p, str) or p.strip("\t\n\r ") != ""
```

### Comparing `weboptout-0.2.2/src/weboptout/http.py` & `weboptout-0.3/src/weboptout/http.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,85 +1,73 @@
 ## Copyright © 2023, Alex J. Champandard.  Licensed under MIT; see LICENSE! ⚘
 
 import asyncio
 import aiohttp
+import warnings
 import itertools
 from dataclasses import dataclass
 from urllib.parse import urljoin
 
 from bs4 import BeautifulSoup
 
-from .types import Status
 from .config import RE_HREF_TOS, RE_TEXT_TOS
 from .utils import cache_to_directory, retrieve_from_database, limit_concurrency
 from .client import instantiate_webdriver
+from .steps import Steps as S
 
 
 __all__ = ["search_tos_for_domain"]
 
 
 def _log_cache_hit(client, url, /, filename, result):
-    if result[-1] != "":
-        client.log(Status.SUCCESS, f"Loaded data request for {url} from {filename}")
-    else:
-        client.log(Status.FAILURE, f"Loaded failed request for {url} from {filename}")
+    with client.setup_log() as report:
+        report(S.RetrieveContent, succeed=bool(result[-1] not in ("", None)), cache=filename, url=url)
 
 
 @cache_to_directory("cache/www", key="url", filter=_log_cache_hit)
 async def _fetch_from_cache_or_network(client, url: str) -> tuple:
     try:
         async with client.get(url) as response:
-            if response.headers.get("Content-Type", "").startswith("image/"):
-                client.log(
-                    Status.FAILURE,
-                    f"Response contains binary content where text/* was expected "
-                    f"from {url}",
-                    headers=dict(response.headers),
-                )
-                return str(response.url), dict(response.headers), ""
+            # Add dict(response.headers) to context
+            # Add response.url to context.
 
-            if "application/xml" in response.headers.get("Content-Type", ""):
-                client.log(
-                    Status.FAILURE,
-                    f"Response contains XML content where text/* was expected "
-                    f"from {url}",
-                    headers=dict(response.headers),
-                )
-                return str(response.url), dict(response.headers), ""
+            html = ""
 
-            if response.status != 200:
-                client.log(
-                    Status.FAILURE,
-                    f"An HTTP error code {response.status} was returned from {url}; "
-                    f"trying to proceed anyway...",
-                    headers=dict(response.headers),
-                )
+            with client.setup_log() as report:
+                report(S.ResolveDomain, success=True, domain=response.url.host)
+                report(S.EstablishConnection, success=True, address=response.connection.transport.get_extra_info('peername') if response.connection else '')
 
-            html = await response.text()
-            if response.status == 200:
-                client.log(
-                    Status.SUCCESS,
-                    f"The HTTP request (code {response.status}) from {url} "
-                    f"returned {len(html):,} bytes.",
-                    headers=dict(response.headers),
+                report(S.RetrieveContent, success=bool(response.status == 200), status_code=response.status, url=url)
+
+                report(
+                    S.ValidateContentFormat,
+                    content_type=(content_type := response.headers.get("Content-Type", "")),
+                    fail=any(t in content_type for t in ("application/", "image/")),
                 )
+
+                try:
+                    html = await response.text()
+                except UnicodeDecodeError as exc:
+                    report(S.ValidateContentEncoding, fail=True, exception=str(exc))
+
+                report(S.ValidateContentLength, fail=len(html) == 0, bytes=len(html))
+
             return str(response.url), dict(response.headers), html
 
     except asyncio.exceptions.TimeoutError as exc:
-        client.log(
-            Status.FAILURE,
-            f"Timeout from HTTP client while resolving {url} server(s).",
-            exception=exc,
-        )
+        with client.setup_log() as report:
+            report(S.ResolveDomain, fail=True, exception=str(exc))
+
     except aiohttp.ClientError as exc:
-        client.log(
-            Status.FAILURE,
-            f"Problem with HTTP client while connecting to {url} server(s).",
-            exception=exc,
-        )
+        with client.setup_log() as report:
+            report(S.EstablishConnection, fail=True, exception=str(exc))
+
+    except AssertionError as exc:
+        with client.setup_log() as report:
+            report(S.EstablishConnection, fail=True, exception=str(exc))
 
     return url, {}, None
 
 
 @retrieve_from_database("data/tos.jsonl", key="url")
 async def _find_tos_links_from_url(client, url: str) -> list[str]:
     url, _, html = await _fetch_from_cache_or_network(client, url)
@@ -90,110 +78,112 @@
     if html == "":
         return url, None
 
     return await _find_tos_links_from_html(client, url, html)
 
 
 async def _find_tos_links_from_html(client, url, html: str) -> list[str]:
-    soup = BeautifulSoup(html, "html.parser")
+    with warnings.catch_warnings(record=True) as w:
+        soup = BeautifulSoup(html, "html.parser")
+    
+    with client.setup_log() as report:
+        links = []
+        report(S.ParsePage, fail=len(w) > 0, url=url, **{'html': html, 'warnings': w} if len(w) > 0 else {})
 
-    all_links = [
-        l
-        for l in soup.find_all("a")
-        if l.get("href") is not None
-        and not (href := l.get("href")).lower().startswith("javascript:")
-        and not any(href.startswith(k) for k in "#?")
-        and not (l.get_text().lower in ["refresh", "reload"])
-    ]
-    if len(all_links) == 0 or any(
-        k in html for k in ("turn on javascript", "enable-javascript.com")
-    ):
-        client.log(
-            Status.FAILURE, f"JavaScript must be enabled to view content from {url}"
-        )
-        return url, []
+        all_links = [
+            l
+            for l in soup.find_all("a")
+            if l.get("href") is not None
+            and not (href := l.get("href")).lower().startswith("javascript:")
+            and not any(href.startswith(k) for k in "#?")
+            and not (l.get_text().lower in ["refresh", "reload"])
+        ]
+
+        report(S.ValidatePageLinks,
+               fail=bool(len(all_links) == 0),
+               filtered_count=len(all_links),
+               original_count=len(soup.find_all("a")),
+        )
+
+        match_links, match_texts = [], []
+        for link in all_links:
+            if RE_HREF_TOS.search(str(link.get("href"))):
+                match_links.append(link)
+            if RE_TEXT_TOS.search(str(link.get_text()).strip()):
+                match_texts.append(link)
+
+        match_texts = sorted(match_texts, key=lambda l: len(l.get_text()))
+        match_links = sorted(match_links, key=lambda l: len(l.get("href")))
+
+        report(
+            S.FindSomeLinksToTerms,
+            fail=not match_links and not match_texts
+        )
+
+        links = [
+            urljoin(url, link.get("href"))
+            for link in sorted(
+                set(match_texts) & set(match_links),
+                key=lambda l: len(l.get("href"))
+            )
+        ]
 
-    match_links, match_texts = [], []
-    for link in all_links:
-        if RE_HREF_TOS.search(str(link.get("href"))):
-            match_links.append(link)
-        if RE_TEXT_TOS.search(str(link.get_text()).strip()):
-            match_texts.append(link)
-
-    match_texts = sorted(match_texts, key=lambda l: len(l.get_text()))
-    match_links = sorted(match_links, key=lambda l: len(l.get("href")))
-
-    if not match_links and not match_texts:
-        client.log(
-            Status.FAILURE,
-            f"No matching links found from {len(all_links)} in ToS at {url}",
+        report(
+            S.FindGoodLinksToTerms,
+            succeed=len(links) > 0
         )
-        return url, []
 
-    match_both = set(match_texts) & set(match_links)
-    if len(match_both) > 0:
-        client.log(
-            Status.SUCCESS,
-            f"Found {len(match_both)} obvious ToS link(s) "
-            f"from {len(match_links)} href matches and {len(match_texts)} "
-            f"text matches.",
-        )
-        match_both = sorted(list(match_both), key=lambda l: len(l.get("href")))
-        return url, list(urljoin(url, link.get("href")) for link in match_both)
+        def valid_link(url):
+            return not any(k in url for k in ["login", "privacy", "signup", "user/", "users/", "tags/", "categories/"])
 
-    client.log(
-        Status.SUCCESS,
-        f"Found {len(set(match_links)|set(match_texts))} ToS candidate links "
-        f"including {len(match_links)} href matches and {len(match_texts)} "
-        f"text matches.",
-    )
-
-    return url, [
-        urljoin(url, l.get("href"))
-        for p in itertools.zip_longest(match_links, match_texts)
-        for l in p
-        if l is not None
-    ]
+        links = [
+            urljoin(url, l.get("href"))
+            for p in itertools.zip_longest(match_links, match_texts)
+            for l in p
+            if (l is not None and valid_link(l.get("href")))
+        ]
 
+    return url, links
 
 
 def _reject_if_header_missing(url, headers, /, filename, result):
     return "User-Agent" not in headers
     
 
 @cache_to_directory("cache/www", key="url", filter=_reject_if_header_missing)
 @limit_concurrency(value=1)
 async def _fetch_from_browser_then_cache_result(url, headers):
     try:
         webdriver = instantiate_webdriver()
-        webdriver.get(url)
+        await webdriver.open_tab(url)
     except Exception as exc: # selenium.common.exceptions.TimeoutException
+        await webdriver.close_tab()
         if "Message: Navigation timed out after" not in str(exc):
             raise
         return url, headers, ""
 
-    def page_is_loading():            
-        x = webdriver.execute_script("return document.readyState")
-        return x == "complete"
-
-    while not page_is_loading():
-        await asyncio.sleep(0.01)
-    await asyncio.sleep(1.0)
+    for i in range(100):
+        if not (await webdriver.is_page_loading(url)):
+            break
+        await asyncio.sleep(0.05)
+    await asyncio.sleep(2.0)
 
-    html = webdriver.execute_script("return document.documentElement.outerHTML")
+    html = await webdriver.get_page_html()
     headers["User-Agent"] = "WebOptOut/Firefox"
+    await webdriver.close_tab()
+
     return url, headers, html
 
 
 @dataclass
 class RequestOptions:
     retry: bool = False
 
 
-async def search_tos_for_domain(client, domain: str) -> str:
+async def search_tos_for_domain(client, domain: str, attempts: int = 4) -> str:
     assert not any(domain.startswith(k) for k in ("https://", "http://"))
 
     # Step 1) find the right domain from the domain.
     while domain.count(".") > 0:
         links = []
         url, links = await _find_tos_links_from_url(client, "https://" + domain)
 
@@ -208,35 +198,26 @@
         return
 
     # Content received but no links.
     if len(links) == 0:
         yield url, "", {}
         return
 
-    # Step 2) find the right page on that domain.
+    # Step 2) find the right page on that domain, maximum four tries.
     visited = set()
-    while len(links) > 0:
+    while len(links) > 0 and len(visited) < attempts:
         url = links.pop(0)
         visited.add(url)
 
         new_url, headers, html = await _fetch_from_cache_or_network(client, url)
         if html is None:
             continue
 
-        client.log(
-            Status.SUCCESS,
-            f"Retrieved Terms Of Service for {url} with {len(html):,} bytes of text.",
-        )
-
         options = RequestOptions()
         yield new_url, html, options
 
         if options.retry:
             url, headers, html = await _fetch_from_browser_then_cache_result(url, headers)
-            client.log(
-                Status.SUCCESS,
-                f"Browsed for Terms Of Service again with Selenium and got {len(html):,} bytes of text.",
-            )
             yield url, html, options
 
         url, further_links = await _find_tos_links_from_html(client, url, html)
         links.extend(l for l in further_links if l not in links and l not in visited)
```

### Comparing `weboptout-0.2.2/src/weboptout/types.py` & `weboptout-0.3/src/weboptout/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,28 +22,29 @@
     including a domain, a URL, a file.
 
     This class is intended to be used via the `rsv` namespace, along with the
     defaults YES, MAYBE, NO.  These can be cloned via the __call__ function to
     create Reservations derived from that default.
     """
 
-    def __init__(self, id: int, summary: str = None, url: str = None, records: list = None):
+    def __init__(self, id: int, url: str = None, process: list = None, outcome: list = None):
         self._id = id
-        self.summary = summary
+
         self.url = url
-        self.records = records or []
+        self.process = process or []
+        self.outcome = outcome or []
 
     def __eq__(self, id: int):
         return self._id == id
 
     def __repr__(self):
-        return f'<weboptout.Reservation id={self._id} url="{self.url}" summary="{self.summary}">'
+        return f'<weboptout.Reservation id={self._id}>'
 
-    def __call__(self, /, summary: str, url: str = None, records: list = None):
-        return Reservation(self._id, summary, url, records)
+    def __call__(self, /, url: str, process: list = None, outcome: list = None):
+        return Reservation(self._id, url, process, outcome)
 
 
 class rsv:
     """
     Namespace with default Reservations that can be cloned and used for comparison.
     """
```

### Comparing `weboptout-0.2.2/src/weboptout/utils.py` & `weboptout-0.3/src/weboptout/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,21 @@
     return _wrapper
 
 
 def limit_concurrency(value: int):
     """
     Decorator to prevent an async function from being called more than N times.
     """
-    semaphore = asyncio.Semaphore(value)
-    def _decorator(fn):
+    def _decorator(fn, __semaphore__: list = []):
         async def _wrapper(*args, **kwargs):
-            async with semaphore:
+            if len(__semaphore__) == 0:
+                loop = asyncio._get_running_loop()
+                __semaphore__.append(asyncio.Semaphore(value, loop=loop))
+
+            async with __semaphore__[0]:
                 return await fn(*args, **kwargs)
         _wrapper.__wrapped__ = fn
         return _wrapper
     return _decorator
 
 
 def cache_to_directory(directory, /, key: str, filter: callable = None):
@@ -170,15 +173,15 @@
 def retrieve_result_from_cache(archive, /, key: str, filter: callable = None):
     archive = pkg_resources.resource_filename(__name__, archive)
     archive = archive.replace('src/weboptout/', '')
     os.makedirs(os.path.dirname(archive), exist_ok=True)
 
     if os.path.isfile(archive):
         lookup = {
-            k: Reservation(v[0], v[1], v[2])
+            k: Reservation(v[0], v[1], v[2], v[3])
             for k, v in pickle.load(open(archive, 'rb')).items()
         }
     else:
         lookup = {}
 
     def _add_to_database(key, r):
         if r.url is None:
@@ -196,15 +199,15 @@
             lookup[pat] = r
             del lookup[match[0]]
         else:
             lookup[key] = r
 
     def _dump_to_disk():
         pickle.dump(
-            {k: (v._id, v.summary, v.url) for k, v in lookup.items()},
+            {k: (v._id, v.url, v.process, v.outcome) for k, v in lookup.items()},
             open(archive, 'wb')
         )
     atexit.register(_dump_to_disk)
 
     def _decorator(fn):
         arg_names = list(inspect.signature(fn).parameters.keys())
         arg_idx = arg_names.index(key)
```

### Comparing `weboptout-0.2.2/src/weboptout/web.py` & `weboptout-0.3/src/weboptout/web.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,40 +7,36 @@
 from .html import check_tos_reservation
 
 
 __all__ = ["check_domain_reservation"]
 
 
 @allow_sync_calls
-@retrieve_result_from_cache("cache/rsv.pkl", key="domain")
+# @retrieve_result_from_cache("cache/rsv.pkl", key="domain")
 async def check_domain_reservation(domain: str) -> Reservation:
     assert not any(domain.startswith(k) for k in ("https://", "http://"))
 
     async with ClientSession() as client:
         async for url, tos, options in search_tos_for_domain(client, domain):
             # No TOS found but at least the server worked.
             if tos == "":
-                return rsv.MAYBE(summary=None, url=url, records=client.log_records)
+                return rsv.MAYBE(url=url, process=client._steps, outcome=client._output)
 
             status = check_tos_reservation(client, url, tos)
 
             # Need to fetch the content again with webdriver?
             if status == Status.RETRY:
                 options.retry = True
                 continue
 
             # Wrong place or wrong language from website...
             if status == Status.ABORT:
-                return rsv.MAYBE(summary=None, url=url, records=client.log_records)
+                return rsv.MAYBE(url=url, process=client._steps, outcome=client._output)
 
             # Not enough text or not enough legal content.
             if status == Status.FAILURE:
                 continue
 
-            return rsv.YES(
-                summary=client.log_records[-1][2]["highlight"],
-                url=url,
-                records=client.log_records,
-            )
+            return rsv.YES(url=url, process=client._steps, outcome=client._output)
 
     # This happens when none of the domains can be looked up.
-    return rsv.ERROR(summary=None, records=client.log_records)
+    return rsv.ERROR(url=None, process=client._steps, outcome=client._output)
```

### Comparing `weboptout-0.2.2/PKG-INFO` & `weboptout-0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weboptout
-Version: 0.2.2
+Version: 0.3
 Summary: Checks the Copyright information of online works and their conditions of use.
 Home-page: https://github.com/alexjc/weboptout
 License: MIT and UNLICENSED
 Author: Alex J. Champandard
 Author-email: 445208+alexjc@users.noreply.github.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,9 +14,9 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Provides-Extra: webdriver
 Requires-Dist: aiohttp (>=3.8)
 Requires-Dist: beautifulsoup4 (>=4.12)
 Requires-Dist: langdetect (>=1.0.9)
-Requires-Dist: selenium (==0.2.2) ; extra == "webdriver"
+Requires-Dist: selenium (==0.3) ; extra == "webdriver"
 Project-URL: Repository, https://github.com/alexjc/weboptout
```

