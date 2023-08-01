# Comparing `tmp/agentbrowser-0.1.4.tar.gz` & `tmp/agentbrowser-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentbrowser-0.1.4.tar", last modified: Tue Jul 18 14:02:18 2023, max compression
+gzip compressed data, was "agentbrowser-0.2.0.tar", last modified: Tue Aug  1 04:49:46 2023, max compression
```

## Comparing `agentbrowser-0.1.4.tar` & `agentbrowser-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:02:18.598078 agentbrowser-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 14:02:06.000000 agentbrowser-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-07-18 14:02:18.598078 agentbrowser-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-18 14:02:06.000000 agentbrowser-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:02:18.594078 agentbrowser-0.1.4/agentbrowser/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 14:02:06.000000 agentbrowser-0.1.4/agentbrowser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-18 14:02:06.000000 agentbrowser-0.1.4/agentbrowser/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-18 14:02:06.000000 agentbrowser-0.1.4/agentbrowser/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-18 14:02:06.000000 agentbrowser-0.1.4/agentbrowser/test_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:02:18.598078 agentbrowser-0.1.4/agentbrowser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-07-18 14:02:18.000000 agentbrowser-0.1.4/agentbrowser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-18 14:02:18.000000 agentbrowser-0.1.4/agentbrowser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:02:18.000000 agentbrowser-0.1.4/agentbrowser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 14:02:18.000000 agentbrowser-0.1.4/agentbrowser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 14:02:18.000000 agentbrowser-0.1.4/agentbrowser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:02:18.598078 agentbrowser-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-18 14:02:06.000000 agentbrowser-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:49:46.141365 agentbrowser-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-01 04:49:33.000000 agentbrowser-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-08-01 04:49:46.141365 agentbrowser-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-08-01 04:49:33.000000 agentbrowser-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:49:46.137365 agentbrowser-0.2.0/agentbrowser/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 04:49:33.000000 agentbrowser-0.2.0/agentbrowser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-08-01 04:49:33.000000 agentbrowser-0.2.0/agentbrowser/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-08-01 04:49:33.000000 agentbrowser-0.2.0/agentbrowser/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-01 04:49:33.000000 agentbrowser-0.2.0/agentbrowser/test_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:49:46.141365 agentbrowser-0.2.0/agentbrowser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-08-01 04:49:46.000000 agentbrowser-0.2.0/agentbrowser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 04:49:46.000000 agentbrowser-0.2.0/agentbrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:49:46.000000 agentbrowser-0.2.0/agentbrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 04:49:46.000000 agentbrowser-0.2.0/agentbrowser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 04:49:46.000000 agentbrowser-0.2.0/agentbrowser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 04:49:46.141365 agentbrowser-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-01 04:49:33.000000 agentbrowser-0.2.0/setup.py
```

### Comparing `agentbrowser-0.1.4/LICENSE` & `agentbrowser-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agentbrowser-0.1.4/agentbrowser/test.py` & `agentbrowser-0.2.0/agentbrowser/test_async.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,69 @@
+import asyncio
+import pytest
 from agentbrowser import (
-    create_page,
-    evaluate_javascript,
-    get_body_html,
-    get_body_text,
-    get_document_html,
-    navigate_to,
+    async_get_browser,
+    async_init_browser,
+    async_navigate_to,
+    async_get_body_html,
+    async_get_body_text,
+    async_get_document_html,
+    async_create_page,
+    async_close_page,
+    async_evaluate_javascript,
 )
-from agentbrowser.browser import get_body_text_raw
+
+from agentbrowser.browser import browser, context
 
 test_article = "https://test-page-to-crawl.vercel.app"
 
+@pytest.mark.asyncio
+async def test_async_create_page():
+    global browser
+    global context
+    browser = None
+    context = None
+    await async_init_browser()
+    test_page = await async_create_page("https://www.google.com/")
+    assert test_page is not None, "Page navigation failed."
+    assert test_page.url == "https://www.google.com/", "Navigation failed."
+    print("test_create_page passed.")
+
+    await async_close_page(test_page)
+    assert test_page.is_closed(), "Page failed to close."
+    print("test_close_page passed.")
 
-def test_navigation():
-    test_page = create_page("https://www.google.com")
+    test_page = await async_create_page("https://www.google.com")
 
     # navigate to google
