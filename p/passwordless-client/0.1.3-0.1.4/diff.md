# Comparing `tmp/passwordless-client-0.1.3.tar.gz` & `tmp/passwordless-client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwordless-client-0.1.3.tar", last modified: Tue Aug  1 12:46:53 2023, max compression
+gzip compressed data, was "passwordless-client-0.1.4.tar", last modified: Tue Aug  1 13:04:39 2023, max compression
```

## Comparing `passwordless-client-0.1.3.tar` & `passwordless-client-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 12:46:53.943906 passwordless-client-0.1.3/
--rw-rw-rw-   0        0        0     3419 2023-08-01 12:46:53.943906 passwordless-client-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2662 2023-08-01 16:43:28.000000 passwordless-client-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 12:46:53.943397 passwordless-client-0.1.3/passwordless_client.egg-info/
--rw-rw-rw-   0        0        0     3419 2023-08-01 12:46:53.000000 passwordless-client-0.1.3/passwordless_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-08-01 12:46:53.000000 passwordless-client-0.1.3/passwordless_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 12:46:53.000000 passwordless-client-0.1.3/passwordless_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-01 12:46:53.000000 passwordless-client-0.1.3/passwordless_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 12:46:53.000000 passwordless-client-0.1.3/passwordless_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 12:46:53.944414 passwordless-client-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      849 2023-08-01 16:43:28.000000 passwordless-client-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:04:39.574367 passwordless-client-0.1.4/
+-rw-rw-rw-   0        0        0     4395 2023-08-01 13:04:39.573862 passwordless-client-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3608 2023-08-01 16:57:10.000000 passwordless-client-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 13:04:39.572848 passwordless-client-0.1.4/passwordless_client.egg-info/
+-rw-rw-rw-   0        0        0     4395 2023-08-01 13:04:39.000000 passwordless-client-0.1.4/passwordless_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-08-01 13:04:39.000000 passwordless-client-0.1.4/passwordless_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 13:04:39.000000 passwordless-client-0.1.4/passwordless_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-01 13:04:39.000000 passwordless-client-0.1.4/passwordless_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 13:04:39.000000 passwordless-client-0.1.4/passwordless_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 13:04:39.574367 passwordless-client-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      849 2023-08-01 13:04:10.000000 passwordless-client-0.1.4/setup.py
```

### Comparing `passwordless-client-0.1.3/PKG-INFO` & `passwordless-client-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,129 +1,160 @@
 Metadata-Version: 2.1
 Name: passwordless-client
-Version: 0.1.3
+Version: 0.1.4
 Summary: A client library for Passwordless.dev API
 Home-page: https://github.com/yourusername/passwordless-client
 Author: Matthew Fiallos
 Author-email: matthew.fiallos@randstadusa.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
+
 # Passwordless.dev Python SDK Client
 
-A Python client library for interacting with the Bitwarden Passwordless.dev API.
+A Python client library for interacting with the Passwordless.dev API.
 
 ## Installation
 
 1. Install the package using pip:
 
 ```bash
 pip install passwordless-client
 ```
 
 ## Usage
 
 ### Configuration
 
-You can store the API secret and public API key in a configuration file for easier management and security.
+You can store the API configurations in a file named `passwordlessconfig.ini` for easier management and security.
 
 #### Creating a Configuration File
 
-Create a file named `config.ini` in the same directory as your script, with the following content:
+Create a file named `passwordlessconfig.ini` in the same directory as your script, with the following content:
 
 ```ini
-[passwordless]
-api_secret = myapplication:secret:your_secret_key
-api_key = your_public_api_key
+[API]
+API_URL = https://v4.passwordless.dev
+API_SECRET = Your-API-Secret-Here
+API_KEY = Your-API-Key-Here
+VERIFY = False
 ```
 
-Replace the values with your actual API secret and public API key.
+The `PasswordlessClient` class will automatically read this file and use the specified configurations when making requests to the Passwordless.dev API.
 
-#### Reading the Configuration in Code
+### Client Initialization
 
-Use the `configparser` module to read the configuration file and pass the keys to the `PasswordlessClient`:
+Initialize the Passwordless client by creating an instance of the `PasswordlessClient` class:
 
 ```python
-import configparser
+from passwordless_client import PasswordlessClient
+
+client = PasswordlessClient()
+```
 
