# Comparing `tmp/borneo-5.3.7.tar.gz` & `tmp/borneo-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/borneo-5.3.7.tar", last modified: Mon Dec 12 21:34:26 2022, max compression
+gzip compressed data, was "borneo-5.4.1.tar", last modified: Tue Aug  1 20:58:21 2023, max compression
```

## Comparing `borneo-5.3.7.tar` & `borneo-5.4.1.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 gmf        (501) wheel        (0)        0 2022-12-12 21:34:26.000000 borneo-5.3.7/
--rw-r--r--   0 gmf        (501) wheel        (0)    21790 2022-12-12 21:34:26.000000 borneo-5.3.7/PKG-INFO
--rw-r--r--   0 gmf        (501) wheel        (0)    19783 2022-12-12 21:23:57.000000 borneo-5.3.7/THIRD_PARTY_LICENSES.txt
--rw-r--r--   0 gmf        (501) wheel        (0)      105 2022-12-12 21:23:57.000000 borneo-5.3.7/MANIFEST.in
--rw-r--r--   0 gmf        (501) wheel        (0)     2619 2022-12-12 21:23:57.000000 borneo-5.3.7/setup.py
--rw-r--r--   0 gmf        (501) wheel        (0)       38 2022-12-12 21:34:26.000000 borneo-5.3.7/setup.cfg
--rw-r--r--   0 gmf        (501) wheel        (0)    17020 2022-12-12 21:23:57.000000 borneo-5.3.7/README.rst
--rwxr-xr-x   0 gmf        (501) wheel        (0)    12217 2022-12-12 21:24:37.000000 borneo-5.3.7/CHANGELOG.rst
--rw-r--r--   0 gmf        (501) wheel        (0)     1870 2022-12-12 21:23:57.000000 borneo-5.3.7/LICENSE.txt
-drwxr-xr-x   0 gmf        (501) wheel        (0)        0 2022-12-12 21:34:26.000000 borneo-5.3.7/src/
-drwxr-xr-x   0 gmf        (501) wheel        (0)        0 2022-12-12 21:34:26.000000 borneo-5.3.7/src/borneo/
--rw-r--r--   0 gmf        (501) wheel        (0)     3198 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/auth.py
--rw-r--r--   0 gmf        (501) wheel        (0)    16136 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/exception.py
--rw-r--r--   0 gmf        (501) wheel        (0)    62216 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/config.py
--rw-r--r--   0 gmf        (501) wheel        (0)      215 2022-12-12 21:24:44.000000 borneo-5.3.7/src/borneo/version.py
-drwxr-xr-x   0 gmf        (501) wheel        (0)        0 2022-12-12 21:34:26.000000 borneo-5.3.7/src/borneo/kv/
--rw-r--r--   0 gmf        (501) wheel        (0)      808 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/kv/exception.py
--rw-r--r--   0 gmf        (501) wheel        (0)      371 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/kv/__init__.py
--rw-r--r--   0 gmf        (501) wheel        (0)    13518 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/kv/kv.py
--rw-r--r--   0 gmf        (501) wheel        (0)   110911 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/query.py
--rw-r--r--   0 gmf        (501) wheel        (0)    22991 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/client.py
--rw-r--r--   0 gmf        (501) wheel        (0)    59306 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/serde.py
--rw-r--r--   0 gmf        (501) wheel        (0)     4313 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/__init__.py
--rw-r--r--   0 gmf        (501) wheel        (0)   187541 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/operations.py
-drwxr-xr-x   0 gmf        (501) wheel        (0)        0 2022-12-12 21:34:26.000000 borneo-5.3.7/src/borneo/iam/
--rw-r--r--   0 gmf        (501) wheel        (0)    19633 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/iam/iam.py
--rw-r--r--   0 gmf        (501) wheel        (0)      261 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/iam/__init__.py
--rw-r--r--   0 gmf        (501) wheel        (0)    71016 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/common.py
--rw-r--r--   0 gmf        (501) wheel        (0)    53754 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/http.py
--rw-r--r--   0 gmf        (501) wheel        (0)    33580 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/stats.py
--rw-r--r--   0 gmf        (501) wheel        (0)    34126 2022-12-12 21:23:57.000000 borneo-5.3.7/src/borneo/driver.py
-drwxr-xr-x   0 gmf        (501) wheel        (0)        0 2022-12-12 21:34:26.000000 borneo-5.3.7/src/borneo.egg-info/
--rw-r--r--   0 gmf        (501) wheel        (0)    21790 2022-12-12 21:34:26.000000 borneo-5.3.7/src/borneo.egg-info/PKG-INFO
--rw-r--r--   0 gmf        (501) wheel        (0)      649 2022-12-12 21:34:26.000000 borneo-5.3.7/src/borneo.egg-info/SOURCES.txt
--rw-r--r--   0 gmf        (501) wheel        (0)       40 2022-12-12 21:34:26.000000 borneo-5.3.7/src/borneo.egg-info/requires.txt
--rw-r--r--   0 gmf        (501) wheel        (0)        7 2022-12-12 21:34:26.000000 borneo-5.3.7/src/borneo.egg-info/top_level.txt
--rw-r--r--   0 gmf        (501) wheel        (0)        1 2022-12-12 21:34:26.000000 borneo-5.3.7/src/borneo.egg-info/dependency_links.txt
+drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2023-08-01 20:58:21.369788 borneo-5.4.1/
+-rwxr-xr-x   0 gfeinber   (503) staff       (20)    13762 2023-08-01 20:49:10.000000 borneo-5.4.1/CHANGELOG.rst
+-rw-r--r--   0 gfeinber   (503) staff       (20)     1870 2023-07-07 15:51:41.000000 borneo-5.4.1/LICENSE.txt
+-rw-r--r--   0 gfeinber   (503) staff       (20)      105 2023-07-07 15:51:41.000000 borneo-5.4.1/MANIFEST.in
+-rw-r--r--   0 gfeinber   (503) staff       (20)    17953 2023-08-01 20:58:21.369627 borneo-5.4.1/PKG-INFO
+-rw-r--r--   0 gfeinber   (503) staff       (20)    17014 2023-07-07 15:51:41.000000 borneo-5.4.1/README.rst
+-rw-r--r--   0 gfeinber   (503) staff       (20)    19783 2023-07-07 15:51:41.000000 borneo-5.4.1/THIRD_PARTY_LICENSES.txt
+-rw-r--r--   0 gfeinber   (503) staff       (20)       38 2023-08-01 20:58:21.369823 borneo-5.4.1/setup.cfg
+-rw-r--r--   0 gfeinber   (503) staff       (20)     2580 2023-07-07 15:51:41.000000 borneo-5.4.1/setup.py
+drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2023-08-01 20:58:21.362482 borneo-5.4.1/src/
+drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2023-08-01 20:58:21.367877 borneo-5.4.1/src/borneo/
+-rw-r--r--   0 gfeinber   (503) staff       (20)     4316 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/__init__.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)     3198 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/auth.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    23978 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/client.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    72485 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/common.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    66359 2023-08-01 19:35:48.000000 borneo-5.4.1/src/borneo/config.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    34126 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/driver.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    16136 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/exception.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    54466 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/http.py
+drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2023-08-01 20:58:21.368870 borneo-5.4.1/src/borneo/iam/
+-rw-r--r--   0 gfeinber   (503) staff       (20)      261 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/iam/__init__.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    19923 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/iam/iam.py
+drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2023-08-01 20:58:21.369364 borneo-5.4.1/src/borneo/kv/
+-rw-r--r--   0 gfeinber   (503) staff       (20)      371 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/kv/__init__.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)      808 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/kv/exception.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    13520 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/kv/kv.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    81993 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/nson.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)     2754 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/nson_protocol.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)   202405 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/operations.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)   109954 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/query.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    34651 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/serde.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    29169 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/serdeutil.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    33675 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/stats.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)      215 2023-08-01 20:49:10.000000 borneo-5.4.1/src/borneo/version.py
+drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2023-08-01 20:58:21.368639 borneo-5.4.1/src/borneo.egg-info/
+-rw-r--r--   0 gfeinber   (503) staff       (20)    17953 2023-08-01 20:58:21.000000 borneo-5.4.1/src/borneo.egg-info/PKG-INFO
+-rw-r--r--   0 gfeinber   (503) staff       (20)      720 2023-08-01 20:58:21.000000 borneo-5.4.1/src/borneo.egg-info/SOURCES.txt
+-rw-r--r--   0 gfeinber   (503) staff       (20)        1 2023-08-01 20:58:21.000000 borneo-5.4.1/src/borneo.egg-info/dependency_links.txt
+-rw-r--r--   0 gfeinber   (503) staff       (20)       40 2023-08-01 20:58:21.000000 borneo-5.4.1/src/borneo.egg-info/requires.txt
+-rw-r--r--   0 gfeinber   (503) staff       (20)        7 2023-08-01 20:58:21.000000 borneo-5.4.1/src/borneo.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `borneo-5.3.7/PKG-INFO` & `borneo-5.4.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,496 +1,495 @@
 Metadata-Version: 2.1
 Name: borneo
-Version: 5.3.7
+Version: 5.4.1
 Summary: Oracle NoSQL Database Python SDK
 Home-page: https://nosql-python-sdk.readthedocs.io/en/stable/index.html
 Author: Oracle
 Author-email: george.feinberg@oracle.com
 License: Universal Permissive License 1.0
-Description: Oracle NoSQL Database Python SDK
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        =====
-        About
-        =====
-        
-        This is the Python SDK for Oracle NoSQL Database. Python 2.7+ and 3.5+ are
-        supported. The SDK provides interfaces, documentation, and examples to help
-        develop Python applications that connect to the Oracle NoSQL Database Cloud
-        Service, Oracle NoSQL Database and to the Oracle NoSQL Cloud Simulator (which
-        runs on a local machine).
-        
-        In order to run the Oracle NoSQL Cloud Simulator, a separate download is
-        necessary from the Oracle NoSQL OTN download page. Throughout the documentation,
-        the Oracle NoSQL Database Cloud Service and Cloud Simulator are referred to as
-        the "cloud service" while the Oracle NoSQL Database is referred to as
-        "on-premise." In the `API reference <https://nosql-python-sdk.readthedocs.io/en/
-        stable/api.html>`_ classes and interfaces are noted if they are only relevant to
-        a specific environment.
-        
-        The on-premise configuration requires a running instance of the Oracle NoSQL
-        database. In addition a running proxy service is required. See `Oracle NoSQL
-        Database Downloads <https://www.oracle.com/database/technologies/nosql-database-
-        server-downloads.html>`_ for downloads, and see `Information about the proxy
-        <https://docs.oracle.com/pls/topic/lookup?ctx=en/database/other-databases/nosql-
-        database/21.2/admin&id=NSADM-GUID-C110AF57-8B35-4C48-A82E-2621C6A5ED72>`_ for
-        proxy configuration information.
-        
-        This project is open source and maintained by Oracle Corp. The home page for the
-        project is `here <https://nosql-python-sdk.readthedocs.io/en/stable/index.
-        html>`_.
-        
-        ============
-        Installation
-        ============
-        
-        The SDK can be installed using pip. If using Python 3 the command may be pip3::
-        
-            pip install borneo
-        
-        If you are using the Oracle NoSQL Database cloud service you will also need to
-        install the oci package::
-        
-            pip install oci
-        
-        See `the installation guide <https://nosql-python-sdk.readthedocs.io/en/stable/
-        installation.html>`_ for additional requirements and and alternative install
-        methods.
-        
-        ========
-        Examples
-        ========
-        
-        Examples can be found `on GitHub <https://github.com/oracle/nosql-python-sdk/
-        tree/master/examples>`_.
-        
-        Examples include simple, standalone programs. They include comments bout how
-        they can be configured and run in the different supported environments.
-        
-        =============
-        Documentation
-        =============
-        
-        The `documentation <https://nosql-python-sdk.readthedocs.io/en/stable>`_ has
-        information on using the SDK as well as an `API reference <https://nosql-python-
-        sdk.readthedocs.io/en/stable/api.html>`_ describing the classes.
-        
-        =======
-        Changes
-        =======
-        
-        See the `Changelog <https://github.com/oracle/nosql-python-sdk/blob/master/
-        CHANGELOG.rst>`_.
-        
-        ====
-        Help
-        ====
-        
-         * Open an issue in the `Issues <https://github.com/oracle/nosql-python-sdk/
-           issues>`_ page.
-         * Email to nosql_sdk_help_grp@oracle.com.
-         * `Oracle NoSQL Developer Forum <https://community.oracle.com/community/
-           groundbreakers/database/nosql_database>`_.
-        
-        When requesting help please be sure to include as much detail as possible,
-        including version of the SDK and **simple**, standalone example code as needed.
-        
-        ==========
-        Quickstart
-        ==========
-        
-        The following is a quick start tutorial to run a simple program in the supported
-        environments. The same template source code is used for all environments. The
-        first step is to cut the program below and paste it into an editor for minor
-        modifications. The instructions assume that is stored as quickstart.py, but you
-        can use any name you like. The quickstart example supports 3 environments:
-        
-        1. Oracle NoSQL Database Cloud Service
-        2. Oracle NoSQL Cloud Simulator
-        3. Oracle NoSQL Database on-premise, using the proxy server
-        
-        See `Running Quickstart`_ to
-        run the quickstart program in different environments. The instructions assume
-        that the *borneo* package has been installed.
-        
-        .. code-block:: pycon
-        
-            #
-            # Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
-            #
-            # Licensed under the Universal Permissive License v 1.0 as shown at
-            #  https://oss.oracle.com/licenses/upl/
-            #
-        
-            #
-            # This is a simple quickstart to demonstrate use of the Python driver for
-            # the Oracle NoSQL Database. It can be used to run against the Oracle NoSQL
-            # Database Cloud Service, against the Cloud Simulator, or against an
-            # on-premise Oracle NoSQL database.
-            #
-            # Usage:
-            #   python quickstart.py <cloud | cloudsim | kvstore>
-            #
-            # Use cloud for the Cloud Service
-            # Use cloudsim for the Cloud Simulator
-            # Use kvstore for the on-premise database
-            #
-            # This example is not intended to be an exhaustive overview of the API,
-            # which has a number of additional operations.
-            #
-            # Requirements:
-            #  1. Python 2.7 or 3.5+
-            #  2. Python dependencies (install using pip or other mechanism):
-            #   o requests
-            #   o oci (only if running against the Cloud Service)
-            #  3. If running against the Cloud Simulator, it can be downloaded from
-            #  here:
-            #   http://www.oracle.com/technetwork/topics/cloud/downloads/index.html
-            #  It requires Java
-            #  4. If running against the Oracle NoSQL Database Cloud Service an account
-            #  must be used.
-            #
-        
-            import sys
-        
-            from borneo import (
-                AuthorizationProvider, DeleteRequest, GetRequest,
-                IllegalArgumentException, NoSQLHandle, NoSQLHandleConfig, PutRequest,
-                QueryRequest, Regions, TableLimits, TableRequest)
-            from borneo.iam import SignatureProvider
-            from borneo.kv import StoreAccessTokenProvider
-        
-        
-            #
-            # EDIT: these values based on desired region and/or endpoint for a local
-            # server
-            #
-            cloud_region = Regions.EU_ZURICH_1
-            cloudsim_endpoint = 'localhost:8080'
-            kvstore_endpoint = 'localhost:80'
-            cloudsim_id = 'cloudsim'  # a fake user id/namespace for the Cloud Simulator
-        
-            # Cloud Service Only
-            #
-            # EDIT: set these variables to the credentials to use if you are not using
-            # a configuration file in ~/.oci/config
-            # Use of these credentials vs a file is determined by a value of tenancy
-            # other than None.
-            #
-            tenancy = None  # tenancy'd OCID (string)
-            user = None  # user's OCID (string)
-            private_key = 'path-to-private-key-or-private-key-content'
-            fingerprint = 'fingerprint for uploaded public key'
-            # pass phrase (string) for private key, or None if not set
-            pass_phrase = None
-        
-        
-            class CloudsimAuthorizationProvider(AuthorizationProvider):
-                """
-                Cloud Simulator Only.
-        
-                This class is used as an AuthorizationProvider when using the Cloud
-                Simulator, which has no security configuration. It accepts a string
-                tenant_id that is used as a simple namespace for tables.
-                """
-        
-                def __init__(self, tenant_id):
-                    super(CloudsimAuthorizationProvider, self).__init__()
-                    self._tenant_id = tenant_id
-        
-                def close(self):
-                    pass
-        
-                def get_authorization_string(self, request=None):
-                    return 'Bearer ' + self._tenant_id
-        
-        
-            def get_handle(nosql_env):
-                """
-                Returns a NoSQLHandle based on the requested environment. The
-                differences among the supported environments are encapsulated in this
-                method.
-                """
-                if nosql_env == 'cloud':
-                    endpoint = cloud_region
-                    #
-                    # Get credentials using SignatureProvider. SignatureProvider has
-                    # several ways to accept credentials. See the documentation:
-                    #  https://nosql-python-sdk.readthedocs.io/en/stable/api/borneo.iam.SignatureProvider.html
-                    #
-                    if tenancy is not None:
-                        print('Using directly provided credentials')
-                        #
-                        # Credentials are provided directly
-                        #
-                        provider = SignatureProvider(tenant_id=tenancy,
-                                                     user_id=user,
-                                                     fingerprint=fingerprint,
-                                                     private_key=private_key,
-                                                     pass_phrase=pass_phrase)
-                    else:
-                        #
-                        # Credentials will come from a file.
-                        #
-                        # By default the file is ~/.oci/config. A config_file = <path>
-                        # argument can be passed to specify a different file.
-                        #
-                        print('Using credentials and DEFAULT profile from ' +
-                              '~/.oci/config')
-                        provider = SignatureProvider()
-                elif nosql_env == 'cloudsim':
-                    print('Using cloud simulator endpoint ' + cloudsim_endpoint)
-                    endpoint = cloudsim_endpoint
-                    provider = CloudsimAuthorizationProvider(cloudsim_id)
-        
-                elif nosql_env == 'kvstore':
-                    print('Using on-premise endpoint ' + kvstore_endpoint)
-                    endpoint = kvstore_endpoint
-                    provider = StoreAccessTokenProvider()
-        
-                else:
-                    raise IllegalArgumentException('Unknown environment: ' + nosql_env)
-        
-                return NoSQLHandle(NoSQLHandleConfig(endpoint, provider))
-        
-        
-            def main():
-        
-                table_name = 'PythonQuickstart'
-        
-                if len(sys.argv) != 2:
-                    print('Usage: python quickstart.py <cloud | cloudsim | kvstore>')
-                    raise SystemExit
-        
-                nosql_env = sys.argv[1:][0]
-                print('Using environment: ' + str(nosql_env))
-        
-                handle = None
-                try:
-        
-                    #
-                    # Create a handle
-                    #
-                    handle = get_handle(nosql_env)
-        
-                    #
-                    # Create a table
-                    #
-                    statement = (
-                        'Create table if not exists {} (id integer, sid integer, ' +
-                        'name string, primary key(shard(sid), id))').format(table_name)
-                    request = TableRequest().set_statement(statement).set_table_limits(
-                        TableLimits(30, 10, 1))
-                    handle.do_table_request(request, 50000, 3000)
-                    print('After create table')
-        
-                    #
-                    # Put a few rows
-                    #
-                    request = PutRequest().set_table_name(table_name)
-                    for i in range(10):
-                        value = {'id': i, 'sid': 0, 'name': 'myname' + str(i)}
-                        request.set_value(value)
-                        handle.put(request)
-                    print('After put of 10 rows')
-        
-                    #
-                    # Get the row
-                    #
-                    request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
-                        table_name)
-                    result = handle.get(request)
-                    print('After get: ' + str(result))
-        
-                    #
-                    # Query, using a range
-                    #
-                    statement = (
-                        'select * from ' + table_name + ' where id > 2 and id < 8')
-                    request = QueryRequest().set_statement(statement)
-                    print('Query results for: ' + statement)
-                    #
-                    # If the :py:meth:`borneo.QueryRequest.is_done` returns False, there
-                    # may be more results, so queries should generally be run in a loop.
-                    # It is possible for single request to return no results but the
-                    # query still not done, indicating that the query loop should
-                    # continue.
-                    #
-                    while True:
-                        result = handle.query(request)
-                        for r in result.get_results():
-                            print('\t' + str(r))
-                        if request.is_done():
-                            break
-        
-                    #
-                    # Delete the row
-                    #
-                    request = DeleteRequest().set_table_name(table_name).set_key(
-                        {'id': 1, 'sid': 0})
-                    result = handle.delete(request)
-                    print('After delete: ' + str(result))
-        
-                    #
-                    # Get again to show deletion
-                    #
-                    request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
-                        table_name)
-                    result = handle.get(request)
-                    print('After get (should be None): ' + str(result))
-        
-                    #
-                    # Drop the table
-                    #
-                    request = TableRequest().set_statement(
-                        'drop table if exists {} '.format(table_name))
-                    result = handle.table_request(request)
-        
-                    #
-                    # Table drop can take time, depending on the state of the system.
-                    # If this wait fails the table will still probably been dropped
-                    #
-                    result.wait_for_completion(handle, 40000, 2000)
-                    print('After drop table')
-        
-                    print('Quickstart is complete')
-                except Exception as e:
-                    print(e)
-                finally:
-                    # If the handle isn't closed Python will not exit properly
-                    if handle is not None:
-                        handle.close()
-        
-        
-            if __name__ == '__main__':
-                main()
-        
-        Running Quickstart
-        ==================
-        
-        Run Against the Oracle NoSQL Database Cloud Service
-        ===================================================
-        
-        Running against the Cloud Service requires an Oracle Cloud account. See
-        `Configure for the Cloud Service <https://nosql-python-sdk.readthedocs.io/en/
-        stable/installation.html#configure-for-the-cloud-service>`_ for information on
-        getting an account and acquiring required credentials.
-        
-        1. Collect the following information:
-        
-         * Tenancy ID
-         * User ID
-         * API signing key (private key file in PEM format)
-         * Fingerprint for the public key uploaded to the user's account
-         * Private key pass phrase, needed only if the private key is encrypted
-        
-        2. Edit *quickstart.py* and add your information. There are 2 ways to supply
-           credentials in the program:
-        
-           * Directly provide the credential information. To use this method, modify the
-             values of the variables at the top of the program: *tenancy*, *user*,
-             *private_key*, *fingerprint*, and *pass_phrase*, setting them to the
-             corresponding information you've collected.
-           * Using a configuration file. In this case the information you've collected
-             goes into a file, ~/.oci/config. `Configure for the Cloud Service <https://
-             nosql-python-sdk.readthedocs.io/en/stable/installation.html#configure-for-
-             the-cloud-service>`_ describes the contents of the file. It will look like
-             this::
-        
-              [DEFAULT]
-              tenancy=<your-tenancy-id>
-              user=<your-user-id>
-              fingerprint=<fingerprint-of-your-public-key>
-              key_file=<path-to-your-private-key-file>
-              pass_phrase=<optional-pass-phrase-for-key-file>
-        
-        3. Decide which region you want to use and modify the *cloud_region* variable to
-           the desired region. See `Regions documentation <https://nosql-python-sdk.
-           readthedocs.io/en/stable/api/borneo.Regions.html>`_ for possible regions. Not
-           all support the Oracle NoSQL Database Cloud Service.
-        
-        4. Run the program:
-        
-        .. code-block:: pycon
-        
-            python quickstart.py cloud
-        
-        Run Against the Oracle NoSQL Cloud Simulator
-        ============================================
-        
-        Running against the Oracle NoSQL Cloud Simulator requires a running Cloud
-        Simulator instance. See `Configure for the Cloud Simulator <https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-cloud-simulator>`_ for information on how to
-        download and start the Cloud Simulator.
-        
-        1. Start the Cloud Simulator based on instructions above. Note the HTTP port
-           used. By default it is *8080* on *localhost*.
-        
-        2. The *quickstart.py* program defaults to *localhost:8080* so if the Cloud
-           Simulator was started using default values no editing is required.
-        
-        3. Run the program:
-        
-        .. code-block:: pycon
-        
-            python quickstart.py cloudsim
-        
-        Run Against Oracle NoSQL on-premise
-        ===================================
-        
-        Running against the Oracle NoSQL Database on-premise requires a running Oracle
-        NoSQL Database instance as well as a running NoSQL Proxy server instance. The
-        program will connect to the proxy server.
-        
-        See `Configure for On-Premise Oracle NoSQL Database <https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-on-premise-oracle-nosql-database>`_ for information on how to
-        download and start the database instance and proxy server. The database and
-        proxy should be started without security enabled for this quickstart program to
-        operate correctly. A secure configuration requires a secure proxy and more
-        complex configuration.
-        
-        1. Start the Oracle NoSQL Database and proxy server based on instructions above.
-           Note the HTTP port used. By default the endpoint is *localhost:80*.
-        
-        2. The *quickstart.py* program defaults to *localhost:80*. If the proxy was
-           started using a different host or port edit the settings accordingly.
-        
-        3. Run the program:
-        
-        .. code-block:: pycon
-        
-            python quickstart.py kvstore
-        
-        =======
-        License
-        =======
-        
-        Copyright (C) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
-        
-        This SDK is licensed under the Universal Permissive License 1.0. See `LICENSE
-        <./LICENSE.txt>`_ for details.
-        
-        ============
-        Contributing
-        ============
-        
-        See `CONTRIBUTING <./CONTRIBUTING.rst>`_
-        
-        ========
-        Security
-        ========
-        
-        See `SECURITY <./SECURITY.rst>`_
-        
 Keywords: database,nosql,cloud,development
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database :: Front-Ends
 Classifier: License :: OSI Approved :: Universal Permissive License (UPL)
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+Oracle NoSQL Database Python SDK
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+=====
+About
+=====
+
+This is the Python SDK for Oracle NoSQL Database. Python versions 3.5+ are
+supported. The SDK provides interfaces, documentation, and examples to help
+develop Python applications that connect to the Oracle NoSQL Database Cloud
+Service, Oracle NoSQL Database and to the Oracle NoSQL Cloud Simulator (which
+runs on a local machine).
+
+In order to run the Oracle NoSQL Cloud Simulator, a separate download is
+necessary from the Oracle NoSQL OTN download page. Throughout the documentation,
+the Oracle NoSQL Database Cloud Service and Cloud Simulator are referred to as
+the "cloud service" while the Oracle NoSQL Database is referred to as
+"on-premise." In the `API reference <https://nosql-python-sdk.readthedocs.io/en/
+stable/api.html>`_ classes and interfaces are noted if they are only relevant to
+a specific environment.
+
+The on-premise configuration requires a running instance of the Oracle NoSQL
+database. In addition a running proxy service is required. See `Oracle NoSQL
+Database Downloads <https://www.oracle.com/database/technologies/nosql-database-
+server-downloads.html>`_ for downloads, and see `Information about the proxy
+<https://docs.oracle.com/pls/topic/lookup?ctx=en/database/other-databases/nosql-
+database/22.3/admin&id=NSADM-GUID-C110AF57-8B35-4C48-A82E-2621C6A5ED72>`_ for
+proxy configuration information.
+
+This project is open source and maintained by Oracle Corp. The home page for the
+project is `here <https://nosql-python-sdk.readthedocs.io/en/stable/index.
+html>`_.
+
+============
+Installation
+============
+
+The SDK can be installed using pip. If using Python 3 the command may be pip3::
+
+    pip install borneo
+
+If you are using the Oracle NoSQL Database cloud service you will also need to
+install the oci package::
+
+    pip install oci
+
+See `the installation guide <https://nosql-python-sdk.readthedocs.io/en/stable/
+installation.html>`_ for additional requirements and and alternative install
+methods.
+
+========
+Examples
+========
+
+Examples can be found `on GitHub <https://github.com/oracle/nosql-python-sdk/
+tree/master/examples>`_.
+
+Examples include simple, standalone programs. They include comments about how
+they can be configured and run in the different supported environments.
+
+=============
+Documentation
+=============
+
+The `documentation <https://nosql-python-sdk.readthedocs.io/en/stable>`_ has
+information on using the SDK as well as an `API reference <https://nosql-python-
+sdk.readthedocs.io/en/stable/api.html>`_ describing the classes.
+
+=======
+Changes
+=======
+
+See the `Changelog <https://github.com/oracle/nosql-python-sdk/blob/master/
+CHANGELOG.rst>`_.
+
+====
+Help
+====
+
+ * Open an issue in the `Issues <https://github.com/oracle/nosql-python-sdk/
+   issues>`_ page.
+ * Email to nosql_sdk_help_grp@oracle.com.
+ * `Oracle NoSQL Developer Forum <https://community.oracle.com/community/
+   groundbreakers/database/nosql_database>`_.
+
+When requesting help please be sure to include as much detail as possible,
+including version of the SDK and **simple**, standalone example code as needed.
+
+==========
+Quickstart
+==========
+
+The following is a quick start tutorial to run a simple program in the supported
+environments. The same template source code is used for all environments. The
+first step is to cut the program below and paste it into an editor for minor
+modifications. The instructions assume that is stored as quickstart.py, but you
+can use any name you like. The quickstart example supports 3 environments:
+
+1. Oracle NoSQL Database Cloud Service
+2. Oracle NoSQL Cloud Simulator
+3. Oracle NoSQL Database on-premise, using the proxy server
+
+See `Running Quickstart`_ to
+run the quickstart program in different environments. The instructions assume
+that the *borneo* package has been installed.
+
+.. code-block:: pycon
+
+    #
+    # Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+    #
+    # Licensed under the Universal Permissive License v 1.0 as shown at
+    #  https://oss.oracle.com/licenses/upl/
+    #
+
+    #
+    # This is a simple quickstart to demonstrate use of the Python driver for
+    # the Oracle NoSQL Database. It can be used to run against the Oracle NoSQL
+    # Database Cloud Service, against the Cloud Simulator, or against an
+    # on-premise Oracle NoSQL database.
+    #
+    # Usage:
+    #   python quickstart.py <cloud | cloudsim | kvstore>
+    #
+    # Use cloud for the Cloud Service
+    # Use cloudsim for the Cloud Simulator
+    # Use kvstore for the on-premise database
+    #
+    # This example is not intended to be an exhaustive overview of the API,
+    # which has a number of additional operations.
+    #
+    # Requirements:
+    #  1. Python 3.5+
+    #  2. Python dependencies (install using pip or other mechanism):
+    #   o requests
+    #   o oci (only if running against the Cloud Service)
+    #  3. If running against the Cloud Simulator, it can be downloaded from
+    #  here:
+    #   http://www.oracle.com/technetwork/topics/cloud/downloads/index.html
+    #  It requires Java
+    #  4. If running against the Oracle NoSQL Database Cloud Service an account
+    #  must be used.
+    #
+
+    import sys
+
+    from borneo import (
+        AuthorizationProvider, DeleteRequest, GetRequest,
+        IllegalArgumentException, NoSQLHandle, NoSQLHandleConfig, PutRequest,
+        QueryRequest, Regions, TableLimits, TableRequest)
+    from borneo.iam import SignatureProvider
+    from borneo.kv import StoreAccessTokenProvider
+
+
+    #
+    # EDIT: these values based on desired region and/or endpoint for a local
+    # server
+    #
+    cloud_region = Regions.EU_ZURICH_1
+    cloudsim_endpoint = 'localhost:8080'
+    kvstore_endpoint = 'localhost:80'
+    cloudsim_id = 'cloudsim'  # a fake user id/namespace for the Cloud Simulator
+
+    # Cloud Service Only
+    #
+    # EDIT: set these variables to the credentials to use if you are not using
+    # a configuration file in ~/.oci/config
+    # Use of these credentials vs a file is determined by a value of tenancy
+    # other than None.
+    #
+    tenancy = None  # tenancy'd OCID (string)
+    user = None  # user's OCID (string)
+    private_key = 'path-to-private-key-or-private-key-content'
+    fingerprint = 'fingerprint for uploaded public key'
+    # pass phrase (string) for private key, or None if not set
+    pass_phrase = None
+
+
+    class CloudsimAuthorizationProvider(AuthorizationProvider):
+        """
+        Cloud Simulator Only.
+
+        This class is used as an AuthorizationProvider when using the Cloud
+        Simulator, which has no security configuration. It accepts a string
+        tenant_id that is used as a simple namespace for tables.
+        """
+
+        def __init__(self, tenant_id):
+            super(CloudsimAuthorizationProvider, self).__init__()
+            self._tenant_id = tenant_id
+
+        def close(self):
+            pass
+
+        def get_authorization_string(self, request=None):
+            return 'Bearer ' + self._tenant_id
+
+
+    def get_handle(nosql_env):
+        """
+        Returns a NoSQLHandle based on the requested environment. The
+        differences among the supported environments are encapsulated in this
+        method.
+        """
+        if nosql_env == 'cloud':
+            endpoint = cloud_region
+            #
+            # Get credentials using SignatureProvider. SignatureProvider has
+            # several ways to accept credentials. See the documentation:
+            #  https://nosql-python-sdk.readthedocs.io/en/stable/api/borneo.iam.SignatureProvider.html
+            #
+            if tenancy is not None:
+                print('Using directly provided credentials')
+                #
+                # Credentials are provided directly
+                #
+                provider = SignatureProvider(tenant_id=tenancy,
+                                             user_id=user,
+                                             fingerprint=fingerprint,
+                                             private_key=private_key,
+                                             pass_phrase=pass_phrase)
+            else:
+                #
+                # Credentials will come from a file.
+                #
+                # By default the file is ~/.oci/config. A config_file = <path>
+                # argument can be passed to specify a different file.
+                #
+                print('Using credentials and DEFAULT profile from ' +
+                      '~/.oci/config')
+                provider = SignatureProvider()
+        elif nosql_env == 'cloudsim':
+            print('Using cloud simulator endpoint ' + cloudsim_endpoint)
+            endpoint = cloudsim_endpoint
+            provider = CloudsimAuthorizationProvider(cloudsim_id)
+
+        elif nosql_env == 'kvstore':
+            print('Using on-premise endpoint ' + kvstore_endpoint)
+            endpoint = kvstore_endpoint
+            provider = StoreAccessTokenProvider()
+
+        else:
+            raise IllegalArgumentException('Unknown environment: ' + nosql_env)
+
+        return NoSQLHandle(NoSQLHandleConfig(endpoint, provider))
+
+
+    def main():
+
+        table_name = 'PythonQuickstart'
+
+        if len(sys.argv) != 2:
+            print('Usage: python quickstart.py <cloud | cloudsim | kvstore>')
+            raise SystemExit
+
+        nosql_env = sys.argv[1:][0]
+        print('Using environment: ' + str(nosql_env))
+
+        handle = None
+        try:
+
+            #
+            # Create a handle
+            #
+            handle = get_handle(nosql_env)
+
+            #
+            # Create a table
+            #
+            statement = (
+                'Create table if not exists {} (id integer, sid integer, ' +
+                'name string, primary key(shard(sid), id))').format(table_name)
+            request = TableRequest().set_statement(statement).set_table_limits(
+                TableLimits(30, 10, 1))
+            handle.do_table_request(request, 50000, 3000)
+            print('After create table')
+
+            #
+            # Put a few rows
+            #
+            request = PutRequest().set_table_name(table_name)
+            for i in range(10):
+                value = {'id': i, 'sid': 0, 'name': 'myname' + str(i)}
+                request.set_value(value)
+                handle.put(request)
+            print('After put of 10 rows')
+
+            #
+            # Get the row
+            #
+            request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
+                table_name)
+            result = handle.get(request)
+            print('After get: ' + str(result))
+
+            #
+            # Query, using a range
+            #
+            statement = (
+                'select * from ' + table_name + ' where id > 2 and id < 8')
+            request = QueryRequest().set_statement(statement)
+            print('Query results for: ' + statement)
+            #
+            # If the :py:meth:`borneo.QueryRequest.is_done` returns False, there
+            # may be more results, so queries should generally be run in a loop.
+            # It is possible for single request to return no results but the
+            # query still not done, indicating that the query loop should
+            # continue.
+            #
+            while True:
+                result = handle.query(request)
+                for r in result.get_results():
+                    print('\t' + str(r))
+                if request.is_done():
+                    break
+
+            #
+            # Delete the row
+            #
+            request = DeleteRequest().set_table_name(table_name).set_key(
+                {'id': 1, 'sid': 0})
+            result = handle.delete(request)
+            print('After delete: ' + str(result))
+
+            #
+            # Get again to show deletion
+            #
+            request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
+                table_name)
+            result = handle.get(request)
+            print('After get (should be None): ' + str(result))
+
+            #
+            # Drop the table
+            #
+            request = TableRequest().set_statement(
+                'drop table if exists {} '.format(table_name))
+            result = handle.table_request(request)
+
+            #
+            # Table drop can take time, depending on the state of the system.
+            # If this wait fails the table will still probably been dropped
+            #
+            result.wait_for_completion(handle, 40000, 2000)
+            print('After drop table')
+
+            print('Quickstart is complete')
+        except Exception as e:
+            print(e)
+        finally:
+            # If the handle isn't closed Python will not exit properly
+            if handle is not None:
+                handle.close()
+
+
+    if __name__ == '__main__':
+        main()
+
+Running Quickstart
+==================
+
+Run Against the Oracle NoSQL Database Cloud Service
+===================================================
+
+Running against the Cloud Service requires an Oracle Cloud account. See
+`Configure for the Cloud Service <https://nosql-python-sdk.readthedocs.io/en/
+stable/installation.html#configure-for-the-cloud-service>`_ for information on
+getting an account and acquiring required credentials.
+
+1. Collect the following information:
+
+ * Tenancy ID
+ * User ID
+ * API signing key (private key file in PEM format)
+ * Fingerprint for the public key uploaded to the user's account
+ * Private key pass phrase, needed only if the private key is encrypted
+
+2. Edit *quickstart.py* and add your information. There are 2 ways to supply
+   credentials in the program:
+
+   * Directly provide the credential information. To use this method, modify the
+     values of the variables at the top of the program: *tenancy*, *user*,
+     *private_key*, *fingerprint*, and *pass_phrase*, setting them to the
+     corresponding information you've collected.
+   * Using a configuration file. In this case the information you've collected
+     goes into a file, ~/.oci/config. `Configure for the Cloud Service <https://
+     nosql-python-sdk.readthedocs.io/en/stable/installation.html#configure-for-
+     the-cloud-service>`_ describes the contents of the file. It will look like
+     this::
+
+      [DEFAULT]
+      tenancy=<your-tenancy-id>
+      user=<your-user-id>
+      fingerprint=<fingerprint-of-your-public-key>
+      key_file=<path-to-your-private-key-file>
+      pass_phrase=<optional-pass-phrase-for-key-file>
+
+3. Decide which region you want to use and modify the *cloud_region* variable to
+   the desired region. See `Regions documentation <https://nosql-python-sdk.
+   readthedocs.io/en/stable/api/borneo.Regions.html>`_ for possible regions. Not
+   all support the Oracle NoSQL Database Cloud Service.
+
+4. Run the program:
+
+.. code-block:: pycon
+
+    python quickstart.py cloud
+
+Run Against the Oracle NoSQL Cloud Simulator
+============================================
+
+Running against the Oracle NoSQL Cloud Simulator requires a running Cloud
+Simulator instance. See `Configure for the Cloud Simulator <https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-cloud-simulator>`_ for information on how to
+download and start the Cloud Simulator.
+
+1. Start the Cloud Simulator based on instructions above. Note the HTTP port
+   used. By default it is *8080* on *localhost*.
+
+2. The *quickstart.py* program defaults to *localhost:8080* so if the Cloud
+   Simulator was started using default values no editing is required.
+
+3. Run the program:
+
+.. code-block:: pycon
+
+    python quickstart.py cloudsim
+
+Run Against Oracle NoSQL on-premise
+===================================
+
+Running against the Oracle NoSQL Database on-premise requires a running Oracle
+NoSQL Database instance as well as a running NoSQL Proxy server instance. The
+program will connect to the proxy server.
+
+See `Configure for On-Premise Oracle NoSQL Database <https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-on-premise-oracle-nosql-database>`_ for information on how to
+download and start the database instance and proxy server. The database and
+proxy should be started without security enabled for this quickstart program to
+operate correctly. A secure configuration requires a secure proxy and more
+complex configuration.
+
+1. Start the Oracle NoSQL Database and proxy server based on instructions above.
+   Note the HTTP port used. By default the endpoint is *localhost:80*.
+
+2. The *quickstart.py* program defaults to *localhost:80*. If the proxy was
+   started using a different host or port edit the settings accordingly.
+
+3. Run the program:
+
+.. code-block:: pycon
+
+    python quickstart.py kvstore
+
+=======
+License
+=======
+
+Copyright (C) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+
+This SDK is licensed under the Universal Permissive License 1.0. See `LICENSE
+<./LICENSE.txt>`_ for details.
+
+============
+Contributing
+============
+
+See `CONTRIBUTING <./CONTRIBUTING.rst>`_
+
+========
+Security
+========
+
+See `SECURITY <./SECURITY.rst>`_
```

### Comparing `borneo-5.3.7/THIRD_PARTY_LICENSES.txt` & `borneo-5.4.1/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `borneo-5.3.7/setup.py` & `borneo-5.4.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,17 +39,17 @@
 
 setup(
     name='borneo',
     url='https://nosql-python-sdk.readthedocs.io/en/stable/index.html',
 
     # Version should match the system release, but may vary as patches
     # are created.
-    version=version,
+    version=str(version),
     description='Oracle NoSQL Database Python SDK',
-    long_description=readme,
+    long_description=str(readme),
     long_description_content_type='text/x-rst',
 
     author='Oracle',
     author_email='george.feinberg@oracle.com',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     include_package_data=True,
@@ -69,15 +69,14 @@
         'Intended Audience :: Developers',
         'Topic :: Database :: Front-Ends',
 
         # License -- must match "license" above
         'License :: OSI Approved :: Universal Permissive License (UPL)',
 
         # Supported Python versions
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
```

