# Comparing `tmp/reddit-account-generator-1.0.0.tar.gz` & `tmp/reddit-account-generator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit-account-generator-1.0.0.tar", last modified: Wed Jul 26 16:10:10 2023, max compression
+gzip compressed data, was "reddit-account-generator-1.1.0.tar", last modified: Tue Aug  1 08:59:31 2023, max compression
```

## Comparing `reddit-account-generator-1.0.0.tar` & `reddit-account-generator-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:10:10.749937 reddit-account-generator-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-26 16:09:58.000000 reddit-account-generator-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-26 16:10:10.749937 reddit-account-generator-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-26 16:09:58.000000 reddit-account-generator-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:10:10.749937 reddit-account-generator-1.0.0/reddit_account_generator/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-26 16:09:58.000000 reddit-account-generator-1.0.0/reddit_account_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 16:09:58.000000 reddit-account-generator-1.0.0/reddit_account_generator/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-26 16:09:58.000000 reddit-account-generator-1.0.0/reddit_account_generator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-26 16:09:58.000000 reddit-account-generator-1.0.0/reddit_account_generator/maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-26 16:09:58.000000 reddit-account-generator-1.0.0/reddit_account_generator/protector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-26 16:09:58.000000 reddit-account-generator-1.0.0/reddit_account_generator/proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-26 16:09:58.000000 reddit-account-generator-1.0.0/reddit_account_generator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:10:10.749937 reddit-account-generator-1.0.0/reddit_account_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-26 16:10:10.000000 reddit-account-generator-1.0.0/reddit_account_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-26 16:10:10.000000 reddit-account-generator-1.0.0/reddit_account_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 16:10:10.000000 reddit-account-generator-1.0.0/reddit_account_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-26 16:10:10.000000 reddit-account-generator-1.0.0/reddit_account_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-26 16:10:10.000000 reddit-account-generator-1.0.0/reddit_account_generator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 16:10:10.749937 reddit-account-generator-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-26 16:09:58.000000 reddit-account-generator-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:59:31.883876 reddit-account-generator-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-08-01 08:59:31.883876 reddit-account-generator-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:59:31.879876 reddit-account-generator-1.1.0/reddit_account_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/reddit_account_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/reddit_account_generator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/reddit_account_generator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/reddit_account_generator/maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/reddit_account_generator/protector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/reddit_account_generator/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/reddit_account_generator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:59:31.883876 reddit-account-generator-1.1.0/reddit_account_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-08-01 08:59:31.000000 reddit-account-generator-1.1.0/reddit_account_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-01 08:59:31.000000 reddit-account-generator-1.1.0/reddit_account_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:59:31.000000 reddit-account-generator-1.1.0/reddit_account_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-01 08:59:31.000000 reddit-account-generator-1.1.0/reddit_account_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 08:59:31.000000 reddit-account-generator-1.1.0/reddit_account_generator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 08:59:31.883876 reddit-account-generator-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/setup.py
```

### Comparing `reddit-account-generator-1.0.0/LICENSE` & `reddit-account-generator-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit-account-generator-1.0.0/PKG-INFO` & `reddit-account-generator-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-account-generator
-Version: 1.0.0
+Version: 1.1.0
 Summary: Automatic reddit account generator on selenium.
 Home-page: https://github.com/cubicbyte/reddit-account-generator
 Author: cubicbyte
 Author-email: bmaruhnenko@gmail.com
 License: MIT
 Keywords: python reddit account-generator account-maker account-generation r-place rplace
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,42 +42,48 @@
 - **Proxy Support**: Since reddit allows you to create 1 account per IP every 10 minutes, this is very important.
 - **Resilience**: The script is able to handle most errors that may occur during the account creation process.
 
 ## Quick info
 
 You still need to activate the accounts via email. But it doesn't take much time.
 
+Firefox should be installed on your system for the script to work.
+
 It is recommended to use proxies, because you can only create 1 account per IP in 10 minutes. See file **proxies.txt** or run `python run_tor.py`
 
 ## TODO:
 - [x] Add automatic browser driver download
 - [x] Add Tor support for easier proxy management
 - [x] Make this a python package
 - [ ] Automatic email verification
 - [ ] Handle error when sub is not available
 
 # Getting started
 