-config = configparser.ConfigParser()
-config.read('config.ini')
+### Register Token
 
-api_secret = config['passwordless']['api_secret']
-# api_key can be accessed similarly if needed
+Register a new token using the `register_token` method:
 
+```python
+result = client.register_token(user_id="some-user-id", username="username@example.com", displayname="John Doe")
 ```
 
+### Sign In Verification
 
+Verify a sign-in token using the `signin_verify` method:
 
-### Importing the Client
+```python
+result = client.signin_verify(token="your-token-here")
+```
 
-Once the package is installed, you can import the `PasswordlessClient` class in your Python script or application:
+### Alias Management
+
+Manage aliases using the `alias` method:
 
 ```python
-from passwordless import PasswordlessClient
+result = client.alias(user_id="user-id", aliases=["alias1@example.com", "alias2@example.com"])
 ```
 
-### Creating a Client Instance
+### Credentials Management
 
-Create an instance of the `PasswordlessClient` class, providing your API private secret:
+List and delete credentials using the `credentials_list` and `credentials_delete` methods:
 
 ```python
-client = PasswordlessClient(api_secret)
+# List credentials
+result = client.credentials_list(user_id="user-id")
+
+# Delete credential
+result = client.credentials_delete(credential_id="credential-id")
 ```
 
-### Using the Client's Methods
+## Example Application
 
-You can now use the various methods provided by the `PasswordlessClient` class to interact with the Passwordless.dev API.
+This section provides an example of how the `PasswordlessClient` class can be used in an application to interact with the Passwordless.dev API.
 
-#### Registering a Token
+### 1. Import and Initialize the Client
+
+First, ensure that the `passwordlessconfig.ini` file is created with the correct configurations as described in the Configuration section.
+
+Then, import and initialize the client:
 
 ```python
-user_id = "107fb578-9559-4540-a0e2-f82ad78852f7"
-username = "pjfry@passwordless.dev"
-displayname = "Philip J Fry"
-response = client.register_token(user_id, username, displayname)
-print(response)
+from passwordless_client import PasswordlessClient
+
+client = PasswordlessClient()  # Reads from passwordlessconfig.ini
 ```
 
-#### Verifying a Sign-In
+### 2. Register a New User
 
 ```python
-token = "d5vzCkL_GvpS4VYtoT3..."
-response = client.signin_verify(token)
-print(response)
+user_id = "some-user-id"
+username = "username@example.com"
+displayname = "John Doe"
+
+result = client.register_token(user_id, username, displayname)
+print("Registration Result:", result)
 ```
 
-#### Adding Aliases
+### 3. Verify a Sign-In Token
 
 ```python
-user_id = "107fb578-9559-4540-a0e2-f82ad78852f7"
-aliases = ["pjfry@passwordless.dev", "benderrules@passwordless.dev"]
-response = client.alias(user_id, aliases)
-print(response)
+token = "your-token-here"
+result = client.signin_verify(token)
+print("Verification Result:", result)
 ```
 
-#### Listing Credentials
+### 4. Manage Aliases
 
 ```python
-user_id = "107fb578-9559-4540-a0e2-f82ad78852f7"
-response = client.credentials_list(user_id)
-print(response)
+aliases = ["alias1@example.com", "alias2@example.com"]
+result = client.alias(user_id, aliases)
+print("Alias Management Result:", result)
 ```
 
-#### Deleting a Credential
+### 5. List and Delete Credentials
 
 ```python
-credential_id = "qgB2ZetBhi0rIcaQK8_HrLQzXXfwKia46_PNjUC2L_w"
-response = client.credentials_delete(credential_id)
-print(response)
+# List credentials
+result = client.credentials_list(user_id)
+print("Credentials List:", result)
+
+# Delete a specific credential
+credential_id = "credential-id"
+result = client.credentials_delete(credential_id)
+print("Credential Deletion Result:", result)
 ```
 
----
+These examples demonstrate a typical workflow for interacting with the Passwordless.dev API. By using the `PasswordlessClient` class, you can easily integrate authentication and authorization features into your Python application.
+
+## License
+
+This project is licensed under the MIT License.
+
+## Contributing
 