### Comparing `borneo-5.3.7/README.rst` & `borneo-5.4.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Oracle NoSQL Database Python SDK
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 =====
 About
 =====
 
-This is the Python SDK for Oracle NoSQL Database. Python 2.7+ and 3.5+ are
+This is the Python SDK for Oracle NoSQL Database. Python versions 3.5+ are
 supported. The SDK provides interfaces, documentation, and examples to help
 develop Python applications that connect to the Oracle NoSQL Database Cloud
 Service, Oracle NoSQL Database and to the Oracle NoSQL Cloud Simulator (which
 runs on a local machine).
 
 In order to run the Oracle NoSQL Cloud Simulator, a separate download is
 necessary from the Oracle NoSQL OTN download page. Throughout the documentation,
@@ -20,15 +20,15 @@
 a specific environment.
 
 The on-premise configuration requires a running instance of the Oracle NoSQL
 database. In addition a running proxy service is required. See `Oracle NoSQL
 Database Downloads <https://www.oracle.com/database/technologies/nosql-database-
 server-downloads.html>`_ for downloads, and see `Information about the proxy
 <https://docs.oracle.com/pls/topic/lookup?ctx=en/database/other-databases/nosql-
-database/21.2/admin&id=NSADM-GUID-C110AF57-8B35-4C48-A82E-2621C6A5ED72>`_ for
+database/22.3/admin&id=NSADM-GUID-C110AF57-8B35-4C48-A82E-2621C6A5ED72>`_ for
 proxy configuration information.
 
 This project is open source and maintained by Oracle Corp. The home page for the
 project is `here <https://nosql-python-sdk.readthedocs.io/en/stable/index.
 html>`_.
 
 ============
@@ -51,15 +51,15 @@
 ========
 Examples
 ========
 
 Examples can be found `on GitHub <https://github.com/oracle/nosql-python-sdk/
 tree/master/examples>`_.
 
-Examples include simple, standalone programs. They include comments bout how
+Examples include simple, standalone programs. They include comments about how
 they can be configured and run in the different supported environments.
 
 =============
 Documentation
 =============
 
 The `documentation <https://nosql-python-sdk.readthedocs.io/en/stable>`_ has
@@ -126,15 +126,15 @@
     # Use cloudsim for the Cloud Simulator
     # Use kvstore for the on-premise database
     #
     # This example is not intended to be an exhaustive overview of the API,
     # which has a number of additional operations.
     #
     # Requirements:
-    #  1. Python 2.7 or 3.5+
+    #  1. Python 3.5+
     #  2. Python dependencies (install using pip or other mechanism):
     #   o requests
     #   o oci (only if running against the Cloud Service)
     #  3. If running against the Cloud Simulator, it can be downloaded from
     #  here:
     #   http://www.oracle.com/technetwork/topics/cloud/downloads/index.html
     #  It requires Java
@@ -450,15 +450,15 @@
 
     python quickstart.py kvstore
 
 =======
 License
 =======
 
-Copyright (C) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+Copyright (C) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
 
 This SDK is licensed under the Universal Permissive License 1.0. See `LICENSE
 <./LICENSE.txt>`_ for details.
 
 ============
 Contributing
 ============
```

### Comparing `borneo-5.3.7/CHANGELOG.rst` & `borneo-5.4.1/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,51 @@
 Change Log
 ~~~~~~~~~~
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog <http://keepachangelog.com/>`_.
 ====================
+
+====================
+ 5.4.1 - 2023-08-01
+====================
+
+IMPORTANT: This release drops support for Python 2 and supports only Python
+3.5 and higher
+
+Added
+_____
+* Cloud only: New regions: mx-monterrey-1, eu-frankfurt-2,
+  eu-madrid-2, eu-jovanovac-1, eu-dcc-rome-1, eu-dcc-zurich-1, us-dcc-phoenix-4,
+  us-saltlake-2, sa-valparaiso-1
+* Support for new, flexible wire protocol (V4) has been added. The previous protocol
+is still supported for communication with servers that do not yet support V4. The
+version negotation is internal and automatic; however, use of V4 features will fail
+at runtime when attempted with an older server. Failure may be an empty or
+undefined result or an exception if the request cannot be serviced at all. The following
+new features or interfaces depend on the new protocol version
+ * added set/get_durability to QueryRequest for queries that modify data
+ * added pagination information to TableUsageResult and TableUsageRequest
+ * added shard percent usage information to TableUsageResult
+ * added IndexInfo.get_field_types to return the type information on an index on a JSON
+field
+ * added the ability to ask for and receive the schema of a query using
+     * PrepareRequest.set_get_query_schema
+     * PreparedStatement.get_query_schema
+ * Cloud only: added use of ETags, DefinedTags and FreeFormTags in TableRequest and TableResult
+* On-premises only. Added support for default namespace and per-request namespace
+  specification
+
+
+Changed
+_______
+
+* Dropped support for Python 2.x
+
+====================
  5.3.7 - 2022-12-12
 ====================
 
 NOTE: version 5.3.6 was skipped
 
 Fixed
 -----
```

### Comparing `borneo-5.3.7/LICENSE.txt` & `borneo-5.4.1/LICENSE.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Copyright (c) 2018-2022 Oracle and/or its affiliates.  All rights reserved.
+Copyright (c) 2018-2023 Oracle and/or its affiliates.  All rights reserved.
 
 The Universal Permissive License (UPL), Version 1.0
 
-Subject to the condition set forth below, permission is hereby granted to any person obtaining a copy of this
-software, associated documentation and/or data (collectively the "Software"), free of charge and under any and
-all copyright rights in the Software, and any and all patent rights owned or freely licensable by each licensor
-hereunder covering either (i) the unmodified Software as contributed to or provided by such licensor, or
-(ii) the Larger Works (as defined below), to deal in both
+Subject to the condition set forth below, permission is hereby granted to any person obtaining a copy
+of this software, associated documentation and/or data (collectively the "Software"), free of charge and
+under any and all copyright rights in the Software, and any and all patent rights owned or freely licensable
+by each licensor hereunder covering either (i) the unmodified Software as contributed to or provided by such
+licensor, or (ii) the Larger Works (as defined below), to deal in both
 
 (a) the Software, and
-(b) any piece of software and/or hardware listed in the lrgrwrks.txt file if one is included with the Software
-(each a “Larger Work” to which the Software is contributed by such licensors),
-
-without restriction, including without limitation the rights to copy, create derivative works of, display,
-perform, and distribute the Software and make, use, sell, offer for sale, import, export, have made, and have
-sold the Software and the Larger Work(s), and to sublicense the foregoing rights on either these or other terms.
+(b) any piece of software and/or hardware listed in the lrgrwrks.txt file if one is included with the
+Software (each a “Larger Work” to which the Software is contributed by such licensors), without restriction,
+including without limitation the rights to copy, create derivative works of, display, perform, and distribute
+the Software and make, use, sell, offer for sale, import, export, have made, and have sold the Software and
+the Larger Work(s), and to sublicense the foregoing rights on either these or other terms.
 
 This license is subject to the following condition:
-The above copyright notice and either this complete permission notice or at a minimum a reference to the UPL must
-be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
-CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
-IN THE SOFTWARE.
+The above copyright notice and either this complete permission notice or at a minimum a reference to the UPL
+must be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
```

### Comparing `borneo-5.3.7/src/borneo/auth.py` & `borneo-5.4.1/src/borneo/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from abc import ABCMeta, abstractmethod
```

### Comparing `borneo-5.3.7/src/borneo/exception.py` & `borneo-5.4.1/src/borneo/exception.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 
 class IllegalArgumentException(RuntimeError):
```

### Comparing `borneo-5.3.7/src/borneo/config.py` & `borneo-5.4.1/src/borneo/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 #
-# Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from abc import ABCMeta, abstractmethod
 from copy import deepcopy
-from enum import Enum
 from os import getenv
 from random import random
 from ssl import SSLContext
 from time import sleep, time
+
+from enum import Enum
 from typing import Callable
 
 try:
     # noinspection PyCompatibility
     from urlparse import urlparse
 except ImportError:
     # noinspection PyUnresolvedReferences,PyCompatibility
     from urllib.parse import urlparse
 
 from .auth import AuthorizationProvider
 from .common import CheckValue, Consistency
 from .exception import (
     IllegalArgumentException, OperationThrottlingException, RetryableException)
 from .operations import Request
+from .serdeutil import SerdeUtil
 
 try:
     from . import iam
 except ImportError:
     import iam
 
 
@@ -240,14 +242,18 @@
     OC5_EP_BASE = 'https://nosql.{0}.oci.oraclecloud5.com'
     OC8_EP_BASE = 'https://nosql.{0}.oci.oraclecloud8.com'
     OC9_EP_BASE = 'https://nosql.{0}.oci.oraclecloud9.com'
     OC10_EP_BASE = 'https://nosql.{0}.oci.oraclecloud10.com'
     OC14_EP_BASE = 'https://nosql.{0}.oci.oraclecloud14.com'
     OC16_EP_BASE = 'https://nosql.{0}.oci.oraclecloud16.com'
     OC17_EP_BASE = 'https://nosql.{0}.oci.oraclecloud17.com'
+    OC19_EP_BASE = 'https://nosql.{0}.oci.oraclecloud.eu'
+    OC20_EP_BASE = 'https://nosql.{0}.oci.oraclecloud20.com'
+    OC22_EP_BASE = 'https://nosql.{0}.oci.oraclecloud22.com'
+    OC24_EP_BASE = 'https://nosql.{0}.oci.oraclecloud24.com'
 
     def __init__(self, region_id):
         self._region_id = region_id
 
     def endpoint(self):
         """
         Returns the NoSQL Database Cloud Service endpoint string for this
@@ -276,14 +282,22 @@
             return str.format(Region.OC10_EP_BASE, self._region_id)
         if self._is_oc14_region():
             return str.format(Region.OC14_EP_BASE, self._region_id)
         if self._is_oc16_region():
             return str.format(Region.OC16_EP_BASE, self._region_id)
         if self._is_oc17_region():
             return str.format(Region.OC17_EP_BASE, self._region_id)
+        if self._is_oc19_region():
+            return str.format(Region.OC19_EP_BASE, self._region_id)
+        if self._is_oc20_region():
+            return str.format(Region.OC20_EP_BASE, self._region_id)
+        if self._is_oc22_region():
+            return str.format(Region.OC22_EP_BASE, self._region_id)
+        if self._is_oc24_region():
+            return str.format(Region.OC24_EP_BASE, self._region_id)
         raise IllegalArgumentException(
             'Unable to find endpoint for unknown region ' + self._region_id)
 
     def get_region_id(self):
         """
         Internal use only.
 
@@ -334,14 +348,30 @@
         # Internal use only
         return Regions.OC16_REGIONS.get(self._region_id) is not None
 
     def _is_oc17_region(self):
         # Internal use only
         return Regions.OC17_REGIONS.get(self._region_id) is not None
 
+    def _is_oc19_region(self):
+        # Internal use only
+        return Regions.OC19_REGIONS.get(self._region_id) is not None
+
+    def _is_oc20_region(self):
+        # Internal use only
+        return Regions.OC20_REGIONS.get(self._region_id) is not None
+
+    def _is_oc22_region(self):
+        # Internal use only
+        return Regions.OC22_REGIONS.get(self._region_id) is not None
+
+    def _is_oc24_region(self):
+        # Internal use only
+        return Regions.OC24_REGIONS.get(self._region_id) is not None
+
 
 class Regions(object):
     """
     Cloud service only.
 
     The class contains the regions in the Oracle Cloud Infrastructure at the
     time of this release. The Oracle NoSQL Database Cloud Service is not
@@ -427,35 +457,41 @@
     ME_DUBAI_1 = Region('me-dubai-1')
     """Region Location: Dubai, UAE"""
     ME_JEDDAH_1 = Region('me-jeddah-1')
     """Region Location: Jeddah, Saudi Arabia"""
 
     MX_QUERETARO_1 = Region('mx-queretaro-1')
     """Region Location: Queretaro, Mexico"""
+    MX_MONTERREY_1 = Region('mx-monterrey-1')
+    """Region Location: Monterrey, Mexico"""
 
     IL_JERUSALEM_1 = Region('il-jerusalem-1')
     """Region Location: Jerusalem, Israel"""
 
     US_ASHBURN_1 = Region('us-ashburn-1')
     """Region Location: Ashburn, VA"""
+    US_CHICAGO_1 = Region('us-chicago-1')
+    """Region Location: Chicago, IL """
     US_PHOENIX_1 = Region('us-phoenix-1')
     """Region Location: Phoenix, AZ"""
+    US_SALTLAKE_2 = Region('us-saltlake-2')
+    """Region Location: Salt Lake City, UT """
     US_SANJOSE_1 = Region('us-sanjose-1')
-    """Region Location: Phoenix, AZ """
-    US_CHICAGO_1 = Region('us-chicago-1')
-    """Region Location: Chicago, IL """
+    """Region Location: San Jose, CA, AZ """
     CA_MONTREAL_1 = Region('ca-montreal-1')
     """Region Location: Montreal, Canada"""
     CA_TORONTO_1 = Region('ca-toronto-1')
     """Region Location: Toronto, Canada"""
 
     SA_SANTIAGO_1 = Region('sa-santiago-1')
     """Region Location: Santiago, Chile"""
     SA_SAOPAULO_1 = Region('sa-saopaulo-1')
     """Region Location: Sao Paulo, Brazil"""
+    SA_VALPARAISO_1 = Region('sa-valparaiso-1')
+    """Region Location: Valparaiso, Chile"""
     SA_VINHEDO_1 = Region('sa-vinhedo-1')
     """Region Location: Vinhedo, Brazil"""
 
     # OC2
     US_LANGLEY_1 = Region('us-langley-1')
     """Region Location: Ashburn, VA"""
     US_LUKE_1 = Region('us-luke-1')
@@ -512,14 +548,34 @@
     """Region Location: Utah"""
 
     # OC17
     US_DCC_PHOENIX_1 = Region('us-dcc-phoenix-1')
     """Region Location: Phoenix, AZ"""
     US_DCC_PHOENIX_2 = Region('us-dcc-phoenix-2')
     """Region Location: Phoenix, AZ"""
+    US_DCC_PHOENIX_4 = Region('us-dcc-phoenix-4')
+    """Region Location: Phoenix, AZ"""
+
+    # OC19
+    EU_FRANKFURT_2 = Region('eu-frankfurt-2')
+    """Region Location: Frankfurt, Germany"""
+    EU_MADRID_2 = Region('eu-madrid-2')
+    """Region Location: Madrid, Spain"""
+
+    # OC20
+    EU_JOVANOVAC_1 = Region('eu-jovanovac-1')
+    """Region Location: Serbia"""
+
+    # OC22
+    EU_DCC_ROME_1 = Region('eu-dcc-rome-1')
+    """Region Location: Rome, Italy"""
+
+    # OC24
+    EU_DCC_ZURICH_1 = Region('eu-dcc-zurich-1')
+    """Region Location: Zurich, Switzerland"""
 
     # OC1
     OC1_REGIONS = dict()
     """A dict containing the OC1 regions."""
     OC1_REGIONS[AF_JOHANNESBURG_1.get_region_id()] = AF_JOHANNESBURG_1
     # APAC
     OC1_REGIONS[AP_CHUNCHEON_1.get_region_id()] = AP_CHUNCHEON_1
@@ -547,24 +603,27 @@
     OC1_REGIONS[EU_PARIS_1.get_region_id()] = EU_PARIS_1
     OC1_REGIONS[EU_STOCKHOLM_1.get_region_id()] = EU_STOCKHOLM_1
     OC1_REGIONS[EU_ZURICH_1.get_region_id()] = EU_ZURICH_1
 
     # LAD
     OC1_REGIONS[SA_SANTIAGO_1.get_region_id()] = SA_SANTIAGO_1
     OC1_REGIONS[SA_SAOPAULO_1.get_region_id()] = SA_SAOPAULO_1
+    OC1_REGIONS[SA_VALPARAISO_1.get_region_id()] = SA_VALPARAISO_1
     OC1_REGIONS[SA_VINHEDO_1.get_region_id()] = SA_VINHEDO_1
 
     # North America
     OC1_REGIONS[US_ASHBURN_1.get_region_id()] = US_ASHBURN_1
     OC1_REGIONS[CA_MONTREAL_1.get_region_id()] = CA_MONTREAL_1
+    OC1_REGIONS[US_CHICAGO_1.get_region_id()] = US_CHICAGO_1
     OC1_REGIONS[US_PHOENIX_1.get_region_id()] = US_PHOENIX_1
     OC1_REGIONS[US_SANJOSE_1.get_region_id()] = US_SANJOSE_1
-    OC1_REGIONS[US_CHICAGO_1.get_region_id()] = US_CHICAGO_1
+    OC1_REGIONS[US_SALTLAKE_2.get_region_id()] = US_SALTLAKE_2
     OC1_REGIONS[CA_TORONTO_1.get_region_id()] = CA_TORONTO_1
     OC1_REGIONS[MX_QUERETARO_1.get_region_id()] = MX_QUERETARO_1
+    OC1_REGIONS[MX_MONTERREY_1.get_region_id()] = MX_MONTERREY_1
 
     OC2_REGIONS = dict()
     """A dict containing the OC2 regions."""
     # OC2
     OC2_REGIONS[US_LANGLEY_1.get_region_id()] = US_LANGLEY_1
     OC2_REGIONS[US_LUKE_1.get_region_id()] = US_LUKE_1
 
@@ -618,14 +677,36 @@
     OC16_REGIONS[US_WESTJORDAN_1.get_region_id()] = US_WESTJORDAN_1
 
     # OC17
     OC17_REGIONS = dict()
     """A dict containing the OC17 regions."""
     OC17_REGIONS[US_DCC_PHOENIX_1.get_region_id()] = US_DCC_PHOENIX_1
     OC17_REGIONS[US_DCC_PHOENIX_2.get_region_id()] = US_DCC_PHOENIX_2
+    OC17_REGIONS[US_DCC_PHOENIX_4.get_region_id()] = US_DCC_PHOENIX_4
+
+    # OC19
+    OC19_REGIONS = dict()
+    """A dict containing the OC19 regions."""
+    OC19_REGIONS[EU_FRANKFURT_2.get_region_id()] = EU_FRANKFURT_2
+    OC19_REGIONS[EU_MADRID_2.get_region_id()] = EU_MADRID_2
+
+    # OC20
+    OC20_REGIONS = dict()
+    """A dict containing the OC20 regions."""
+    OC20_REGIONS[EU_JOVANOVAC_1.get_region_id()] = EU_JOVANOVAC_1
+
+    # OC22
+    OC22_REGIONS = dict()
+    """A dict containing the OC22 regions."""
+    OC22_REGIONS[EU_DCC_ROME_1.get_region_id()] = EU_DCC_ROME_1
+
+    # OC24
+    OC24_REGIONS = dict()
+    """A dict containing the OC22 regions."""
+    OC24_REGIONS[EU_DCC_ZURICH_1.get_region_id()] = EU_DCC_ZURICH_1
 
     @staticmethod
     def get_oc1_regions():
         # Internal use only
         return Regions.OC1_REGIONS.values()
 
     @staticmethod
@@ -675,14 +756,34 @@
 
     @staticmethod
     def get_oc17_regions():
         # Internal use only
         return Regions.OC17_REGIONS.values()
 
     @staticmethod
+    def get_oc19_regions():
+        # Internal use only
+        return Regions.OC19_REGIONS.values()
+
+    @staticmethod
+    def get_oc20_regions():
+        # Internal use only
+        return Regions.OC20_REGIONS.values()
+
+    @staticmethod
+    def get_oc22_regions():
+        # Internal use only
+        return Regions.OC22_REGIONS.values()
+
+    @staticmethod
+    def get_oc24_regions():
+        # Internal use only
+        return Regions.OC24_REGIONS.values()
+
+    @staticmethod
     def from_region_id(region_id):
         """
         Returns the Region associated with the string value supplied, or None if
         the string does not represent a known region.
 
         :param region_id: the string value of the region.
         :type region_id: str
@@ -710,18 +811,25 @@
             region = Regions.OC10_REGIONS.get(region_id)
         if region is None:
             region = Regions.OC14_REGIONS.get(region_id)
         if region is None:
             region = Regions.OC16_REGIONS.get(region_id)
         if region is None:
             region = Regions.OC17_REGIONS.get(region_id)
+        if region is None:
+            region = Regions.OC19_REGIONS.get(region_id)
+        if region is None:
+            region = Regions.OC20_REGIONS.get(region_id)
+        if region is None:
+            region = Regions.OC22_REGIONS.get(region_id)
+        if region is None:
+            region = Regions.OC24_REGIONS.get(region_id)
         return region
 
 
-# python 2.7 ??? class StatsProfile(object):
 class StatsProfile(Enum):
     """
     The following semantics are attached to the StatsProfile values:
        - NONE: no stats are logged.
        - REGULAR: per request: counters, errors, latencies, delays, retries
        - MORE: stats above plus 95th and 99th percentile latencies.
        - ALL: stats above plus per query information
@@ -868,43 +976,32 @@
         self._proxy_password = None
         self._ssl_ca_certs = None
         self._ssl_ciphers = None
         self._ssl_ctx = None
         self._ssl_protocol = None
         self._logger = None
         self._is_default_logger = True
+        self._serial_version = SerdeUtil.DEFAULT_SERIAL_VERSION
+        self._default_namespace = None
 
         profile_property = getenv(self._STATS_PROFILE_PROPERTY,
-            self._DEFAULT_STATS_PROFILE.name.lower())
+                                  self._DEFAULT_STATS_PROFILE.name.lower())
         try:
             self._stats_profile = StatsProfile[profile_property.upper()]
         except KeyError:
             self._stats_profile = StatsProfile.NONE
-        # python2.7 ???
-        # "none" is the value of: self._DEFAULT_STATS_PROFILE.name.lower()
-        # profile_property = getenv(self._STATS_PROFILE_PROPERTY, "none").upper()
-        # if "NONE" == profile_property:
-        #     self._stats_profile = StatsProfile.NONE
-        # elif "REGULAR" == profile_property:
-        #     self._stats_profile = StatsProfile.REGULAR
-        # elif "MORE" == profile_property:
-        #     self._stats_profile = StatsProfile.MORE
-        # elif "ALL" == profile_property:
-        #     self._stats_profile = StatsProfile.ALL
-        # else:
-        #     self._stats_profile = StatsProfile.NONE
-
 
         self._stats_interval = getenv(self._STATS_INTERVAL_PROPERTY,
-            self._DEFAULT_STATS_INTERVAL)
+                                      self._DEFAULT_STATS_INTERVAL)
         self._stats_interval = int(self._stats_interval)
 
         self._stats_pretty_print = getenv(self._STATS_PRETTY_PRINT_PROPERTY,
-            self._DEFAULT_STATS_PRETTY_PRINT)
+                                          self._DEFAULT_STATS_PRETTY_PRINT)
         self._stats_pretty_print = bool(self._stats_pretty_print)
+        # noinspection PyTypeChecker
         self._stats_handler = None  # type: Callable
 
     def get_service_url(self):
         """
         Returns the url to use for the :py:class:`NoSQLHandle` connection.
 
         :returns: the url.
@@ -1627,15 +1724,15 @@
         Registers a user defined stats handler. The handler is called at the end
         of the interval with a structure containing the logged stat values.
 
         Note: setting a stats handler will not affect the stats log entries.
         """
         if not isinstance(stats_handler, Callable):
             raise IllegalArgumentException(
-                'stats_hadler must be of Callable type')
+                'stats_handler must be of Callable type')
         self._stats_handler = stats_handler
         return self
 
     def get_stats_handler(self):
         # type: (...) -> Callable
         """
         Returns the registered stats handler.
@@ -1692,7 +1789,40 @@
         """
         Enable JSON pretty print for easier human reading.
         Default is disabled.
         """
         CheckValue.check_boolean(pretty_print, "pretty_print")
         self._stats_pretty_print = pretty_print
         return self
+
+    def get_serial_version(self):
+        return self._serial_version
+
+    def set_serial_version(self, version):
+        self._serial_version = version
+
+    def set_default_namespace(self, namespace):
+        """
+        On-premises only.
+
+        Sets the default namespace to use for requests that use a table
+        name
+
+        :param namespace: the default namespace.
+        :type namespace: str
+        :returns: self
+        :versionadded: 5.4.0
+        """
+        self._default_namespace = namespace
+        return self
+
+    def get_default_namespace(self):
+        """
+        On-premises only.
+
+        Returns the default namespace or None if not set.
+
+        :returns: the default namespace or None.
+        :rtype: str
+        :versionadded: 5.4.0
+        """
+        return self._default_namespace
```

### Comparing `borneo-5.3.7/src/borneo/kv/exception.py` & `borneo-5.4.1/src/borneo/kv/exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from borneo.exception import NoSQLException
```

### Comparing `borneo-5.3.7/src/borneo/kv/kv.py` & `borneo-5.4.1/src/borneo/kv/kv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #
-# Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from base64 import b64encode
 from json import loads
-from requests import ConnectionError, Session, codes
 from threading import Lock, Timer
 from time import time
 from traceback import format_exc
+
+from requests import ConnectionError, Session, codes
+
 try:
     # noinspection PyCompatibility
     from urlparse import urlparse
 except ImportError:
     # noinspection PyUnresolvedReferences,PyCompatibility
     from urllib.parse import urlparse
```

### Comparing `borneo-5.3.7/src/borneo/query.py` & `borneo-5.4.1/src/borneo/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #
-# Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from abc import ABCMeta, abstractmethod
-from datetime import datetime
 from collections import OrderedDict
+from datetime import datetime
 from decimal import Decimal, setcontext
-from sys import getsizeof, version_info
-
-try:
-    from sys import maxint as maxvalue
-except ImportError:
-    from sys import maxsize as maxvalue
+from sys import getsizeof
+from sys import maxsize as maxvalue
 
 from .common import ByteOutputStream, CheckValue, Empty, JsonNone, enum
 from .exception import (
     IllegalArgumentException, IllegalStateException, NoSQLException,
     QueryException, QueryStateException, RetryableException)
 
+from .serdeutil import SerdeUtil
+
 try:
     from . import serde
 except ImportError:
     import serde
 
 
 class PlanIterState(object):