+> **Note** Python 3.7+ is required
+
 ## Script installation
 
 1. Clone this repository to your local machine:
 
 ```shell
 git clone https://github.com/cubicbyte/reddit-account-generator.git
 cd reddit-account-generator
 ```
 
 2. Install the required dependencies:
 
 ```shell
-pip install -r requirements.txt
+pip install -r requirements-cli.txt
 ```
 
 ## Script usage
 
+> **Note** **Firefox should be installed on your system for the script to work**
+
 > **Note** **You need to use Tor (not browser) or proxy, because you can only create 1 account per IP in 10 minutes**
 
 #### Using Tor (recommended)
 Run this command and follow the instructions:
 ```shell
 python run_tor.py
 ```
@@ -142,40 +148,44 @@
 username = 'PolishCardinal69'
 password = '31vV3X1zy8YP'
 
 # Create account
 create_account(email, username, password)
 
 # Protect account from being suspended of being a bot
-protect_account(username)
+protect_account(username, password)
 
 # Done!
 ```
 
 Using proxy:
     
 ```python
-from reddit_account_generator.proxies import Proxy
+from reddit_account_generator import create_account, protect_account, install_driver
+from reddit_account_generator.proxies import TorProxy
 
-...
+email = 'your-email@gmail.com'
+# Username and password will be generated automatically
 
 proxy = TorProxy(TOR_IP, TOR_PORT, TOR_PASSWORD, TOR_CONTROL_PORT, TOR_DELAY)
 
-create_account(email, username, password, proxy=proxy.get_next())
-protect_account(username, password)  # Proxy not required
+uname, pwd = create_account(email, proxy=proxy.get_next())
+protect_account(username=uname, password=pwd)  # Proxy not required
 ```
 
 
 ## Requirements
 
-- Python 3.5+
+- Python 3.7+
 - [selenium](https://pypi.org/project/selenium/)
 - [selenium-recaptcha-solver](https://pypi.org/project/selenium-recaptcha-solver/)
 - [random-username](https://pypi.org/project/random-username/)
 - [webdriverdownloader](https://pypi.org/project/webdriverdownloader/)
+- [stem](https://pypi.org/project/stem/)
+- [coloredlogs](https://pypi.org/project/coloredlogs/) *optional
 
 ## Contributing
 
 Contributions to this project are welcome! Feel free to open issues or submit pull requests.
 
 ## License
```

### Comparing `reddit-account-generator-1.0.0/README.md` & `reddit-account-generator-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,42 +26,48 @@
 - **Proxy Support**: Since reddit allows you to create 1 account per IP every 10 minutes, this is very important.
 - **Resilience**: The script is able to handle most errors that may occur during the account creation process.
 
 ## Quick info
 
 You still need to activate the accounts via email. But it doesn't take much time.
 
+Firefox should be installed on your system for the script to work.
+
 It is recommended to use proxies, because you can only create 1 account per IP in 10 minutes. See file **proxies.txt** or run `python run_tor.py`
 
 ## TODO:
 - [x] Add automatic browser driver download
 - [x] Add Tor support for easier proxy management
 - [x] Make this a python package
 - [ ] Automatic email verification
 - [ ] Handle error when sub is not available
 
 # Getting started
 
+> **Note** Python 3.7+ is required
+
 ## Script installation
 
 1. Clone this repository to your local machine:
 
 ```shell
 git clone https://github.com/cubicbyte/reddit-account-generator.git
 cd reddit-account-generator
 ```
 
 2. Install the required dependencies:
 
 ```shell
-pip install -r requirements.txt
+pip install -r requirements-cli.txt
 ```
 
 ## Script usage
 
+> **Note** **Firefox should be installed on your system for the script to work**
+
 > **Note** **You need to use Tor (not browser) or proxy, because you can only create 1 account per IP in 10 minutes**
 
 #### Using Tor (recommended)
 Run this command and follow the instructions:
 ```shell
 python run_tor.py
 ```
@@ -126,40 +132,44 @@
 username = 'PolishCardinal69'
 password = '31vV3X1zy8YP'
 
 # Create account
 create_account(email, username, password)
 
 # Protect account from being suspended of being a bot
-protect_account(username)
+protect_account(username, password)
 
 # Done!
 ```
 
 Using proxy:
     
 ```python
-from reddit_account_generator.proxies import Proxy
+from reddit_account_generator import create_account, protect_account, install_driver
+from reddit_account_generator.proxies import TorProxy
 
