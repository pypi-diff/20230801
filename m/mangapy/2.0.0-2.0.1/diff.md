# Comparing `tmp/mangapy-2.0.0.tar.gz` & `tmp/mangapy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mangapy-2.0.0.tar", last modified: Mon Jul 31 16:01:02 2023, max compression
+gzip compressed data, was "mangapy-2.0.1.tar", last modified: Tue Aug  1 19:23:11 2023, max compression
```

## Comparing `mangapy-2.0.0.tar` & `mangapy-2.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-07-31 16:01:02.354396 mangapy-2.0.0/
--rw-r--r--   0 alessandro   (501) staff       (20)     1067 2019-12-11 18:08:50.000000 mangapy-2.0.0/LICENSE
--rw-r--r--   0 alessandro   (501) staff       (20)     2603 2023-07-31 16:01:02.354077 mangapy-2.0.0/PKG-INFO
--rw-r--r--   0 alessandro   (501) staff       (20)     1946 2023-07-31 15:59:06.000000 mangapy-2.0.0/README.md
-drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-07-31 16:01:02.350561 mangapy-2.0.0/mangapy/
--rw-r--r--   0 alessandro   (501) staff       (20)       51 2020-03-13 14:35:31.000000 mangapy-2.0.0/mangapy/__init__.py
--rw-r--r--   0 alessandro   (501) staff       (20)     4524 2023-07-31 15:59:06.000000 mangapy-2.0.0/mangapy/chapter_archiver.py
--rw-r--r--   0 alessandro   (501) staff       (20)     9061 2023-07-31 15:59:06.000000 mangapy-2.0.0/mangapy/cli.py
--rw-r--r--   0 alessandro   (501) staff       (20)     6714 2023-07-31 15:59:06.000000 mangapy-2.0.0/mangapy/fanfox.py
--rw-r--r--   0 alessandro   (501) staff       (20)      994 2023-07-31 15:59:06.000000 mangapy-2.0.0/mangapy/mangarepository.py
-drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-07-31 16:01:02.353131 mangapy-2.0.0/mangapy.egg-info/
--rw-r--r--   0 alessandro   (501) staff       (20)     2603 2023-07-31 16:01:02.000000 mangapy-2.0.0/mangapy.egg-info/PKG-INFO
--rw-r--r--   0 alessandro   (501) staff       (20)      358 2023-07-31 16:01:02.000000 mangapy-2.0.0/mangapy.egg-info/SOURCES.txt
--rw-r--r--   0 alessandro   (501) staff       (20)        1 2023-07-31 16:01:02.000000 mangapy-2.0.0/mangapy.egg-info/dependency_links.txt
--rw-r--r--   0 alessandro   (501) staff       (20)       45 2023-07-31 16:01:02.000000 mangapy-2.0.0/mangapy.egg-info/entry_points.txt
--rw-r--r--   0 alessandro   (501) staff       (20)       32 2023-07-31 16:01:02.000000 mangapy-2.0.0/mangapy.egg-info/requires.txt
--rw-r--r--   0 alessandro   (501) staff       (20)        8 2023-07-31 16:01:02.000000 mangapy-2.0.0/mangapy.egg-info/top_level.txt
--rw-r--r--   0 alessandro   (501) staff       (20)      100 2021-03-23 11:11:45.000000 mangapy-2.0.0/pyproject.toml
--rw-r--r--   0 alessandro   (501) staff       (20)       38 2023-07-31 16:01:02.354493 mangapy-2.0.0/setup.cfg
--rw-r--r--   0 alessandro   (501) staff       (20)     1109 2023-07-31 15:59:06.000000 mangapy-2.0.0/setup.py
-drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-07-31 16:01:02.353553 mangapy-2.0.0/tests/
--rw-r--r--   0 alessandro   (501) staff       (20)     2282 2020-07-31 15:33:31.000000 mangapy-2.0.0/tests/test_fanfox.py
+drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-08-01 19:23:11.892252 mangapy-2.0.1/
+-rw-r--r--   0 alessandro   (501) staff       (20)     1067 2019-12-11 18:08:50.000000 mangapy-2.0.1/LICENSE
+-rw-r--r--   0 alessandro   (501) staff       (20)     2603 2023-08-01 19:23:11.891668 mangapy-2.0.1/PKG-INFO
+-rw-r--r--   0 alessandro   (501) staff       (20)     1946 2023-07-31 15:59:06.000000 mangapy-2.0.1/README.md
+drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-08-01 19:23:11.887820 mangapy-2.0.1/mangapy/
+-rw-r--r--   0 alessandro   (501) staff       (20)       51 2020-03-13 14:35:31.000000 mangapy-2.0.1/mangapy/__init__.py
+-rw-r--r--   0 alessandro   (501) staff       (20)     4524 2023-07-31 15:59:06.000000 mangapy-2.0.1/mangapy/chapter_archiver.py
+-rw-r--r--   0 alessandro   (501) staff       (20)     9061 2023-07-31 15:59:06.000000 mangapy-2.0.1/mangapy/cli.py
+-rw-r--r--   0 alessandro   (501) staff       (20)     7412 2023-08-01 12:42:26.000000 mangapy-2.0.1/mangapy/fanfox.py
+-rw-r--r--   0 alessandro   (501) staff       (20)      994 2023-07-31 15:59:06.000000 mangapy-2.0.1/mangapy/mangarepository.py
+drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-08-01 19:23:11.890642 mangapy-2.0.1/mangapy.egg-info/
+-rw-r--r--   0 alessandro   (501) staff       (20)     2603 2023-08-01 19:23:11.000000 mangapy-2.0.1/mangapy.egg-info/PKG-INFO
+-rw-r--r--   0 alessandro   (501) staff       (20)      358 2023-08-01 19:23:11.000000 mangapy-2.0.1/mangapy.egg-info/SOURCES.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)        1 2023-08-01 19:23:11.000000 mangapy-2.0.1/mangapy.egg-info/dependency_links.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)       45 2023-08-01 19:23:11.000000 mangapy-2.0.1/mangapy.egg-info/entry_points.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)       32 2023-08-01 19:23:11.000000 mangapy-2.0.1/mangapy.egg-info/requires.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)        8 2023-08-01 19:23:11.000000 mangapy-2.0.1/mangapy.egg-info/top_level.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)      100 2021-03-23 11:11:45.000000 mangapy-2.0.1/pyproject.toml
+-rw-r--r--   0 alessandro   (501) staff       (20)       38 2023-08-01 19:23:11.892384 mangapy-2.0.1/setup.cfg
+-rw-r--r--   0 alessandro   (501) staff       (20)     1109 2023-08-01 13:03:22.000000 mangapy-2.0.1/setup.py
+drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-08-01 19:23:11.891037 mangapy-2.0.1/tests/
+-rw-r--r--   0 alessandro   (501) staff       (20)     2962 2023-08-01 13:03:12.000000 mangapy-2.0.1/tests/test_fanfox.py
```

### Comparing `mangapy-2.0.0/LICENSE` & `mangapy-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mangapy-2.0.0/PKG-INFO` & `mangapy-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangapy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Manga downloader
 Home-page: https://github.com/alemar11/mangapy
 Author: Alessandro Marzoli
 Author-email: me@alessandromarzoli.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mangapy-2.0.0/README.md` & `mangapy-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mangapy-2.0.0/mangapy/chapter_archiver.py` & `mangapy-2.0.1/mangapy/chapter_archiver.py`

 * *Files identical despite different names*

### Comparing `mangapy-2.0.0/mangapy/cli.py` & `mangapy-2.0.1/mangapy/cli.py`

 * *Files identical despite different names*

### Comparing `mangapy-2.0.0/mangapy/fanfox.py` & `mangapy-2.0.1/mangapy/fanfox.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from mangapy import log
 from mangapy.mangarepository import MangaRepository, Manga, Chapter, Page
 from bs4 import BeautifulSoup
 from typing import List
 
 
 def unpack(p, a, c, k, e=None, d=None):