@@ -293,15 +291,15 @@
         if PlanIter.TRACEDESER:
             print('Done Deserializing ' + value + ' iter')
         return op_iter
 
     @staticmethod
     def deserialize_iters(bis):
         iters = list()
-        num_args = serde.BinaryProtocol.read_sequence_length(bis)
+        num_args = SerdeUtil.read_sequence_length(bis)
         count = 0
         while count < num_args:
             iters.append(PlanIter.deserialize_iter(bis))
             count += 1
         return iters
 
     @staticmethod
@@ -326,15 +324,15 @@
             raise IllegalArgumentException(
                 str(index) + 'is invalid, it must be in a range 0 ~ ' +
                 str(num_values))
         return index
 
     @staticmethod
     def read_sort_specs(bis):
-        length = serde.BinaryProtocol.read_sequence_length(bis)
+        length = SerdeUtil.read_sequence_length(bis)
         if length == -1:
             return None
         specs = list()
         count = 0
         while count < length:
             specs.append(SortSpec(bis))
             count += 1
@@ -464,15 +462,15 @@
         self._ordinal = bis.read_short_int()
         self._code = self._ordinal
         """
         Whether this iterator performs addition/subtraction or
         multiplication/division.
         """
         self._args = self.deserialize_iters(bis)
-        self._ops = serde.BinaryProtocol.read_string(bis)
+        self._ops = SerdeUtil.read_string(bis)
         """
         If self._code == PlanIter.FUNC_CODE.OP_ADD_SUB, self._ops is a string of
         '+' and/or '-' chars, containing one such char per input value. For
         example, if the arithmetic expression is (arg1 + arg2 - arg3 + arg4)
         self._ops is '++-+'.
 
         If self._code == PlanIter.FUNC_CODE.OP_MULT_DIV, self._ops is a string
@@ -523,16 +521,16 @@
         return PlanIter.PlanIterKind.value_of(ArithOpIter.PlanIterKind.ARITH_OP)
 
     def next(self, rcb):
         state = rcb.get_state(self.state_pos)
         if state.is_done():
             return False
         res_type = (
-            serde.BinaryProtocol.FIELD_VALUE_TYPE.DOUBLE if self._have_real_div
-            else serde.BinaryProtocol.FIELD_VALUE_TYPE.INTEGER)
+            SerdeUtil.FIELD_VALUE_TYPE.DOUBLE if self._have_real_div
+            else SerdeUtil.FIELD_VALUE_TYPE.INTEGER)
         # Determine the type of the result for the expression by iterating its
         # components, enforcing the promotion rules for numeric types.
         #
         # Start with INTEGER, unless we have any div operator, in which case
         # start with DOUBLE.
         for i in range(len(self._args)):
             arg_iter = self._args[i]
@@ -543,98 +541,95 @@
             arg_val = rcb.get_reg_val(arg_iter.get_result_reg())
             if arg_val is None:
                 res = None
                 rcb.set_reg_val(self.result_reg, res)
                 state.done()
                 return True
             if isinstance(arg_val, float):
-                if (res_type == serde.BinaryProtocol.FIELD_VALUE_TYPE.INTEGER or
-                        res_type == serde.BinaryProtocol.FIELD_VALUE_TYPE.LONG):
-                    res_type = serde.BinaryProtocol.FIELD_VALUE_TYPE.DOUBLE
+                if (res_type == SerdeUtil.FIELD_VALUE_TYPE.INTEGER or
+                        res_type == SerdeUtil.FIELD_VALUE_TYPE.LONG):
+                    res_type = SerdeUtil.FIELD_VALUE_TYPE.DOUBLE
             elif isinstance(arg_val, int):
                 pass
-            elif version_info.major == 2 and CheckValue.is_long(arg_val):
-                if res_type == serde.BinaryProtocol.FIELD_VALUE_TYPE.INTEGER:
-                    res_type = serde.BinaryProtocol.FIELD_VALUE_TYPE.LONG
             elif isinstance(arg_val, Decimal):
-                res_type = serde.BinaryProtocol.FIELD_VALUE_TYPE.NUMBER
+                res_type = SerdeUtil.FIELD_VALUE_TYPE.NUMBER
             else:
                 raise QueryException(
                     'Operand in arithmetic operation has illegal type\n' +
                     'Operand : ' + str(i) + ' type :\n' + str(type(arg_val)),
                     self.get_location())
-        if res_type == serde.BinaryProtocol.FIELD_VALUE_TYPE.DOUBLE:
+        if res_type == SerdeUtil.FIELD_VALUE_TYPE.DOUBLE:
             res = float(self._init_result)
-        elif res_type == serde.BinaryProtocol.FIELD_VALUE_TYPE.INTEGER:
+        elif res_type == SerdeUtil.FIELD_VALUE_TYPE.INTEGER:
+            res = self._init_result
+        elif res_type == SerdeUtil.FIELD_VALUE_TYPE.LONG:
             res = self._init_result
-        elif res_type == serde.BinaryProtocol.FIELD_VALUE_TYPE.LONG:
-            res = long(self._init_result)
-        elif res_type == serde.BinaryProtocol.FIELD_VALUE_TYPE.NUMBER:
+        elif res_type == SerdeUtil.FIELD_VALUE_TYPE.NUMBER:
             res = None
         else:
             raise QueryStateException(
                 'Invalid result type code: ' + str(res_type))
         for i in range(len(self._args)):
             arg_iter = self._args[i]
             arg_val = rcb.get_reg_val(arg_iter.get_result_reg())
             assert arg_val is not None
             if self._code == PlanIter.FUNC_CODE.OP_ADD_SUB:
                 if self._ops[i] == '+':
                     if ((res_type ==
-                         serde.BinaryProtocol.FIELD_VALUE_TYPE.DOUBLE) or
+                         SerdeUtil.FIELD_VALUE_TYPE.DOUBLE) or
                             (res_type ==
-                             serde.BinaryProtocol.FIELD_VALUE_TYPE.INTEGER) or
+                             SerdeUtil.FIELD_VALUE_TYPE.INTEGER) or
                             (res_type ==
-                             serde.BinaryProtocol.FIELD_VALUE_TYPE.LONG)):
+                             SerdeUtil.FIELD_VALUE_TYPE.LONG)):
                         res += arg_val
                     elif (res_type ==
-                          serde.BinaryProtocol.FIELD_VALUE_TYPE.NUMBER):
+                          SerdeUtil.FIELD_VALUE_TYPE.NUMBER):
                         if res is None:
                             res = arg_val
                         else:
                             res += arg_val
                 else:
                     if ((res_type ==
-                         serde.BinaryProtocol.FIELD_VALUE_TYPE.DOUBLE) or
+                         SerdeUtil.FIELD_VALUE_TYPE.DOUBLE) or
                             (res_type ==
-                             serde.BinaryProtocol.FIELD_VALUE_TYPE.INTEGER) or
+                             SerdeUtil.FIELD_VALUE_TYPE.INTEGER) or
                             (res_type ==
-                             serde.BinaryProtocol.FIELD_VALUE_TYPE.LONG)):
+                             SerdeUtil.FIELD_VALUE_TYPE.LONG)):
                         res -= arg_val
                     elif (res_type ==
-                          serde.BinaryProtocol.FIELD_VALUE_TYPE.NUMBER):
+                          SerdeUtil.FIELD_VALUE_TYPE.NUMBER):
                         if res is None:
                             res = -arg_val
                         else:
                             res -= arg_val
             else:
                 if self._ops[i] == '*':
                     if ((res_type ==
-                         serde.BinaryProtocol.FIELD_VALUE_TYPE.DOUBLE) or
+                         SerdeUtil.FIELD_VALUE_TYPE.DOUBLE) or
                             (res_type ==
-                             serde.BinaryProtocol.FIELD_VALUE_TYPE.INTEGER) or
+                             SerdeUtil.FIELD_VALUE_TYPE.INTEGER) or
                             (res_type ==
-                             serde.BinaryProtocol.FIELD_VALUE_TYPE.LONG)):
+                             SerdeUtil.FIELD_VALUE_TYPE.LONG)):
                         res *= arg_val
                     elif (res_type ==
-                          serde.BinaryProtocol.FIELD_VALUE_TYPE.NUMBER):
+                          SerdeUtil.FIELD_VALUE_TYPE.NUMBER):
                         if res is None:
                             res = arg_val
                         else:
                             res *= arg_val
                 else:
                     if ((res_type ==
-                         serde.BinaryProtocol.FIELD_VALUE_TYPE.DOUBLE) or
+                         SerdeUtil.FIELD_VALUE_TYPE.DOUBLE) or
                             (res_type ==
-                             serde.BinaryProtocol.FIELD_VALUE_TYPE.INTEGER) or
+                             SerdeUtil.FIELD_VALUE_TYPE.INTEGER) or
                             (res_type ==
-                             serde.BinaryProtocol.FIELD_VALUE_TYPE.LONG)):
+                             SerdeUtil.FIELD_VALUE_TYPE.LONG)):
                         res /= arg_val
                     elif (res_type ==
-                          serde.BinaryProtocol.FIELD_VALUE_TYPE.NUMBER):
+                          SerdeUtil.FIELD_VALUE_TYPE.NUMBER):
                         if res is None:
                             res = Decimal(1)
                         else:
                             res /= arg_val
         rcb.set_reg_val(self.result_reg, res)
         state.done()
         return True
@@ -711,15 +706,15 @@
     self._id:\n
     The variable id. It is used as an index into a list of field values in the
     RCB that stores the values of the external vars.
     """
 
     def __init__(self, bis):
         super(ExternalVarRefIter, self).__init__(bis)
-        self._name = serde.BinaryProtocol.read_string(bis)
+        self._name = SerdeUtil.read_string(bis)
         self._id = PlanIter.read_positive_int(bis)
 
     def close(self, rcb):
         state = rcb.get_state(self.state_pos)
         if state is None:
             return
         state.close()
@@ -771,15 +766,15 @@
     FieldStepIter returns the value of a field in an input dict. It is used by
     the driver to implement column references in the SELECT list (see SFWIter).
     """
 
     def __init__(self, bis):
         super(FieldStepIter, self).__init__(bis)
         self._input_iter = self.deserialize_iter(bis)
-        self._field_name = serde.BinaryProtocol.read_string(bis)
+        self._field_name = SerdeUtil.read_string(bis)
 
     def close(self, rcb):
         state = rcb.get_state(self.state_pos)
         if state is None:
             return
         self._input_iter.close(rcb)
         state.close()
@@ -1004,15 +999,15 @@
 
 class GroupIter(PlanIter):
 
     def __init__(self, bis):
         super(GroupIter, self).__init__(bis)
         self._input = self.deserialize_iter(bis)
         self.num_gb_columns = bis.read_int()
-        self._column_names = serde.BinaryProtocol.read_string_array(bis)
+        self._column_names = SerdeUtil.read_string_array(bis)
         num_aggrs = len(self._column_names) - self.num_gb_columns
         self._aggr_funcs = [0] * num_aggrs
         for i in range(num_aggrs):
             self._aggr_funcs[i] = bis.read_short_int()
         self._is_distinct = bis.read_boolean()
         self._remove_produced_result = bis.read_boolean()
         self._count_memory = bis.read_boolean()
@@ -1061,15 +1056,15 @@
                     i = 0
                     while i < self.num_gb_columns:
                         res[self._column_names[i]] = gb_tuple.values[i]
                         i += 1
                     for i in range(i, len(self._column_names)):
                         aggr = self._get_aggr_value(aggr_tuple, i)
                         res[self._column_names[i]] = aggr
-                    res = serde.BinaryProtocol.convert_value_to_none(res)
+                    res = SerdeUtil.convert_value_to_none(res)
                     rcb.set_reg_val(self.result_reg, res)
                     if self._remove_produced_result:
                         state.results.pop(gb_tuple)
                     return True
                 except KeyError:
                     # Dictionary is empty.
                     state.done()
@@ -1122,15 +1117,15 @@
                 if rcb.get_trace_level() >= 3:
                     rcb.trace('Started new group:\n' +
                               GroupIter._print_result(gb_tuple, aggr_tuple))
                 if self.num_gb_columns == len(self._column_names):
                     res = dict()
                     for i in range(self.num_gb_columns):
                         res[self._column_names[i]] = gb_tuple.values[i]
-                    res = serde.BinaryProtocol.convert_value_to_none(res)
+                    res = SerdeUtil.convert_value_to_none(res)
                     rcb.set_reg_val(self.result_reg, res)
                     return True
             else:
                 for i in range(self.num_gb_columns, len(self._column_names)):
                     self._aggregate(rcb, aggr_tuple, i,
                                     in_tuple.get(self._column_names[i]))
                 if rcb.get_trace_level() >= 3:
@@ -1233,39 +1228,37 @@
                 self.value = None
             else:
                 assert False
 
         def add(self, rcb, count_memory, val, ctx):
             setcontext(ctx)
             sz = 0
-            if CheckValue.is_int(val) or CheckValue.is_long(val):
+            if CheckValue.is_int_value(val):
                 self.got_numeric_input = True
                 if CheckValue.is_digit(self.value):
                     self.value += val
                 else:
                     assert False
             elif isinstance(val, float):
                 self.got_numeric_input = True
-                if (CheckValue.is_int(self.value) or
-                        CheckValue.is_long(self.value)):
+                if CheckValue.is_int_value(self.value):
                     if count_memory:
                         sz = PlanIter.sizeof(self.value)
                     self.value += val
                     if count_memory:
                         rcb.inc_memory_consumption(
                             PlanIter.sizeof(self.value) - sz)
                 elif (isinstance(self.value, float) or
                       isinstance(self.value, Decimal)):
                     self.value += val
                 else:
                     assert False
             elif isinstance(val, Decimal):
                 self.got_numeric_input = True
-                if (CheckValue.is_int(self.value) or
-                        CheckValue.is_long(self.value) or
+                if (CheckValue.is_int_value(self.value) or
                         isinstance(self.value, float)):
                     if count_memory:
                         sz = PlanIter.sizeof(self.value)
                     self.value += val
                     if count_memory:
                         rcb.inc_memory_consumption(
                             PlanIter.sizeof(self.value) - sz)
@@ -1341,20 +1334,20 @@
 
     def __init__(self, bis):
         super(ReceiveIter, self).__init__(bis)
         # The distribution kind of the query.
         self.distribution_kind = bis.read_short_int()
         # Used for sorting queries. It specifies the names of the top-level
         # fields that contain the values on which to sort the received results.
-        self.sort_fields = serde.BinaryProtocol.read_string_array(bis)
+        self.sort_fields = SerdeUtil.read_string_array(bis)
         self.sort_specs = PlanIter.read_sort_specs(bis)
         # Used for duplicate elimination. It specifies the names of the
         # top-level fields that contain the primary-key values within the
         # received results .
-        self._prim_key_fields = serde.BinaryProtocol.read_string_array(bis)
+        self._prim_key_fields = SerdeUtil.read_string_array(bis)
 
     def close(self, rcb):
         state = rcb.get_state(self.state_pos)
         if state is None:
             return
         state.close()
 
@@ -1570,15 +1563,15 @@
                 state.done()
                 return False
             res = scanner.next_local()
             if res is not None:
                 if rcb.get_trace_level() >= 1:
                     rcb.trace('ReceiveIter._sorting_next() : got result :\n' +
                               str(res))
-                res = serde.BinaryProtocol.convert_value_to_none(res)
+                res = SerdeUtil.convert_value_to_none(res)
                 rcb.set_reg_val(self.result_reg, res)
                 if not scanner.is_done():
                     ReceiveIter.add_scanner(state.sorted_scanners, scanner)
                 else:
                     if rcb.get_trace_level() >= 1:
                         rcb.trace(
                             'ReceiveIter._sorting_next() : done with ' +
@@ -1616,24 +1609,24 @@
             rcb.set_reached_limit(True)
             return False
 
     @staticmethod
     def _write_value(out, value, i):
         if isinstance(value, float):
             out.write_float(value)
-        elif CheckValue.is_int(value):
-            serde.BinaryProtocol.write_packed_int(out, value)
-        elif CheckValue.is_long(value):
-            serde.BinaryProtocol.write_packed_long(out, value)
+        elif CheckValue.is_int_value(value):
+            SerdeUtil.write_packed_int(out, value)
+        elif CheckValue.is_long_value(value):
+            SerdeUtil.write_packed_long(out, value)
         elif CheckValue.is_str(value):
-            serde.BinaryProtocol.write_string(out, value)
+            SerdeUtil.write_string(out, value)
         elif isinstance(value, datetime):
-            serde.BinaryProtocol.write_datetime(out, value)
+            SerdeUtil.write_datetime(out, value)
         elif isinstance(value, Decimal):
-            serde.BinaryProtocol.write_decimal(out, value)
+            SerdeUtil.write_decimal(out, value)
         else:
             raise QueryStateException(
                 'Unexpected type for primary key column : ' + str(type(value)) +
                 ', at result column ' + str(i))
 
     class ReceiveIterState(PlanIterState):
 
@@ -1870,17 +1863,17 @@
     partial groups/aggregates received from the proxy.
 
     (c) implement offset and limit.
     """
 
     def __init__(self, bis):
         super(SFWIter, self).__init__(bis)
-        self._column_names = serde.BinaryProtocol.read_string_array(bis)
+        self._column_names = SerdeUtil.read_string_array(bis)
         self._num_gb_columns = bis.read_int()
-        self._from_var_name = serde.BinaryProtocol.read_string(bis)
+        self._from_var_name = SerdeUtil.read_string(bis)
         self._is_select_star = bis.read_boolean()
         self.column_iters = self.deserialize_iters(bis)
         self._from_iter = self.deserialize_iter(bis)
         self._offset_iter = self.deserialize_iter(bis)
         self._limit_iter = self.deserialize_iter(bis)
 
     def close(self, rcb):
@@ -2187,15 +2180,15 @@
     It is used by the driver to implement the geo_near function, which sorts
     results by distance.
     """
 
     def __init__(self, bis, kind):
         super(SortIter, self).__init__(bis)
         self._input = self.deserialize_iter(bis)
-        self._sort_fields = serde.BinaryProtocol.read_string_array(bis)
+        self._sort_fields = SerdeUtil.read_string_array(bis)
         self._sort_specs = PlanIter.read_sort_specs(bis)
         if kind == PlanIter.PlanIterKind.SORT2:
             self._count_memory = bis.read_boolean()
         else:
             self._count_memory = True
 
     def close(self, rcb):
@@ -2241,15 +2234,15 @@
                 if self._count_memory:
                     rcb.inc_memory_consumption(self.sizeof(val))
                 more = self._input.next(rcb)
             if rcb.reached_limit():
                 return False
             state.set_state(PlanIterState.STATE.RUNNING)
         if state.curr_result < len(state.results):
-            val = serde.BinaryProtocol.convert_value_to_none(
+            val = SerdeUtil.convert_value_to_none(
                 state.results[state.curr_result])
             rcb.set_reg_val(self.result_reg, val)
             state.results[state.curr_result] = None
             state.curr_result += 1
             return True
         state.done()
         return False
@@ -2316,15 +2309,15 @@
 
     self._name:
     The name of the variable. Used only when displaying the execution plan.
     """
 
     def __init__(self, bis):
         super(VarRefIter, self).__init__(bis)
-        self._name = serde.BinaryProtocol.read_string(bis)
+        self._name = SerdeUtil.read_string(bis)
 
     def close(self, rcb):
         state = rcb.get_state(self.state_pos)
         if state is None:
             return
         state.close()
 
@@ -2647,17 +2640,16 @@
         result.set_continuation_key(self._continuation_key)
         result.set_read_kb(self._rcb.get_read_kb())
         result.set_read_units(self._rcb.get_read_units())
         result.set_write_kb(self._rcb.get_write_kb())
         self._results = None
         self._rcb.reset_kb_consumption()
 
-    def copy(self, queryRequest):
-        # type: (QueryRequest) -> QueryDriver
-        copy = QueryDriver(queryRequest)
+    def copy(self, query_request):
+        copy = QueryDriver(query_request)
         copy._client = self._client
         copy._topology_info = self._topology_info
         copy._prep_cost = self._prep_cost
         copy._results = self._results
         copy._error = self._error
         # leave _continuation_key and _rcb null to start from the beginning
         # copy._continuation_key = self._continuation_key
```

### Comparing `borneo-5.3.7/src/borneo/client.py` & `borneo-5.4.1/src/borneo/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 #
-# Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from logging import DEBUG
 from multiprocessing import pool
 from platform import python_version
-from requests import Session
 from sys import version_info
 from threading import Lock
 from time import time
 
+from requests import Session
+
 from .common import (
     ByteOutputStream, CheckValue, HttpConstants, LogUtils, SSLAdapter,
     TableLimits, synchronized)
 from .config import DefaultRetryHandler
 from .exception import (IllegalArgumentException,
                         OperationNotSupportedException, RequestSizeLimitException)
 from .http import RateLimiterMap, RequestUtils
 from .kv import StoreAccessTokenProvider
 from .operations import GetTableRequest, QueryResult, TableRequest, WriteRequest
 from .query import QueryDriver
-from .serde import BinaryProtocol
-from .version import __version__
+from .serdeutil import SerdeUtil
 from .stats import StatsControl
+from .version import __version__
 
 
 class Client(object):
     DEFAULT_MAX_CONTENT_LENGTH = 32 * 1024 * 1024
     LIMITER_REFRESH_NANOS = 600000000000
     TRACE_LEVEL = 0
 
@@ -46,14 +47,16 @@
             Client.DEFAULT_MAX_CONTENT_LENGTH if max_content_length == 0
             else max_content_length)
         self._request_id = 1
         self._proxy_host = config.get_proxy_host()
         self._proxy_port = config.get_proxy_port()
         self._proxy_username = config.get_proxy_username()
         self._proxy_password = config.get_proxy_password()
+        self._proxy_version = None
+        self._kv_version = None
         self._retry_handler = config.get_retry_handler()
         if self._retry_handler is None:
             self._retry_handler = DefaultRetryHandler()
         self._shut_down = False
         self._user_agent = self._make_user_agent()
         self._auth_provider = config.get_authorization_provider()
         if self._auth_provider is None:
@@ -87,15 +90,15 @@
         #
         adapter = SSLAdapter(
             ssl_ctx, pool_connections=self._pool_connections,
             pool_maxsize=self._pool_maxsize, max_retries=5, pool_block=True)
         self._sess.mount(self._url.scheme + '://', adapter)
         if self._proxy_host is not None:
             self._check_and_set_proxy(self._sess)
-        self.serial_version = BinaryProtocol.DEFAULT_SERIAL_VERSION
+        self.serial_version = config.get_serial_version()
         # StoreAccessTokenProvider means onprem
         self._is_cloud = not isinstance(self._auth_provider, StoreAccessTokenProvider)
         if config.get_rate_limiting_enabled() and self._is_cloud:
             self._logutils.log_debug(
                 'Starting client with rate limiting enabled')
             self._rate_limiter_map = RateLimiterMap()
             self._table_limit_update_map = dict()
@@ -220,44 +223,46 @@
                    'Accept': 'application/octet-stream',
                    'User-Agent': self._user_agent}
 
         # set the session cookie if available
         if self._session_cookie is not None:
             headers['Cookie'] = self._session_cookie
 
-        # We expressly check size limit below based on onprem versus cloud. Set
-        # the request to not check size limit inside self._write_content().
-        request.set_check_request_size(False)
+        # set namespace if configured
+        namespace = request.get_namespace()
+        if namespace is None:
+            namespace = self._config.get_default_namespace()
+        if namespace is not None:
+            headers[HttpConstants.REQUEST_NAMESPACE_HEADER] = namespace
+
         content = self.serialize_request(request, headers)
         content_len = len(content)
         # If on-premise the auth_provider will always be a
         # StoreAccessTokenProvider. If so, check against configurable limit.
         # Otherwise check against internal hardcoded cloud limit.
         if isinstance(self._auth_provider, StoreAccessTokenProvider):
             if content_len > self._max_content_length:
                 raise RequestSizeLimitException(
                     'The request size of ' + str(content_len) + ' exceeded ' +
                     'the limit of ' + str(self._max_content_length))
-        else:
-            request.set_check_request_size(True)
-            BinaryProtocol.check_request_size_limit(request, content_len)
         if request.get_compartment() is None:
             request.set_compartment_internal(
                 self._config.get_default_compartment())
         if self._logutils.is_enabled_for(DEBUG):
             self._logutils.log_debug('Request: ' + request.__class__.__name__)
         request_id = self._next_request_id()
         headers[HttpConstants.REQUEST_ID_HEADER] = request_id
         self.check_request(request)
         # TODO: look at avoiding creating this object on each request
         request_utils = RequestUtils(
             self._sess, self._logutils, request, self._retry_handler, self,
             self._rate_limiter_map)
         return request_utils.do_post_request(self._request_uri, headers,
-            content, timeout_ms, self._stats_control)
+                                             content, timeout_ms,
+                                             self._stats_control)
 
     # set the session cookie if in return headers (see RequestUtils in http.py)
     @synchronized
     def set_session_cookie(self, cookie):
         # only grab the "session=value" portion of the header
         value = cookie.partition(';')[0]
         if self._logutils.is_enabled_for(DEBUG):
@@ -486,31 +491,39 @@
 
         The current minimum value is 2.
         :returns: true if the version was decremented, false otherwise.
         :rtype: bool
         """
         if self.serial_version > 2:
             self.serial_version -= 1
+            msg = ('Unsupported protocol error, decrementing serial ' +
+                   'version to ' + str(self.serial_version) +
+                   ' and retrying')
+            self._logutils.log_info(msg)
             return True
         return False
 
     def _write_content(self, request):
         """
         Serializes the request payload, sent as http content.
 
         :param request: the request to be executed by the server.
         :type request: Request
         :returns: the bytearray that contains the content.
         :rtype: bytearray
         """
         content = bytearray()
         bos = ByteOutputStream(content)
-        BinaryProtocol.write_serial_version(bos, self.serial_version)
-        request.create_serializer().serialize(
-            request, bos, self.serial_version)
+
+        # serial version used is up to the Request, in order to
+        # (1) support multiple protocol versions and
+        # (2) support the version on a per-Request basis
+        version = request.get_serial_version(self.serial_version)
+        SerdeUtil.write_serial_version(bos, version)
+        request.create_serializer(version).serialize(request, bos, version)
         return content
 
     def serialize_request(self, request, headers):
         """
         Serializes the request payload and sets the Content-Length
         header to the correct value.
 