-...
+email = 'your-email@gmail.com'
+# Username and password will be generated automatically
 
 proxy = TorProxy(TOR_IP, TOR_PORT, TOR_PASSWORD, TOR_CONTROL_PORT, TOR_DELAY)
 
-create_account(email, username, password, proxy=proxy.get_next())
-protect_account(username, password)  # Proxy not required
+uname, pwd = create_account(email, proxy=proxy.get_next())
+protect_account(username=uname, password=pwd)  # Proxy not required
 ```
 
 
 ## Requirements
 
-- Python 3.5+
+- Python 3.7+
 - [selenium](https://pypi.org/project/selenium/)
 - [selenium-recaptcha-solver](https://pypi.org/project/selenium-recaptcha-solver/)
 - [random-username](https://pypi.org/project/random-username/)
 - [webdriverdownloader](https://pypi.org/project/webdriverdownloader/)
+- [stem](https://pypi.org/project/stem/)
+- [coloredlogs](https://pypi.org/project/coloredlogs/) *optional
 
 ## Contributing
 
 Contributions to this project are welcome! Feel free to open issues or submit pull requests.
 
 ## License
```

### Comparing `reddit-account-generator-1.0.0/reddit_account_generator/maker.py` & `reddit-account-generator-1.1.0/reddit_account_generator/maker.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,58 @@
 import time
 import logging
 
-from selenium.common.exceptions import TimeoutException, WebDriverException
+from selenium.common.exceptions import TimeoutException, WebDriverException, NoSuchElementException, ElementClickInterceptedException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
-from selenium_recaptcha_solver import RecaptchaSolver
+from selenium_recaptcha_solver import RecaptchaSolver, RecaptchaException
 
-from .utils import setup_firefox_driver, try_to_click
+from .utils import setup_firefox_driver, try_to_click, generate_password, generate_username
 from .exceptions import *
 
 PAGE_LOAD_TIMEOUT_S = 60
 DRIVER_TIMEOUT_S = 60
 MICRO_DELAY_S = 1
 
+_logger = logging.getLogger(__name__)
 
-def create_account(email: str, username: str, password: str,
-                   proxies: dict[str, str] | None = None, hide_browser: bool = True):
+
+def create_account(email: str, username: str | None = None, password: str | None = None,
+                   proxies: dict[str, str] | None = None, hide_browser: bool = True) -> tuple[str, str]:
     """Create a Reddit account."""
 
-    logging.info('Creating account with username %s', username)
+    _logger.info('Creating reddit account')
     driver = setup_firefox_driver(proxies, hide_browser)
 
     if PAGE_LOAD_TIMEOUT_S is not None:
         driver.set_page_load_timeout(PAGE_LOAD_TIMEOUT_S)
 
+    if password is None:
+        password = generate_password()
+
     try:  # try/except to quit driver if error occurs
 
         # Open website
+        _logger.debug('Opening registration page')
         try:
             driver.get('https://www.reddit.com/register/')
         except WebDriverException:
             raise TimeoutException('Website takes too long to load. Probably a problem with the proxy.')
 
+        # Checking if IP is blocked
+        try:
+            first_h1 = driver.find_element(By.TAG_NAME, 'h1')
+            if first_h1.text == 'whoa there, pardner!':
+                raise IPCooldownException('Your IP is temporarily blocked. Try again later.')
+        except NoSuchElementException:
+            pass
+
         # Enter email and go to next page
+        _logger.debug('Entering email')
         email_input = driver.find_element(By.ID, 'regEmail')
         email_submit = driver.find_element(By.CSS_SELECTOR, 'button[data-step="email"]')
         email_input.click()
         email_input.send_keys(email)
         try_to_click(email_submit, delay=MICRO_DELAY_S)
 
         # Check for email error
@@ -45,24 +60,38 @@
         try:
             email_err = driver.find_element(By.CLASS_NAME, 'AnimatedForm__errorMessage')
         except:
             pass
         else:
             if email_err.text != '':
                 if 'again' in email_err.text.lower():
-                    raise EMailCooldownException(email_err.text)
+                    raise SessionExpiredException(email_err.text)
                 raise Exception(email_err.text)
 
         # Wait until page loads
         WebDriverWait(driver, DRIVER_TIMEOUT_S).until(EC.element_to_be_clickable((By.ID, 'regUsername')))
 
         # Enter username