-This `README.md` file provides a basic introduction to the `PasswordlessClient` class, how to install the package, and how to use the different methods. It can be expanded with additional information as needed.
+Please refer to the CONTRIBUTING.md file for details on contributing to this project.
```

### Comparing `passwordless-client-0.1.3/README.md` & `passwordless-client-0.1.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,113 +1,144 @@
+
 # Passwordless.dev Python SDK Client
 
-A Python client library for interacting with the Bitwarden Passwordless.dev API.
+A Python client library for interacting with the Passwordless.dev API.
 
 ## Installation
 
 1. Install the package using pip:
 
 ```bash
 pip install passwordless-client
 ```
 
 ## Usage
 
 ### Configuration
 
-You can store the API secret and public API key in a configuration file for easier management and security.
+You can store the API configurations in a file named `passwordlessconfig.ini` for easier management and security.
 
 #### Creating a Configuration File
 
-Create a file named `config.ini` in the same directory as your script, with the following content:
+Create a file named `passwordlessconfig.ini` in the same directory as your script, with the following content:
 
 ```ini
-[passwordless]
-api_secret = myapplication:secret:your_secret_key
-api_key = your_public_api_key
+[API]
+API_URL = https://v4.passwordless.dev
+API_SECRET = Your-API-Secret-Here
+API_KEY = Your-API-Key-Here
+VERIFY = False
 ```
 
-Replace the values with your actual API secret and public API key.
+The `PasswordlessClient` class will automatically read this file and use the specified configurations when making requests to the Passwordless.dev API.
 
-#### Reading the Configuration in Code
+### Client Initialization
 
-Use the `configparser` module to read the configuration file and pass the keys to the `PasswordlessClient`:
+Initialize the Passwordless client by creating an instance of the `PasswordlessClient` class:
 
 ```python
-import configparser
+from passwordless_client import PasswordlessClient
+
+client = PasswordlessClient()
+```
 
-config = configparser.ConfigParser()
-config.read('config.ini')
+### Register Token
 
-api_secret = config['passwordless']['api_secret']
-# api_key can be accessed similarly if needed
+Register a new token using the `register_token` method:
 
+```python
+result = client.register_token(user_id="some-user-id", username="username@example.com", displayname="John Doe")
 ```
 
+### Sign In Verification
 
+Verify a sign-in token using the `signin_verify` method:
 
-### Importing the Client
+```python
+result = client.signin_verify(token="your-token-here")
+```
 
-Once the package is installed, you can import the `PasswordlessClient` class in your Python script or application:
+### Alias Management
+
+Manage aliases using the `alias` method:
 
 ```python
-from passwordless import PasswordlessClient
+result = client.alias(user_id="user-id", aliases=["alias1@example.com", "alias2@example.com"])
 ```
 
-### Creating a Client Instance
+### Credentials Management
 
-Create an instance of the `PasswordlessClient` class, providing your API private secret:
+List and delete credentials using the `credentials_list` and `credentials_delete` methods:
 
 ```python
-client = PasswordlessClient(api_secret)
+# List credentials
+result = client.credentials_list(user_id="user-id")
+
+# Delete credential
+result = client.credentials_delete(credential_id="credential-id")
 ```
 
-### Using the Client's Methods
+## Example Application
 
-You can now use the various methods provided by the `PasswordlessClient` class to interact with the Passwordless.dev API.
+This section provides an example of how the `PasswordlessClient` class can be used in an application to interact with the Passwordless.dev API.
 
-#### Registering a Token
+### 1. Import and Initialize the Client
+
+First, ensure that the `passwordlessconfig.ini` file is created with the correct configurations as described in the Configuration section.
+
+Then, import and initialize the client:
 
 ```python
-user_id = "107fb578-9559-4540-a0e2-f82ad78852f7"
-username = "pjfry@passwordless.dev"
-displayname = "Philip J Fry"
-response = client.register_token(user_id, username, displayname)
-print(response)
+from passwordless_client import PasswordlessClient
+
+client = PasswordlessClient()  # Reads from passwordlessconfig.ini
 ```
 
-#### Verifying a Sign-In
+### 2. Register a New User
 
 ```python
-token = "d5vzCkL_GvpS4VYtoT3..."
-response = client.signin_verify(token)
-print(response)
+user_id = "some-user-id"
+username = "username@example.com"
+displayname = "John Doe"
+
+result = client.register_token(user_id, username, displayname)
+print("Registration Result:", result)
 ```
 