@@ -523,7 +536,21 @@
         """
         content = self._write_content(request)
         headers.update({'Content-Length': str(len(content))})
         return content
 
     def get_stats_control(self):
         return self._stats_control
+
+    def get_proxy_version(self):
+        return self._proxy_version
+
+    def get_kv_version(self):
+        return self._kv_version
+
+    def set_proxy_info(self, proxy_header):
+        if self._proxy_version is None and proxy_header is not None:
+            versions = proxy_header.split()
+            # bail if not of correct format
+            if len(versions) == 2:
+                self._proxy_version = versions[0].split('=')[1]
+                self._kv_version = versions[1].split('=')[1]
```

### Comparing `borneo-5.3.7/src/borneo/serde.py` & `borneo-5.4.1/src/borneo/serde.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,448 +1,162 @@
 #
-# Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
-from abc import ABCMeta, abstractmethod
 from collections import OrderedDict
 from datetime import datetime
-from dateutil import parser, tz
 from decimal import (
     Context, Decimal, ROUND_05UP, ROUND_CEILING, ROUND_DOWN, ROUND_FLOOR,
     ROUND_HALF_DOWN, ROUND_HALF_EVEN, ROUND_HALF_UP, ROUND_UP)
-from sys import version_info
 
 from .common import (
-    CheckValue, Empty, IndexInfo, JsonNone, PackedInteger, PreparedStatement,
-    PutOption, State, SystemState, TableLimits, TableUsage, TimeUnit, Version,
-    enum)
-from .exception import (
-    BatchOperationNumberLimitException, DeploymentException,
-    EvolutionLimitException, IllegalArgumentException, IllegalStateException,
-    IndexExistsException, IndexLimitException, IndexNotFoundException,
-    InvalidAuthorizationException, KeySizeLimitException, NoSQLException,
-    OperationNotSupportedException, OperationThrottlingException,
-    ReadThrottlingException, RequestSizeLimitException, RequestTimeoutException,
-    ResourceExistsException, ResourceNotFoundException, RowSizeLimitException,
-    SecurityInfoNotReadyException, SystemException, TableExistsException,
-    TableLimitException, TableNotFoundException, TableSizeException,
-    UnauthorizedException, UnsupportedProtocolException,
-    WriteThrottlingException)
-from .kv import AuthenticationException
+    CheckValue, Empty, IndexInfo, JsonNone, PreparedStatement,
+    TableLimits, TableUsage, TimeUnit, Version)
+from .exception import IllegalStateException
 from .query import PlanIter, QueryDriver, TopologyInfo
+from .serdeutil import (SerdeUtil, RequestSerializer)
 
 try:
     from . import operations
 except ImportError:
     import operations
 
+math_name_to_value = {ROUND_UP: 0,
+                      ROUND_DOWN: 1,
+                      ROUND_CEILING: 2,
+                      ROUND_FLOOR: 3,
+                      ROUND_HALF_UP: 4,
+                      ROUND_HALF_DOWN: 5,
+                      ROUND_HALF_EVEN: 6,
+                      ROUND_05UP: 8}
+math_value_to_name = {0: ROUND_UP,
+                      1: ROUND_DOWN,
+                      2: ROUND_CEILING,
+                      3: ROUND_FLOOR,
+                      4: ROUND_HALF_UP,
+                      5: ROUND_HALF_DOWN,
+                      6: ROUND_HALF_EVEN,
+                      8: ROUND_05UP}
+
 
 class BinaryProtocol(object):
     """
     A base class for binary protocol serialization and constant protocol values.
     Constants are used instead of relying on ordering of values in enumerations
     or other derived protocol state.
     """
-    TRACE_LEVEL = 0
-
-    # Serial version of the protocol.
-    DEFAULT_SERIAL_VERSION = 3
-
-    # The max size of WriteMultiple request.
-    BATCH_REQUEST_SIZE_LIMIT = 25 * 1024 * 1024
-
-    # The limit on the max read KB during a operation
-    READ_KB_LIMIT = 2 * 1024
-
-    # The max size of request.
-    REQUEST_SIZE_LIMIT = 2 * 1024 * 1024
-
-    # Field value type.
-    FIELD_VALUE_TYPE = enum(ARRAY=0,
-                            BINARY=1,
-                            BOOLEAN=2,
-                            DOUBLE=3,
-                            INTEGER=4,
-                            LONG=5,
-                            MAP=6,
-                            STRING=7,
-                            TIMESTAMP=8,
-                            NUMBER=9,
-                            JSON_NULL=10,
-                            NULL=11,
-                            EMPTY=12)
-
-    # Operation codes
-    OP_CODE = enum(DELETE=0,
-                   DELETE_IF_VERSION=1,
-                   GET=2,
-                   PUT=3,
-                   PUT_IF_ABSENT=4,
-                   PUT_IF_PRESENT=5,
-                   PUT_IF_VERSION=6,
-                   QUERY=7,
-                   PREPARE=8,
-                   WRITE_MULTIPLE=9,
-                   MULTI_DELETE=10,
-                   GET_TABLE=11,
-                   GET_INDEXES=12,
-                   GET_TABLE_USAGE=13,
-                   LIST_TABLES=14,
-                   TABLE_REQUEST=15,
-                   SCAN=16,
-                   INDEX_SCAN=17,
-                   CREATE_TABLE=18,
-                   ALTER_TABLE=19,
-                   DROP_TABLE=20,
-                   CREATE_INDEX=21,
-                   DROP_INDEX=22,
-                   # added in V2.
-                   SYSTEM_REQUEST=23,
-                   SYSTEM_STATUS_REQUEST=24)
-
-    # System Operation state.
-    SYSTEM_STATE = enum(COMPLETE=0,
-                        WORKING=1)
-
-    # Table state.
-    TABLE_STATE = enum(ACTIVE=0,
-                       CREATING=1,
-                       DROPPED=2,
-                       DROPPING=3,
-                       UPDATING=4)
-
-    """
-    Error codes for user-generated errors, range from 1 to 50(exclusive).
-    These include illegal arguments, exceeding size limits for some objects,
-    resource not found, etc.
-    """
-    USER_ERROR = enum(UNKNOWN_OPERATION=1,
-                      TABLE_NOT_FOUND=2,
-                      INDEX_NOT_FOUND=3,
-                      ILLEGAL_ARGUMENT=4,
-                      ROW_SIZE_LIMIT_EXCEEDED=5,
-                      KEY_SIZE_LIMIT_EXCEEDED=6,
-                      BATCH_OP_NUMBER_LIMIT_EXCEEDED=7,
-                      REQUEST_SIZE_LIMIT_EXCEEDED=8,
-                      TABLE_EXISTS=9,
-                      INDEX_EXISTS=10,
-                      INVALID_AUTHORIZATION=11,
-                      INSUFFICIENT_PERMISSION=12,
-                      RESOURCE_EXISTS=13,
-                      RESOURCE_NOT_FOUND=14,
-                      TABLE_LIMIT_EXCEEDED=15,
-                      INDEX_LIMIT_EXCEEDED=16,
-                      BAD_PROTOCOL_MESSAGE=17,
-                      EVOLUTION_LIMIT_EXCEEDED=18,
-                      TABLE_DEPLOYMENT_LIMIT_EXCEEDED=19,
-                      TENANT_DEPLOYMENT_LIMIT_EXCEEDED=20,
-                      # added in V2.
-                      OPERATION_NOT_SUPPORTED=21,
-                      ETAG_MISMATCH=22,
-                      CANNOT_CANCEL_WORK_REQUEST=23,
-                      # added in V3
-                      UNSUPPORTED_PROTOCOL=24)
-
-    # Error codes for user throttling, range from 50 to 100(exclusive).
-    THROTTLING_ERROR = enum(READ_LIMIT_EXCEEDED=50,
-                            WRITE_LIMIT_EXCEEDED=51,
-                            SIZE_LIMIT_EXCEEDED=52,
-                            OPERATION_LIMIT_EXCEEDED=53)
-
-    """
-    Retry-able server issues, range from 100 to 125(exclusive).
-    These are internal problems, presumably temporary, and need to be sent back
-    to the application for retry.
-    """
-    SERVER_RETRY_ERROR = enum(REQUEST_TIMEOUT=100,
-                              SERVER_ERROR=101,
-                              SERVICE_UNAVAILABLE=102,
-                              SECURITY_INFO_UNAVAILABLE=104,
-                              # added in V2.
-                              RETRY_AUTHENTICATION=105)
-
-    """
-    Other server issues, begin from 125.
-    These include server illegal state, unknown server error, etc.
-    They might be retry-able, or not.
-    """
-    SERVER_OTHER_ERROR = enum(UNKNOWN_ERROR=125,
-                              ILLEGAL_STATE=126)
-
-    """
-    in V3 and above, TableLimits includes a mode
-    """
-    CAPACITY_MODE = enum(PROVISIONED=1,
-                         ON_DEMAND=2)
-
-    @staticmethod
-    def check_request_size_limit(request, request_size):
-        # Checks if the request size exceeds the limit.
-        if not request.get_check_request_size():
-            return
-        request_size_limit = (
-            BinaryProtocol.BATCH_REQUEST_SIZE_LIMIT if
-            isinstance(request, operations.WriteMultipleRequest) else
-            BinaryProtocol.REQUEST_SIZE_LIMIT)
-        if request_size > request_size_limit:
-            raise RequestSizeLimitException(
-                'The request size of ' + str(request_size) +
-                ' exceeded the limit of ' + str(request_size_limit))
-
-    @staticmethod
-    def convert_value_to_none(value):
-        if isinstance(value, dict):
-            return {key: BinaryProtocol.convert_value_to_none(val)
-                    for (key, val) in value.items()}
-        if isinstance(value, list):
-            return [BinaryProtocol.convert_value_to_none(val) for val in
-                    value]
-        if isinstance(value, Empty) or isinstance(value, JsonNone):
-            return None
-        return value
 
     @staticmethod
     def deserialize_consumed_capacity(bis, result):
-        result.set_read_units(BinaryProtocol.read_packed_int(bis))
-        result.set_read_kb(BinaryProtocol.read_packed_int(bis))
-        result.set_write_kb(BinaryProtocol.read_packed_int(bis))
+        result.set_read_units(SerdeUtil.read_packed_int(bis))
+        result.set_read_kb(SerdeUtil.read_packed_int(bis))
+        result.set_write_kb(SerdeUtil.read_packed_int(bis))
 
     @staticmethod
     def deserialize_system_result(bis):
         result = operations.SystemResult()
-        result.set_state(BinaryProtocol.get_operation_state(bis.read_byte()))
-        result.set_operation_id(BinaryProtocol.read_string(bis))
-        result.set_statement(BinaryProtocol.read_string(bis))
-        result.set_result_string(BinaryProtocol.read_string(bis))
+        result.set_state(SerdeUtil.get_operation_state(bis.read_byte()))
+        result.set_operation_id(SerdeUtil.read_string(bis))
+        result.set_statement(SerdeUtil.read_string(bis))
+        result.set_result_string(SerdeUtil.read_string(bis))
         return result
 
     @staticmethod
     def deserialize_generated_value(bis, result):
         has_generated_value = bis.read_boolean()
         if not has_generated_value:
             return
-        result.set_generated_value(BinaryProtocol.convert_value_to_none(
+        result.set_generated_value(SerdeUtil.convert_value_to_none(
             BinaryProtocol.read_field_value(bis)))
 
     @staticmethod
     def deserialize_table_result(bis, result, serial_version):
         has_info = bis.read_boolean()
         if has_info:
-            result.set_compartment_id(BinaryProtocol.read_string(bis))
-            result.set_table_name(BinaryProtocol.read_string(bis))
+            result.set_compartment_id(SerdeUtil.read_string(bis))
+            result.set_table_name(SerdeUtil.read_string(bis))
             result.set_state(
-                BinaryProtocol._get_table_state(bis.read_byte()))
+                SerdeUtil.get_table_state(bis.read_byte()))
             has_static_state = bis.read_boolean()
             if has_static_state:
-                read_kb = BinaryProtocol.read_packed_int(bis)
-                write_kb = BinaryProtocol.read_packed_int(bis)
-                storage_gb = BinaryProtocol.read_packed_int(bis)
-                capacity_mode = BinaryProtocol.CAPACITY_MODE.PROVISIONED
+                read_kb = SerdeUtil.read_packed_int(bis)
+                write_kb = SerdeUtil.read_packed_int(bis)
+                storage_gb = SerdeUtil.read_packed_int(bis)
+                capacity_mode = SerdeUtil.CAPACITY_MODE.PROVISIONED
                 if serial_version > 2:
                     capacity_mode = bis.read_byte()
                 # on-prem tables may return all 0 because of protocol
                 # limitations that lump the schema with limits. Return None to
                 # user for those cases.
                 if not (read_kb == 0 and write_kb == 0 and storage_gb == 0):
                     result.set_table_limits(
                         TableLimits(read_kb, write_kb, storage_gb, capacity_mode))
-                result.set_schema(BinaryProtocol.read_string(bis))
-            result.set_operation_id(BinaryProtocol.read_string(bis))
+                result.set_schema(SerdeUtil.read_string(bis))
+            result.set_operation_id(SerdeUtil.read_string(bis))
 
     @staticmethod
     def deserialize_write_response(bis, result, serial_version):
         return_info = bis.read_boolean()
         if not return_info:
             return
         # Existing info always includes both value and version.
-        result.set_existing_value(BinaryProtocol.convert_value_to_none(
+        result.set_existing_value(SerdeUtil.convert_value_to_none(
             BinaryProtocol.read_field_value(bis)))
         result.set_existing_version(BinaryProtocol.read_version(bis))
         if serial_version > 2:
-            result.set_existing_modification_time(BinaryProtocol.read_packed_long(bis))
+            result.set_existing_modification_time(SerdeUtil.read_packed_long(bis))
         else:
             result.set_existing_modification_time(0)
 
     @staticmethod
-    def get_operation_state(state):
-        if state == BinaryProtocol.SYSTEM_STATE.COMPLETE:
-            return SystemState.COMPLETE
-        elif state == BinaryProtocol.SYSTEM_STATE.WORKING:
-            return SystemState.WORKING
-        else:
-            raise IllegalStateException(
-                'Unknown system operation state ' + str(state))
-
-    @staticmethod
-    def map_exception(code, msg):
-        # Maps the error code returned from the server into a local string.
-        if (code == BinaryProtocol.SERVER_OTHER_ERROR.UNKNOWN_ERROR or
-                code == BinaryProtocol.USER_ERROR.UNKNOWN_OPERATION):
-            return NoSQLException('Unknown error: ' + msg)
-        elif code == BinaryProtocol.SERVER_OTHER_ERROR.ILLEGAL_STATE:
-            return IllegalStateException(msg)
-        elif code == BinaryProtocol.SERVER_RETRY_ERROR.REQUEST_TIMEOUT:
-            return RequestTimeoutException(msg)
-        elif code == BinaryProtocol.SERVER_RETRY_ERROR.RETRY_AUTHENTICATION:
-            return AuthenticationException(msg)
-        elif code == (
-                BinaryProtocol.SERVER_RETRY_ERROR.SECURITY_INFO_UNAVAILABLE):
-            return SecurityInfoNotReadyException(msg)
-        elif (code == BinaryProtocol.SERVER_RETRY_ERROR.SERVICE_UNAVAILABLE or
-              code == BinaryProtocol.SERVER_RETRY_ERROR.SERVER_ERROR):
-            return SystemException(msg)
-        elif code == BinaryProtocol.THROTTLING_ERROR.OPERATION_LIMIT_EXCEEDED:
-            return OperationThrottlingException(msg)
-        elif code == BinaryProtocol.THROTTLING_ERROR.READ_LIMIT_EXCEEDED:
-            return ReadThrottlingException(msg)
-        elif code == BinaryProtocol.THROTTLING_ERROR.SIZE_LIMIT_EXCEEDED:
-            return TableSizeException(msg)
-        elif code == BinaryProtocol.THROTTLING_ERROR.WRITE_LIMIT_EXCEEDED:
-            return WriteThrottlingException(msg)
-        elif code == BinaryProtocol.USER_ERROR.BAD_PROTOCOL_MESSAGE:
-            # V2 proxy will return this message if V3 is used in the driver
-            if "Invalid driver serial version" in msg:
-                return UnsupportedProtocolException(msg)
-            return IllegalArgumentException('Bad protocol message: ' + msg)
-        elif (code ==
-              BinaryProtocol.USER_ERROR.BATCH_OP_NUMBER_LIMIT_EXCEEDED):
-            return BatchOperationNumberLimitException(msg)
-        elif code == BinaryProtocol.USER_ERROR.EVOLUTION_LIMIT_EXCEEDED:
-            return EvolutionLimitException(msg)
-        elif code == BinaryProtocol.USER_ERROR.ILLEGAL_ARGUMENT:
-            return IllegalArgumentException(msg)
-        elif code == BinaryProtocol.USER_ERROR.INDEX_EXISTS:
-            return IndexExistsException(msg)
-        elif code == BinaryProtocol.USER_ERROR.INDEX_LIMIT_EXCEEDED:
-            return IndexLimitException(msg)
-        elif code == BinaryProtocol.USER_ERROR.INDEX_NOT_FOUND:
-            return IndexNotFoundException(msg)
-        elif code == BinaryProtocol.USER_ERROR.INSUFFICIENT_PERMISSION:
-            return UnauthorizedException(msg)
-        elif code == BinaryProtocol.USER_ERROR.INVALID_AUTHORIZATION:
-            return InvalidAuthorizationException(msg)
-        elif code == BinaryProtocol.USER_ERROR.KEY_SIZE_LIMIT_EXCEEDED:
-            return KeySizeLimitException(msg)
-        elif code == BinaryProtocol.USER_ERROR.OPERATION_NOT_SUPPORTED:
-            return OperationNotSupportedException(msg)
-        elif (code ==
-              BinaryProtocol.USER_ERROR.REQUEST_SIZE_LIMIT_EXCEEDED):
-            return RequestSizeLimitException(msg)
-        elif code == BinaryProtocol.USER_ERROR.RESOURCE_EXISTS:
-            return ResourceExistsException(msg)
-        elif code == BinaryProtocol.USER_ERROR.RESOURCE_NOT_FOUND:
-            return ResourceNotFoundException(msg)
-        elif code == BinaryProtocol.USER_ERROR.ROW_SIZE_LIMIT_EXCEEDED:
-            return RowSizeLimitException(msg)
-        elif code == BinaryProtocol.USER_ERROR.TABLE_EXISTS:
-            return TableExistsException(msg)
-        elif code == BinaryProtocol.USER_ERROR.TABLE_LIMIT_EXCEEDED:
-            return TableLimitException(msg)
-        elif code == BinaryProtocol.USER_ERROR.TABLE_NOT_FOUND:
-            return TableNotFoundException(msg)
-        elif (code == BinaryProtocol.USER_ERROR.TABLE_DEPLOYMENT_LIMIT_EXCEEDED
-              or code == (
-                      BinaryProtocol.USER_ERROR.TENANT_DEPLOYMENT_LIMIT_EXCEEDED)):
-            return DeploymentException(msg)
-        elif code == BinaryProtocol.USER_ERROR.UNSUPPORTED_PROTOCOL:
-            return UnsupportedProtocolException(msg)
-        else:
-            return NoSQLException(
-                'Unknown error code ' + str(code) + ': ' + msg)
-
-    @staticmethod
-    def read_bytearray(bis):
-        """
-        Reads a possibly None byte array as a
-        :py:meth:`read_sequence_length` followed by the array contents.
-
-        :param bis: the byte input stream.
-        :type bis: ByteInputStream
-        :returns: the array or None.
-        :rtype: bytearray
-        """
-        length = BinaryProtocol.read_sequence_length(bis)
-        if length < -1:
-            raise IOError('Invalid length of byte array: ' + str(length))
-        if length == -1:
-            return None
-        if length == 0:
-            return bytearray()
-        buf = bytearray(length)
-        bis.read_fully(buf)
-        return buf
-
-    @staticmethod
-    def read_bytearray_with_int(bis):
-        # Reads a byte array that has a not-packed integer size.
-        length = bis.read_int()
-        if length <= 0:
-            raise IOError('Invalid length for prepared query: ' + str(length))
-        buf = bytearray(length)
-        bis.read_fully(buf)
-        return buf
-
-    @staticmethod
-    def read_datetime(bis):
-        # Deserialize a datetime value. Timezone is UTC, object is naive, not
-        # timezone aware
-        return parser.parse(BinaryProtocol.read_string(bis))
-
-    @staticmethod
-    def read_decimal(bis):
-        # Deserialize a decimal value.
-        a = BinaryProtocol.read_string(bis)
-        return Decimal(a)
-
-    @staticmethod
     def read_dict(bis):
         # Read length.
         bis.read_int()
         size = bis.read_int()
         result = OrderedDict()
         count = 0
         while count < size:
-            key = BinaryProtocol.read_string(bis)
+            key = SerdeUtil.read_string(bis)
             value = BinaryProtocol.read_field_value(bis)
             result[key] = value
             count += 1
         return result
 
     @staticmethod
     def read_field_value(bis):
         # Deserialize a generic field value.
         t = bis.read_byte()
-        if t == BinaryProtocol.FIELD_VALUE_TYPE.ARRAY:
+        if t == SerdeUtil.FIELD_VALUE_TYPE.ARRAY:
             return BinaryProtocol.read_list(bis)
-        elif t == BinaryProtocol.FIELD_VALUE_TYPE.BINARY:
-            return BinaryProtocol.read_bytearray(bis)
-        elif t == BinaryProtocol.FIELD_VALUE_TYPE.BOOLEAN:
+        elif t == SerdeUtil.FIELD_VALUE_TYPE.BINARY:
+            return SerdeUtil.read_bytearray(bis, False)
+        elif t == SerdeUtil.FIELD_VALUE_TYPE.BOOLEAN:
             return bis.read_boolean()
-        elif t == BinaryProtocol.FIELD_VALUE_TYPE.DOUBLE:
+        elif t == SerdeUtil.FIELD_VALUE_TYPE.DOUBLE:
             return bis.read_float()
-        elif t == BinaryProtocol.FIELD_VALUE_TYPE.EMPTY:
+        elif t == SerdeUtil.FIELD_VALUE_TYPE.EMPTY:
             return Empty()
-        elif t == BinaryProtocol.FIELD_VALUE_TYPE.INTEGER:
-            return BinaryProtocol.read_packed_int(bis)
-        elif t == BinaryProtocol.FIELD_VALUE_TYPE.JSON_NULL:
+        elif t == SerdeUtil.FIELD_VALUE_TYPE.INTEGER:
+            return SerdeUtil.read_packed_int(bis)
+        elif t == SerdeUtil.FIELD_VALUE_TYPE.JSON_NULL:
             return JsonNone()
-        elif t == BinaryProtocol.FIELD_VALUE_TYPE.LONG:
-            return BinaryProtocol.read_packed_long(bis)
-        elif t == BinaryProtocol.FIELD_VALUE_TYPE.MAP:
+        elif t == SerdeUtil.FIELD_VALUE_TYPE.LONG:
+            return SerdeUtil.read_packed_long(bis)
+        elif t == SerdeUtil.FIELD_VALUE_TYPE.MAP:
             return BinaryProtocol.read_dict(bis)
-        elif t == BinaryProtocol.FIELD_VALUE_TYPE.STRING:
-            return BinaryProtocol.read_string(bis)
-        elif t == BinaryProtocol.FIELD_VALUE_TYPE.TIMESTAMP:
-            return BinaryProtocol.read_datetime(bis)
-        elif t == BinaryProtocol.FIELD_VALUE_TYPE.NUMBER:
-            return BinaryProtocol.read_decimal(bis)
-        elif t == BinaryProtocol.FIELD_VALUE_TYPE.NULL:
+        elif t == SerdeUtil.FIELD_VALUE_TYPE.STRING:
+            return SerdeUtil.read_string(bis)
+        elif t == SerdeUtil.FIELD_VALUE_TYPE.TIMESTAMP:
+            return SerdeUtil.read_datetime(bis)
+        elif t == SerdeUtil.FIELD_VALUE_TYPE.NUMBER:
+            return SerdeUtil.read_decimal(bis)
+        elif t == SerdeUtil.FIELD_VALUE_TYPE.NULL:
             return None
         else:
             raise IllegalStateException('Unknown value type code: ' + str(t))
 
     @staticmethod
     def read_list(bis):
         # Read length.
@@ -453,187 +167,67 @@
         while count < length:
             result.append(BinaryProtocol.read_field_value(bis))
             count += 1
         return result
 
     @staticmethod
     def read_math_context(bis):
-        value_to_name = {0: ROUND_UP,
-                         1: ROUND_DOWN,
-                         2: ROUND_CEILING,
-                         3: ROUND_FLOOR,
-                         4: ROUND_HALF_UP,
-                         5: ROUND_HALF_DOWN,
-                         6: ROUND_HALF_EVEN,
-                         8: ROUND_05UP}
         code = bis.read_byte()
         if code == 0:
             return None
         elif code == 1:
             return Context(prec=7, rounding=ROUND_HALF_EVEN)
         elif code == 2:
             return Context(prec=16, rounding=ROUND_HALF_EVEN)
         elif code == 3:
             return Context(prec=34, rounding=ROUND_HALF_EVEN)
         elif code == 4:
             return Context(prec=0, rounding=ROUND_HALF_UP)
         elif code == 5:
             precision = bis.read_int()
-            rounding_mode = value_to_name.get(bis.read_int())
+            rounding_mode = math_value_to_name.get(bis.read_int())
             return Context(prec=precision, rounding=rounding_mode)
         else:
             raise IOError('Unknown MathContext code.')
 
     @staticmethod
-    def read_packed_int(bis):
-        """
-        Reads a packed integer from the input and returns it.
-
-        :param bis: the byte input stream.
-        :type bis: ByteInputStream
-        :returns: the integer that was read.
-        :rtype: int
-        """
-        buf = bytearray(PackedInteger.MAX_LENGTH)
-        bis.read_fully(buf, 0, 1)
-        length = PackedInteger.get_read_sorted_int_length(buf, 0)
-        bis.read_fully(buf, 1, length)
-        return PackedInteger.read_sorted_int(buf, 0)
-
-    @staticmethod
-    def read_packed_int_array(bis):
-        """
-        Reads a possibly None int array as a sequence length followed by the
-        array contents.
-
-        :param bis: the byte input stream.
-        :type bis: ByteInputStream
-        :returns: the array or None.
-        :rtype: list
-        """
-        length = BinaryProtocol.read_sequence_length(bis)
-        if length < -1:
-            raise IOError('Invalid length of byte array: ' + str(length))
-        if length == -1:
-            return None
-        array = [0] * length
-        for i in range(length):
-            array[i] = BinaryProtocol.read_packed_int(bis)
-        return array
-
-    @staticmethod
-    def read_packed_long(bis):
-        """
-        Reads a packed long from the input and returns it.
-
-        :param bis: the byte input stream.
-        :type bis: ByteInputStream
-        :returns: the long that was read.
-        :rtype: int for python 3 and long for python 2
-        """
-        buf = bytearray(PackedInteger.MAX_LONG_LENGTH)
-        bis.read_fully(buf, 0, 1)
-        length = PackedInteger.get_read_sorted_long_length(buf, 0)
-        bis.read_fully(buf, 1, length)
-        return PackedInteger.read_sorted_long(buf, 0)
-
-    @staticmethod
-    def read_sequence_length(bis):
-        """
-        Reads the length of a possibly None sequence.  The length is represented
-        as a :py:meth:`PackedInteger.read_packed_int`, with -1 interpreted as
-        meaning None, and other negative values not permitted. Although we don't
-        enforce maximum sequence lengths yet, this entrypoint provides a place
-        to do that.
-
-        :param bis: the byte input stream.
-        :type bis: ByteInputStream
-        :returns: the sequence length or -1 for None.
-        :rtype: int
-        """
-        result = BinaryProtocol.read_packed_int(bis)
-        if result < -1:
-            raise IOError('Invalid sequence length: ' + str(result))
-        return result
-
-    @staticmethod
-    def read_string(bis):
-        """
-        Reads a possibly None string from an input stream in standard UTF-8
-        format.
-
-        First reads a packed int representing the length of the UTF-8 encoding
-        of the string, or a negative value for None, followed by the string
-        contents in UTF-8 format for a non-empty string, if any.
-
-        :param bis: the byte input stream.
-        :type bis: ByteInputStream
-        :returns: the string or None.
-        :rtype: str or None
-        """
-        length = BinaryProtocol.read_packed_int(bis)
-        if length < -1:
-            raise IOError('Invalid length of String: ' + str(length))
-        if length == -1:
-            return None
-        if length == 0:
-            return str()
-        buf = bytearray(length)
-        bis.read_fully(buf)
-        if version_info.major == 2:
-            return str(buf)
-        return buf.decode('utf-8')
-
-    @staticmethod
-    def read_string_array(bis):
-        length = BinaryProtocol.read_sequence_length(bis)
-        if length < -1:
-            raise IOError('Invalid length of byte array: ' + str(length))
-        if length == -1:
-            return None
-        array = list()
-        for i in range(length):
-            array.append(BinaryProtocol.read_string(bis))
-        return array
-
-    @staticmethod
     def read_topology_info(bis):
-        seq_num = BinaryProtocol.read_packed_int(bis)
-        BinaryProtocol.trace(
+        seq_num = SerdeUtil.read_packed_int(bis)
+        SerdeUtil.trace(
             'read_topology_info: seq_num = ' + str(seq_num), 4)
         if seq_num < -1:
             raise IOError('Invalid topology sequence number: ' + str(seq_num))
         if seq_num == -1:
             # No topology info sent by proxy.
             return None
-        shard_ids = BinaryProtocol.read_packed_int_array(bis)
+        shard_ids = SerdeUtil.read_packed_int_array(bis)
         return TopologyInfo(seq_num, shard_ids)
 
     @staticmethod
     def read_version(bis):
-        return Version.create_version(BinaryProtocol.read_bytearray(bis))
+        return Version.create_version(SerdeUtil.read_bytearray(bis, False))
 
     # Writes fields from ReadRequest.
     @staticmethod
     def serialize_read_request(request, bos):
         BinaryProtocol.serialize_request(request, bos)
-        BinaryProtocol.write_string(bos, request.get_table_name())
+        SerdeUtil.write_string(bos, request.get_table_name())
         bos.write_byte(request.get_consistency())
 
     # Writes fields from WriteRequest
     @staticmethod
     def serialize_write_request(request, bos, serial_version):
         BinaryProtocol.serialize_request(request, bos)
-        BinaryProtocol.write_string(bos, request.get_table_name())
+        SerdeUtil.write_string(bos, request.get_table_name())
         bos.write_boolean(request.get_return_row())
         BinaryProtocol.write_durability(request, bos, serial_version)
 
     @staticmethod
     def serialize_request(request, bos):
-        BinaryProtocol.write_packed_int(bos, request.get_timeout())
+        SerdeUtil.write_packed_int(bos, request.get_timeout())
 
     @staticmethod
     def write_durability(request, bos, serial_version):
         if serial_version < 3:
             return
         dur = request.get_durability()
         if dur is None:
@@ -641,73 +235,34 @@
             return
         val = dur.master_sync
         val |= (dur.replica_sync << 2)
         val |= (dur.replica_ack << 4)
         bos.write_byte(val)
 
     @staticmethod
-    def trace(msg, level):
-        if level <= BinaryProtocol.TRACE_LEVEL:
-            print('DRIVER: ' + msg)
-
-    @staticmethod
-    def write_bytearray(bos, value):
-        """
-        Writes a possibly None byte array as a sequence length followed by the
-        array contents.
-
-        :param bos: the byte output stream.
-        :type bos: ByteOutputStream
-        :param value: the bytearray or None.
-        :type value: bytearray or None
-        """
-        length = -1 if value is None else len(value)
-        BinaryProtocol.write_sequence_length(bos, length)
-        if length > 0:
-            bos.write_bytearray(value)
-
-    @staticmethod
-    def write_bytearray_with_int(bos, value):
-        # Writes a byte array with a full 4-byte int length.
-        bos.write_int(len(value))
-        bos.write_bytearray(value)
-
-    @staticmethod
-    def write_datetime(bos, value):
-        # Serialize a datetime value.
-        if value.tzinfo is not None:
-            value = value.astimezone(tz.UTC)
-        BinaryProtocol.write_string(bos, value.isoformat())
-
-    @staticmethod
-    def write_decimal(bos, value):
-        # Serialize a decimal value.
-        BinaryProtocol.write_string(bos, str(value))
-
-    @staticmethod
     def write_dict(bos, value):
         # Serialize a dict.
         # Leave an integer-sized space for length.
         offset = bos.get_offset()
         bos.write_int(0)
         start = bos.get_offset()
         bos.write_int(len(value))
         for key in value:
-            BinaryProtocol.write_string(bos, key)
+            SerdeUtil.write_string(bos, key)
             BinaryProtocol.write_field_value(bos, value[key])
         # Update the length value.
         bos.write_int_at_offset(offset, bos.get_offset() - start)
 
     @staticmethod
     def write_field_range(bos, field_range):
         if field_range is None:
             bos.write_boolean(False)
             return
         bos.write_boolean(True)
-        BinaryProtocol.write_string(bos, field_range.get_field_path())
+        SerdeUtil.write_string(bos, field_range.get_field_path())
         if field_range.get_start() is not None:
             bos.write_boolean(True)
             BinaryProtocol.write_field_value(bos, field_range.get_start())
             bos.write_boolean(field_range.get_start_inclusive())
         else:
             bos.write_boolean(False)
         if field_range.get_end() is not None:
@@ -716,36 +271,36 @@
             bos.write_boolean(field_range.get_end_inclusive())
         else:
             bos.write_boolean(False)
 
     @staticmethod
     def write_field_value(bos, value):
         # Serialize a generic field value.
-        bos.write_byte(BinaryProtocol._get_type(value))
+        bos.write_byte(SerdeUtil.get_type(value))
         if value is not None:
             if isinstance(value, list):
                 BinaryProtocol.write_list(bos, value)
             elif isinstance(value, bytearray):
-                BinaryProtocol.write_bytearray(bos, value)
+                SerdeUtil.write_bytearray(bos, value)
             elif isinstance(value, bool):
                 bos.write_boolean(value)
             elif isinstance(value, float):
                 bos.write_float(value)
-            elif CheckValue.is_int(value):
-                BinaryProtocol.write_packed_int(bos, value)
-            elif CheckValue.is_long(value):
-                BinaryProtocol.write_packed_long(bos, value)
+            elif CheckValue.is_int_value(value):
+                SerdeUtil.write_packed_int(bos, value)
+            elif CheckValue.is_long_value(value):
+                SerdeUtil.write_packed_long(bos, value)
             elif isinstance(value, dict):
                 BinaryProtocol.write_dict(bos, value)
             elif CheckValue.is_str(value):
-                BinaryProtocol.write_string(bos, value)
+                SerdeUtil.write_string(bos, value)
             elif isinstance(value, datetime):
-                BinaryProtocol.write_datetime(bos, value)
+                SerdeUtil.write_datetime(bos, value)
             elif isinstance(value, Decimal) or CheckValue.is_overlong(value):
-                BinaryProtocol.write_decimal(bos, value)
+                SerdeUtil.write_decimal(bos, value)
             else:
                 raise IllegalStateException(
                     'Unknown value type ' + str(type(value)))
 
     @staticmethod
     def write_list(bos, value):
         # Serialize a list.
@@ -757,209 +312,53 @@
         for item in value:
             BinaryProtocol.write_field_value(bos, item)
         # Update the length value.
         bos.write_int_at_offset(offset, bos.get_offset() - start)
 
     @staticmethod
     def write_math_context(bos, math_context):
-        name_to_value = {ROUND_UP: 0,
-                         ROUND_DOWN: 1,
-                         ROUND_CEILING: 2,
-                         ROUND_FLOOR: 3,
-                         ROUND_HALF_UP: 4,
-                         ROUND_HALF_DOWN: 5,
-                         ROUND_HALF_EVEN: 6,
-                         ROUND_05UP: 8}
         if math_context is None:
             bos.write_byte(0)
         else:
             bos.write_byte(5)
             bos.write_int(math_context.prec)
-            bos.write_int(name_to_value.get(math_context.rounding))
+            bos.write_int(math_name_to_value.get(math_context.rounding))
 
     @staticmethod
     def write_op_code(bos, op):
         # Writes the opcode for the operation.
         bos.write_byte(op)
 
     @staticmethod
-    def write_packed_int(bos, value):
-        """
-        Writes a packed integer to the byte output stream.
-
-        :param bos: the byte output stream.
-        :type bos: ByteOutputStream
-        :param value: the integer to be written.
-        :type value: int
-        :returns: the length of bytes written.
-        :rtype: int
-        """
-        buf = bytearray(PackedInteger.MAX_LENGTH)
-        offset = PackedInteger.write_sorted_int(buf, 0, value)
-        bos.write_bytearray(buf, 0, offset)
-        return offset
-
-    @staticmethod
-    def write_packed_long(bos, value):
-        """
-        Writes a packed long to the byte output stream.
-
-        :param bos: the byte output stream.
-        :type bos: ByteOutputStream
-        :param value: the long to be written.
-        :type value: int for python 3 and long for python 2
-        """
-        buf = bytearray(PackedInteger.MAX_LONG_LENGTH)
-        offset = PackedInteger.write_sorted_long(buf, 0, value)
-        bos.write_bytearray(buf, 0, offset)
-
-    @staticmethod
     def write_record(bos, record):
         """
         Writes a dict.
 
         This is public to allow a caller to get the size of a value outside of
         the context of serialization.
         """
         BinaryProtocol.write_field_value(bos, record)
 
     @staticmethod
-    def write_sequence_length(bos, length):
-        """
-        Writes a sequence length. The length is represented as a packed int,
-        with -1 representing None. Although we don't enforce maximum sequence
-        lengths yet, this entrypoint provides a place to do that.
-
-        :param bos: the byte output stream.
-        :type bos: ByteOutputStream
-        :param length: the sequence length or -1.
-        :type length: int
-        :raises IllegalArgumentException: raises the exception if length is less
-            than -1.
-        """
-        if length < -1:
-            raise IllegalArgumentException(
-                'Invalid sequence length: ' + str(length))
-        BinaryProtocol.write_packed_int(bos, length)
-
-    @staticmethod
-    def write_serial_version(bos, serial_version):
-        # Writes the (short) serial version
-        bos.write_short_int(serial_version)
-
-    @staticmethod
-    def write_string(bos, value):
-        """
-        Writes a possibly None or empty string to an output stream using
-        standard UTF-8 format.
-
-        First writes a packed int representing the length of the UTF-8 encoding
-        of the string, or -1 if the string is None, followed by the UTF-8
-        encoding for non-empty strings.
-
-        :param bos: the byte output stream.
-        :type bos: ByteOutputStream
-        :param value: the string or None.
-        :type value: str or None
-        :returns: the number of bytes that the string take.
-        :rtype: int
-        """
-        if value is None:
-            return BinaryProtocol.write_packed_int(bos, -1)
-        try:
-            buf = bytearray(value.encode('utf-8'))
-        except UnicodeDecodeError:
-            buf = bytearray(value)
-        length = len(buf)
-        int_len = BinaryProtocol.write_packed_int(bos, length)
-        if length > 0:
-            bos.write_bytearray(buf)
-        return int_len + length
-
-    @staticmethod
     def write_ttl(bos, ttl):
         if ttl is None:
-            BinaryProtocol.write_packed_long(bos, -1)
+            SerdeUtil.write_packed_long(bos, -1)
             return
-        BinaryProtocol.write_packed_long(bos, ttl.get_value())
+        SerdeUtil.write_packed_long(bos, ttl.get_value())
         if ttl.unit_is_days():
             bos.write_byte(TimeUnit.DAYS)
         elif ttl.unit_is_hours():
             bos.write_byte(TimeUnit.HOURS)
         else:
             raise IllegalStateException('Invalid TTL unit in ttl ' + str(ttl))
 
     @staticmethod
     def write_version(bos, version):
         CheckValue.check_not_none(version, 'array')
-        BinaryProtocol.write_bytearray(bos, version.get_bytes())
-
-    @staticmethod
-    def _get_table_state(state):
-        if state == BinaryProtocol.TABLE_STATE.ACTIVE:
-            return State.ACTIVE
-        elif state == BinaryProtocol.TABLE_STATE.CREATING:
-            return State.CREATING
-        elif state == BinaryProtocol.TABLE_STATE.DROPPED:
-            return State.DROPPED
-        elif state == BinaryProtocol.TABLE_STATE.DROPPING:
-            return State.DROPPING
-        elif state == BinaryProtocol.TABLE_STATE.UPDATING:
-            return State.UPDATING
-        else:
-            raise IllegalStateException('Unknown table state ' + str(state))
-
-    @staticmethod
-    def _get_type(value):
-        if isinstance(value, list):
-            return BinaryProtocol.FIELD_VALUE_TYPE.ARRAY
-        elif isinstance(value, bytearray):
-            return BinaryProtocol.FIELD_VALUE_TYPE.BINARY
-        elif isinstance(value, bool):
-            return BinaryProtocol.FIELD_VALUE_TYPE.BOOLEAN
-        elif isinstance(value, float):
-            return BinaryProtocol.FIELD_VALUE_TYPE.DOUBLE
-        elif CheckValue.is_int(value):
-            return BinaryProtocol.FIELD_VALUE_TYPE.INTEGER
-        elif CheckValue.is_long(value):
-            return BinaryProtocol.FIELD_VALUE_TYPE.LONG
-        elif isinstance(value, dict):
-            return BinaryProtocol.FIELD_VALUE_TYPE.MAP
-        elif CheckValue.is_str(value):
-            return BinaryProtocol.FIELD_VALUE_TYPE.STRING
-        elif isinstance(value, datetime):
-            return BinaryProtocol.FIELD_VALUE_TYPE.TIMESTAMP
-        elif isinstance(value, Decimal) or CheckValue.is_overlong(value):
-            return BinaryProtocol.FIELD_VALUE_TYPE.NUMBER
-        elif value is None:
-            return BinaryProtocol.FIELD_VALUE_TYPE.NULL
-        else:
-            raise IllegalStateException(
-                'Unknown value type ' + str(type(value)))
-
-
-class RequestSerializer(object):
-    """
-    Base class of different kinds of RequestSerializer.
-    """
-    __metaclass__ = ABCMeta
-
-    @abstractmethod
-    def serialize(self, request, bos, serial_version):
-        """
-        Method used to serialize the request.
-        """
-        pass
-
-    @abstractmethod
-    def deserialize(self, request, bis, serial_version):
-        """
-        Method used to deserialize the request.
-        """
-        pass
+        SerdeUtil.write_bytearray(bos, version.get_bytes())
 
 
 class DeleteRequestSerializer(RequestSerializer):
     """
     The flag indicates if the serializer is used for a standalone request or a
     sub operation of WriteMultiple request.
 