+        _logger.debug('Entering username and password')
+        try:
+            # Get random username suggested by reddit
+            random_username = driver.find_element(By.XPATH, '/html/body/div/main/div[2]/div/div/div[2]/div[2]/div/div/a[1]')
+        except NoSuchElementException:
+            # Sometimes reddit doesn't suggest any username
+            username = generate_username()
+
         username_input = driver.find_element(By.ID, 'regUsername')
-        try_to_click(username_input, delay=MICRO_DELAY_S)
-        username_input.send_keys(username)
+        if username is not None:
+            # Enter given username
+            try_to_click(username_input, delay=MICRO_DELAY_S)
+            username_input.send_keys(username)
+        else:
+            # Click first reddit sugegsted name
+            try_to_click(random_username, delay=MICRO_DELAY_S)
+            username = random_username.text
 
         # Enter password
         password_input = driver.find_element(By.ID, 'regPassword')
         try_to_click(password_input, delay=MICRO_DELAY_S)
         password_input.send_keys(password)
 
         # Check for username and password errors
@@ -82,22 +111,31 @@
 
         if password_err.text != '':
             if 'character' in password_err.text.lower():
                 raise PasswordLengthException(password_err.text)
             raise Exception(password_err.text)
         
         # Solve captcha
+        _logger.debug('Solving captcha')
         WebDriverWait(driver, DRIVER_TIMEOUT_S).until(EC.element_to_be_clickable((By.XPATH, '//iframe[@title="reCAPTCHA"]')))
         recaptcha_iframe = driver.find_element(By.XPATH, '//iframe[@title="reCAPTCHA"]')
 
         if recaptcha_iframe.is_displayed():
             solver = RecaptchaSolver(driver)
-            solver.click_recaptcha_v2(iframe=recaptcha_iframe)
+            for _ in range(5):
+                try:
+                    solver.click_recaptcha_v2(iframe=recaptcha_iframe)
+                    break
+                except ElementClickInterceptedException:
+                    pass
+            else:
+                raise RecaptchaException('Could not solve captcha')
 
         # Submit registration
+        _logger.debug('Submitting registration')
         submit_btn = driver.find_element(By.CSS_SELECTOR, 'button[data-step="username-and-password"]')
         WebDriverWait(driver, DRIVER_TIMEOUT_S).until(EC.element_to_be_clickable(submit_btn))
         try_to_click(submit_btn, delay=MICRO_DELAY_S)
 
         # Check if submitted
         time.sleep(MICRO_DELAY_S)
         submit_err = driver.find_element(By.CSS_SELECTOR, 'span[data-step="username-and-password"]')
@@ -113,7 +151,8 @@
         # Account created!
 
     except Exception as e:  # quit driver if error occurs
         driver.quit()
         raise e
 
     driver.quit()
+    return username, password
```

### Comparing `reddit-account-generator-1.0.0/reddit_account_generator/protector.py` & `reddit-account-generator-1.1.0/reddit_account_generator/protector.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     'linux',
     'pcmasterrace',
     'clashroyale',
     'minecraft',
     'cursed_comments',
     'shitposting',
 ]