-#### Adding Aliases
+### 3. Verify a Sign-In Token
 
 ```python
-user_id = "107fb578-9559-4540-a0e2-f82ad78852f7"
-aliases = ["pjfry@passwordless.dev", "benderrules@passwordless.dev"]
-response = client.alias(user_id, aliases)
-print(response)
+token = "your-token-here"
+result = client.signin_verify(token)
+print("Verification Result:", result)
 ```
 
-#### Listing Credentials
+### 4. Manage Aliases
 
 ```python
-user_id = "107fb578-9559-4540-a0e2-f82ad78852f7"
-response = client.credentials_list(user_id)
-print(response)
+aliases = ["alias1@example.com", "alias2@example.com"]
+result = client.alias(user_id, aliases)
+print("Alias Management Result:", result)
 ```
 
-#### Deleting a Credential
+### 5. List and Delete Credentials
 
 ```python
-credential_id = "qgB2ZetBhi0rIcaQK8_HrLQzXXfwKia46_PNjUC2L_w"
-response = client.credentials_delete(credential_id)
-print(response)
+# List credentials
+result = client.credentials_list(user_id)
+print("Credentials List:", result)
+
+# Delete a specific credential
+credential_id = "credential-id"
+result = client.credentials_delete(credential_id)
+print("Credential Deletion Result:", result)
 ```
 
----
+These examples demonstrate a typical workflow for interacting with the Passwordless.dev API. By using the `PasswordlessClient` class, you can easily integrate authentication and authorization features into your Python application.
+
+## License
+
+This project is licensed under the MIT License.
+
+## Contributing
 
-This `README.md` file provides a basic introduction to the `PasswordlessClient` class, how to install the package, and how to use the different methods. It can be expanded with additional information as needed.
+Please refer to the CONTRIBUTING.md file for details on contributing to this project.
```

### Comparing `passwordless-client-0.1.3/passwordless_client.egg-info/PKG-INFO` & `passwordless-client-0.1.4/passwordless_client.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,129 +1,160 @@
 Metadata-Version: 2.1
 Name: passwordless-client
-Version: 0.1.3
+Version: 0.1.4
 Summary: A client library for Passwordless.dev API
 Home-page: https://github.com/yourusername/passwordless-client
 Author: Matthew Fiallos
 Author-email: matthew.fiallos@randstadusa.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
+
 # Passwordless.dev Python SDK Client
 
-A Python client library for interacting with the Bitwarden Passwordless.dev API.
+A Python client library for interacting with the Passwordless.dev API.
 
 ## Installation
 
 1. Install the package using pip:
 
 ```bash
 pip install passwordless-client
 ```
 
 ## Usage
 
 ### Configuration
 
-You can store the API secret and public API key in a configuration file for easier management and security.
+You can store the API configurations in a file named `passwordlessconfig.ini` for easier management and security.
 
 #### Creating a Configuration File
 
-Create a file named `config.ini` in the same directory as your script, with the following content:
+Create a file named `passwordlessconfig.ini` in the same directory as your script, with the following content:
 
 ```ini
-[passwordless]
-api_secret = myapplication:secret:your_secret_key
-api_key = your_public_api_key
+[API]
+API_URL = https://v4.passwordless.dev
+API_SECRET = Your-API-Secret-Here
+API_KEY = Your-API-Key-Here
+VERIFY = False
 ```
 
-Replace the values with your actual API secret and public API key.
+The `PasswordlessClient` class will automatically read this file and use the specified configurations when making requests to the Passwordless.dev API.
 
-#### Reading the Configuration in Code
+### Client Initialization
 
-Use the `configparser` module to read the configuration file and pass the keys to the `PasswordlessClient`:
+Initialize the Passwordless client by creating an instance of the `PasswordlessClient` class:
 
 ```python
-import configparser
+from passwordless_client import PasswordlessClient
+
+client = PasswordlessClient()
+```
 
-config = configparser.ConfigParser()
-config.read('config.ini')
+### Register Token
 
-api_secret = config['passwordless']['api_secret']
-# api_key can be accessed similarly if needed
+Register a new token using the `register_token` method:
 
+```python
+result = client.register_token(user_id="some-user-id", username="username@example.com", displayname="John Doe")
 ```
 