@@ -968,16 +367,16 @@
     """
 
     def __init__(self, is_sub_request=False):
         self._is_sub_request = is_sub_request
 
     def serialize(self, request, bos, serial_version):
         match_version = request.get_match_version()
-        op_code = (BinaryProtocol.OP_CODE.DELETE if match_version is None else
-                   BinaryProtocol.OP_CODE.DELETE_IF_VERSION)
+        op_code = (SerdeUtil.OP_CODE.DELETE if match_version is None else
+                   SerdeUtil.OP_CODE.DELETE_IF_VERSION)
         BinaryProtocol.write_op_code(bos, op_code)
         if self._is_sub_request:
             bos.write_boolean(request.get_return_row())
         else:
             BinaryProtocol.serialize_write_request(request, bos, serial_version)
         BinaryProtocol.write_field_value(bos, request.get_key())
         if match_version is not None:
@@ -990,133 +389,133 @@
         BinaryProtocol.deserialize_write_response(bis, result, serial_version)
         return result
 
 
 class GetIndexesRequestSerializer(RequestSerializer):
 
     def serialize(self, request, bos, serial_version):
-        BinaryProtocol.write_op_code(bos, BinaryProtocol.OP_CODE.GET_INDEXES)
+        BinaryProtocol.write_op_code(bos, SerdeUtil.OP_CODE.GET_INDEXES)
         BinaryProtocol.serialize_request(request, bos)
-        BinaryProtocol.write_string(bos, request.get_table_name())
+        SerdeUtil.write_string(bos, request.get_table_name())
         if request.get_index_name() is not None:
             bos.write_boolean(True)
-            BinaryProtocol.write_string(bos, request.get_index_name())
+            SerdeUtil.write_string(bos, request.get_index_name())
         else:
             bos.write_boolean(False)
 
     def deserialize(self, request, bis, serial_version):
         result = operations.GetIndexesResult()
-        num_indexes = BinaryProtocol.read_packed_int(bis)
+        num_indexes = SerdeUtil.read_packed_int(bis)
         indexes = list()
         count = 0
         while count < num_indexes:
             indexes.append(self._deserialize_index_info(bis))
             count += 1
         result.set_indexes(indexes)
         return result
 
     @staticmethod
     def _deserialize_index_info(bis):
-        index_name = BinaryProtocol.read_string(bis)
-        num_fields = BinaryProtocol.read_packed_int(bis)
+        index_name = SerdeUtil.read_string(bis)
+        num_fields = SerdeUtil.read_packed_int(bis)
         field_names = list()
         count = 0
         while count < num_fields:
-            field_names.append(BinaryProtocol.read_string(bis))
+            field_names.append(SerdeUtil.read_string(bis))
             count += 1
         return IndexInfo(index_name, field_names)
 
 
 class GetRequestSerializer(RequestSerializer):
 
     def serialize(self, request, bos, serial_version):
-        BinaryProtocol.write_op_code(bos, BinaryProtocol.OP_CODE.GET)
+        BinaryProtocol.write_op_code(bos, SerdeUtil.OP_CODE.GET)
         BinaryProtocol.serialize_read_request(request, bos)
         BinaryProtocol.write_field_value(bos, request.get_key())
 
     def deserialize(self, request, bis, serial_version):
         result = operations.GetResult()
         BinaryProtocol.deserialize_consumed_capacity(bis, result)
         has_row = bis.read_boolean()
         if has_row:
-            result.set_value(BinaryProtocol.convert_value_to_none(
+            result.set_value(SerdeUtil.convert_value_to_none(
                 BinaryProtocol.read_field_value(bis)))
-            result.set_expiration_time(BinaryProtocol.read_packed_long(bis))
+            result.set_expiration_time(SerdeUtil.read_packed_long(bis))
             result.set_version(BinaryProtocol.read_version(bis))
             if serial_version > 2:
-                result.set_modification_time(BinaryProtocol.read_packed_long(bis))
+                result.set_modification_time(SerdeUtil.read_packed_long(bis))
             else:
                 result.set_modification_time(0)
         return result
 
 
 class GetTableRequestSerializer(RequestSerializer):
 
     def serialize(self, request, bos, serial_version):
-        BinaryProtocol.write_op_code(bos, BinaryProtocol.OP_CODE.GET_TABLE)
+        BinaryProtocol.write_op_code(bos, SerdeUtil.OP_CODE.GET_TABLE)
         BinaryProtocol.serialize_request(request, bos)
-        BinaryProtocol.write_string(bos, request.get_table_name())
-        BinaryProtocol.write_string(bos, request.get_operation_id())
+        SerdeUtil.write_string(bos, request.get_table_name())
+        SerdeUtil.write_string(bos, request.get_operation_id())
 
     def deserialize(self, request, bis, serial_version):
         result = operations.TableResult()
         BinaryProtocol.deserialize_table_result(bis, result, serial_version)
         return result
 
 
 class ListTablesRequestSerializer(RequestSerializer):
 
     def serialize(self, request, bos, serial_version):
-        BinaryProtocol.write_op_code(bos, BinaryProtocol.OP_CODE.LIST_TABLES)
+        BinaryProtocol.write_op_code(bos, SerdeUtil.OP_CODE.LIST_TABLES)
         BinaryProtocol.serialize_request(request, bos)
         bos.write_int(request.get_start_index())
         bos.write_int(request.get_limit())
         # new in V2.
-        BinaryProtocol.write_string(bos, request.get_namespace())
+        SerdeUtil.write_string(bos, request.get_namespace())
 
     def deserialize(self, request, bis, serial_version):
         result = operations.ListTablesResult()
-        num_tables = BinaryProtocol.read_packed_int(bis)
+        num_tables = SerdeUtil.read_packed_int(bis)
         tables = list()
         count = 0
         while count < num_tables:
-            tables.append(BinaryProtocol.read_string(bis))
+            tables.append(SerdeUtil.read_string(bis))
             count += 1
         result.set_tables(tables)
-        result.set_last_index_returned(BinaryProtocol.read_packed_int(bis))
+        result.set_last_index_returned(SerdeUtil.read_packed_int(bis))
         return result
 
 
 class MultiDeleteRequestSerializer(RequestSerializer):
 
     def serialize(self, request, bos, serial_version):
-        BinaryProtocol.write_op_code(bos, BinaryProtocol.OP_CODE.MULTI_DELETE)
+        BinaryProtocol.write_op_code(bos, SerdeUtil.OP_CODE.MULTI_DELETE)
         BinaryProtocol.serialize_request(request, bos)
-        BinaryProtocol.write_string(bos, request.get_table_name())
+        SerdeUtil.write_string(bos, request.get_table_name())
         BinaryProtocol.write_durability(request, bos, serial_version)
         BinaryProtocol.write_field_value(bos, request.get_key())
         BinaryProtocol.write_field_range(bos, request.get_range())
-        BinaryProtocol.write_packed_int(bos, request.get_max_write_kb())
-        BinaryProtocol.write_bytearray(bos, request.get_continuation_key())
+        SerdeUtil.write_packed_int(bos, request.get_max_write_kb())
+        SerdeUtil.write_bytearray(bos, request.get_continuation_key())
 
     def deserialize(self, request, bis, serial_version):
         result = operations.MultiDeleteResult()
         BinaryProtocol.deserialize_consumed_capacity(bis, result)
-        result.set_num_deletions(BinaryProtocol.read_packed_int(bis))
-        result.set_continuation_key(BinaryProtocol.read_bytearray(bis))
+        result.set_num_deletions(SerdeUtil.read_packed_int(bis))
+        result.set_continuation_key(SerdeUtil.read_bytearray(bis, False))
         return result
 
 
 class PrepareRequestSerializer(RequestSerializer):
 
     # Prepare a query.
     def serialize(self, request, bos, serial_version):
-        BinaryProtocol.write_op_code(bos, BinaryProtocol.OP_CODE.PREPARE)
+        BinaryProtocol.write_op_code(bos, SerdeUtil.OP_CODE.PREPARE)
         BinaryProtocol.serialize_request(request, bos)
-        BinaryProtocol.write_string(bos, request.get_statement())
+        SerdeUtil.write_string(bos, request.get_statement())
         bos.write_short_int(QueryDriver.QUERY_VERSION)
         bos.write_boolean(request.get_query_plan())
 
     def deserialize(self, request, bis, serial_version):
         result = operations.PrepareResult()
         BinaryProtocol.deserialize_consumed_capacity(bis, result)
         prep_stmt = PrepareRequestSerializer.deserialize_internal(
@@ -1135,44 +534,44 @@
         byte (number of tables)
         namespace (string)
         tablename (string)
         operation (1 byte)
         """
         saved_offset = bis.get_offset()
         bis.set_offset(saved_offset + 37)
-        namespace = BinaryProtocol.read_string(bis)
-        table_name = BinaryProtocol.read_string(bis)
+        namespace = SerdeUtil.read_string(bis)
+        table_name = SerdeUtil.read_string(bis)
         operation = bis.read_byte()
         bis.set_offset(saved_offset)
 
-        proxy_statement = BinaryProtocol.read_bytearray_with_int(bis)
+        proxy_statement = SerdeUtil.read_bytearray_with_int(bis)
         num_iterators = 0
         num_registers = 0
         external_vars = None
         topology_info = None
         query_plan = None
         if get_query_plan:
-            query_plan = BinaryProtocol.read_string(bis)
+            query_plan = SerdeUtil.read_string(bis)
         driver_plan = PlanIter.deserialize_iter(bis)
         if driver_plan is not None:
             num_iterators = bis.read_int()
             num_registers = bis.read_int()
-            BinaryProtocol.trace(
+            SerdeUtil.trace(
                 'PREP-RESULT: Query Plan:\n' + driver_plan.display() + '\n', 1)
             length = bis.read_int()
             if length > 0:
                 external_vars = dict()
                 for i in range(length):
-                    var_name = BinaryProtocol.read_string(bis)
+                    var_name = SerdeUtil.read_string(bis)
                     var_id = bis.read_int()
                     external_vars[var_name] = var_id
             topology_info = BinaryProtocol.read_topology_info(bis)
         return PreparedStatement(
-            sql_text, query_plan, topology_info, proxy_statement, driver_plan,
-            num_iterators, num_registers, external_vars,
+            sql_text, query_plan, None, topology_info, proxy_statement,
+            driver_plan, num_iterators, num_registers, external_vars,
             namespace, table_name, operation)
 
 
 class PutRequestSerializer(RequestSerializer):
     """
     The flag indicates if the serializer is used for a standalone request or a
     sub operation of WriteMultiple request.
@@ -1181,22 +580,22 @@
     timeout, namespace and table_name will be skipped during serialization.
     """
 
     def __init__(self, is_sub_request=False):
         self._is_sub_request = is_sub_request
 
     def serialize(self, request, bos, serial_version):
-        op = self._get_op_code(request)
+        op = SerdeUtil.get_put_op_code(request)
         BinaryProtocol.write_op_code(bos, op)
         if self._is_sub_request:
             bos.write_boolean(request.get_return_row())
         else:
             BinaryProtocol.serialize_write_request(request, bos, serial_version)
         bos.write_boolean(request.get_exact_match())
-        BinaryProtocol.write_packed_int(bos, request.get_identity_cache_size())
+        SerdeUtil.write_packed_int(bos, request.get_identity_cache_size())
         BinaryProtocol.write_record(bos, request.get_value())
         bos.write_boolean(request.get_update_ttl())
         BinaryProtocol.write_ttl(bos, request.get_ttl())
         if request.get_match_version() is not None:
             BinaryProtocol.write_version(bos, request.get_match_version())
 
     def deserialize(self, request, bis, serial_version):
@@ -1207,90 +606,72 @@
             result.set_version(BinaryProtocol.read_version(bis))
         # return row info.
         BinaryProtocol.deserialize_write_response(bis, result, serial_version)
         # generated identity column value
         BinaryProtocol.deserialize_generated_value(bis, result)
         return result
 
-    @staticmethod
-    def _get_op_code(request):
-        """
-        Assumes that the request has been validated and only one of the if
-        options is set, if any.
-        """
-        request_op = request.get_option()
-        if request_op is None:
-            return BinaryProtocol.OP_CODE.PUT
-        elif request_op is PutOption.IF_ABSENT:
-            return BinaryProtocol.OP_CODE.PUT_IF_ABSENT
-        elif request_op is PutOption.IF_PRESENT:
-            return BinaryProtocol.OP_CODE.PUT_IF_PRESENT
-        elif request_op is PutOption.IF_VERSION:
-            return BinaryProtocol.OP_CODE.PUT_IF_VERSION
-        else:
-            raise IllegalStateException('Unknown Options ' + str(request_op))
-
 
 class QueryRequestSerializer(RequestSerializer):
 
     def serialize(self, request, bos, serial_version):
         # write unconditional state first.
-        BinaryProtocol.write_op_code(bos, BinaryProtocol.OP_CODE.QUERY)
+        BinaryProtocol.write_op_code(bos, SerdeUtil.OP_CODE.QUERY)
         BinaryProtocol.serialize_request(request, bos)
         bos.write_byte(request.get_consistency())
-        BinaryProtocol.write_packed_int(bos, request.get_limit())
-        BinaryProtocol.write_packed_int(bos, request.get_max_read_kb())
-        BinaryProtocol.write_bytearray(bos, request.get_cont_key())
+        SerdeUtil.write_packed_int(bos, request.get_limit())
+        SerdeUtil.write_packed_int(bos, request.get_max_read_kb())
+        SerdeUtil.write_bytearray(bos, request.get_cont_key())
         bos.write_boolean(request.is_prepared())
         # The following 7 fields were added in V2.
         bos.write_short_int(QueryDriver.QUERY_VERSION)
         bos.write_byte(request.get_trace_level())
-        BinaryProtocol.write_packed_int(bos, request.get_max_write_kb())
+        SerdeUtil.write_packed_int(bos, request.get_max_write_kb())
         BinaryProtocol.write_math_context(bos, request.get_math_context())
-        BinaryProtocol.write_packed_int(bos, request.topology_seq_num())
-        BinaryProtocol.write_packed_int(bos, request.get_shard_id())
+        SerdeUtil.write_packed_int(bos, request.topology_seq_num())
+        SerdeUtil.write_packed_int(bos, request.get_shard_id())
         bos.write_boolean(request.is_prepared() and request.is_simple_query())
         if request.is_prepared():
             ps = request.get_prepared_statement()
-            BinaryProtocol.write_bytearray_with_int(bos, ps.get_statement())
+            SerdeUtil.write_bytearray_with_int(bos, ps.get_statement())
             if ps.get_variables() is not None:
                 variables = ps.get_variables()
-                BinaryProtocol.write_packed_int(bos, len(variables))
+                SerdeUtil.write_packed_int(bos, len(variables))
                 for key in variables:
-                    BinaryProtocol.write_string(bos, key)
+                    SerdeUtil.write_string(bos, key)
                     BinaryProtocol.write_field_value(bos, variables[key])
             else:
-                BinaryProtocol.write_packed_int(bos, 0)
+                SerdeUtil.write_packed_int(bos, 0)
         else:
-            BinaryProtocol.write_string(bos, request.get_statement())
+            SerdeUtil.write_string(bos, request.get_statement())
 
     def deserialize(self, request, bis, serial_version):
         prep = request.get_prepared_statement()
         is_prepared = prep is not None
         result = operations.QueryResult(request)
         num_rows = bis.read_int()
         is_sort_phase1_result = bis.read_boolean()
         results = list()
         count = 0
         while count < num_rows:
             results.append(BinaryProtocol.read_field_value(bis))
             count += 1
         if is_sort_phase1_result:
             result.set_is_in_phase1(bis.read_boolean())
-            pids = BinaryProtocol.read_packed_int_array(bis)
+            pids = SerdeUtil.read_packed_int_array(bis)
             if pids is not None:
                 result.set_pids(pids)
                 result.set_num_results_per_pid(
-                    BinaryProtocol.read_packed_int_array(bis))
+                    SerdeUtil.read_packed_int_array(bis))
                 cont_keys = list()
                 for i in range(len(pids)):
-                    cont_keys.append(BinaryProtocol.read_bytearray(bis))
+                    cont_keys.append(SerdeUtil.read_bytearray(bis, False))
                 result.set_partition_cont_keys(cont_keys)
         BinaryProtocol.deserialize_consumed_capacity(bis, result)
-        result.set_continuation_key(BinaryProtocol.read_bytearray(bis))
+        result.set_continuation_key(SerdeUtil.read_bytearray(bis, False))
         request.set_cont_key(result.get_continuation_key())
         # In V2, if the QueryRequest was not initially prepared, the prepared
         # statement created at the proxy is returned back along with the query
         # results, so that the preparation does not need to be done during each
         # query batch.
         if not is_prepared:
             prep = PrepareRequestSerializer.deserialize_internal(
@@ -1308,61 +689,61 @@
                 result.set_reached_limit(bis.read_boolean())
                 topology_info = BinaryProtocol.read_topology_info(bis)
                 driver = request.get_driver()
                 if topology_info is not None:
                     prep.set_topology_info(topology_info)
                     driver.set_topology_info(topology_info)
         else:
-            results = BinaryProtocol.convert_value_to_none(results)
+            results = SerdeUtil.convert_value_to_none(results)
         result.set_results(results)
         return result
 
 
 class SystemRequestSerializer(RequestSerializer):
 
     def serialize(self, request, bos, serial_version):
         BinaryProtocol.write_op_code(
-            bos, BinaryProtocol.OP_CODE.SYSTEM_REQUEST)
+            bos, SerdeUtil.OP_CODE.SYSTEM_REQUEST)
         BinaryProtocol.serialize_request(request, bos)
-        BinaryProtocol.write_string(bos, request.get_statement())
+        SerdeUtil.write_string(bos, request.get_statement())
 
     def deserialize(self, request, bis, serial_version):
         return BinaryProtocol.deserialize_system_result(bis)
 
 
 class SystemStatusRequestSerializer(RequestSerializer):
 
     def serialize(self, request, bos, serial_version):
         BinaryProtocol.write_op_code(
-            bos, BinaryProtocol.OP_CODE.SYSTEM_STATUS_REQUEST)
+            bos, SerdeUtil.OP_CODE.SYSTEM_STATUS_REQUEST)
         BinaryProtocol.serialize_request(request, bos)
-        BinaryProtocol.write_string(bos, request.get_operation_id())
-        BinaryProtocol.write_string(bos, request.get_statement())
+        SerdeUtil.write_string(bos, request.get_operation_id())
+        SerdeUtil.write_string(bos, request.get_statement())
 
     def deserialize(self, request, bis, serial_version):
         return BinaryProtocol.deserialize_system_result(bis)
 
 
 class TableRequestSerializer(RequestSerializer):
 
     def serialize(self, request, bos, serial_version):
-        BinaryProtocol.write_op_code(bos, BinaryProtocol.OP_CODE.TABLE_REQUEST)
+        BinaryProtocol.write_op_code(bos, SerdeUtil.OP_CODE.TABLE_REQUEST)
         BinaryProtocol.serialize_request(request, bos)
-        BinaryProtocol.write_string(bos, request.get_statement())
+        SerdeUtil.write_string(bos, request.get_statement())
         limits = request.get_table_limits()
         if limits is not None:
             bos.write_boolean(True)
             bos.write_int(limits.get_read_units())
             bos.write_int(limits.get_write_units())
             bos.write_int(limits.get_storage_gb())
             if serial_version > 2:
                 bos.write_byte(limits.get_mode())
             if request.get_table_name() is not None:
                 bos.write_boolean(True)
-                BinaryProtocol.write_string(bos, request.get_table_name())
+                SerdeUtil.write_string(bos, request.get_table_name())
             else:
                 bos.write_boolean(False)
         else:
             bos.write_boolean(False)
 
     def deserialize(self, request, bis, serial_version):
         result = operations.TableResult()
@@ -1370,108 +751,103 @@
         return result
 
 
 class TableUsageRequestSerializer(RequestSerializer):
 
     def serialize(self, request, bos, serial_version):
         BinaryProtocol.write_op_code(
-            bos, BinaryProtocol.OP_CODE.GET_TABLE_USAGE)
+            bos, SerdeUtil.OP_CODE.GET_TABLE_USAGE)
         BinaryProtocol.serialize_request(request, bos)
-        BinaryProtocol.write_string(bos, request.get_table_name())
-        BinaryProtocol.write_packed_long(bos, request.get_start_time())
-        BinaryProtocol.write_packed_long(bos, request.get_end_time())
-        BinaryProtocol.write_packed_int(bos, request.get_limit())
+        SerdeUtil.write_string(bos, request.get_table_name())
+        SerdeUtil.write_packed_long(bos, request.get_start_time())
+        SerdeUtil.write_packed_long(bos, request.get_end_time())
+        SerdeUtil.write_packed_int(bos, request.get_limit())
 
     def deserialize(self, request, bis, serial_version):
         result = operations.TableUsageResult()
         # don't use tenant_id, but it's in the result
-        BinaryProtocol.read_string(bis)
-        result.set_table_name(BinaryProtocol.read_string(bis))
-        num_results = BinaryProtocol.read_packed_int(bis)
+        SerdeUtil.read_string(bis)
+        result.set_table_name(SerdeUtil.read_string(bis))
+        num_results = SerdeUtil.read_packed_int(bis)
         usage_records = list()
         count = 0
         while count < num_results:
             usage_records.append(self._deserialize_usage(bis))
             count += 1
         result.set_usage_records(usage_records)
         return result
 
     @staticmethod
     def _deserialize_usage(bis):
-        start_time_ms = BinaryProtocol.read_packed_long(bis)
-        seconds_in_period = BinaryProtocol.read_packed_int(bis)
-        read_units = BinaryProtocol.read_packed_int(bis)
-        write_units = BinaryProtocol.read_packed_int(bis)
-        storage_gb = BinaryProtocol.read_packed_int(bis)
-        read_throttle_count = BinaryProtocol.read_packed_int(bis)
-        write_throttle_count = BinaryProtocol.read_packed_int(bis)
-        storage_throttle_count = BinaryProtocol.read_packed_int(bis)
+        start_time_ms = SerdeUtil.read_packed_long(bis)
+        seconds_in_period = SerdeUtil.read_packed_int(bis)
+        read_units = SerdeUtil.read_packed_int(bis)
+        write_units = SerdeUtil.read_packed_int(bis)
+        storage_gb = SerdeUtil.read_packed_int(bis)
+        read_throttle_count = SerdeUtil.read_packed_int(bis)
+        write_throttle_count = SerdeUtil.read_packed_int(bis)
+        storage_throttle_count = SerdeUtil.read_packed_int(bis)
         usage = TableUsage(start_time_ms, seconds_in_period, read_units,
                            write_units, storage_gb, read_throttle_count,
-                           write_throttle_count, storage_throttle_count)
+                           write_throttle_count, storage_throttle_count, 0)
         return usage
 
 
 class WriteMultipleRequestSerializer(RequestSerializer):
 
     def serialize(self, request, bos, serial_version):
         put_serializer = PutRequestSerializer(True)
         delete_serializer = DeleteRequestSerializer(True)
         num = request.get_num_operations()
 
         # OpCode
         BinaryProtocol.write_op_code(
-            bos, BinaryProtocol.OP_CODE.WRITE_MULTIPLE)
+            bos, SerdeUtil.OP_CODE.WRITE_MULTIPLE)
         BinaryProtocol.serialize_request(request, bos)
 
         # TableName
         # If all ops use the same table name, write that
         # single table name to the output stream.
         # If any of them are different, write all table
         # names, comma-separated.
         if request.is_single_table():
-            BinaryProtocol.write_string(bos, request.get_table_name())
+            SerdeUtil.write_string(bos, request.get_table_name())
         else:
             table_names = ""
             for op in request.get_operations():
                 if len(table_names) > 0:
                     table_names += ","
                 table_names += op.get_request().get_table_name()
-            BinaryProtocol.write_string(bos, table_names)
+            SerdeUtil.write_string(bos, table_names)
 
         # Number of operations
-        BinaryProtocol.write_packed_int(bos, num)
+        SerdeUtil.write_packed_int(bos, num)
 
         # Durability settings
         BinaryProtocol.write_durability(request, bos, serial_version)
 
         # Operations
         for op in request.get_operations():
-            start = bos.get_offset()
 
             # Abort if successful flag
             bos.write_boolean(op.is_abort_if_unsuccessful())
             req = op.get_request()
-            req.set_check_request_size(request.get_check_request_size())
             if str(req) == 'PutRequest':
                 put_serializer.serialize(req, bos, serial_version)
             else:
                 assert str(req) == 'DeleteRequest'
                 delete_serializer.serialize(req, bos, serial_version)
-            # Check each sub request size limit.
-            BinaryProtocol.check_request_size_limit(
-                req, (bos.get_offset() - start))
 
     def deserialize(self, request, bis, serial_version):
         result = operations.WriteMultipleResult()
         # Success flag
         succeed = bis.read_boolean()
         BinaryProtocol.deserialize_consumed_capacity(bis, result)
         if succeed:
-            num = BinaryProtocol.read_packed_int(bis)
+            num = SerdeUtil.read_packed_int(bis)
             count = 0
             while count < num:
                 result.add_result(self._create_operation_result(bis, serial_version))
                 count += 1
         else:
             result.set_failed_operation_index(bis.read_byte())
             result.add_result(self._create_operation_result(bis, serial_version))
```

### Comparing `borneo-5.3.7/src/borneo/__init__.py` & `borneo-5.4.1/src/borneo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #
-# Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 # This environment variable suppresses the import of all services
 # when importing from the OCI SDK. It can greatly speed up
 # program startup
 import os
-os.environ['OCI_PYTHON_SDK_NO_SERVICE_IMPORTS']='1'
+
+os.environ['OCI_PYTHON_SDK_NO_SERVICE_IMPORTS'] = '1'
 
 from . import iam
 from . import kv
 from .auth import AuthorizationProvider
 from .common import (
     Consistency, Durability, FieldRange, PutOption, ResourcePrincipalClaimKeys, State,
     SystemState, TableLimits, TimeToLive, TimeUnit, UserInfo, Version,
```

### Comparing `borneo-5.3.7/src/borneo/operations.py` & `borneo-5.4.1/src/borneo/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,66 @@
 #
-# Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 from abc import abstractmethod
 from datetime import datetime
-from dateutil import parser, tz
 from decimal import Context, ROUND_HALF_EVEN
 from json import loads
-from time import mktime, sleep, time
+from time import sleep, time
+
+from dateutil import tz
 
 from .common import (
     CheckValue, Consistency, Durability, FieldRange, PreparedStatement,
     PutOption, State, SystemState, TableLimits, TimeToLive, Version,
     deprecated)
 from .exception import (
     IllegalArgumentException, RequestTimeoutException)
 from .http import RateLimiter
 from .serde import (
-    BinaryProtocol, DeleteRequestSerializer, GetIndexesRequestSerializer,
-    GetRequestSerializer, GetTableRequestSerializer,
-    ListTablesRequestSerializer, MultiDeleteRequestSerializer,
+    DeleteRequestSerializer, GetIndexesRequestSerializer,
+    GetRequestSerializer, GetTableRequestSerializer, ListTablesRequestSerializer,
+    MultiDeleteRequestSerializer,
     PrepareRequestSerializer, PutRequestSerializer, QueryRequestSerializer,
     SystemRequestSerializer, SystemStatusRequestSerializer,
     TableRequestSerializer, TableUsageRequestSerializer,
     WriteMultipleRequestSerializer)
+from .serdeutil import SerdeUtil
+
 try:
     from . import config
+    from . import serdeutil
 except ImportError:
     import config
+    import serdeutil
+
+import borneo.nson
 
 
 class Request(object):
     """
     A request is a class used as a base for all requests types. Public state and
-    methods are implemented by extending classes.
+    methods are implemented by extending classes. This pattern is used so that
+    fluent construction works properly for the extending classes
     """
 
     def __init__(self):
-        self._check_request_size = True
         # Cloud service only.
         self._compartment = None
         self._read_rate_limiter = None
         self._retry_stats = None
         self._start_time_ms = 0
         self._table_name = None
         self._timeout_ms = 0
         self._write_rate_limiter = None
         self._rate_limit_delayed_ms = 0
+        self._namespace = None
 
     def add_retry_delay_ms(self, millis):
         """
         Internal use only.
 
         This adds time to the total time spent processing retries during a
         single request processing operation.
@@ -92,18 +100,14 @@
         Internal use only.
 
         :returns: True if the request expects to do writes (incur write units).
         :rtype: boolean
         """
         return False
 
-    def get_check_request_size(self):
-        # Internal use only.
-        return self._check_request_size
-
     def get_compartment(self):
         """
         Cloud service only.
 
         Get the compartment id or name if set for the request.
 
         :returns: compartment id or name if set for the request, otherwise None
@@ -214,19 +218,14 @@
 
         Increments the number of retries during the request operation.
         """
         if self._retry_stats is None:
             self._retry_stats = RetryStats()
         self._retry_stats.increment_retries()
 
-    def set_check_request_size(self, check_request_size):
-        # Internal use only.
-        self._check_request_size = check_request_size
-        return self
-
     def set_compartment_internal(self, compartment):
         """
         Internal use only.
 
         Sets the compartment id or name to use for the operation.
 
         :param compartment: the compartment name or id.
@@ -341,14 +340,45 @@
         :type table_name: str or None
         :raises IllegalArgumentException: raises the exception if table_name is
             not a string.
         """
         CheckValue.check_str(table_name, 'table_name', True)
         self._table_name = table_name
 
+    def set_namespace(self, namespace):
+        """
+        Internal use only
+
+        On-premises only
+
+        Sets the namespace to use for the operation. This will override
+        any configured default value.
+
+        :param namespace: the namespace
+        :type namespace: str
+        :raises IllegalArgumentException: raises the exception if namespace is
+            not a string.
+        :versionadded: 5.4.0
+        """
+        CheckValue.check_str(namespace, 'namespace', True)
+        self._namespace = namespace
+
+    def get_namespace(self):
+        """
+        On-premises only
+
+        Returns the namespace to use for the operation or None if not
+        set.
+
+        :returns: namespace, or None if not set.
+        :rtype: str
+        :versionadded: 5.4.0
+        """
+        return self._namespace
+
     def _set_timeout(self, timeout_ms):
         CheckValue.check_int_gt_zero(timeout_ms, 'timeout_ms')
         self._timeout_ms = timeout_ms
 
     def get_rate_limit_delayed_ms(self):
         """
         Get the time the operation was delayed due to rate limiting. Cloud only.
@@ -406,17 +436,14 @@
         super(WriteRequest, self).__init__()
         self._return_row = False
         self._durability = None
 
     def __str__(self):
         return 'WriteRequest'
 
-    def __str__(self):
-        return 'WriteRequest'
-
     def does_writes(self):
         return True
 
     def _set_return_row(self, return_row):
         CheckValue.check_boolean(return_row, 'return_row')
         self._return_row = return_row
 
@@ -435,24 +462,25 @@
 
     def _get_durability(self):
         return self._durability
 
     def _validate_write_request(self, request_name):
         if self.get_table_name() is None:
             raise IllegalArgumentException(
-                 "{} requires table name".format(request_name))
+                "{} requires table name".format(request_name))
 
     def get_durability(self):
         pass
 
     def get_request_name(self):
         # type: () -> str
         return "Write"
 
-    def get_type_name(self):
+    @staticmethod
+    def get_type_name():
         # type: () -> str
         return "Write"
 
 
 class ReadRequest(Request):
     """
     Represents a base class for read operations such as
@@ -497,14 +525,15 @@
                 request_name + ' requires table name.')
 
     def get_request_name(self):
         # type: () -> str
         return "Read"
 
 
+# noinspection PyUnusedLocal
 class DeleteRequest(WriteRequest):
     """
     Represents the input to a :py:meth:`NoSQLHandle.delete` operation.
 
     This request can be used to perform unconditional and conditional deletes:
         * Delete any existing row. This is the default.
         * Succeed only if the row exists and and its :py:class:`Version`
@@ -720,22 +749,29 @@
     def validate(self):
         # Validates the state of the object when complete.
         self._validate_write_request('DeleteRequest')
         if self._key is None:
             raise IllegalArgumentException('DeleteRequest requires a key.')
 
     @staticmethod
-    def create_serializer():
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        if serial_version >= SerdeUtil.SERIAL_VERSION_4:
+            return borneo.nson.DeleteRequestSerializer()
         return DeleteRequestSerializer()
 
     def get_request_name(self):
         # type: () -> str
         return "Delete"
 
 
+# noinspection PyUnusedLocal
 class GetIndexesRequest(Request):
     """
     Represents the argument of a :py:meth:`NoSQLHandle.get_indexes` operation
     which returns the information of a specific index or all indexes of the
     specified table, as returned in :py:class:`GetIndexesResult`.
 
     The table name is a required parameter.
@@ -842,22 +878,29 @@
 
     def validate(self):
         if self.get_table_name() is None:
             raise IllegalArgumentException(
                 'GetIndexesRequest requires a table name.')
 
     @staticmethod