-    navigate_to(
+    await async_navigate_to(
         "https://www.yahoo.com",
         test_page,
     )
 
     assert test_page.url != "https://www.google.com", "Navigation failed."
     assert test_page is not None, "Page navigation failed."
-    print("test_navigation passed.")
+    print("test_async_navigation passed.")
 
-
-def test_body_html():
-    test_page = create_page(test_article)
-    body_html = get_body_html(test_page)
+    body_html = await async_get_body_html(test_page)
     assert body_html is not None, "Failed to get body html."
-    print("test_body_html passed.")
-
+    print("test_async_body_html passed.")
 
-def test_document_html():
-    test_page = create_page(test_article)
-    html = get_document_html(test_page)
+    html = await async_get_document_html(test_page)
     assert html is not None, "Failed to get document html."
-    print("test_document_html passed.")
+    print("test_async_document_html passed.")
 
-
-def test_body_text():
-    test_page = create_page(test_article)
-    body = get_body_text(test_page)
+    body = await async_get_body_text(test_page)
     assert body is not None, "Failed to get body text."
-    print("test_body_text passed.")
-
-
-def test_body_text_raw():
-    test_page = create_page(test_article)
-    body_text_raw = get_body_text_raw(test_page)
-    assert body_text_raw is not None, "Failed to get raw body text."
-    print("test_body_text_raw passed.")
-
+    print("test_async_body_text passed.")
 
-def test_javascript_evaluation():
-    test_page = create_page(test_article)
-    result = evaluate_javascript(
+    result = await async_evaluate_javascript(
         """
         var x = 1;
         var y = 2;
         var z = x + y;
         z;
         """,
         test_page,
     )
     assert result == 3, "Javascript evaluation failed."
-    print("test_javascript_evaluation passed.")
+    print("test_async_javascript_evaluation passed.")
```

### Comparing `agentbrowser-0.1.4/agentbrowser/test_async.py` & `agentbrowser-0.2.0/agentbrowser/test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,96 @@
-import asyncio
-import pytest
 from agentbrowser import (
-    async_get_browser,
-    async_init_browser,
-    async_navigate_to,
-    async_get_body_html,
-    async_get_body_text,
-    async_get_document_html,
-    async_create_page,
-    async_close_page,
-    async_evaluate_javascript,
-    async_get_body_text_raw,
+    create_page,
+    evaluate_javascript,
+    get_body_html,
+    get_body_text,
+    get_document_html,
+    navigate_to
 )
-from agentbrowser.browser import get_body_text_raw
+from agentbrowser.browser import close_page, get_page_title, init_browser, get_browser, screenshot_page
 
 test_article = "https://test-page-to-crawl.vercel.app"
 
 
-@pytest.fixture(scope="function")
-async def browser_fixture(request):
-    # Initialize a new event loop for this test
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
+def test_get_browser():
+    browser = get_browser()
+    assert browser is not None, "Failed to get the browser"
+    print("test_get_browser passed.")
 
-    # Initialize the browser
-    await async_init_browser()
-    assert await async_get_browser() is not None, "Browser initialization failed."
 
-    async def fin():
-        # cleanup after tests
-        if await async_get_browser() is not None:
-            await (await async_get_browser()).close()
+def test_init_browser():
+    init_browser()
+    browser = get_browser()
+    assert browser is not None, "Failed to initialize the browser"
+    print("test_init_browser passed.")
 
-        loop.run_until_complete(
-            asyncio.sleep(0.250)
-        )  # gives tasks a bit of time to finish
 
-    request.addfinalizer(fin)
-
-    yield
-
-
-@pytest.mark.asyncio
-async def test_async_create_page(browser_fixture):
-    test_page = await async_create_page("https://www.google.com/")
-    assert test_page is not None, "Page navigation failed."
-    assert test_page.url == "https://www.google.com/", "Navigation failed."
-    print("test_create_page passed.")
-
-    await async_close_page(test_page)
-    assert test_page.isClosed(), "Page failed to close."
-    print("test_close_page passed.")
-
-    test_page = await async_create_page("https://www.google.com")
+def test_navigation():
+    test_page = create_page("https://www.google.com")
 
     # navigate to google
-    await async_navigate_to(
+    navigate_to(
         "https://www.yahoo.com",
         test_page,
+        wait_until="domcontentloaded",
     )
 
     assert test_page.url != "https://www.google.com", "Navigation failed."
     assert test_page is not None, "Page navigation failed."
-    print("test_async_navigation passed.")
+    print("test_navigation passed.")
+
+
+def test_get_page_title():
+    test_page = create_page("https://www.google.com")
+    title = get_page_title(test_page)
+    assert title == "Google", "Failed to get the correct page title."
+    print("test_get_page_title passed.")
 
-    body_html = await async_get_body_html(test_page)
+
+def test_screenshot_page():
+    test_page = create_page("https://www.google.com")
+    screenshot = screenshot_page(test_page)
+    assert screenshot is not None, "Failed to take a screenshot."
+    print("test_screenshot_page passed.")
+
+
+def test_close_page():
+    test_page = create_page("https://www.google.com")
+    close_page(test_page)
+    assert test_page.is_closed(), "Failed to close the page."
+    print("test_close_page passed.")
+
+
+def test_body_html():
+    test_page = create_page(test_article)
+    body_html = get_body_html(test_page)
     assert body_html is not None, "Failed to get body html."
-    print("test_async_body_html passed.")
+    print("test_body_html passed.")
 
-    html = await async_get_document_html(test_page)
+
+def test_document_html():
+    test_page = create_page(test_article)
+    html = get_document_html(test_page)
     assert html is not None, "Failed to get document html."
-    print("test_async_document_html passed.")
+    print("test_document_html passed.")
+
 
-    body = await async_get_body_text(test_page)
+def test_body_text():
+    test_page = create_page(test_article)
+    body = get_body_text(test_page)
     assert body is not None, "Failed to get body text."
-    print("test_async_body_text passed.")
+    print("test_body_text passed.")
 
-    body_text_raw = await async_get_body_text_raw(test_page)
-    assert body_text_raw is not None, "Failed to get raw body text."
-    print("test_async_body_text_raw passed.")
 
-    result = await async_evaluate_javascript(
+def test_javascript_evaluation():
+    test_page = create_page(test_article)
+    result = evaluate_javascript(
         """
         var x = 1;
         var y = 2;
         var z = x + y;
         z;
         """,
         test_page,
     )
     assert result == 3, "Javascript evaluation failed."
-    print("test_async_javascript_evaluation passed.")
+    print("test_javascript_evaluation passed.")
```

### Comparing `agentbrowser-0.1.4/setup.py` & `agentbrowser-0.2.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,24 +8,24 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="agentbrowser",
-    version="0.1.4",
-    description="A browser for your agent, built on Chrome and Pyppeteer.",
+    version="0.2.0",
+    description="A browser for your agent, built on Playwright.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/lalalune/agentbrowser",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
     packages=["agentbrowser"],
-    install_requires=["pyppeteer"],
+    install_requires=["playwright"],
     readme="README.md",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
```