-    def baseN(num, b, numerals="0123456789abcdefghijklmnopqrstuvwxyz"):
+    def baseN(num, b, numerals="0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"):
         return ((num == 0) and numerals[0]) or (baseN(num // b, b, numerals).lstrip(numerals[0]) + numerals[num % b])
 
     while (c):
         c -= 1
         if (k[c]):
             p = re.sub("\\b" + baseN(c, a) + "\\b",  k[c], p)
     return p
@@ -158,29 +158,39 @@
         if response is None or response.status_code != 200:
             return None
 
         content = response.text
         soup = BeautifulSoup(content, features="html.parser")
         page_numbers = soup.findAll("a", {"data-page": True})
 
-        if not len(page_numbers):
-            return []
-
-        page_numbers = map(lambda x: int(x['data-page']), page_numbers)
-
-        last_page_number = max(page_numbers)
-
         links = []
-        for i in range(0, int(last_page_number / 2 + .5)):
-            data = self._one_link_helper(content, (i * 2) + 1, base_url)
-            links += self._parse_links(self._get_urls(data))
-
         pages = []
-        for i, link in enumerate(links):
-            pages.append(Page(i, link))
+
+        if not len(page_numbers):
+            # sometimes all the images are loaded in the same html page
+            scripts = soup.find_all("script", {"type": "text/javascript"})
+            if not scripts:
+                return []
+            eval_script = next((script for script in scripts if script.text.startswith("eval")), None).text
+            images_content = self._get_urls(eval_script)
+            links = re.search(r'(?<=newImgs=\[)[^]]+(?=\])', images_content).group(0).split(',')
+            for i, link in enumerate(links):
+                formatted_link = link.replace("'", "")
+                pages.append(Page(i, formatted_link))
+        else:
+            # standard flow
+            page_numbers = map(lambda x: int(x['data-page']), page_numbers)
+            last_page_number = max(page_numbers)
+
+            for i in range(0, int(last_page_number / 2 + .5)):
+                data = self._one_link_helper(content, (i * 2) + 1, base_url)
+                links += self._parse_links(self._get_urls(data))
+        
+            for i, link in enumerate(links):
+                pages.append(Page(i, link))
 
         return pages
 
 
 if __name__ == '__main__':
     repo = FanFoxRepository()
     manga = repo.search('naruto')
```

### Comparing `mangapy-2.0.0/mangapy/mangarepository.py` & `mangapy-2.0.1/mangapy/mangarepository.py`

 * *Files identical despite different names*

### Comparing `mangapy-2.0.0/mangapy.egg-info/PKG-INFO` & `mangapy-2.0.1/mangapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangapy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Manga downloader
 Home-page: https://github.com/alemar11/mangapy
 Author: Alessandro Marzoli
 Author-email: me@alessandromarzoli.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mangapy-2.0.0/setup.py` & `mangapy-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup(
     author="Alessandro Marzoli",
     author_email="me@alessandromarzoli.com",
     name='mangapy',
     license="MIT",
     description='Manga downloader',
-    version='2.0.0',
+    version='2.0.1',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/alemar11/mangapy',
     packages=find_packages(),
     python_requires=">=3.11",
     install_requires=['bs4', 'pillow', 'pyyaml', 'requests', 'tqdm'],
     classifiers=[
```

### Comparing `mangapy-2.0.0/tests/test_fanfox.py` & `mangapy-2.0.1/tests/test_fanfox.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,31 @@
 
 def test_fetch_not_existing_manga():
     repository = FanFoxRepository()
     manga = repository.search('this manga doesn\'t exists')
     assert manga is None
 
 
+def test_fetch_manga_chapter_where_all_the_images_are_in_the_same_page():
+    repository = FanFoxRepository()
+    manga = repository.search('ahiru no sora')
+    assert manga is not None
+    assert len(manga.chapters) >= 165, "It should contain at least 165 chapters (expected more)"
+    chapter = next((chapter for chapter in manga.chapters if chapter.number == 164.0), None)
+    assert chapter is not None
+    print(chapter.number)
+    pages = chapter.pages()
+    chapter_count = 0
+    for page in pages:
+        chapter_count += 1
+        assert page.number is not None
+        assert page.url is not None
+    assert chapter_count == 18, "The chapter should contain 18 pages"
+
+
 def test_fetch_manga():
     repository = FanFoxRepository()
     manga = repository.search('kimetsu no yaiba')
     assert manga is not None
     assert len(manga.chapters) >= 209, "It should contain at least 209 chapters"
     firstChapter = manga.chapters[0]
     assert firstChapter is not None
```