-    def create_serializer():
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        if serial_version >= SerdeUtil.SERIAL_VERSION_4:
+            return borneo.nson.GetIndexesRequestSerializer()
         return GetIndexesRequestSerializer()
 
     def get_request_name(self):
         # type: () -> str
         return "GetIndexes"
 
 
+# noinspection PyUnusedLocal
 class GetRequest(ReadRequest):
     """
     Represents the input to a :py:meth:`NoSQLHandle.get` operation which returns
     a single row based on the specified key.
 
     The table name and key are required parameters.
     """
@@ -904,14 +947,30 @@
         parameter.
 
         :returns: the key.
         :rtype: dict
         """
         return self._key
 
+    def set_namespace(self, namespace):
+        """
+        On-premises only
+
+        Sets the namespace to use for the operation. This will override
+        any configured default value.
+
+        :param namespace: the namespace
+        :type namespace: str
+        :raises IllegalArgumentException: raises the exception if namespace is
+            not a string.
+        :versionadded: 5.4.0
+        """
+        super(GetRequest, self).set_namespace(namespace)
+        return self
+
     def set_table_name(self, table_name):
         """
         Sets the table name to use for the operation. This is a required
         parameter.
 
         :param table_name: the table name.
         :type table_name: str
@@ -1000,22 +1059,29 @@
     def validate(self):
         # Validates the state of the members of this class for use.
         self._validate_read_request('GetRequest')
         if self._key is None:
             raise IllegalArgumentException('GetRequest requires a key.')
 
     @staticmethod
-    def create_serializer():
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        if serial_version >= SerdeUtil.SERIAL_VERSION_4:
+            return borneo.nson.GetRequestSerializer()
         return GetRequestSerializer()
 
     def get_request_name(self):
         # type: () -> str
         return "Get"
 
 
+# noinspection PyUnusedLocal
 class GetTableRequest(Request):
     """
     Represents the argument of a :py:meth:`NoSQLHandle.get_table` operation
     which returns static information associated with a table, as returned in
     :py:class:`TableResult`. This information only changes in response to a
     change in table schema or a change in provisioned throughput or capacity for
     the table.
@@ -1026,14 +1092,30 @@
     def __init__(self):
         super(GetTableRequest, self).__init__()
         self._operation_id = None
 
     def __str__(self):
         return 'GetTableRequest'
 
+    def set_namespace(self, namespace):
+        """
+        On-premises only
+
+        Sets the namespace to use for the operation. This will override
+        any configured default value.
+
+        :param namespace: the namespace
+        :type namespace: str
+        :raises IllegalArgumentException: raises the exception if namespace is
+            not a string.
+        :versionadded: 5.4.0
+        """
+        super(GetTableRequest, self).set_namespace(namespace)
+        return self
+
     def set_table_name(self, table_name):
         """
         Sets the table name to use for the request.
 
         :param table_name: the table name. This is a required parameter.
         :type table_name: str
         :returns: self.
@@ -1132,15 +1214,21 @@
 
     def validate(self):
         if self.get_table_name() is None:
             raise IllegalArgumentException(
                 'GetTableRequest requires a table name.')
 
     @staticmethod
-    def create_serializer():
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        if serial_version >= SerdeUtil.SERIAL_VERSION_4:
+            return borneo.nson.GetTableRequestSerializer()
         return GetTableRequestSerializer()
 
     def get_request_name(self):
         # type: () -> str
         return "GetTable"
 
 
@@ -1304,15 +1392,21 @@
     def validate(self):
         if self._start_index < 0 or self._limit < 0:
             raise IllegalArgumentException(
                 'ListTables: start index and number of tables must be ' +
                 'non-negative.')
 
     @staticmethod
-    def create_serializer():
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        if serial_version >= SerdeUtil.SERIAL_VERSION_4:
+            return borneo.nson.ListTablesRequestSerializer()
         return ListTablesRequestSerializer()
 
     def get_request_name(self):
         # type: () -> str
         return "ListTables"
 
 
@@ -1346,16 +1440,29 @@
         self._range = None
         self._max_write_kb = 0
         self._durability = None
 
     def __str__(self):
         return 'MultiDeleteRequest'
 
-    def __str__(self):
-        return 'MultiDeleteRequest'
+    def set_namespace(self, namespace):
+        """
+        On-premises only
+
+        Sets the namespace to use for the operation. This will override
+        any configured default value.
+
+        :param namespace: the namespace
+        :type namespace: str
+        :raises IllegalArgumentException: raises the exception if namespace is
+            not a string.
+        :versionadded: 5.4.0
+        """
+        super(MultiDeleteRequest, self).set_namespace(namespace)
+        return self
 
     def set_table_name(self, table_name):
         """
         Sets the table name to use for the operation. This is a required
         parameter.
 
         :param table_name: the table name.
@@ -1567,15 +1674,21 @@
         if self._key is None:
             raise IllegalArgumentException(
                 'MultiDeleteRequest requires a key.')
         if self._range is not None:
             self._range.validate()
 
     @staticmethod
-    def create_serializer():
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        if serial_version >= SerdeUtil.SERIAL_VERSION_4:
+            return borneo.nson.MultiDeleteRequestSerializer()
         return MultiDeleteRequestSerializer()
 
     def get_request_name(self):
         # type: () -> str
         return "MultiDelete"
 
 
@@ -1593,18 +1706,35 @@
     The statement is required parameter.
     """
 
     def __init__(self):
         super(PrepareRequest, self).__init__()
         self._statement = None
         self._get_query_plan = False
+        self._get_query_schema = False
 
     def __str__(self):
         return 'PrepareRequest'
 
+    def set_namespace(self, namespace):
+        """
+        On-premises only
+
+        Sets the namespace to use for the operation. This will override
+        any configured default value.
+
+        :param namespace: the namespace
+        :type namespace: str
+        :raises IllegalArgumentException: raises the exception if namespace is
+            not a string.
+        :versionadded: 5.4.0
+        """
+        super(PrepareRequest, self).set_namespace(namespace)
+        return self
+
     def set_table_name(self, table_name):
         """
         Sets the table name for a query operation. This is used by rate limiting
         logic to manage internal rate limiters.
 
         :param table_name: the name (or OCID) of the table.
         :type table_name: str
@@ -1662,40 +1792,69 @@
             is not a str.
         """
         self.set_compartment_internal(compartment)
         return self
 
     def set_get_query_plan(self, get_query_plan):
         """
-        Sets whether a printout of the query execution plan should be included
-        in the :py:class:`PrepareResult`.
+        Sets whether a JSON representation of the query execution plan should
+        be included in the :py:class:`PreparedStatement`.
 
-        :param get_query_plan: True if a printout of the query execution plan
-            should be included in the :py:class:`PrepareResult`. False
+        :param get_query_plan: True if a the query execution plan
+            should be included in the :py:class:`PreparedStatement`. False
             otherwise.
         :type get_query_plan: bool
         :returns: self.
         :raises IllegalArgumentException: raises the exception if get_query_plan
             is not a boolean.
         """
         CheckValue.check_boolean(get_query_plan, 'get_query_plan')
         self._get_query_plan = get_query_plan
         return self
 
     def get_query_plan(self):
         """
-        Returns whether a printout of the query execution plan should be include
-        in the :py:class:`PrepareResult`.
+        Returns whether a JSON representation of the query execution plan should
+        be included in the :py:class:`PreparedStatement`.
 
-        :returns: whether a printout of the query execution plan should be
-            include in the :py:class:`PrepareResult`.
+        :returns: whether the the query execution plan should be
+            included in the :py:class:`PreparedStatement`.
         :rtype: bool
         """
         return self._get_query_plan
 
+    def set_get_query_schema(self, get_query_schema):
+        """
+        Sets whether a JSON representation of the schema of the query should
+        be included in the :py:class:`PreparedStatement`.
+
+        :param: get_query_schema: True if a JSON representation of the schema
+        of the query should be included in the :py:class:`PreparedStatement`.
+        :type get_query_schema: bool
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if get_query_schema
+            is not a boolean.
+        :versionadded: 5.4.0
+        """
+        CheckValue.check_boolean(get_query_schema, 'get_query_schema')
+        self._get_query_schema = get_query_schema
+        return self
+
+    def get_query_schema(self):
+        """
+        Returns whether a JSON representation of the schema of the query should
+        be included in the :py:class:`PreparedStatement`.
+
+        :returns: True if a JSON representation of the schema
+        of the query should be included in the :py:class:`PreparedStatement`.
+        :rtype: bool
+        :versionadded: 5.4.0
+        """
+        return self._get_query_schema
+
     def set_timeout(self, timeout_ms):
         """
         Sets the request timeout value, in milliseconds. This overrides any
         default value set in :py:class:`NoSQLHandleConfig`. The value must be
         positive.
 
         :param timeout_ms: the timeout value, in milliseconds.
@@ -1719,15 +1878,21 @@
 
     def validate(self):
         if self._statement is None:
             raise IllegalArgumentException(
                 'PrepareRequest requires a statement.')
 
     @staticmethod
-    def create_serializer():
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        if serial_version >= SerdeUtil.SERIAL_VERSION_4:
+            return borneo.nson.PrepareRequestSerializer()
         return PrepareRequestSerializer()
 
     def get_request_name(self):
         # type: () -> str
         return "Prepare"
 
 
@@ -2034,14 +2199,30 @@
         of 0 indicates that the timeout has not been set.
 
         :returns: the timeout value.
         :rtype: int
         """
         return super(PutRequest, self).get_timeout()
 
+    def set_namespace(self, namespace):
+        """
+        On-premises only
+
+        Sets the namespace to use for the operation. This will override
+        any configured default value.
+
+        :param namespace: the namespace
+        :type namespace: str
+        :raises IllegalArgumentException: raises the exception if namespace is
+            not a string.
+        :versionadded: 5.4.0
+        """
+        super(PutRequest, self).set_namespace(namespace)
+        return self
+
     def set_table_name(self, table_name):
         """
         Sets the table name to use for the operation.
 
         :param table_name: the table name.
         :type table_name: str
         :returns: self.
@@ -2128,15 +2309,21 @@
                 'PutOption.IF_VERSION.')
         if self._update_ttl and self._ttl is not None:
             raise IllegalArgumentException(
                 'PutRequest: only one of set_use_table_default_ttl or set_ttl' +
                 ' may be specified')
 
     @staticmethod
-    def create_serializer():
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        if serial_version >= SerdeUtil.SERIAL_VERSION_4:
+            return borneo.nson.PutRequestSerializer()
         return PutRequestSerializer()
 
     def get_request_name(self):
         # type: () -> str
         return "Put"
 
 
@@ -2191,14 +2378,15 @@
         self._trace_level = 0
         self._limit = 0
         self._max_read_kb = 0
         self._max_write_kb = 0
         self._max_memory_consumption = 1024 * 1024 * 1024
         self._math_context = Context(prec=7, rounding=ROUND_HALF_EVEN)
         self._consistency = None
+        self._durability = None
         self._statement = None
         self._prepared_statement = None
         self._continuation_key = None
         # If shardId is >= 0, the QueryRequest should be executed only at the
         # shard with this id. This is the case only for advanced queries that do
         # sorting.
         self._shard_id = -1
@@ -2221,14 +2409,15 @@
         internal_req.set_trace_level(self._trace_level)
         internal_req.set_limit(self._limit)
         internal_req.set_max_read_kb(self._max_read_kb)
         internal_req.set_max_write_kb(self._max_write_kb)
         internal_req.set_max_memory_consumption(self._max_memory_consumption)
         internal_req.set_math_context(self._math_context)
         internal_req.set_consistency(self._consistency)
+        internal_req.set_durability(self._durability)
         internal_req.set_prepared_statement(self._prepared_statement)
         internal_req.driver = self.driver
         internal_req.is_internal = True
         return internal_req
 
     def copy(self):
         """
@@ -2246,14 +2435,16 @@
         copy.set_limit(self._limit)
         copy.set_max_read_kb(self._max_read_kb)
         copy.set_max_write_kb(self._max_write_kb)
         copy.set_max_memory_consumption(self._max_memory_consumption)
         copy.set_math_context(self._math_context)
         if self._consistency is not None:
             copy.set_consistency(self._consistency)
+        if self._durability is not None:
+            copy.set_durability(self._durability)
         if self._prepared_statement is not None:
             copy.set_prepared_statement(self._prepared_statement)
         copy._statement = self._statement
         # leave continuationKey null to start from the beginning
         # copy._continuation_key = self._continuation_key
         self.is_internal = False
         self._shard_id = -1
@@ -2489,14 +2680,38 @@
         Returns the consistency set for this request, or None if not set.
 
         :returns: the consistency
         :rtype: Consistency
         """
         return self._consistency
 
+    def set_durability(self, durability):
+        """
+        On-premise only. Sets the durability to use for the operation. Only
+        used for queries that do writes or deletes.
+
+        :param durability: the Durability to use
+        :type durability: Durability
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if Durability
+            is not valid
+        :versionadded: 5.4.0
+        """
+        self._durability = durability
+        return self
+
+    def get_durability(self):
+        """
+        On-premise only. Gets the durability to use for the operation or
+        None if not set
+        :returns: the Durability
+        :versionadded: 5.4.0
+        """
+        return self._durability
+
     @deprecated
     def set_continuation_key(self, continuation_key):
         """
         Sets the continuation key. This is used to continue an operation that
         returned this key in its :py:class:`QueryResult`.
 
         :param continuation_key: the key which should have been obtained from
@@ -2677,15 +2892,21 @@
 
     def validate(self):
         if self._statement is None and self._prepared_statement is None:
             raise IllegalArgumentException(
                 'Either statement or prepared statement should be set.')
 
     @staticmethod
-    def create_serializer():
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        if serial_version >= SerdeUtil.SERIAL_VERSION_4:
+            return borneo.nson.QueryRequestSerializer()
         return QueryRequestSerializer()
 
     def get_request_name(self):
         # type: () -> str
         return "Query"
 
 
@@ -2778,15 +2999,21 @@
 
     def validate(self):
         if self._statement is None:
             raise IllegalArgumentException(
                 'SystemRequest requires a statement.')
 
     @staticmethod
-    def create_serializer():
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        if serial_version >= SerdeUtil.SERIAL_VERSION_4:
+            return borneo.nson.SystemRequestSerializer()
         return SystemRequestSerializer()
 
     def get_request_name(self):
         # type: () -> str
         return "System"
 
 
@@ -2900,15 +3127,21 @@
 
     def validate(self):
         if self._operation_id is None:
             raise IllegalArgumentException(
                 'SystemStatusRequest requires an operation id.')
 
     @staticmethod
-    def create_serializer():
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        if serial_version >= SerdeUtil.SERIAL_VERSION_4:
+            return borneo.nson.SystemStatusRequestSerializer()
         return SystemStatusRequestSerializer()
 
     def get_request_name(self):
         # type: () -> str
         return "SystemStatus"
 
 
@@ -2929,21 +3162,24 @@
     limits without a query statement. If all three are specified it is an error.
 
     Execution of operations specified by this request is implicitly
     asynchronous. These are potentially long-running operations.
     :py:meth:`NoSQLHandle.table_request` returns a :py:class:`TableResult`
     instance that can be used to poll until the table reaches the desired state.
 
-    The statement is required parameter.
+    The statement is required parameter unless modifying limits.
     """
 
     def __init__(self):
         super(TableRequest, self).__init__()
         self._statement = None
         self._limits = None
+        self._defined_tags = None  # a dict, with str values
+        self._match_etag = None
+        self._free_form_tags = None  # a dict, wih str values
 
     def __str__(self):
         return ('TableRequest: [name=' + str(self.get_table_name()) +
                 ', statement=' + str(self._statement) + ', limits=' +
                 str(self._limits) + ']')
 
     def set_statement(self, statement):
@@ -3025,14 +3261,102 @@
         Returns the table limits, or None if not set.
 
         :returns: the limits.
         :rtype: TableLimits
         """
         return self._limits
 
+    def set_defined_tags(self, tags):
+        """
+        Cloud service only.
+
+        Sets defined tags
+
+        :param tags the tags
+        :type tags: dict(str, dict(str, object))
+        :versionadded: 5.4.0
+        """
+        self._defined_tags = tags
+
+    def get_defined_tags(self):
+        """
+        Cloud service only.
+
+        Returns the defined tags or None if not set
+
+        :returns: the defined tags.
+        :rtype: dict(str, dict(str, object))
+        :versionadded: 5.4.0
+        """
+        return self._defined_tags
+
+    def set_free_form_tags(self, tags):
+        """
+        Cloud service only.
+
+        Sets free_form tags
+
+        :param tags the tags
+        :type tags: dict(str, str)
+        :versionadded: 5.4.0
+        """
+        self._free_form_tags = tags
+
+    def get_free_form_tags(self):
+        """
+        Returns the free_form tags or None if not set
+
+        :returns: the free_form tags.
+        :rtype: dict(str, str)
+        :versionadded: 5.4.0
+        """
+        return self._free_form_tags
+
+    def set_match_etag(self, etag):
+        """
+        Cloud service only.
+
+        Sets a ETag to match for the operation to proceed. The ETag must be
+        non-null and have been previously returned in :py:class:`TableResult`.
+        The ETag is a form of optimistic concurrency control allowing an
+        application to ensure no unexpected modifications have been made to the
+        table.
+
+        :param etag the tag
+        :type etag: str
+        :versionadded: 5.4.0
+        """
+        self._match_etag = etag
+
+    def get_match_etag(self):
+        """
+        Cloud service only.
+
+        :returns: the match etag or None if not set
+        :rtype: str
+        :versionadded: 5.4.0
+        """
+        return self._match_etag
+
+    def set_namespace(self, namespace):
+        """
+        On-premises only
+
+        Sets the namespace to use for the operation. This will override
+        any configured default value.
+
+        :param namespace: the namespace
+        :type namespace: str
+        :raises IllegalArgumentException: raises the exception if namespace is
+            not a string.
+        :versionadded: 5.4.0
+        """
+        super(TableRequest, self).set_namespace(namespace)
+        return self
+
     def set_table_name(self, table_name):
         """
         Sets the table name to use for the operation. The table name is only
         used to modify the limits of an existing table, and must not be set for
         any other operation.
 
         :param table_name: the name of the table.
@@ -3096,15 +3420,21 @@
             raise IllegalArgumentException(
                 'TableRequest cannot have both table name and statement.')
 
         if self._limits is not None:
             self._limits.validate()
 
     @staticmethod
-    def create_serializer():
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        if serial_version >= SerdeUtil.SERIAL_VERSION_4:
+            return borneo.nson.TableRequestSerializer()
         return TableRequestSerializer()
 
     def get_request_name(self):
         # type: () -> str
         return "Table"
 
 
@@ -3129,14 +3459,31 @@
     """
 
     def __init__(self):
         super(TableUsageRequest, self).__init__()
         self._start_time = 0
         self._end_time = 0
         self._limit = 0
+        self._start_index = 0
+
+    def set_namespace(self, namespace):
+        """
+        On-premises only
+
+        Sets the namespace to use for the operation. This will override
+        any configured default value.
+
+        :param namespace: the namespace
+        :type namespace: str
+        :raises IllegalArgumentException: raises the exception if namespace is
+            not a string.
+        :versionadded: 5.4.0
+        """
+        super(TableUsageRequest, self).set_namespace(namespace)
+        return self
 
     def set_table_name(self, table_name):
         """
         Sets the table name to use for the request. This is a required
         parameter.
 
         :param table_name: the table name.
@@ -3187,15 +3534,15 @@
         :type start_time: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if start_time is
             a negative number and is not an ISO 8601 formatted string.
         """
         self._check_time(start_time)
         if isinstance(start_time, str):
-            start_time = self._iso_time_to_timestamp(start_time)
+            start_time = SerdeUtil.iso_time_to_ms(start_time)
         self._start_time = start_time
         return self
 
     def get_start_time(self):
         """
         Returns the start time to use for the request in milliseconds since the
         Epoch.
@@ -3232,15 +3579,15 @@
         :type end_time: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if end_time is a
             negative number and is not an ISO 8601 formatted string.
         """
         self._check_time(end_time)
         if isinstance(end_time, str):
-            end_time = self._iso_time_to_timestamp(end_time)
+            end_time = SerdeUtil.iso_time_to_ms(end_time)
         self._end_time = end_time
         return self
 
     def get_end_time(self):
         """
         Returns the end time to use for the request in milliseconds since the
         Epoch.
@@ -3284,14 +3631,41 @@
         Returns the limit to the number of usage records desired.
 
         :returns: the numeric limit.
         :rtype: int
         """
         return self._limit
 
+    def set_start_index(self, start_index):
+        """
+        Sets the index to use to start returning usage records within the
+        specified range. This is related to the last_returned_index from a
+        previous request and can be used to page usage records. If not set
+        the list starts a 0
+        :param start_index: the numeric index.
+        :type start_index: int
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if start_index
+        is a negative number.
+        :versionadded: 5.4.0
+        """
+        CheckValue.check_int_ge_zero(start_index, 'start_index')
+        self._start_index = start_index
+        return self
+
+    def get_start_index(self):
+        """
+        Returns the start_index for usage records desired.
+
+        :returns: the numeric start_index.
+        :rtype: int
+        :versionadded: 5.4.0
+        """
+        return self._start_index
+
     def set_timeout(self, timeout_ms):
         """
         Sets the request timeout value, in milliseconds. This overrides any
         default value set in :py:class:`NoSQLHandleConfig`. The value must be
         positive.
 
         :param timeout_ms: the timeout value, in milliseconds.
@@ -3322,33 +3696,31 @@
             raise IllegalArgumentException(
                 'TableUsageRequest requires a table name.')
         if self._start_time > self._end_time > 0:
             raise IllegalArgumentException(
                 'TableUsageRequest: end time must be greater than start time.')
 
     @staticmethod
-    def create_serializer():
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        if serial_version >= SerdeUtil.SERIAL_VERSION_4:
+            return borneo.nson.TableUsageRequestSerializer()
         return TableUsageRequestSerializer()
 
     @staticmethod
     def _check_time(dt):
-        if (not (CheckValue.is_int(dt) or CheckValue.is_long(dt) or
-                 CheckValue.is_str(dt)) or
+        if (not (isinstance(dt, int) or CheckValue.is_str(dt)) or
                 not CheckValue.is_str(dt) and dt < 0):
             raise IllegalArgumentException(
                 'dt must be an integer that is not negative or an ISO ' +
                 '8601 formatted string. Got:' + str(dt))
 
-    @staticmethod
-    def _iso_time_to_timestamp(dt):
-        dt = parser.parse(dt)
-        if dt.tzinfo is not None:
-            dt = dt.astimezone(tz.UTC)
-        return int(mktime(dt.timetuple()) * 1000) + dt.microsecond // 1000
-
     def get_request_name(self):
         # type: () -> str
         return "TableUsage"
 
 
 class WriteMultipleRequest(Request):
     """
@@ -3404,24 +3776,26 @@
                 'DeleteRequest as parameter. Got: ' + str(request))
         CheckValue.check_boolean(abort_if_unsuccessful,
                                  'abort_if_unsuccessful')
         table_name = self.get_table_name()
         if table_name is None:
             self.set_table_name(request.get_table_name())
         else:
-            if self.get_top_table_name(request.get_table_name().lower()) \
+            if WriteMultipleRequest.get_top_table_name(
+                    request.get_table_name().lower()) \
                     != table_name.lower():
                 raise IllegalArgumentException(
                     'The parent table_name used for the operation is '
                     'different from that of others: ' + table_name)
         request.validate()
         self._ops.append(self.OperationRequest(request, abort_if_unsuccessful))
         return self
 
-    def get_top_table_name(self, table_name: str):
+    @staticmethod
+    def get_top_table_name(table_name):
         pos = table_name.find('.')
         if pos == -1:
             return table_name
         return table_name[0:pos]
 
     def is_single_table(self):
         if len(self._ops) < 2:
@@ -3561,15 +3935,21 @@
         return True
 
     def validate(self):
         if not self._ops:
             raise IllegalArgumentException('The requests list is empty.')
 
     @staticmethod
-    def create_serializer():
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        if serial_version >= SerdeUtil.SERIAL_VERSION_4:
+            return borneo.nson.WriteMultipleRequestSerializer()
         return WriteMultipleRequestSerializer()
 
     class OperationRequest(object):
 
         # A wrapper of WriteRequest that contains an additional flag
         # abort_if_unsuccessful. Internal for now
         def __init__(self, request, abort_if_unsuccessful):
@@ -4018,14 +4398,15 @@
         """
         Returns the index of the last table name returned. This can be provided
         to :py:class:`ListTablesRequest` to be used as a starting point for
         listing tables.
 
         :returns: the index.
         :rtype: int
+        :versionadded: 5.4.0
         """
         return self._last_index_returned
 
 
 class MultiDeleteResult(Result):
     """
     Represents the result of a :py:meth:`NoSQLHandle.multi_delete` operation.
@@ -4555,15 +4936,14 @@
     with no RETURNING clause return a dictionary indicating the number of rows
     deleted, for example {'numRowsDeleted': 2}.
 
     :versionadded: 5.3.6
     """
 
     def __init__(self, request, handle):
-        # type: (QueryRequest, NoSQLHandle) -> None
         # NoSQLHandle handle
         super(QueryIterableResult, self).__init__()
         self.request = request
         self.handle = handle
         self.readKB = 0
         self.readUnits = 0
         self.writeKB = 0
@@ -4607,111 +4987,102 @@
 
         :returns: the write KBytes consumed.
         :rtype: int
         """
         return self.writeKB
 
     def __iter__(self):
-        # type: () -> QueryIterator
         return QueryIterator(self)
 
 
 class QueryIterator:
     """
     QueryIterator iterates over all results of a query.
 
     :versionadded: 5.3.6
     """
+
     def __init__(self, iterable):
-        # type: (QueryIterableResult) -> None
         self._iterable = iterable
         self._internalRequest = iterable.request.copy()
-        self._internalResult = None
+        self._internal_result = None
         self._partialResultList = None
         self._partialResultIter = None
         self._next = None
         self._closed = False
 
     def _compute(self):
-        # type: () -> None
         if self._closed:
             return
         if self._partialResultList is None:
-            self._internalResult = \
+            self._internal_result = \
                 self._iterable.handle.query(self._internalRequest)
-            self._partialResultList = self._internalResult.get_results()
+            self._partialResultList = self._internal_result.get_results()
             self._partialResultIter = self._partialResultList.__iter__()
             try:
                 self._next = next(self._partialResultIter)
                 return
             except StopIteration:
-                hasNext = False
-            self.set_stats(self._internalResult)
+                has_next = False
+            self.set_stats(self._internal_result)
         else:
             try:
                 self._next = next(self._partialResultIter)
                 return
             except StopIteration:
-                hasNext = False
+                has_next = False
 
-        while not hasNext and not self._internalRequest.is_done():
-            self._internalResult = \
+        while not has_next and not self._internalRequest.is_done():
+            self._internal_result = \
                 self._iterable.handle.query(self._internalRequest)
-            self._partialResultList = self._internalResult.get_results()
+            self._partialResultList = self._internal_result.get_results()
             self._partialResultIter = self._partialResultList.__iter__()
-            hasNext = True
+            has_next = True
             try:
                 self._next = next(self._partialResultIter)
             except StopIteration:
-                hasNext = False
-            self.set_stats(self._internalResult)
+                has_next = False
+            self.set_stats(self._internal_result)
 
         if self._internalRequest.is_done():
             self._internalRequest.close()
-            if not hasNext:
+            if not has_next:
                 self._closed = True
 
-    def set_stats(self, internalResult):
-        # type: (QueryResult) -> None
-        self._iterable.readKB += internalResult.get_read_kb()
-        self._iterable.readUnits += internalResult.get_read_units()
-        self._iterable.writeKB += internalResult.get_write_kb()
+    def set_stats(self, internal_result):
+        self._iterable.readKB += internal_result.get_read_kb()
+        self._iterable.readUnits += internal_result.get_read_units()
+        self._iterable.writeKB += internal_result.get_write_kb()
         self._iterable.set_rate_limit_delayed_ms(
             self._iterable.get_rate_limit_delayed_ms() +
-            internalResult.get_rate_limit_delayed_ms())
+            internal_result.get_rate_limit_delayed_ms())
         self._iterable.set_read_kb(self._iterable.get_read_kb() +
-                                   internalResult.get_read_kb())
+                                   internal_result.get_read_kb())
         self._iterable.set_read_units(self._iterable.get_read_units() +
-                                      internalResult.get_read_units())
+                                      internal_result.get_read_units())
         self._iterable.set_write_kb(self._iterable.get_write_kb() +
-                                    internalResult.get_write_kb())
+                                    internal_result.get_write_kb())
         self._iterable.set_write_units(self._iterable.get_write_units() +
-                                       internalResult.get_write_units())
-        if internalResult.get_retry_stats() is not None:
+                                       internal_result.get_write_units())
+        if internal_result.get_retry_stats() is not None:
             if self._iterable.get_retry_stats() is None:
                 self._iterable.set_retry_stats(RetryStats())
             self._iterable.get_retry_stats().add_delay_ms(
-                internalResult.get_retry_stats().get_delay_ms())
+                internal_result.get_retry_stats().get_delay_ms())
             self._iterable.get_retry_stats().increment_retries(
-                internalResult.get_retry_stats().get_retries())
+                internal_result.get_retry_stats().get_retries())
             self._iterable.get_retry_stats().add_exceptions(
-                internalResult.get_retry_stats().get_exceptions_map())
+                internal_result.get_retry_stats().get_exceptions_map())
 
     def __next__(self):
-        # type: () -> dict[str, Object]
         self._compute()
         if self._closed:
             raise StopIteration
         return self._next
 
-    # for python2 compatibility
-    def next(self):
-        # type: () -> dict[str, Object]
-        return self.__next__()
-
 
 class SystemResult(Result):
     """
     On-premise only.
 
     SystemResult is returned from :py:meth:`NoSQLHandle.system_status` and
     :py:meth:`NoSQLHandle.system_request` operations. It encapsulates the state
@@ -4742,15 +5113,15 @@
         self._operation_id = None
         self._result_string = None
         self._state = 0
         self._statement = None
 
     def __str__(self):
         return ('SystemResult [statement=' + self._statement + ', state=' +
-                BinaryProtocol.get_operation_state(self._state) +
+                SerdeUtil.get_operation_state(self._state) +
                 ', operation_id=' + self._operation_id + ', result_string=' +
                 self._result_string + ']')
 
     def set_operation_id(self, operation_id):
         # Sets the operation id for the operation.
         self._operation_id = operation_id
         return self
@@ -4811,14 +5182,17 @@
         Returns the statement used for the operation.
 
         :returns: the statement.
         :rtype: str
         """
         return self._statement
 
+    def get_state(self):
+        return self._state
+
     def wait_for_completion(self, handle, wait_millis, delay_millis):
         """
         Waits for the operation to be complete. This is a blocking, polling
         style wait that delays for the specified number of milliseconds between
         each polling operation.
 
         This instance is modified with any changes in state.
@@ -4883,41 +5257,73 @@
 
     :py:meth:`NoSQLHandle.get_table` is synchronous, returning static
     information about the table as well as its current state.
     """
 
     def __init__(self):
         super(TableResult, self).__init__()
-        self._compartment_id = None
+        self._compartment_or_namespace = None
         self._table_name = None
         self._state = None
         self._limits = None
         self._schema = None
         self._operation_id = None
+        self._ocid = None
+        self._ddl = None
+        self._defined_tags = None  # dict(str, dict(str, object))
+        self._match_etag = None  # str
+        self._free_form_tags = None  # dict(str, str)
 
     def __str__(self):
-        return ('table ' + str(self._table_name) + '[' + self._state + '] ' +
-                str(self._limits) + ' schema [' + str(self._schema) +
-                '] operation_id = ' + str(self._operation_id))
+        tres = ('table name=' + str(self._table_name) + ', state=' +
+                self._state)
+        if self._limits is not None:
+            tres += ', limits=' + str(self._limits)
+
+        # only print one of DDL or schema, preferring DDL
+        if self._ddl is not None:
+            tres += ', ddl=' + str(self._ddl)
+        elif self._schema is not None:
+            tres += ', schema=[' + str(self._schema) + ']'
+
+        if self._ocid is not None:
+            tres += ', ocid=' + str(self._ocid)
+        return tres
 
     def set_compartment_id(self, compartment_id):
         # Internal use only.
-        self._compartment_id = compartment_id
+        self._compartment_or_namespace = compartment_id
+        return self
+
+    def set_namespace(self, namespace):
+        # Internal use only.
+        self._compartment_or_namespace = namespace
         return self
 
     def get_compartment_id(self):
         """
         Cloud service only.
 
         Returns compartment id of the target table.
 
         :returns: compartment id.
         :rtype: str
         """
-        return self._compartment_id
+        return self._compartment_or_namespace
+
+    def get_namespace(self):
+        """
+        On-premise service only.
+
+        Returns the namespace of the table or null if it is not in a namespace.
+
+        :returns: namespace
+        :rtype: str
+        """
+        return self._compartment_or_namespace
 
     def set_table_name(self, table_name):
         self._table_name = table_name
         return self
 
     def get_table_name(self):
         """