+### Sign In Verification
 
+Verify a sign-in token using the `signin_verify` method:
 
-### Importing the Client
+```python
+result = client.signin_verify(token="your-token-here")
+```
 
-Once the package is installed, you can import the `PasswordlessClient` class in your Python script or application:
+### Alias Management
+
+Manage aliases using the `alias` method:
 
 ```python
-from passwordless import PasswordlessClient
+result = client.alias(user_id="user-id", aliases=["alias1@example.com", "alias2@example.com"])
 ```
 
-### Creating a Client Instance
+### Credentials Management
 
-Create an instance of the `PasswordlessClient` class, providing your API private secret:
+List and delete credentials using the `credentials_list` and `credentials_delete` methods:
 
 ```python
-client = PasswordlessClient(api_secret)
+# List credentials
+result = client.credentials_list(user_id="user-id")
+
+# Delete credential
+result = client.credentials_delete(credential_id="credential-id")
 ```
 
-### Using the Client's Methods
+## Example Application
 
-You can now use the various methods provided by the `PasswordlessClient` class to interact with the Passwordless.dev API.
+This section provides an example of how the `PasswordlessClient` class can be used in an application to interact with the Passwordless.dev API.
 
-#### Registering a Token
+### 1. Import and Initialize the Client
+
+First, ensure that the `passwordlessconfig.ini` file is created with the correct configurations as described in the Configuration section.
+
+Then, import and initialize the client:
 
 ```python
-user_id = "107fb578-9559-4540-a0e2-f82ad78852f7"
-username = "pjfry@passwordless.dev"
-displayname = "Philip J Fry"
-response = client.register_token(user_id, username, displayname)
-print(response)
+from passwordless_client import PasswordlessClient
+
+client = PasswordlessClient()  # Reads from passwordlessconfig.ini
 ```
 
-#### Verifying a Sign-In
+### 2. Register a New User
 
 ```python
-token = "d5vzCkL_GvpS4VYtoT3..."
-response = client.signin_verify(token)
-print(response)
+user_id = "some-user-id"
+username = "username@example.com"
+displayname = "John Doe"
+
+result = client.register_token(user_id, username, displayname)
+print("Registration Result:", result)
 ```
 
-#### Adding Aliases
+### 3. Verify a Sign-In Token
 
 ```python
-user_id = "107fb578-9559-4540-a0e2-f82ad78852f7"
-aliases = ["pjfry@passwordless.dev", "benderrules@passwordless.dev"]
-response = client.alias(user_id, aliases)
-print(response)
+token = "your-token-here"
+result = client.signin_verify(token)
+print("Verification Result:", result)
 ```
 
-#### Listing Credentials
+### 4. Manage Aliases
 
 ```python
-user_id = "107fb578-9559-4540-a0e2-f82ad78852f7"
-response = client.credentials_list(user_id)
-print(response)
+aliases = ["alias1@example.com", "alias2@example.com"]
+result = client.alias(user_id, aliases)
+print("Alias Management Result:", result)
 ```
 
-#### Deleting a Credential
+### 5. List and Delete Credentials
 
 ```python
-credential_id = "qgB2ZetBhi0rIcaQK8_HrLQzXXfwKia46_PNjUC2L_w"
-response = client.credentials_delete(credential_id)
-print(response)
+# List credentials
+result = client.credentials_list(user_id)
+print("Credentials List:", result)
+
+# Delete a specific credential
+credential_id = "credential-id"
+result = client.credentials_delete(credential_id)
+print("Credential Deletion Result:", result)
 ```
 
----
+These examples demonstrate a typical workflow for interacting with the Passwordless.dev API. By using the `PasswordlessClient` class, you can easily integrate authentication and authorization features into your Python application.
+
+## License
+
+This project is licensed under the MIT License.
+
+## Contributing
 
-This `README.md` file provides a basic introduction to the `PasswordlessClient` class, how to install the package, and how to use the different methods. It can be expanded with additional information as needed.
+Please refer to the CONTRIBUTING.md file for details on contributing to this project.
```

### Comparing `passwordless-client-0.1.3/setup.py` & `passwordless-client-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='passwordless-client',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Matthew Fiallos',
     author_email='matthew.fiallos@randstadusa.com',
     description='A client library for Passwordless.dev API',
```