+_logger = logging.getLogger(__name__)
 
 
 def protect_account(username: str, password: str,
                     proxies: dict[str, str] | None = None, hide_browser: bool = True):
     """
     Prevent account blocking due to suspicion of being a bot.
 
@@ -49,28 +50,31 @@
 
     if PAGE_LOAD_TIMEOUT_S is not None:
         driver.set_page_load_timeout(PAGE_LOAD_TIMEOUT_S)
 
     try:  # try/except to quit driver if error occurs
 
         # Open login website
+        _logger.debug('Opening login page')
         try:
             driver.get('https://www.reddit.com/login/')
         except WebDriverException:
             raise TimeoutException('Website takes too long to load. Probably a problem with the proxy.')
         
         # Enter username and password
+        _logger.debug('Entering username and password')
         username_input = driver.find_element(By.ID, 'loginUsername')
         password_input = driver.find_element(By.ID, 'loginPassword')
         try_to_click(username_input, delay=MICRO_DELAY_S)
         username_input.send_keys(username)
         try_to_click(password_input, delay=MICRO_DELAY_S)
         password_input.send_keys(password)
 
         # Submit login
+        _logger.debug('Submitting login')
         submit_btn = driver.find_element(By.CSS_SELECTOR, 'button[type="submit"]')
         WebDriverWait(driver, DRIVER_TIMEOUT_S).until(EC.element_to_be_clickable(submit_btn))
         try_to_click(submit_btn, delay=MICRO_DELAY_S)
 
         # Check if submitted
         time.sleep(MICRO_DELAY_S)
         submit_err = driver.find_element(By.CLASS_NAME, 'AnimatedForm__errorMessage')
@@ -79,18 +83,21 @@
             if 'incorrect' in submit_err.text.lower():
                 raise IncorrectUsernameOrPasswordException(submit_err.text)
             raise Exception(submit_err.text)
 
         # Logged in!
 
         # Go to random subreddit
+        sub = random.choice(subs)
+        _logger.debug('Going to subreddit r/%s', sub)
         WebDriverWait(driver, DRIVER_TIMEOUT_S).until(EC.url_matches('https://www.reddit.com*'))
-        driver.get(f'https://www.reddit.com/r/{random.choice(subs)}/')
+        driver.get(f'https://www.reddit.com/r/{sub}/')
 
         # Subscribe
+        _logger.debug('Subscribing to subreddit r/%s', sub)
         subscribe_btn = driver.find_element(By.XPATH, '//button[text()="Join"]')
         WebDriverWait(driver, DRIVER_TIMEOUT_S).until(EC.element_to_be_clickable(subscribe_btn))
         try_to_click(subscribe_btn, delay=MICRO_DELAY_S)
 
         # Done!
 
     except Exception as e:  # quit driver if error occurs
```

### Comparing `reddit-account-generator-1.0.0/reddit_account_generator/proxies.py` & `reddit-account-generator-1.1.0/reddit_account_generator/proxies.py`

 * *Files identical despite different names*

### Comparing `reddit-account-generator-1.0.0/reddit_account_generator/utils.py` & `reddit-account-generator-1.1.0/reddit_account_generator/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import time
 import random
 import string
 import secrets
 
 import requests
 from selenium import webdriver
+from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.remote.webelement import WebElement
 from random_username.generate import generate_username as _generate_username
 
 
 def generate_username() -> str:
     username = _generate_username(1)[0] + str(random.randint(100, 1000))
     return username
@@ -48,16 +49,37 @@
     try:
         r = requests.get('https://check.torproject.org/api/ip', proxies={'https': f'socks5h://{ip}:{port}'}, timeout=5)
         return r.json()['IsTor'] is True
     except Exception:
         return False
 
 
+def setup_chrome_driver(proxies: dict[str, str] | None = None, hide_browser: bool = True) -> webdriver.Chrome:
+    options = webdriver.ChromeOptions()
+    options.add_argument('--lang=en-US')
+
+    if hide_browser:
+        options.add_argument('--headless')
+
+    # Set up proxies if available
+    if proxies is not None:
+        if 'http' in proxies:
+            options.add_argument(f'--proxy-server=http://{proxies["http"]}')
+        if 'https' in proxies:
+            options.add_argument(f'--proxy-server=https://{proxies["https"]}')
+        if 'socks' in proxies:
+            # Only SOCKS5 is supported
+            options.add_argument(f'--proxy-server=socks5://{proxies["socks"]}')
+
+    return webdriver.Chrome(options=options, service_log_path=os.devnull)
+
+
 def setup_firefox_driver(proxies: dict[str, str] | None = None, hide_browser: bool = True) -> webdriver.Firefox:
     options = webdriver.FirefoxOptions()
+    options.set_preference('intl.accept_languages', 'en-US')
 
     if hide_browser:
         options.add_argument('--headless')
 
     # Set up proxies if available
     if proxies is not None:
         options.set_preference('network.proxy.type', 1)
@@ -76,17 +98,18 @@
             options.set_preference('network.proxy.socks', socks_ip)
             options.set_preference('network.proxy.socks_port', int(socks_port))
             options.set_preference('network.proxy.socks_remote_dns', False)
 
     return webdriver.Firefox(options=options, service_log_path=os.devnull)
 
 
-def try_to_click(element: WebElement, delay: int | float = 0.5, max_tries: int = 10) -> bool:
+def try_to_click(element: WebElement, delay: int | float = 0.5, max_tries: int = 20) -> bool:
     """Try to click an element multiple times."""
-    while max_tries > 0:
+    retries = 0
+    while retries < max_tries:
         try:
             element.click()
             return
-        except Exception as e:
-            max_tries -= 1
+        except:
+            retries += 1
             time.sleep(delay)
-    raise e
+    raise TimeoutException(f'Could not click element after {max_tries} tries.')
```

### Comparing `reddit-account-generator-1.0.0/reddit_account_generator.egg-info/PKG-INFO` & `reddit-account-generator-1.1.0/reddit_account_generator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-account-generator
-Version: 1.0.0
+Version: 1.1.0
 Summary: Automatic reddit account generator on selenium.
 Home-page: https://github.com/cubicbyte/reddit-account-generator
 Author: cubicbyte
 Author-email: bmaruhnenko@gmail.com
 License: MIT
 Keywords: python reddit account-generator account-maker account-generation r-place rplace
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,42 +42,48 @@
 - **Proxy Support**: Since reddit allows you to create 1 account per IP every 10 minutes, this is very important.
 - **Resilience**: The script is able to handle most errors that may occur during the account creation process.
 
 ## Quick info
 
 You still need to activate the accounts via email. But it doesn't take much time.
 
+Firefox should be installed on your system for the script to work.
+
 It is recommended to use proxies, because you can only create 1 account per IP in 10 minutes. See file **proxies.txt** or run `python run_tor.py`
 
 ## TODO:
 - [x] Add automatic browser driver download
 - [x] Add Tor support for easier proxy management
 - [x] Make this a python package
 - [ ] Automatic email verification
 - [ ] Handle error when sub is not available
 
 # Getting started
 
+> **Note** Python 3.7+ is required
+
 ## Script installation
 
 1. Clone this repository to your local machine:
 
 ```shell
 git clone https://github.com/cubicbyte/reddit-account-generator.git
 cd reddit-account-generator
 ```
 
 2. Install the required dependencies:
 
 ```shell
-pip install -r requirements.txt
+pip install -r requirements-cli.txt
 ```
 
 ## Script usage
 
+> **Note** **Firefox should be installed on your system for the script to work**
+
 > **Note** **You need to use Tor (not browser) or proxy, because you can only create 1 account per IP in 10 minutes**
 
 #### Using Tor (recommended)
 Run this command and follow the instructions:
 ```shell
 python run_tor.py
 ```
@@ -142,40 +148,44 @@
 username = 'PolishCardinal69'
 password = '31vV3X1zy8YP'
 
 # Create account
 create_account(email, username, password)
 
 # Protect account from being suspended of being a bot
-protect_account(username)
+protect_account(username, password)
 
 # Done!
 ```
 
 Using proxy:
     
 ```python
-from reddit_account_generator.proxies import Proxy
+from reddit_account_generator import create_account, protect_account, install_driver
+from reddit_account_generator.proxies import TorProxy
 
-...
+email = 'your-email@gmail.com'
+# Username and password will be generated automatically
 
 proxy = TorProxy(TOR_IP, TOR_PORT, TOR_PASSWORD, TOR_CONTROL_PORT, TOR_DELAY)
 
-create_account(email, username, password, proxy=proxy.get_next())
-protect_account(username, password)  # Proxy not required
+uname, pwd = create_account(email, proxy=proxy.get_next())
+protect_account(username=uname, password=pwd)  # Proxy not required
 ```
 
 
 ## Requirements
 
-- Python 3.5+
+- Python 3.7+
 - [selenium](https://pypi.org/project/selenium/)
 - [selenium-recaptcha-solver](https://pypi.org/project/selenium-recaptcha-solver/)
 - [random-username](https://pypi.org/project/random-username/)
 - [webdriverdownloader](https://pypi.org/project/webdriverdownloader/)
+- [stem](https://pypi.org/project/stem/)
+- [coloredlogs](https://pypi.org/project/coloredlogs/) *optional
 
 ## Contributing
 
 Contributions to this project are welcome! Feel free to open issues or submit pull requests.
 
 ## License
```

### Comparing `reddit-account-generator-1.0.0/reddit_account_generator.egg-info/SOURCES.txt` & `reddit-account-generator-1.1.0/reddit_account_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reddit-account-generator-1.0.0/setup.py` & `reddit-account-generator-1.1.0/setup.py`

 * *Files identical despite different names*