@@ -4981,14 +5387,86 @@
         operation.
 
         :returns: the operation id for an asynchronous operation.
         :rtype: str
         """
         return self._operation_id
 
+    def get_ddl(self):
+        """
+        Returns the DDL (create table) statement used to create this table if
+        available. If the table has been altered since initial creation the
+        statement is also altered to reflect the current table schema. This
+        value, when non-null, is functionally equivalent to the schema
+        returned by :py:meth:`set_schema`.
+        table.
+
+        :returns: the ddl statement used to create the table
+        :rtype: str
+        :versionadded: 5.4.0
+        """
+        return self._ddl
+
+    def get_table_id(self):
+        """
+        Cloud service only.
+        Returns the OCID of the table. This value will be null if used with the
+        on-premise service.
+
+        :returns: the table OCID
+        :rtype: str
+        :versionadded: 5.4.0
+        """
+        return self._ocid
+
+    def get_match_etag(self):
+        """
+        Cloud service only.
+
+        :returns: the tag
+        :rtype: str
+        :versionadded: 5.4.0
+        """
+        return self._match_etag
+
+    def get_defined_tags(self):
+        """
+        Cloud service only.
+
+        :returns: the tags
+        :rtype: dict(str, dict(str, object))
+        :versionadded: 5.4.0
+        """
+        return self._defined_tags
+
+    def get_free_form_tags(self):
+        """
+        Cloud service only.
+
+        :returns: the tags
+        :rtype: dict(str, str)
+        :versionadded: 5.4.0
+        """
+        return self._free_form_tags
+
+    def set_ddl(self, value):
+        self._ddl = value
+
+    def set_table_id(self, value):
+        self._ocid = value
+
+    def set_match_etag(self, value):
+        self._match_etag = value
+
+    def set_defined_tags(self, value):
+        self._defined_tags = value
+
+    def set_free_form_tags(self, value):
+        self._free_form_tags = value
+
     def wait_for_completion(self, handle, wait_millis, delay_millis):
         """
         Waits for a table operation to complete. Table operations are
         asynchronous. This is a blocking, polling style wait that delays for the
         specified number of milliseconds between each polling operation. This
         call returns when the table reaches a *terminal* state, which is either
         State.ACTIVE or State.DROPPED.
@@ -5024,15 +5502,15 @@
             raise IllegalArgumentException(
                 'Wait milliseconds must be a minimum of ' + str(default_delay) +
                 ' and greater than delay milliseconds')
         start_time = int(round(time() * 1000))
         delay_s = float(delay_ms) / 1000
         get_table = GetTableRequest().set_table_name(
             self._table_name).set_operation_id(
-            self._operation_id).set_compartment(self._compartment_id)
+            self._operation_id).set_compartment(self._compartment_or_namespace)
         res = None
         while True:
             cur_time = int(round(time() * 1000))
             if cur_time - start_time > wait_millis:
                 raise RequestTimeoutException(
                     'Operation not completed in expected time', wait_millis)
             if res is not None:
@@ -5054,14 +5532,15 @@
 
     TableUsageResult is returned from :py:meth:`NoSQLHandle.get_table_usage`.
     It encapsulates the dynamic state of the requested table.
     """
 
     def __init__(self):
         super(TableUsageResult, self).__init__()
+        self._last_index_returned = 0
         self._table_name = None
         self._usage_records = None
 
     def __str__(self):
         if self._usage_records is None:
             records_str = 'None'
         else:
@@ -5096,14 +5575,27 @@
         :py:class:`TableUsageRequest` used.
 
         :returns: an list of usage records.
         :type: list(TableUsage)
         """
         return self._usage_records
 
+    def set_last_index_returned(self, last_index_returned):
+        self._last_index_returned = last_index_returned
+        return self
+
+    def get_last_index_returned(self):
+        """
+        Returns the index of the last usage record returned
+
+        :returns: the index.
+        :rtype: int
+        """
+        return self._last_index_returned
+
 
 class WriteMultipleResult(Result):
     """
     Represents the result of a :py:meth:`NoSQLHandle.write_multiple` operation.
 
     If the WriteMultiple succeeds, the execution result of each sub operation
     can be retrieved using :py:meth:`get_results`.
@@ -5369,26 +5861,24 @@
         :param e: the exception class.
         :type e: Exception
         """
         num = self.get_num_exceptions(e) + 1
         self._exception_map[e] = num
 
     def get_exceptions_map(self):
-        # type: () -> dict[Object, int]
         """
         Internal use only.
 
         Returns the map of exceptions.
 
         :versionadded: 5.3.6
         """
         return self._exception_map
 
     def add_exceptions(self, ex_map):
-        # type: (dict[Object, int]) -> None
         """
         Internal use only.
 
         Adds all exceptions to the stats object.
 
         This increments the exception count and adds to the count of this type
         of exception class.
```

### Comparing `borneo-5.3.7/src/borneo/iam/iam.py` & `borneo-5.4.1/src/borneo/iam/iam.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 #
-# Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
-OCI_PYTHON_SDK_NO_SERVICE_IMPORTS=True
+OCI_PYTHON_SDK_NO_SERVICE_IMPORTS = True
 
 from os import path
-from requests import Request
 from threading import Lock, Timer
 from time import sleep, time
+
+from requests import Request
+
 try:
+    # noinspection PyUnresolvedReferences
     from oci.signer import Signer
+    # noinspection PyUnresolvedReferences
     from oci.auth.signers import SecurityTokenSigner
+    # noinspection PyUnresolvedReferences
     from oci.auth.signers import EphemeralResourcePrincipalSigner
+    # noinspection PyUnresolvedReferences
     from oci.auth.signers import InstancePrincipalsSecurityTokenSigner
+    # noinspection PyUnresolvedReferences
     from oci.auth.signers import get_resource_principals_signer
+    # noinspection PyUnresolvedReferences
     from oci.config import from_file
+
     oci = 'yes'
 except ImportError:
     oci = None
 
 from borneo.auth import AuthorizationProvider
 from borneo.common import (
     CheckValue, HttpConstants, LogUtils, Memoize, synchronized)
@@ -140,16 +149,16 @@
             raise IllegalArgumentException(
                 'Access token cannot be cached longer than ' +
                 str(SignatureProvider.MAX_ENTRY_LIFE_TIME) + ' seconds.')
 
         self._region = None
         if provider is not None:
             if not isinstance(
-                provider,
-                (Signer, SecurityTokenSigner)):
+                    provider,
+                    (Signer, SecurityTokenSigner)):
                 raise IllegalArgumentException(
                     'provider should be an instance of oci.signer.Signer or ' +
                     'oci.auth.signers.SecurityTokenSigner.')
             self._provider = provider
             if region is not None:
                 region_id = region
             else:
@@ -401,26 +410,26 @@
         :returns: tenant OCID of user.
         :rtype: str
         """
         if isinstance(self._provider, Signer):
             return self._provider.api_key.split('/')[0]
 
     def _refresh_task(self):
-        timeout =  self._refresh_ahead
+        timeout = self._refresh_ahead
         start_ms = int(round(time() * 1000))
         error_logged = False
         while True:
             try:
                 # refresh security token before create new signature
                 if (isinstance(
-                    self._provider,
-                    InstancePrincipalsSecurityTokenSigner) or
-                    isinstance(
-                    self._provider,
-                    EphemeralResourcePrincipalSigner)):
+                        self._provider,
+                        InstancePrincipalsSecurityTokenSigner) or
+                        isinstance(
+                            self._provider,
+                            EphemeralResourcePrincipalSigner)):
                     self._provider.refresh_security_token()
 
                 self.get_signature_details_internal()
                 return
             except Exception as e:
                 # Ignore the refresh failure, then sleep and try again until
                 # the timeout. Log the failure the first time only. If the
@@ -430,15 +439,15 @@
                 # the user as an exception
                 if not error_logged:
                     self._logutils.log_error(
                         'Unable to refresh cached request signature, ' + str(e))
                     error_logged = True
 
             # check for timeout in the loop
-            if (int(round(time() * 1000)) - start_ms >= timeout):
+            if int(round(time() * 1000)) - start_ms >= timeout:
                 self._logutils.log_error(
                     'Request signature refresh timed out after ' + str(timeout))
                 break
             sleep(0.1)
 
         # if we get here the refresh failed and timed out. Cancel the timer.
         # It will get re-created when the next in-line call to get signature
```

### Comparing `borneo-5.3.7/src/borneo/common.py` & `borneo-5.4.1/src/borneo/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #
-# Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from datetime import datetime
 from decimal import Decimal
 from functools import wraps
 from logging import Logger
 from struct import pack, unpack
-from sys import version_info
 from threading import Lock
 from time import time
 from warnings import simplefilter, warn
 
 from dateutil import tz
 from requests import adapters
 
@@ -51,14 +50,17 @@
     a bytearray.
     """
 
     def __init__(self, content):
         self._content = content
         self._offset = 0
 
+    def get_content(self):
+        return self._content
+
     def get_offset(self):
         return self._offset
 
     def read_boolean(self):
         res = bool(self.read_byte())
         return res
 
@@ -100,36 +102,47 @@
         self.read_fully(buf)
         res, = unpack('>h', buf)
         return res
 
     def set_offset(self, offset):
         self._offset = offset
 
+    def skip(self, length):
+        self._offset += length
+
 
 class ByteOutputStream(object):
     """
     The ByteOutputStream provides methods to write data with different type into
     a bytearray.
     """
 
     def __init__(self, content):
         self._content = content
 
+    def get_content(self):
+        return self._content
+
     def get_offset(self):
         return len(self._content)
 
     def write_boolean(self, value):
         val_s = pack('?', value)
         self.write_value(val_s)
 
     def write_byte(self, value):
         val_s = pack('B', value)
         self.write_value(val_s)
 
     def write_bytearray(self, value, start=0, end=None):
+        # optimize (?) full concatenate
+        if start == 0 and end is None:
+            self._content.extend(value)
+            return
+
         if end is None:
             end = len(value)
         for index in range(start, end):
             self._content.append(value[index])
 
     def write_float(self, value):
         val_s = pack('>d', value)
@@ -147,15 +160,21 @@
 
     def write_short_int(self, value):
         val_s = pack('>h', value)
         self.write_value(val_s)
 
     def write_value(self, value):
         val_b = bytearray(value)
-        self.write_bytearray(val_b)
+        self._content.extend(val_b)
+
+    def get_byte_at(self, index):
+        return self._content[index]
+
+    def get_last_byte(self):
+        return self._content[-1]
 
 
 class CheckValue(object):
 
     @staticmethod
     def check_boolean(data, name):
         if data is not True and data is not False:
@@ -170,30 +189,28 @@
     def check_float_gt_zero(data, name):
         if not CheckValue.is_digit(data) or data <= 0.0:
             raise IllegalArgumentException(
                 name + ' must be a positive digital number. Got:' + str(data))
 
     @staticmethod
     def check_int(data, name):
-        if not (CheckValue.is_int(data) or CheckValue.is_long(data)):
+        if not isinstance(data, int):
             raise IllegalArgumentException(
                 name + ' must be an integer. Got:' + str(data))
 
     @staticmethod
     def check_int_ge_zero(data, name):
-        if (not (CheckValue.is_int(data) or CheckValue.is_long(data)) or
-                data < 0):
+        if not isinstance(data, int) or data < 0:
             raise IllegalArgumentException(
                 name + ' must be an integer that is not negative. Got:' +
                 str(data))
 
     @staticmethod
     def check_int_gt_zero(data, name):
-        if (not (CheckValue.is_int(data) or CheckValue.is_long(data)) or
-                data <= 0):
+        if not isinstance(data, int) or data <= 0:
             raise IllegalArgumentException(
                 name + ' must be an positive integer. Got:' + str(data))
 
     @staticmethod
     def check_list(data, name):
         if not isinstance(data, list):
             raise IllegalArgumentException(name + ' must be a list.')
@@ -213,50 +230,50 @@
         if (not allow_none and data is None or data is not None and
                 (not CheckValue.is_str(data) or len(data) == 0)):
             raise IllegalArgumentException(
                 name + ' must be a string that is not empty.')
 
     @staticmethod
     def is_digit(data):
-        if (CheckValue.is_int(data) or CheckValue.is_long(data) or
+        if (isinstance(data, int) or
                 isinstance(data, float) or isinstance(data, Decimal)):
             return True
         return False
 
+    # returns True if the data is of type int and its value is in the
+    # range of a 32-bit integer
     @staticmethod
-    def is_int(data):
-        if ((version_info.major == 2 and isinstance(data, int) or
-             version_info.major == 3 and isinstance(data, int)) and
+    def is_int_value(data):
+        if (isinstance(data, int) and
                 -pow(2, 31) <= data < pow(2, 31)):
             return True
         return False
 
+    # returns True if the data is of type int and its value is larger than
+    # that of a 32-bit integer and in the range of a 64-bit integer
+    #
+    # NOTE: It is sufficient to just validate that it's an int and
+    # is out of range for a 32-bit integer value
     @staticmethod
-    def is_long(data):
-        if ((version_info.major == 2 and isinstance(data, (int, long)) or
-             version_info.major == 3 and isinstance(data, int)) and
-                not CheckValue.is_int(data) and
-                -pow(2, 63) <= data < pow(2, 63)):
+    def is_long_value(data):
+        if (isinstance(data, int) and
+                not CheckValue.is_int_value(data)):
             return True
         return False
 
     @staticmethod
     def is_overlong(data):
-        if ((version_info.major == 2 and isinstance(data, long) or
-             version_info.major == 3 and isinstance(data, int)) and
+        if (isinstance(data, int) and
                 (data < -pow(2, 63) or data >= pow(2, 63))):
             return True
         return False
 
     @staticmethod
     def is_str(data):
-        if (version_info.major == 2 and isinstance(data, (str, unicode)) or
-                version_info.major == 3 and isinstance(data, str)):
-            return True
-        return False
+        return isinstance(data, str)
 
 
 class Consistency(object):
     """
     Set the consistency for read requests.
     """
     ABSOLUTE = 0
@@ -459,14 +476,20 @@
     # http level rather than the frame level, and consequently does not have
     # access to the stream id.
     REQUEST_ID_HEADER = 'x-nosql-request-id'
 
     # The name of the (request-target) header.
     REQUEST_TARGET = '(request-target)'
 
+    # Default namespace header
+    REQUEST_NAMESPACE_HEADER = 'x-nosql-default-ns'
+
+    # Proxy version info
+    RESPONSE_PROXY_INFO = 'x-nosql-version'
+
     # Creates a URI path from the arguments
     def _make_path(*args):
         path = args[0]
         for index in range(1, len(args)):
             path += '/' + args[index]
         return path
 
@@ -476,22 +499,23 @@
 
     # The path denoting a NoSQL request
     NOSQL_DATA_PATH = _make_path(NOSQL_VERSION, 'nosql/data')
 
 
 class IndexInfo(object):
     """
-    IndexInfo represents the information about a single index including its name
-    and field names. Instances of this class are returned in
+    IndexInfo represents the information about a single index including its
+    name, field names and field types. Instances of this class are returned in
     :py:class:`GetIndexesResult`.
     """
 
-    def __init__(self, index_name, field_names):
+    def __init__(self, index_name, field_names, field_types=None):
         self._index_name = index_name
         self._field_names = field_names
+        self._field_types = field_types
 
     def __str__(self):
         return ('IndexInfo [indexName=' + self._index_name + ', fields=[' +
                 ','.join(self._field_names) + ']]')
 
     def get_index_name(self):
         """
@@ -507,14 +531,24 @@
         Returns the list of field names that define the index.
 
         :returns: the field names.
         :rtype: list(str)
         """
         return self._field_names
 
+    def get_field_types(self):
+        """
+        Returns the list of types of fields that define the index.
+
+        :returns: the field types.
+        :rtype: list(str)
+        :versionadded: 5.4.0
+        """
+        return self._field_types
+
 
 class JsonNone(object):
     """
     Represents an JSON NONE field value.
     """
 
     def __str__(self):
@@ -713,15 +747,15 @@
         and returns the next offset to be written.
 
         :param buf: the buffer to write to.
         :type buf: bytearray
         :param offset: the offset in the buffer at which to start writing.
         :type offset: int
         :param value: the long integer to be written.
-        :type value: int for python 3 and long for python 2
+        :type value: int
         :returns: the offset past the bytes written.
         :rtype: int
 
         Values in the inclusive range [-119,120] are stored in a single byte.
         For values outside that range, the first byte stores the number of
         additional bytes. The additional bytes store (value + 119 for negative
         and value - 121 for positive) as an unsigned big endian integer.
@@ -958,31 +992,28 @@
         returns it.
 
         :param buf: the buffer to read from.
         :type buf: bytearray
         :param offset: the offset in the buffer at which to start reading.
         :type offset: int
         :returns: the long integer that was read.
-        :rtype: int for python 3 and long for python 2
+        :rtype: int
         """
         # The first byte of the buf stores the length of the value part.
         b1 = buf[offset] & 0xff
         offset += 1
         # Adjust the byte_len to the real length of the value part.
         if b1 < 0x08:
             byte_len = 0x08 - b1
             negative = True
         elif b1 > 0xf7:
             byte_len = b1 - 0xf7
             negative = False
         else:
-            try:
-                return long(b1 - 127)
-            except NameError:
-                return b1 - 127
+            return b1 - 127
 
         """
         The following bytes on the buf store the value as a big endian integer.
         We extract the significant bytes from the buf and put them into the
         value in big endian order.
         """
         if negative:
@@ -1016,18 +1047,15 @@
         After obtaining the adjusted value, we have to adjust it back to the
         original value.
         """
         if negative:
             value -= 119
         else:
             value += 121
-        try:
-            return long(value)
-        except NameError:
-            return value
+        return value
 
 
 class PreparedStatement(object):
     """
     A class encapsulating a prepared query statement. It includes state that can
     be sent to a server and executed without re-parsing the query. It includes
     bind variables which may be set for each successive use of the query. The
@@ -1040,29 +1068,30 @@
     A single instance of PreparedStatement is thread-safe if bind variables are
     not used. If bind variables are to be used and the statement shared among
     threads additional instances of PreparedStatement can be constructed using
     :py:meth:`copy_statement`.
     """
     OPCODE_SELECT = 5
 
-    def __init__(self, sql_text, query_plan, topology_info, proxy_statement,
-                 driver_plan, num_iterators, num_registers, external_vars,
-                 namespace, table_name, operation):
+    def __init__(self, sql_text, query_plan, query_schema, topology_info,
+                 proxy_statement, driver_plan, num_iterators, num_registers,
+                 external_vars, namespace, table_name, operation):
         """
         Constructs a PreparedStatement. Construction is hidden to eliminate
         application access to the underlying statement, reducing the chance of
         corruption.
         """
         # 10 is arbitrary. TODO: put magic number in it for validation?
         if proxy_statement is None or len(proxy_statement) < 10:
             raise IllegalArgumentException(
                 'Invalid prepared query, cannot be None.')
 
         self._sql_text = sql_text
         self._query_plan = query_plan
+        self._query_schema = query_schema
         # Applicable to advanced queries only.
         self._topology_info = topology_info
         # The serialized PreparedStatement created at the backend store. It is
         # opaque for the driver. It is received from the proxy and sent back to
         # the proxy every time a new batch of results is needed.
         self._proxy_statement = proxy_statement
         # The part of the query plan that must be executed at the driver. It is
@@ -1104,15 +1133,15 @@
         is immutable, but does not share its variables.
 
         :returns: a new PreparedStatement using this instance's prepared query.
             Bind variables are uninitialized.
         :rtype: PreparedStatement
         """
         return PreparedStatement(
-            self._sql_text, self._query_plan, self._topology_info,
+            self._sql_text, self._query_plan, self._query_schema, self._topology_info,
             self._proxy_statement, self._driver_query_plan, self._num_iterators,
             self._num_registers, self._variables, self._namespace,
             self._table_name, self._operation)
 
     def does_writes(self):
         # if it's not SELECT, it does writes.
         return self._operation != PreparedStatement.OPCODE_SELECT
@@ -1130,14 +1159,25 @@
         requested in the :py:class:`PrepareRequest`; None otherwise.
 
         :returns: the string representation of the query execution plan.
         :rtype: bool
         """
         return self._query_plan
 
+    def get_query_schema(self):
+        """
+        Returns a string representation of the query schema if it was
+        requested in the :py:class:`PrepareRequest`; None otherwise.
+
+        :returns: the string representation of the query schema.
+        :rtype: bool
+        :versionadded: 5.4.0
+        """
+        return self._query_schema
+
     def get_sql_text(self):
         """
         Returns the SQL text of this PreparedStatement.
 
         :returns: the SQL text of this PreparedStatement.
         :rtype: str
         """
@@ -1205,16 +1245,17 @@
         :type variable: str or int
         :param value: the value.
         :type value: a value matching the type of the field
         :returns: self.
         :raises IllegalArgumentException: raises the exception if variable is
             not a string or positive integer.
         """
-        if (not (CheckValue.is_str(variable) or CheckValue.is_int(variable)) or
-                CheckValue.is_int(variable) and variable <= 0):
+        if (not (CheckValue.is_str(variable) or
+                 CheckValue.is_int_value(variable)) or
+                CheckValue.is_int_value(variable) and variable <= 0):
             raise IllegalArgumentException(
                 'variable must be a string or positive integer.')
         if isinstance(variable, str):
             if self._bound_variables is None:
                 self._bound_variables = dict()
             if (self._variables is not None and
                     self._variables.get(variable) is None):
@@ -1657,34 +1698,38 @@
     information about read and write throughput consumed during that period as
     well as the current information regarding storage capacity. In addition the
     count of throttling exceptions for the period is reported.
     """
 
     def __init__(self, start_time_ms, seconds_in_period, read_units,
                  write_units, storage_gb, read_throttle_count,
-                 write_throttle_count, storage_throttle_count):
+                 write_throttle_count, storage_throttle_count,
+                 max_shard_usage_percent):
         # Internal use only.
         self._start_time_ms = start_time_ms
         self._seconds_in_period = seconds_in_period
         self._read_units = read_units
         self._write_units = write_units
         self._storage_gb = storage_gb
         self._read_throttle_count = read_throttle_count
         self._write_throttle_count = write_throttle_count
         self._storage_throttle_count = storage_throttle_count
+        self._max_shard_usage_percent = max_shard_usage_percent
 
     def __str__(self):
         return ('TableUsage [start_time_ms=' + str(self._start_time_ms) +
                 ', seconds_in_period=' + str(self._seconds_in_period) +
                 ', read_units=' + str(self._read_units) + ', write_units=' +
                 str(self._write_units) + ', storage_gb=' +
                 str(self._storage_gb) + ', read_throttle_count=' +
                 str(self._read_throttle_count) + ', write_throttle_count=' +
                 str(self._write_throttle_count) + ', storage_throttle_count=' +
-                str(self._storage_throttle_count) + ']')
+                str(self._storage_throttle_count) +
+                ', max_shard_usage_percent=' +
+                str(self._max_shard_usage_percent) + ']')
 
     def get_start_time(self):
         """
         Returns the start time for this usage record in milliseconds since
         the Epoch.
 
         :returns: the start time.
@@ -1769,14 +1814,25 @@
         the time period.
 
         :returns: the number of throttling exceptions.
         :rtype: int
         """
         return self._storage_throttle_count
 
+    def get_max_shard_usage_percent(self):
+        """
+        Returns the percentage of allowed storage usage for the shard with the
+        highest usage percentage across all table shards. This can be used as a
+        gauge of toal storage available as well as a hint for key distribution.
+        :returns: the percentage
+        :rtype: int
+        :versionadded: 5.4.0
+        """
+        return self._max_shard_usage_percent
+
 
 class TimeUnit(object):
     """
     The time unit to use.
     """
     HOURS = 1
     """Set TimeUnit.HOURS to use hour as time unit"""
```

### Comparing `borneo-5.3.7/src/borneo/http.py` & `borneo-5.4.1/src/borneo/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 #
-# Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from abc import ABCMeta, abstractmethod
 from io import UnsupportedOperation
 from logging import DEBUG
 from threading import Lock
 from time import sleep, time
 
 from requests import ConnectionError, Timeout, codes
 
-from .common import ByteInputStream, CheckValue, synchronized
+from .common import ByteInputStream, CheckValue, HttpConstants, synchronized
 from .exception import (
     IllegalStateException, NoSQLException,
     ReadThrottlingException, RequestTimeoutException, RetryableException,
     SecurityInfoNotReadyException, UnsupportedProtocolException,
     WriteThrottlingException)
+from .serdeutil import SerdeUtil
 
 try:
     from . import config
     from . import kv
     from . import operations
-    from . import serde
 except ImportError:
     import config
     import kv
     import operations
-    import serde
 
 
 class HttpResponse(object):
 
     # Class to package HTTP response output and status code.
     def __init__(self, content, status_code):
         self._content = content
@@ -139,14 +138,15 @@
         :type uri: str
         :param headers: HTTP headers of this request.
         :type headers: dict
         :param payload: payload in string.
         :type payload: bytearray
         :param timeout_ms: request timeout in milliseconds.
         :type timeout_ms: int
+        :param stats_config: configuration for stats usage
         :returns: HTTP response, a object encapsulate status code and response.
         :rtype: HttpResponse or Result
         """
         return self._do_request('POST', uri, headers, payload, timeout_ms,
                                 stats_config)
 
     def do_put_request(self, uri, headers, payload, timeout_ms):
@@ -286,14 +286,16 @@
                     network_time = int(round(
                         (time() - network_time) * 1000000)) / 1000
                 if self._logutils.is_enabled_for(DEBUG):
                     self._logutils.log_debug(
                         'Response: ' + self._request.__class__.__name__ +
                         ', status: ' + str(response.status_code))
                 if self._request is not None:
+                    self._client.set_proxy_info(
+                        response.headers.get(HttpConstants.RESPONSE_PROXY_INFO))
                     res = self._process_response(
                         self._request, response.content, response.status_code)
                     if (isinstance(res, operations.TableResult) and
                             self._rate_limiter_map is not None):
                         # Update rate limiter settings for table.
                         tl = res.get_table_limits()
                         self._client.update_rate_limiters(
@@ -404,15 +406,16 @@
                 continue
             except UnsupportedProtocolException as upe:
                 if self._client.decrement_serial_version():
                     if self._request is not None:
                         payload = self._client.serialize_request(self._request,
                                                                  headers)
                     self._request.increment_retries()
-                    exception = upe
+                    # don't set exception for this case -- it is misleading
+                    # exception = upe
                     continue
                 self._logutils.log_error(
                     'Client execution UnsupportedProtocolException: ' + str(upe))
                 raise upe
             except NoSQLException as nse:
                 self._logutils.log_error(
                     'Client execution NoSQLException: ' + str(nse))
@@ -524,15 +527,15 @@
     def _process_response(self, request, content, status):
         """
         Convert the url_response into a suitable return value.
 
         :param request: the request executed by the server.
         :type request: Request
         :param content: the content of the response from the server.
-        :type content: bytes for python 3 and str for python 2
+        :type content: bytes
         :param status: the status code of the response from the server.
         :type status: int
         :returns: the programmatic response object.
         :rtype: Result
         """
         if status == codes.ok:
             bis = ByteInputStream(bytearray(content))
@@ -549,69 +552,81 @@
             get from the server.
         :type bis: ByteInputStream
         :param request: the request executed by the server.
         :type request: Request
         :returns: the result of processing the successful request.
         :rtype: Result
         """
-        code = bis.read_byte()
+        #
+        # this call gives the Request an opinion on which serial version
+        # to use
+        #
+        version = request.get_serial_version(self._client.serial_version)
+        if version <= 3:
+            # V3 and earlier protocols start with an error byte (0 is no error)
+            code = bis.read_byte()
+        else:
+            # V4 starts with an NSON MAP. If the type is correct then treat it
+            # as a V4 response. If it's not correct then it's a V3
+            # error code from a V3 proxy. If it's a V4 map, code will be 0
+            code = SerdeUtil.check_for_map(bis)
         if code == 0:
-            res = request.create_serializer().deserialize(
-                request, bis, self._client.serial_version)
+            res = request.create_serializer(version).deserialize(
+                request, bis, version)
             if request.is_query_request():
                 if not request.is_simple_query():
                     request.get_driver().set_client(self._client)
             return res
 
         """
         Operation failed. Handle the failure and throw an appropriate
         exception.
         """
-        err = serde.BinaryProtocol.read_string(bis)
+        err = SerdeUtil.read_string(bis)
 
         # special case for TNF errors on WriteMultiple with many tables
-        if code == serde.BinaryProtocol.USER_ERROR.TABLE_NOT_FOUND and \
+        if code == SerdeUtil.USER_ERROR.TABLE_NOT_FOUND and \
                 isinstance(request, operations.WriteMultipleRequest):
             raise self._handle_write_multiple_table_not_found(code, err, request)
 
-        raise serde.BinaryProtocol.map_exception(code, err)
+        raise SerdeUtil.map_exception(code, err)
 
     @staticmethod
     def _handle_write_multiple_table_not_found(code, err, wm_request):
         """
         Special case for TNF errors on WriteMultiple with many tables.
         Earlier server versions do not support this and will return a
         Table Not Found error with the table names in a single string,
         separated by commas, with no brackets, like:
           table1,table2,table3
 
         Later versions may legitimately return Table Not Found,
         but table names will be inside a bracketed list, like:
           [table1, table2, table3]
         """
-        if code != serde.BinaryProtocol.USER_ERROR.TABLE_NOT_FOUND or \
+        if code != SerdeUtil.USER_ERROR.TABLE_NOT_FOUND or \
                 wm_request.is_single_table() or \
-                err.index(",") < 0 or \
-                err.index("[") >= 0:
-            raise serde.BinaryProtocol.map_exception(code, err)
+                err.find(",") < 0 or \
+                err.find("[") >= 0:
+            raise SerdeUtil.map_exception(code, err)
         raise UnsupportedProtocolException(
             "WriteMultiple requests " +
             "using multiple tables are not supported by the " +
             "version of the connected server.")
 
     @staticmethod
     def _process_not_ok_response(content, status):
         """
         Process not OK response. The method typically throws an appropriate
         exception. A normal return indicates that the method declined to handle
         the response and it's the caller's responsibility to take appropriate
         action.
 
         :param content: content of the response from the server.
-        :type content: bytes for python 3 and str for python 2
+        :type content: bytes
         :param status: the status code of the response from the server.
         :type status: int
         """
         if status == codes.bad:
             length = len(content)
             err_msg = (content if length > 0 else str(status))
             raise NoSQLException('Error response: ' + err_msg)
```

### Comparing `borneo-5.3.7/src/borneo/stats.py` & `borneo-5.4.1/src/borneo/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #
-# Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 import pprint
 import sys
 import uuid
-from collections.abc import Callable
 from datetime import datetime
 from logging import INFO
 from threading import Timer, Lock
 from time import localtime
 from typing import Any, Dict
 
+from collections.abc import Callable
 from . import StatsProfile
-from .exception import SecurityInfoNotReadyException, ThrottlingException, \
-    IllegalArgumentException
+from .exception import (SecurityInfoNotReadyException, ThrottlingException,
+                        IllegalArgumentException)
 from .common import LogUtils, synchronized, CheckValue
 from .kv.exception import AuthenticationException
 from .version import __version__
 
 
 class StatsControl:
     """
@@ -286,15 +286,16 @@
         self._profile = config.get_stats_profile()
         self._interval = config.get_stats_interval()
         self._pretty_print = config.get_stats_pretty_print()
         self._stats_handler = config.get_stats_handler()
 
         self._enable_collection = False
 
-        self._stats = None   # type: Stats
+        # noinspection PyTypeChecker
+        self._stats = None  # type: Stats
         self._id = str(uuid.uuid4())[:8]
 
         if self._profile is not StatsProfile.NONE:
             self._logutils.set_level(INFO)
             self._logutils.log_info(StatsControl.LOG_PREFIX +
                                     "{\"sdkName\": \"Oracle NoSQL SDK for "
                                     "Python" +
@@ -486,15 +487,15 @@
 
 
 class QueryEntryStat:
     """
     Statistics for a certain query.
     """
 
-    def __init__(self, profile, query_request):
+    def __init__(self, profile):
         self._plan = None
         self._does_writes = False
         self._count = 0
         self._unprepared = 0
         self._simple = False
         self._req_stats = ReqStats(profile)
 
@@ -554,19 +555,19 @@
         q_stat.observe(error, retries, retry_delay, rate_limit_delay,
                        auth_count, throttle_count, req_size, res_size,
                        network_latency)
 
     def get_extra_query_stat_entry(self, query_request):
         # type: (borneo.QueryRequest) -> QueryEntryStat
         sql = query_request.get_statement()
-        if sql is None and self._prepared_statement is not None:
-            sql = self._prepared_statement.get_sql_text()
+        if sql is None and query_request.get_prepared_statement() is not None:
+            sql = query_request.get_prepared_statement().get_sql_text()
         q_stat = self._queries.get(sql)
         if q_stat is None:
-            q_stat = QueryEntryStat(self._profile, query_request)
+            q_stat = QueryEntryStat(self._profile)
             self._queries[sql] = q_stat
         if q_stat.get_plan() is None:
             if query_request.get_prepared_statement() is not None:
                 prep_stmt = query_request.get_prepared_statement()
                 q_stat._plan = prep_stmt.print_driver_plan()
                 q_stat._does_writes = prep_stmt.does_writes()
         return q_stat
@@ -584,15 +585,15 @@
 
 class Percentile:
     """
     Implements storing and computation of percentiles for a given set of values.
     """
 
     def __init__(self):
-        self._values = []    # type: [int]
+        self._values = []  # type: [int]
 
     def add_value(self, network_latency):
         # type: (int) -> None
         self._values.append(network_latency)
 
     def get_percentile(self, percentiles):
         # type: ([float]) -> [int]
@@ -613,14 +614,15 @@
         parr = self.get_percentile([0.95, 0.99])
         return parr[0], parr[1]
 
     def clear(self):
         self._values = []
 
 
+# noinspection PyPep8Naming
 class ReqStats:
     """
     Statistics per type of request.
     """
 
     def __init__(self, profile):
         # type: (StatsProfile) -> None
@@ -739,21 +741,22 @@
         self._requestLatencyMin = sys.maxsize
         self._requestLatencyMax = 0
         self._requestLatencySum = 0
         if self._requestLatencyPercentile is not None:
             self._requestLatencyPercentile.clear()
 
 
+# noinspection PyPep8Naming
 class Stats:
     """
     Implements all the statistics.
     """
     _stats_control = None  # type: StatsControl
-    _timer = None         # type: RepeatedTimer
-    _requests = None      # type: Dict[str, ReqStats]
+    _timer = None  # type: RepeatedTimer
+    _requests = None  # type: Dict[str, ReqStats]
 
     _request_names = ["Delete", "Get", "GetIndexes", "GetTable",
                       "ListTables", "MultiDelete", "Prepare", "Put", "Query",
                       "System", "SystemStatus", "Table", "TableUsage",
                       "WriteMultiple", "Write"]
 
     def __init__(self, stats_control):
@@ -783,16 +786,16 @@
 
     @synchronized
     def log_client_stats(self):
         self.__log_client_stats()
 
     def __log_client_stats(self):
         handler = self._stats_control.get_stats_handler()
-        log = self._stats_control.get_logger() is not None and \
-                 self._stats_control.get_logger().isEnabledFor(INFO)
+        log = (self._stats_control.get_logger() is not None and
+               self._stats_control.get_logger().isEnabledFor(INFO))
 
         if handler is not None or log:
             stats = self.__generate_stats()
             self.clear()
 
             if handler is not None:
                 handler(stats)
```

### Comparing `borneo-5.3.7/src/borneo/driver.py` & `borneo-5.4.1/src/borneo/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from json import loads
 from logging import FileHandler, Formatter, WARNING, getLogger
```

### Comparing `borneo-5.3.7/src/borneo.egg-info/PKG-INFO` & `borneo-5.4.1/src/borneo.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,496 +1,495 @@
 Metadata-Version: 2.1
 Name: borneo
-Version: 5.3.7
+Version: 5.4.1
 Summary: Oracle NoSQL Database Python SDK
 Home-page: https://nosql-python-sdk.readthedocs.io/en/stable/index.html
 Author: Oracle
 Author-email: george.feinberg@oracle.com
 License: Universal Permissive License 1.0
-Description: Oracle NoSQL Database Python SDK
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        =====
-        About
-        =====
-        
-        This is the Python SDK for Oracle NoSQL Database. Python 2.7+ and 3.5+ are
-        supported. The SDK provides interfaces, documentation, and examples to help
-        develop Python applications that connect to the Oracle NoSQL Database Cloud
-        Service, Oracle NoSQL Database and to the Oracle NoSQL Cloud Simulator (which
-        runs on a local machine).
-        
-        In order to run the Oracle NoSQL Cloud Simulator, a separate download is
-        necessary from the Oracle NoSQL OTN download page. Throughout the documentation,
-        the Oracle NoSQL Database Cloud Service and Cloud Simulator are referred to as
-        the "cloud service" while the Oracle NoSQL Database is referred to as
-        "on-premise." In the `API reference <https://nosql-python-sdk.readthedocs.io/en/
-        stable/api.html>`_ classes and interfaces are noted if they are only relevant to
-        a specific environment.
-        
-        The on-premise configuration requires a running instance of the Oracle NoSQL
-        database. In addition a running proxy service is required. See `Oracle NoSQL
-        Database Downloads <https://www.oracle.com/database/technologies/nosql-database-
-        server-downloads.html>`_ for downloads, and see `Information about the proxy
-        <https://docs.oracle.com/pls/topic/lookup?ctx=en/database/other-databases/nosql-
-        database/21.2/admin&id=NSADM-GUID-C110AF57-8B35-4C48-A82E-2621C6A5ED72>`_ for
-        proxy configuration information.
-        
-        This project is open source and maintained by Oracle Corp. The home page for the
-        project is `here <https://nosql-python-sdk.readthedocs.io/en/stable/index.
-        html>`_.
-        
-        ============
-        Installation
-        ============
-        
-        The SDK can be installed using pip. If using Python 3 the command may be pip3::
-        
-            pip install borneo
-        
-        If you are using the Oracle NoSQL Database cloud service you will also need to
-        install the oci package::
-        
-            pip install oci
-        
-        See `the installation guide <https://nosql-python-sdk.readthedocs.io/en/stable/
-        installation.html>`_ for additional requirements and and alternative install
-        methods.
-        
-        ========
-        Examples
-        ========
-        
-        Examples can be found `on GitHub <https://github.com/oracle/nosql-python-sdk/
-        tree/master/examples>`_.
-        
-        Examples include simple, standalone programs. They include comments bout how
-        they can be configured and run in the different supported environments.
-        
-        =============
-        Documentation
-        =============
-        
-        The `documentation <https://nosql-python-sdk.readthedocs.io/en/stable>`_ has
-        information on using the SDK as well as an `API reference <https://nosql-python-
-        sdk.readthedocs.io/en/stable/api.html>`_ describing the classes.
-        
-        =======
-        Changes
-        =======
-        
-        See the `Changelog <https://github.com/oracle/nosql-python-sdk/blob/master/
-        CHANGELOG.rst>`_.
-        
-        ====
-        Help
-        ====
-        
-         * Open an issue in the `Issues <https://github.com/oracle/nosql-python-sdk/
-           issues>`_ page.
-         * Email to nosql_sdk_help_grp@oracle.com.
-         * `Oracle NoSQL Developer Forum <https://community.oracle.com/community/
-           groundbreakers/database/nosql_database>`_.
-        
-        When requesting help please be sure to include as much detail as possible,
-        including version of the SDK and **simple**, standalone example code as needed.
-        
-        ==========
-        Quickstart
-        ==========
-        
-        The following is a quick start tutorial to run a simple program in the supported
-        environments. The same template source code is used for all environments. The
-        first step is to cut the program below and paste it into an editor for minor
-        modifications. The instructions assume that is stored as quickstart.py, but you
-        can use any name you like. The quickstart example supports 3 environments:
-        
-        1. Oracle NoSQL Database Cloud Service
-        2. Oracle NoSQL Cloud Simulator
-        3. Oracle NoSQL Database on-premise, using the proxy server
-        
-        See `Running Quickstart`_ to
-        run the quickstart program in different environments. The instructions assume
-        that the *borneo* package has been installed.
-        
-        .. code-block:: pycon
-        
-            #
-            # Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
-            #
-            # Licensed under the Universal Permissive License v 1.0 as shown at
-            #  https://oss.oracle.com/licenses/upl/
-            #
-        
-            #
-            # This is a simple quickstart to demonstrate use of the Python driver for
-            # the Oracle NoSQL Database. It can be used to run against the Oracle NoSQL
-            # Database Cloud Service, against the Cloud Simulator, or against an
-            # on-premise Oracle NoSQL database.
-            #
-            # Usage:
-            #   python quickstart.py <cloud | cloudsim | kvstore>
-            #
-            # Use cloud for the Cloud Service
-            # Use cloudsim for the Cloud Simulator
-            # Use kvstore for the on-premise database
-            #
-            # This example is not intended to be an exhaustive overview of the API,
-            # which has a number of additional operations.
-            #
-            # Requirements:
-            #  1. Python 2.7 or 3.5+
-            #  2. Python dependencies (install using pip or other mechanism):
-            #   o requests
-            #   o oci (only if running against the Cloud Service)
-            #  3. If running against the Cloud Simulator, it can be downloaded from
-            #  here:
-            #   http://www.oracle.com/technetwork/topics/cloud/downloads/index.html
-            #  It requires Java
-            #  4. If running against the Oracle NoSQL Database Cloud Service an account
-            #  must be used.
-            #
-        
-            import sys
-        
-            from borneo import (
-                AuthorizationProvider, DeleteRequest, GetRequest,
-                IllegalArgumentException, NoSQLHandle, NoSQLHandleConfig, PutRequest,
-                QueryRequest, Regions, TableLimits, TableRequest)
-            from borneo.iam import SignatureProvider
-            from borneo.kv import StoreAccessTokenProvider
-        
-        
-            #
-            # EDIT: these values based on desired region and/or endpoint for a local
-            # server
-            #
-            cloud_region = Regions.EU_ZURICH_1
-            cloudsim_endpoint = 'localhost:8080'
-            kvstore_endpoint = 'localhost:80'
-            cloudsim_id = 'cloudsim'  # a fake user id/namespace for the Cloud Simulator
-        
-            # Cloud Service Only
-            #
-            # EDIT: set these variables to the credentials to use if you are not using
-            # a configuration file in ~/.oci/config
-            # Use of these credentials vs a file is determined by a value of tenancy
-            # other than None.
-            #
-            tenancy = None  # tenancy'd OCID (string)
-            user = None  # user's OCID (string)
-            private_key = 'path-to-private-key-or-private-key-content'
-            fingerprint = 'fingerprint for uploaded public key'
-            # pass phrase (string) for private key, or None if not set
-            pass_phrase = None
-        
-        
-            class CloudsimAuthorizationProvider(AuthorizationProvider):
-                """
-                Cloud Simulator Only.
-        
-                This class is used as an AuthorizationProvider when using the Cloud
-                Simulator, which has no security configuration. It accepts a string
-                tenant_id that is used as a simple namespace for tables.
-                """
-        
-                def __init__(self, tenant_id):
-                    super(CloudsimAuthorizationProvider, self).__init__()
-                    self._tenant_id = tenant_id
-        
-                def close(self):
-                    pass
-        
-                def get_authorization_string(self, request=None):
-                    return 'Bearer ' + self._tenant_id
-        
-        
-            def get_handle(nosql_env):
-                """
-                Returns a NoSQLHandle based on the requested environment. The
-                differences among the supported environments are encapsulated in this
-                method.
-                """
-                if nosql_env == 'cloud':
-                    endpoint = cloud_region
-                    #
-                    # Get credentials using SignatureProvider. SignatureProvider has
-                    # several ways to accept credentials. See the documentation:
-                    #  https://nosql-python-sdk.readthedocs.io/en/stable/api/borneo.iam.SignatureProvider.html
-                    #
-                    if tenancy is not None:
-                        print('Using directly provided credentials')
-                        #
-                        # Credentials are provided directly
-                        #
-                        provider = SignatureProvider(tenant_id=tenancy,
-                                                     user_id=user,
-                                                     fingerprint=fingerprint,
-                                                     private_key=private_key,
-                                                     pass_phrase=pass_phrase)
-                    else:
-                        #
-                        # Credentials will come from a file.
-                        #
-                        # By default the file is ~/.oci/config. A config_file = <path>
-                        # argument can be passed to specify a different file.
-                        #
-                        print('Using credentials and DEFAULT profile from ' +
-                              '~/.oci/config')
-                        provider = SignatureProvider()
-                elif nosql_env == 'cloudsim':
-                    print('Using cloud simulator endpoint ' + cloudsim_endpoint)
-                    endpoint = cloudsim_endpoint
-                    provider = CloudsimAuthorizationProvider(cloudsim_id)
-        
-                elif nosql_env == 'kvstore':
-                    print('Using on-premise endpoint ' + kvstore_endpoint)
-                    endpoint = kvstore_endpoint
-                    provider = StoreAccessTokenProvider()
-        
-                else:
-                    raise IllegalArgumentException('Unknown environment: ' + nosql_env)
-        
-                return NoSQLHandle(NoSQLHandleConfig(endpoint, provider))
-        
-        
-            def main():
-        
-                table_name = 'PythonQuickstart'
-        
-                if len(sys.argv) != 2:
-                    print('Usage: python quickstart.py <cloud | cloudsim | kvstore>')
-                    raise SystemExit
-        
-                nosql_env = sys.argv[1:][0]
-                print('Using environment: ' + str(nosql_env))
-        
-                handle = None
-                try:
-        
-                    #
-                    # Create a handle
-                    #
-                    handle = get_handle(nosql_env)
-        
-                    #
-                    # Create a table
-                    #
-                    statement = (
-                        'Create table if not exists {} (id integer, sid integer, ' +
-                        'name string, primary key(shard(sid), id))').format(table_name)
-                    request = TableRequest().set_statement(statement).set_table_limits(
-                        TableLimits(30, 10, 1))
-                    handle.do_table_request(request, 50000, 3000)
-                    print('After create table')
-        
-                    #
-                    # Put a few rows
-                    #
-                    request = PutRequest().set_table_name(table_name)
-                    for i in range(10):
-                        value = {'id': i, 'sid': 0, 'name': 'myname' + str(i)}
-                        request.set_value(value)
-                        handle.put(request)
-                    print('After put of 10 rows')
-        
-                    #
-                    # Get the row
-                    #
-                    request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
-                        table_name)
-                    result = handle.get(request)
-                    print('After get: ' + str(result))
-        
-                    #
-                    # Query, using a range
-                    #
-                    statement = (
-                        'select * from ' + table_name + ' where id > 2 and id < 8')
-                    request = QueryRequest().set_statement(statement)
-                    print('Query results for: ' + statement)
-                    #
-                    # If the :py:meth:`borneo.QueryRequest.is_done` returns False, there
-                    # may be more results, so queries should generally be run in a loop.
-                    # It is possible for single request to return no results but the
-                    # query still not done, indicating that the query loop should
-                    # continue.
-                    #
-                    while True:
-                        result = handle.query(request)
-                        for r in result.get_results():
-                            print('\t' + str(r))
-                        if request.is_done():
-                            break
-        
-                    #
-                    # Delete the row
-                    #
-                    request = DeleteRequest().set_table_name(table_name).set_key(
-                        {'id': 1, 'sid': 0})
-                    result = handle.delete(request)
-                    print('After delete: ' + str(result))
-        
-                    #
-                    # Get again to show deletion
-                    #
-                    request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
-                        table_name)
-                    result = handle.get(request)
-                    print('After get (should be None): ' + str(result))
-        
-                    #
-                    # Drop the table
-                    #
-                    request = TableRequest().set_statement(
-                        'drop table if exists {} '.format(table_name))
-                    result = handle.table_request(request)
-        
-                    #
-                    # Table drop can take time, depending on the state of the system.
-                    # If this wait fails the table will still probably been dropped
-                    #
-                    result.wait_for_completion(handle, 40000, 2000)
-                    print('After drop table')
-        
-                    print('Quickstart is complete')
-                except Exception as e:
-                    print(e)
-                finally:
-                    # If the handle isn't closed Python will not exit properly
-                    if handle is not None:
-                        handle.close()
-        
-        
-            if __name__ == '__main__':
-                main()
-        
-        Running Quickstart
-        ==================
-        
-        Run Against the Oracle NoSQL Database Cloud Service
-        ===================================================
-        
-        Running against the Cloud Service requires an Oracle Cloud account. See
-        `Configure for the Cloud Service <https://nosql-python-sdk.readthedocs.io/en/
-        stable/installation.html#configure-for-the-cloud-service>`_ for information on
-        getting an account and acquiring required credentials.
-        
-        1. Collect the following information:
-        
-         * Tenancy ID
-         * User ID
-         * API signing key (private key file in PEM format)
-         * Fingerprint for the public key uploaded to the user's account
-         * Private key pass phrase, needed only if the private key is encrypted
-        
-        2. Edit *quickstart.py* and add your information. There are 2 ways to supply
-           credentials in the program:
-        
-           * Directly provide the credential information. To use this method, modify the
-             values of the variables at the top of the program: *tenancy*, *user*,
-             *private_key*, *fingerprint*, and *pass_phrase*, setting them to the
-             corresponding information you've collected.
-           * Using a configuration file. In this case the information you've collected
-             goes into a file, ~/.oci/config. `Configure for the Cloud Service <https://
-             nosql-python-sdk.readthedocs.io/en/stable/installation.html#configure-for-
-             the-cloud-service>`_ describes the contents of the file. It will look like
-             this::
-        
-              [DEFAULT]
-              tenancy=<your-tenancy-id>
-              user=<your-user-id>
-              fingerprint=<fingerprint-of-your-public-key>
-              key_file=<path-to-your-private-key-file>
-              pass_phrase=<optional-pass-phrase-for-key-file>
-        
-        3. Decide which region you want to use and modify the *cloud_region* variable to
-           the desired region. See `Regions documentation <https://nosql-python-sdk.
-           readthedocs.io/en/stable/api/borneo.Regions.html>`_ for possible regions. Not
-           all support the Oracle NoSQL Database Cloud Service.
-        
-        4. Run the program:
-        
-        .. code-block:: pycon
-        
-            python quickstart.py cloud
-        
-        Run Against the Oracle NoSQL Cloud Simulator
-        ============================================
-        
-        Running against the Oracle NoSQL Cloud Simulator requires a running Cloud
-        Simulator instance. See `Configure for the Cloud Simulator <https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-cloud-simulator>`_ for information on how to
-        download and start the Cloud Simulator.
-        
-        1. Start the Cloud Simulator based on instructions above. Note the HTTP port
-           used. By default it is *8080* on *localhost*.
-        
-        2. The *quickstart.py* program defaults to *localhost:8080* so if the Cloud
-           Simulator was started using default values no editing is required.
-        
-        3. Run the program:
-        
-        .. code-block:: pycon
-        
-            python quickstart.py cloudsim
-        
-        Run Against Oracle NoSQL on-premise
-        ===================================
-        
-        Running against the Oracle NoSQL Database on-premise requires a running Oracle
-        NoSQL Database instance as well as a running NoSQL Proxy server instance. The
-        program will connect to the proxy server.
-        
-        See `Configure for On-Premise Oracle NoSQL Database <https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-on-premise-oracle-nosql-database>`_ for information on how to
-        download and start the database instance and proxy server. The database and
-        proxy should be started without security enabled for this quickstart program to
-        operate correctly. A secure configuration requires a secure proxy and more
-        complex configuration.
-        
-        1. Start the Oracle NoSQL Database and proxy server based on instructions above.
-           Note the HTTP port used. By default the endpoint is *localhost:80*.
-        
-        2. The *quickstart.py* program defaults to *localhost:80*. If the proxy was
-           started using a different host or port edit the settings accordingly.
-        
-        3. Run the program:
-        
-        .. code-block:: pycon
-        
-            python quickstart.py kvstore
-        
-        =======
-        License
-        =======
-        
-        Copyright (C) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
-        
-        This SDK is licensed under the Universal Permissive License 1.0. See `LICENSE
-        <./LICENSE.txt>`_ for details.
-        
-        ============
-        Contributing
-        ============
-        
-        See `CONTRIBUTING <./CONTRIBUTING.rst>`_
-        
-        ========
-        Security
-        ========
-        
-        See `SECURITY <./SECURITY.rst>`_
-        
 Keywords: database,nosql,cloud,development
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database :: Front-Ends
 Classifier: License :: OSI Approved :: Universal Permissive License (UPL)
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+Oracle NoSQL Database Python SDK
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+=====
+About
+=====
+
+This is the Python SDK for Oracle NoSQL Database. Python versions 3.5+ are
+supported. The SDK provides interfaces, documentation, and examples to help
+develop Python applications that connect to the Oracle NoSQL Database Cloud
+Service, Oracle NoSQL Database and to the Oracle NoSQL Cloud Simulator (which
+runs on a local machine).
+
+In order to run the Oracle NoSQL Cloud Simulator, a separate download is
+necessary from the Oracle NoSQL OTN download page. Throughout the documentation,
+the Oracle NoSQL Database Cloud Service and Cloud Simulator are referred to as
+the "cloud service" while the Oracle NoSQL Database is referred to as
+"on-premise." In the `API reference <https://nosql-python-sdk.readthedocs.io/en/
+stable/api.html>`_ classes and interfaces are noted if they are only relevant to
+a specific environment.
+
+The on-premise configuration requires a running instance of the Oracle NoSQL
+database. In addition a running proxy service is required. See `Oracle NoSQL
+Database Downloads <https://www.oracle.com/database/technologies/nosql-database-
+server-downloads.html>`_ for downloads, and see `Information about the proxy
+<https://docs.oracle.com/pls/topic/lookup?ctx=en/database/other-databases/nosql-
+database/22.3/admin&id=NSADM-GUID-C110AF57-8B35-4C48-A82E-2621C6A5ED72>`_ for
+proxy configuration information.
+
+This project is open source and maintained by Oracle Corp. The home page for the
+project is `here <https://nosql-python-sdk.readthedocs.io/en/stable/index.
+html>`_.
+
+============
+Installation
+============
+
+The SDK can be installed using pip. If using Python 3 the command may be pip3::
+
+    pip install borneo
+
+If you are using the Oracle NoSQL Database cloud service you will also need to
+install the oci package::
+
+    pip install oci
+
+See `the installation guide <https://nosql-python-sdk.readthedocs.io/en/stable/
+installation.html>`_ for additional requirements and and alternative install
+methods.
+
+========
+Examples
+========
+
+Examples can be found `on GitHub <https://github.com/oracle/nosql-python-sdk/
+tree/master/examples>`_.
+
+Examples include simple, standalone programs. They include comments about how
+they can be configured and run in the different supported environments.
+
+=============
+Documentation
+=============
+
+The `documentation <https://nosql-python-sdk.readthedocs.io/en/stable>`_ has
+information on using the SDK as well as an `API reference <https://nosql-python-
+sdk.readthedocs.io/en/stable/api.html>`_ describing the classes.
+
+=======
+Changes
+=======
+
+See the `Changelog <https://github.com/oracle/nosql-python-sdk/blob/master/
+CHANGELOG.rst>`_.
+
+====
+Help
+====
+
+ * Open an issue in the `Issues <https://github.com/oracle/nosql-python-sdk/
+   issues>`_ page.
+ * Email to nosql_sdk_help_grp@oracle.com.
+ * `Oracle NoSQL Developer Forum <https://community.oracle.com/community/
+   groundbreakers/database/nosql_database>`_.
+
+When requesting help please be sure to include as much detail as possible,
+including version of the SDK and **simple**, standalone example code as needed.
+
+==========
+Quickstart
+==========
+
+The following is a quick start tutorial to run a simple program in the supported
+environments. The same template source code is used for all environments. The
+first step is to cut the program below and paste it into an editor for minor
+modifications. The instructions assume that is stored as quickstart.py, but you
+can use any name you like. The quickstart example supports 3 environments:
+
+1. Oracle NoSQL Database Cloud Service
+2. Oracle NoSQL Cloud Simulator
+3. Oracle NoSQL Database on-premise, using the proxy server
+
+See `Running Quickstart`_ to
+run the quickstart program in different environments. The instructions assume
+that the *borneo* package has been installed.
+
+.. code-block:: pycon
+
+    #
+    # Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
+    #
+    # Licensed under the Universal Permissive License v 1.0 as shown at
+    #  https://oss.oracle.com/licenses/upl/
+    #
+
+    #
+    # This is a simple quickstart to demonstrate use of the Python driver for
+    # the Oracle NoSQL Database. It can be used to run against the Oracle NoSQL
+    # Database Cloud Service, against the Cloud Simulator, or against an
+    # on-premise Oracle NoSQL database.
+    #
+    # Usage:
+    #   python quickstart.py <cloud | cloudsim | kvstore>
+    #
+    # Use cloud for the Cloud Service
+    # Use cloudsim for the Cloud Simulator
+    # Use kvstore for the on-premise database
+    #
+    # This example is not intended to be an exhaustive overview of the API,
+    # which has a number of additional operations.
+    #
+    # Requirements:
+    #  1. Python 3.5+
+    #  2. Python dependencies (install using pip or other mechanism):
+    #   o requests
+    #   o oci (only if running against the Cloud Service)
+    #  3. If running against the Cloud Simulator, it can be downloaded from
+    #  here:
+    #   http://www.oracle.com/technetwork/topics/cloud/downloads/index.html
+    #  It requires Java
+    #  4. If running against the Oracle NoSQL Database Cloud Service an account
+    #  must be used.
+    #
+
+    import sys
+
+    from borneo import (
+        AuthorizationProvider, DeleteRequest, GetRequest,
+        IllegalArgumentException, NoSQLHandle, NoSQLHandleConfig, PutRequest,
+        QueryRequest, Regions, TableLimits, TableRequest)
+    from borneo.iam import SignatureProvider
+    from borneo.kv import StoreAccessTokenProvider
+
+
+    #
+    # EDIT: these values based on desired region and/or endpoint for a local
+    # server
+    #
+    cloud_region = Regions.EU_ZURICH_1
+    cloudsim_endpoint = 'localhost:8080'
+    kvstore_endpoint = 'localhost:80'
+    cloudsim_id = 'cloudsim'  # a fake user id/namespace for the Cloud Simulator
+
+    # Cloud Service Only
+    #
+    # EDIT: set these variables to the credentials to use if you are not using
+    # a configuration file in ~/.oci/config
+    # Use of these credentials vs a file is determined by a value of tenancy
+    # other than None.
+    #
+    tenancy = None  # tenancy'd OCID (string)
+    user = None  # user's OCID (string)
+    private_key = 'path-to-private-key-or-private-key-content'
+    fingerprint = 'fingerprint for uploaded public key'
+    # pass phrase (string) for private key, or None if not set
+    pass_phrase = None
+
+
+    class CloudsimAuthorizationProvider(AuthorizationProvider):
+        """
+        Cloud Simulator Only.
+
+        This class is used as an AuthorizationProvider when using the Cloud
+        Simulator, which has no security configuration. It accepts a string
+        tenant_id that is used as a simple namespace for tables.
+        """
+
+        def __init__(self, tenant_id):
+            super(CloudsimAuthorizationProvider, self).__init__()
+            self._tenant_id = tenant_id
+
+        def close(self):
+            pass
+
+        def get_authorization_string(self, request=None):
+            return 'Bearer ' + self._tenant_id
+
+
+    def get_handle(nosql_env):
+        """
+        Returns a NoSQLHandle based on the requested environment. The
+        differences among the supported environments are encapsulated in this
+        method.
+        """
+        if nosql_env == 'cloud':
+            endpoint = cloud_region
+            #
+            # Get credentials using SignatureProvider. SignatureProvider has
+            # several ways to accept credentials. See the documentation:
+            #  https://nosql-python-sdk.readthedocs.io/en/stable/api/borneo.iam.SignatureProvider.html
+            #
+            if tenancy is not None:
+                print('Using directly provided credentials')
+                #
+                # Credentials are provided directly
+                #
+                provider = SignatureProvider(tenant_id=tenancy,
+                                             user_id=user,
+                                             fingerprint=fingerprint,
+                                             private_key=private_key,
+                                             pass_phrase=pass_phrase)
+            else:
+                #
+                # Credentials will come from a file.
+                #
+                # By default the file is ~/.oci/config. A config_file = <path>
+                # argument can be passed to specify a different file.
+                #
+                print('Using credentials and DEFAULT profile from ' +
+                      '~/.oci/config')
+                provider = SignatureProvider()
+        elif nosql_env == 'cloudsim':
+            print('Using cloud simulator endpoint ' + cloudsim_endpoint)
+            endpoint = cloudsim_endpoint
+            provider = CloudsimAuthorizationProvider(cloudsim_id)
+
+        elif nosql_env == 'kvstore':
+            print('Using on-premise endpoint ' + kvstore_endpoint)
+            endpoint = kvstore_endpoint
+            provider = StoreAccessTokenProvider()
+
+        else:
+            raise IllegalArgumentException('Unknown environment: ' + nosql_env)
+
+        return NoSQLHandle(NoSQLHandleConfig(endpoint, provider))
+
+
+    def main():
+
+        table_name = 'PythonQuickstart'
+
+        if len(sys.argv) != 2:
+            print('Usage: python quickstart.py <cloud | cloudsim | kvstore>')
+            raise SystemExit
+
+        nosql_env = sys.argv[1:][0]
+        print('Using environment: ' + str(nosql_env))
+
+        handle = None
+        try:
+
+            #
+            # Create a handle
+            #
+            handle = get_handle(nosql_env)
+
+            #
+            # Create a table
+            #
+            statement = (
+                'Create table if not exists {} (id integer, sid integer, ' +
+                'name string, primary key(shard(sid), id))').format(table_name)
+            request = TableRequest().set_statement(statement).set_table_limits(
+                TableLimits(30, 10, 1))
+            handle.do_table_request(request, 50000, 3000)
+            print('After create table')
+
+            #
+            # Put a few rows
+            #
+            request = PutRequest().set_table_name(table_name)
+            for i in range(10):
+                value = {'id': i, 'sid': 0, 'name': 'myname' + str(i)}
+                request.set_value(value)
+                handle.put(request)
+            print('After put of 10 rows')
+
+            #
+            # Get the row
+            #
+            request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
+                table_name)
+            result = handle.get(request)
+            print('After get: ' + str(result))
+
+            #
+            # Query, using a range
+            #
+            statement = (
+                'select * from ' + table_name + ' where id > 2 and id < 8')
+            request = QueryRequest().set_statement(statement)
+            print('Query results for: ' + statement)
+            #
+            # If the :py:meth:`borneo.QueryRequest.is_done` returns False, there
+            # may be more results, so queries should generally be run in a loop.
+            # It is possible for single request to return no results but the
+            # query still not done, indicating that the query loop should
+            # continue.
+            #
+            while True:
+                result = handle.query(request)
+                for r in result.get_results():
+                    print('\t' + str(r))
+                if request.is_done():
+                    break
+
+            #
+            # Delete the row
+            #
+            request = DeleteRequest().set_table_name(table_name).set_key(
+                {'id': 1, 'sid': 0})
+            result = handle.delete(request)
+            print('After delete: ' + str(result))
+
+            #
+            # Get again to show deletion
+            #
+            request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
+                table_name)
+            result = handle.get(request)
+            print('After get (should be None): ' + str(result))
+
+            #
+            # Drop the table
+            #
+            request = TableRequest().set_statement(
+                'drop table if exists {} '.format(table_name))
+            result = handle.table_request(request)
+
+            #
+            # Table drop can take time, depending on the state of the system.
+            # If this wait fails the table will still probably been dropped
+            #
+            result.wait_for_completion(handle, 40000, 2000)
+            print('After drop table')
+
+            print('Quickstart is complete')
+        except Exception as e:
+            print(e)
+        finally:
+            # If the handle isn't closed Python will not exit properly
+            if handle is not None:
+                handle.close()
+
+
+    if __name__ == '__main__':
+        main()
+
+Running Quickstart
+==================
+
+Run Against the Oracle NoSQL Database Cloud Service
+===================================================
+
+Running against the Cloud Service requires an Oracle Cloud account. See
+`Configure for the Cloud Service <https://nosql-python-sdk.readthedocs.io/en/
+stable/installation.html#configure-for-the-cloud-service>`_ for information on
+getting an account and acquiring required credentials.
+
+1. Collect the following information:
+
+ * Tenancy ID
+ * User ID
+ * API signing key (private key file in PEM format)
+ * Fingerprint for the public key uploaded to the user's account
+ * Private key pass phrase, needed only if the private key is encrypted
+
+2. Edit *quickstart.py* and add your information. There are 2 ways to supply
+   credentials in the program:
+
+   * Directly provide the credential information. To use this method, modify the
+     values of the variables at the top of the program: *tenancy*, *user*,
+     *private_key*, *fingerprint*, and *pass_phrase*, setting them to the
+     corresponding information you've collected.
+   * Using a configuration file. In this case the information you've collected
+     goes into a file, ~/.oci/config. `Configure for the Cloud Service <https://
+     nosql-python-sdk.readthedocs.io/en/stable/installation.html#configure-for-
+     the-cloud-service>`_ describes the contents of the file. It will look like
+     this::
+
+      [DEFAULT]
+      tenancy=<your-tenancy-id>
+      user=<your-user-id>
+      fingerprint=<fingerprint-of-your-public-key>
+      key_file=<path-to-your-private-key-file>
+      pass_phrase=<optional-pass-phrase-for-key-file>
+
+3. Decide which region you want to use and modify the *cloud_region* variable to
+   the desired region. See `Regions documentation <https://nosql-python-sdk.
+   readthedocs.io/en/stable/api/borneo.Regions.html>`_ for possible regions. Not
+   all support the Oracle NoSQL Database Cloud Service.
+
+4. Run the program:
+
+.. code-block:: pycon
+
+    python quickstart.py cloud
+
+Run Against the Oracle NoSQL Cloud Simulator
+============================================
+
+Running against the Oracle NoSQL Cloud Simulator requires a running Cloud
+Simulator instance. See `Configure for the Cloud Simulator <https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-cloud-simulator>`_ for information on how to
+download and start the Cloud Simulator.
+
+1. Start the Cloud Simulator based on instructions above. Note the HTTP port
+   used. By default it is *8080* on *localhost*.
+
+2. The *quickstart.py* program defaults to *localhost:8080* so if the Cloud
+   Simulator was started using default values no editing is required.
+
+3. Run the program:
+
+.. code-block:: pycon
+
+    python quickstart.py cloudsim
+
+Run Against Oracle NoSQL on-premise
+===================================
+
+Running against the Oracle NoSQL Database on-premise requires a running Oracle
+NoSQL Database instance as well as a running NoSQL Proxy server instance. The
+program will connect to the proxy server.
+
+See `Configure for On-Premise Oracle NoSQL Database <https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-on-premise-oracle-nosql-database>`_ for information on how to
+download and start the database instance and proxy server. The database and
+proxy should be started without security enabled for this quickstart program to
+operate correctly. A secure configuration requires a secure proxy and more
+complex configuration.
+
+1. Start the Oracle NoSQL Database and proxy server based on instructions above.
+   Note the HTTP port used. By default the endpoint is *localhost:80*.
+
+2. The *quickstart.py* program defaults to *localhost:80*. If the proxy was
+   started using a different host or port edit the settings accordingly.
+
+3. Run the program:
+
+.. code-block:: pycon
+
+    python quickstart.py kvstore
+
+=======
+License
+=======
+
+Copyright (C) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+
+This SDK is licensed under the Universal Permissive License 1.0. See `LICENSE
+<./LICENSE.txt>`_ for details.
+
+============
+Contributing
+============
+
+See `CONTRIBUTING <./CONTRIBUTING.rst>`_
+
+========
+Security
+========
+
+See `SECURITY <./SECURITY.rst>`_
```

### Comparing `borneo-5.3.7/src/borneo.egg-info/SOURCES.txt` & `borneo-5.4.1/src/borneo.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -8,17 +8,20 @@
 src/borneo/auth.py
 src/borneo/client.py
 src/borneo/common.py
 src/borneo/config.py
 src/borneo/driver.py
 src/borneo/exception.py
 src/borneo/http.py
+src/borneo/nson.py
+src/borneo/nson_protocol.py
 src/borneo/operations.py
 src/borneo/query.py
 src/borneo/serde.py
+src/borneo/serdeutil.py
 src/borneo/stats.py
 src/borneo/version.py
 src/borneo.egg-info/PKG-INFO
 src/borneo.egg-info/SOURCES.txt
 src/borneo.egg-info/dependency_links.txt
 src/borneo.egg-info/requires.txt
 src/borneo.egg-info/top_level.txt
```

