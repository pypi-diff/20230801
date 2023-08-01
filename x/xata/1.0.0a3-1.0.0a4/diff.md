# Comparing `tmp/xata-1.0.0a3.tar.gz` & `tmp/xata-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xata-1.0.0a3.tar", max compression
+gzip compressed data, was "xata-1.0.0a4.tar", max compression
```

## Comparing `xata-1.0.0a3.tar` & `xata-1.0.0a4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-07-07 13:58:14.054969 xata-1.0.0a3/LICENSE
--rw-r--r--   0        0        0     1156 2023-07-07 13:58:14.054969 xata-1.0.0a3/README.md
--rw-r--r--   0        0        0      818 2023-07-07 13:58:14.086971 xata-1.0.0a3/pyproject.toml
--rw-r--r--   0        0        0      873 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/__init__.py
--rw-r--r--   0        0        0      769 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/__init__.py
--rw-r--r--   0        0        0     2694 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/authentication.py
--rw-r--r--   0        0        0    12773 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/branch.py
--rw-r--r--   0        0        0     7627 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/databases.py
--rw-r--r--   0        0        0     8958 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/files.py
--rw-r--r--   0        0        0     6103 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/invites.py
--rw-r--r--   0        0        0    12076 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/migrations.py
--rw-r--r--   0        0        0    12641 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/records.py
--rw-r--r--   0        0        0    31571 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/search_and_filter.py
--rw-r--r--   0        0        0    12638 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/table.py
--rw-r--r--   0        0        0     2544 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/users.py
--rw-r--r--   0        0        0     7478 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/workspaces.py
--rw-r--r--   0        0        0     3186 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api_response.py
--rw-r--r--   0        0        0    13637 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/client.py
--rw-r--r--   0        0        0     1188 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/errors.py
--rw-r--r--   0        0        0    15894 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/helpers.py
--rw-r--r--   0        0        0     3077 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/namespace.py
--rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 xata-1.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-01 07:12:10.555548 xata-1.0.0a4/LICENSE
+-rw-r--r--   0        0        0     1083 2023-08-01 07:12:10.555548 xata-1.0.0a4/README.md
+-rw-r--r--   0        0        0      818 2023-08-01 07:12:10.583549 xata-1.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0      873 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/__init__.py
+-rw-r--r--   0        0        0      769 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/api/__init__.py
+-rw-r--r--   0        0        0     2995 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/api/authentication.py
+-rw-r--r--   0        0        0    13898 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/api/branch.py
+-rw-r--r--   0        0        0     8389 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/api/databases.py
+-rw-r--r--   0        0        0     8962 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/api/files.py
+-rw-r--r--   0        0        0     6742 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/api/invites.py
+-rw-r--r--   0        0        0    13228 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/api/migrations.py
+-rw-r--r--   0        0        0    13684 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/api/records.py
+-rw-r--r--   0        0        0    33149 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/api/search_and_filter.py
+-rw-r--r--   0        0        0    13796 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/api/table.py
+-rw-r--r--   0        0        0     2771 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/api/users.py
+-rw-r--r--   0        0        0     8262 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/api/workspaces.py
+-rw-r--r--   0        0        0     3080 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/api_request.py
+-rw-r--r--   0        0        0     3186 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/api_response.py
+-rw-r--r--   0        0        0    13444 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/client.py
+-rw-r--r--   0        0        0     1188 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/errors.py
+-rw-r--r--   0        0        0    15894 2023-08-01 07:12:10.619552 xata-1.0.0a4/xata/helpers.py
+-rw-r--r--   0        0        0     1796 1970-01-01 00:00:00.000000 xata-1.0.0a4/PKG-INFO
```

### Comparing `xata-1.0.0a3/LICENSE` & `xata-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a3/README.md` & `xata-1.0.0a4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 <p align="center">
-  <img width="200" src="https://raw.githubusercontent.com/xataio/company/main/logo/non-resizable/for-light-backgrounds/colored-with-text.png#gh-light-mode-only" />
-  <img width="200" src="https://raw.githubusercontent.com/xataio/company/main/logo/non-resizable/for-dark-backgrounds/colored-with-text.png#gh-dark-mode-only" />
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="./assets/logo_dark.svg">
+    <source media="(prefers-color-scheme: light)" srcset="./assets/logo_light.svg">
+    <img width="400" alt="Xata" src="./assets/logo_dark.svg">
+  </picture>
 </p>
 
 # Python SDK for Xata
 
 [![Documentation Status](https://readthedocs.org/projects/xata-py/badge/?version=latest)](https://xata-py.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/xata.svg)](https://badge.fury.io/py/xata)
 
 Simple Python client for xata.io databases. Currently work in progress.
```

### Comparing `xata-1.0.0a3/pyproject.toml` & `xata-1.0.0a4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xata"
-version = "1.0.0a3"
+version = "1.0.0a4"
 description = "Python client for Xata.io"
 authors = ["Xata <support@xata.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 documentation = "https://xata-py.readthedocs.io"
 
 [tool.poetry.dependencies]
```

### Comparing `xata-1.0.0a3/xata/__init__.py` & `xata-1.0.0a4/xata/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a3/xata/api/__init__.py` & `xata-1.0.0a4/xata/api/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a3/xata/api/authentication.py` & `xata-1.0.0a4/xata/api/users.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,80 +14,83 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 
 # ------------------------------------------------------- #
-# Authentication
-# Authentication and API Key management.
+# Users
+# Users management
 # Specification: core:v1.0
 # ------------------------------------------------------- #
 
+from xata.api_request import ApiRequest
 from xata.api_response import ApiResponse
-from xata.namespace import Namespace
 
 
-class Authentication(Namespace):
+class Users(ApiRequest):
 
     scope = "core"
 
-    def get_user_api_keys(self) -> ApiResponse:
+    def get(self) -> ApiResponse:
         """
-        Retrieve a list of existing user API keys
+        Return details of the user making the request
 
-        Path: /user/keys
+        Reference: https://xata.io/docs/api-reference/user#get-user-details
+        Path: /user
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
 
         :returns ApiResponse
         """
-        url_path = "/user/keys"
+        url_path = "/user"
         return self.request("GET", url_path)
 
-    def create_user_api_keys(self, key_name: str) -> ApiResponse:
+    def update(self, payload: dict) -> ApiResponse:
         """
-        Create and return new API key
+        Update user info
 
-        Path: /user/keys/{key_name}
-        Method: POST
+        Reference: https://xata.io/docs/api-reference/user#update-user-info
+        Path: /user
+        Method: PUT
         Response status codes:
-        - 201: OK
+        - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
-        :param key_name: str API Key name
+        :param payload: dict content
 
         :returns ApiResponse
         """
-        url_path = f"/user/keys/{key_name}"
-        return self.request("POST", url_path)
+        url_path = "/user"
+        headers = {"content-type": "application/json"}
+        return self.request("PUT", url_path, headers, payload)
 
-    def delete_user_api_keys(self, key_name: str) -> ApiResponse:
+    def delete(self) -> ApiResponse:
         """
-        Delete an existing API key
+        Delete the user making the request
 
-        Path: /user/keys/{key_name}
+        Reference: https://xata.io/docs/api-reference/user#delete-user
+        Path: /user
         Method: DELETE
         Response status codes:
         - 204: No Content
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
 
-        :param key_name: str API Key name
 
         :returns ApiResponse
         """
-        url_path = f"/user/keys/{key_name}"
+        url_path = "/user"
         return self.request("DELETE", url_path)
```

### Comparing `xata-1.0.0a3/xata/api/branch.py` & `xata-1.0.0a4/xata/api/branch.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,26 +19,27 @@
 
 # ------------------------------------------------------- #
 # Branch
 # Branch management.
 # Specification: workspace:v1.0
 # ------------------------------------------------------- #
 
+from xata.api_request import ApiRequest
 from xata.api_response import ApiResponse
-from xata.namespace import Namespace
 
 
-class Branch(Namespace):
+class Branch(ApiRequest):
 
     scope = "workspace"
 
     def list(self, db_name: str) -> ApiResponse:
         """
         List all available Branches
 
+        Reference: https://xata.io/docs/api-reference/dbs/db_name#list-branches
         Path: /dbs/{db_name}
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -53,14 +54,15 @@
         url_path = f"/dbs/{db_name}"
         return self.request("GET", url_path)
 
     def get_details(self, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Get branch schema and metadata
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name#get-branch-schema-and-metadata
         Path: /db/{db_branch_name}
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -77,14 +79,15 @@
         url_path = f"/db/{db_branch_name}"
         return self.request("GET", url_path)
 
     def create(self, payload: dict, db_name: str = None, branch_name: str = None, from_: str = None) -> ApiResponse:
         """
         Create Database branch
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name#create-database-branch
         Path: /db/{db_branch_name}
         Method: PUT
         Response status codes:
         - 201: Created
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -99,22 +102,23 @@
         :param from_: str = None Name of source branch to branch the new schema from
 
         :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}"
         if from_ is not None:
-            url_path += "?from={from_}"
+            url_path += f"?from={from_}"
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
     def delete(self, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Delete the branch in the database and all its resources
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name#delete-database-branch
         Path: /db/{db_branch_name}
         Method: DELETE
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -132,14 +136,15 @@
         url_path = f"/db/{db_branch_name}"
         return self.request("DELETE", url_path)
 
     def get_metadata(self, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Get Branch Metadata
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/metadata#get-branch-metadata
         Path: /db/{db_branch_name}/metadata
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -156,14 +161,15 @@
         url_path = f"/db/{db_branch_name}/metadata"
         return self.request("GET", url_path)
 
     def update_metadata(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Update the branch metadata
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/metadata#update-branch-metadata
         Path: /db/{db_branch_name}/metadata
         Method: PUT
         Response status codes:
         - 204: No Content
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -181,14 +187,15 @@
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
     def get_stats(self, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Get branch usage metrics.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/stats#branch-stats
         Path: /db/{db_branch_name}/stats
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Example response
         - 401: Authentication Error
         - 404: Example response
@@ -209,14 +216,15 @@
         """
         Lists all the git branches in the mapping, and their associated Xata branches.  Example
         response:  ```json {   "mappings": [       {         "gitBranch": "main",
         "xataBranch": "main"       },       {         "gitBranch": "gitBranch1",
         "xataBranch": "xataBranch1"       }       {         "gitBranch": "xataBranch2",
         "xataBranch": "xataBranch2"       }   ] } ```
 
+        Reference: https://xata.io/docs/api-reference/dbs/db_name/gitBranches#list-git-branches-mapping
         Path: /dbs/{db_name}/gitBranches
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 5XX: Unexpected Error
@@ -237,14 +245,15 @@
         a 400 error is returned.  If the git branch is already present in the mapping, the old
         entry is overwritten, and a warning message is included in the response.  If the git
         branch is added and didn't exist before, the response code is 204. If the git branch
         existed and it was overwritten, the response code is 201.  Example request:  ```json //
         POST https://tutorial-ng7s8c.xata.sh/dbs/demo/gitBranches {   "gitBranch": "fix/bug123",
         "xataBranch": "fix_bug" } ```
 
+        Reference: https://xata.io/docs/api-reference/dbs/db_name/gitBranches#link-a-git-branch-to-a-xata-branch
         Path: /dbs/{db_name}/gitBranches
         Method: POST
         Response status codes:
         - 201: Operation was successful with warnings
         - 204: Operation was successful without warnings
         - 400: Bad Request
         - 401: Authentication Error
@@ -264,14 +273,15 @@
     def remove_git_branches_entry(self, db_name: str, git_branch: str) -> ApiResponse:
         """
         Removes an entry from the mapping of git branches to Xata branches.  The name of the git
         branch must be passed as a query parameter.  If the git branch is not found, the endpoint
         returns a 404 status code.  Example request:  ```json // DELETE https://tutorial-
         ng7s8c.xata.sh/dbs/demo/gitBranches?gitBranch=fix%2Fbug123 ```
 
+        Reference: https://xata.io/docs/api-reference/dbs/db_name/gitBranches#unlink-a-git-branch-to-a-xata-branch
         Path: /dbs/{db_name}/gitBranches
         Method: DELETE
         Response status codes:
         - 204: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: The git branch was not found in the mapping
@@ -281,15 +291,15 @@
         :param db_name: str The Database Name
         :param git_branch: str The Git Branch to remove from the mapping
 
         :returns ApiResponse
         """
         url_path = f"/dbs/{db_name}/gitBranches"
         if git_branch is not None:
-            url_path += "?gitBranch={git_branch}"
+            url_path += f"?gitBranch={git_branch}"
         return self.request("DELETE", url_path)
 
     def resolve(self, db_name: str, git_branch: str = None, fallback_branch: str = None) -> ApiResponse:
         """
         In order to resolve the database branch, the following algorithm is used: * if the
         `gitBranch` was provided and is found in the [git branches mapping](/api-
         reference/dbs/db_name/gitBranches), the associated Xata branch is returned * else, if a
@@ -297,14 +307,15 @@
         `fallbackBranch` is provided and a branch with that name exists, return it * else, return
         the default branch of the DB (`main` or the first branch)  Example call:  ```json // GET
         https://tutorial-
         ng7s8c.xata.sh/dbs/demo/dbs/demo/resolveBranch?gitBranch=test&fallbackBranch=tsg ```
         Example response:  ```json {   "branch": "main",   "reason": {     "code":
         "DEFAULT_BRANCH",     "message": "Default branch for this database (main)"   } } ```
 
+        Reference: https://xata.io/docs/api-reference/dbs/db_name/resolveBranch#resolve-a-git-branch-to-a-xata-branch
         Path: /dbs/{db_name}/resolveBranch
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 5XX: Unexpected Error
```

### Comparing `xata-1.0.0a3/xata/api/databases.py` & `xata-1.0.0a4/xata/api/databases.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,26 +19,27 @@
 
 # ------------------------------------------------------- #
 # Databases
 # Workspace databases management.
 # Specification: core:v1.0
 # ------------------------------------------------------- #
 
+from xata.api_request import ApiRequest
 from xata.api_response import ApiResponse
-from xata.namespace import Namespace
 
 
-class Databases(Namespace):
+class Databases(ApiRequest):
 
     scope = "core"
 
     def list(self, workspace_id: str = None) -> ApiResponse:
         """
         List all databases available in your Workspace.
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id/dbs#list-databases
         Path: /workspaces/{workspace_id}/dbs
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 5XX: Unexpected Error
@@ -53,14 +54,15 @@
         url_path = f"/workspaces/{workspace_id}/dbs"
         return self.request("GET", url_path)
 
     def get_metadata(self, db_name: str, workspace_id: str = None) -> ApiResponse:
         """
         Retrieve metadata of the given database
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id/dbs/db_name#get-database-metadata
         Path: /workspaces/{workspace_id}/dbs/{db_name}
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -79,14 +81,15 @@
 
     def create(
         self, db_name: str, workspace_id: str = None, region: str = None, branch_name: str = None
     ) -> ApiResponse:
         """
         Create Database with identifier name
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id/dbs/db_name#create-database
         Path: /workspaces/{workspace_id}/dbs/{db_name}
         Method: PUT
         Response status codes:
         - 201: Created
         - 400: Bad Request
         - 401: Authentication Error
         - 422: Example response
@@ -111,14 +114,15 @@
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
     def delete(self, db_name: str, workspace_id: str = None) -> ApiResponse:
         """
         Delete a database and all of its branches and tables permanently.
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id/dbs/db_name#delete-database
         Path: /workspaces/{workspace_id}/dbs/{db_name}
         Method: DELETE
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -135,14 +139,15 @@
         url_path = f"/workspaces/{workspace_id}/dbs/{db_name}"
         return self.request("DELETE", url_path)
 
     def update_metadata(self, db_name: str, payload: dict, workspace_id: str = None) -> ApiResponse:
         """
         Update the color of the selected database
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id/dbs/db_name#update-database-metadata
         Path: /workspaces/{workspace_id}/dbs/{db_name}
         Method: PATCH
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -161,14 +166,15 @@
         headers = {"content-type": "application/json"}
         return self.request("PATCH", url_path, headers, payload)
 
     def rename(self, db_name: str, new_name: str, workspace_id: str = None) -> ApiResponse:
         """
         Change the name of an existing database
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id/dbs/db_name/rename#rename-database
         Path: /workspaces/{workspace_id}/dbs/{db_name}/rename
         Method: POST
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 422: Example response
@@ -189,14 +195,15 @@
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def get_regions(self, workspace_id: str = None) -> ApiResponse:
         """
         List regions available to create a database on
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id/regions#list-available-regions
         Path: /workspaces/{workspace_id}/regions
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 5XX: Unexpected Error
```

### Comparing `xata-1.0.0a3/xata/api/files.py` & `xata-1.0.0a4/xata/api/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 
 # ------------------------------------------------------- #
 # Files
 # Files
 # Specification: core:v1.0
 # ------------------------------------------------------- #
 
+from xata.api_request import ApiRequest
 from xata.api_response import ApiResponse
-from xata.namespace import Namespace
 
 
-class Files(Namespace):
+class Files(ApiRequest):
 
     scope = "workspace"
 
     def get_item(
         self,
         table_name: str,
         record_id: str,
```

### Comparing `xata-1.0.0a3/xata/api/invites.py` & `xata-1.0.0a4/xata/api/invites.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,26 +19,27 @@
 
 # ------------------------------------------------------- #
 # Invites
 # Manage user invites.
 # Specification: core:v1.0
 # ------------------------------------------------------- #
 
+from xata.api_request import ApiRequest
 from xata.api_response import ApiResponse
-from xata.namespace import Namespace
 
 
-class Invites(Namespace):
+class Invites(ApiRequest):
 
     scope = "core"
 
     def new(self, payload: dict, workspace_id: str = None) -> ApiResponse:
         """
         Invite some user to join the workspace with the given role
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id/invites#invite-a-user-to-join-the-workspace
         Path: /workspaces/{workspace_id}/invites
         Method: POST
         Response status codes:
         - 201: Created
         - 400: Bad Request
         - 401: Authentication Error
         - 403: Authentication Error
@@ -59,14 +60,15 @@
         return self.request("POST", url_path, headers, payload)
 
     def cancel(self, invite_id: str, workspace_id: str = None) -> ApiResponse:
         """
         This operation provides a way to cancel invites by deleting them.  Already accepted
         invites cannot be deleted.
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id/invites/invite_id#deletes-an-invite
         Path: /workspaces/{workspace_id}/invites/{invite_id}
         Method: DELETE
         Response status codes:
         - 204: No Content
         - 400: Bad Request
         - 401: Authentication Error
         - 403: Authentication Error
@@ -85,14 +87,15 @@
 
     def update(self, invite_id: str, payload: dict, workspace_id: str = None) -> ApiResponse:
         """
         This operation provides a way to update an existing invite.  Updates are performed in-
         place; they do not change the invite link, the expiry time, nor do they re-notify the
         recipient of the invite.
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id/invites/invite_id#updates-an-existing-invite
         Path: /workspaces/{workspace_id}/invites/{invite_id}
         Method: PATCH
         Response status codes:
         - 200: Updated successfully.
         - 400: Bad Request
         - 401: Authentication Error
         - 403: Authentication Error
@@ -114,14 +117,15 @@
         return self.request("PATCH", url_path, headers, payload)
 
     def accept(self, invite_key: str, workspace_id: str = None) -> ApiResponse:
         """
         Accept the invitation to join a workspace.  If the operation succeeds the user will be a
         member of the workspace
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id/invites/invite_key/accept#accept-the-invitation-to-join-a-workspace
         Path: /workspaces/{workspace_id}/invites/{invite_key}/accept
         Method: POST
         Response status codes:
         - 204: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 403: Authentication Error
@@ -139,14 +143,15 @@
         return self.request("POST", url_path)
 
     def resend(self, invite_id: str, workspace_id: str = None) -> ApiResponse:
         """
         This operation provides a way to resend an Invite notification.  Invite notifications can
         only be sent for Invites not yet accepted.
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id/invites/invite_id/resend#resend-invite-notification
         Path: /workspaces/{workspace_id}/invites/{invite_id}/resend
         Method: POST
         Response status codes:
         - 204: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 403: Authentication Error
```

### Comparing `xata-1.0.0a3/xata/api/migrations.py` & `xata-1.0.0a4/xata/api/migrations.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,26 +19,27 @@
 
 # ------------------------------------------------------- #
 # Migrations
 # Branch schema migrations and history.
 # Specification: workspace:v1.0
 # ------------------------------------------------------- #
 
+from xata.api_request import ApiRequest
 from xata.api_response import ApiResponse
-from xata.namespace import Namespace
 
 
-class Migrations(Namespace):
+class Migrations(ApiRequest):
 
     scope = "workspace"
 
     def get_history(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Get branch migration history [deprecated]
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/migrations#get-branch-migration-history-[deprecated]
         Path: /db/{db_branch_name}/migrations
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -57,14 +58,15 @@
         headers = {"content-type": "application/json"}
         return self.request("GET", url_path, headers, payload)
 
     def get_plan(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Compute a migration plan from a target schema the branch should be migrated too.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/migrations/plan#compute-migration-plan-[deprecated]
         Path: /db/{db_branch_name}/migrations/plan
         Method: POST
         Response status codes:
         - 200: Example response
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -82,14 +84,15 @@
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def execute_plan(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Apply a migration plan to the branch
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/migrations/execute#migrate-branch-[deprecated]
         Path: /db/{db_branch_name}/migrations/execute
         Method: POST
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -107,14 +110,15 @@
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def get_schema_history(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Query schema history.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/schema/history#query-schema-history.
         Path: /db/{db_branch_name}/schema/history
         Method: POST
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -135,14 +139,15 @@
 
     def compare_branch_with_user_schema(
         self, payload: dict, db_name: str = None, branch_name: str = None
     ) -> ApiResponse:
         """
         Compare branch with user schema.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/schema/compare#compare-branch-with-user-schema.
         Path: /db/{db_branch_name}/schema/compare
         Method: POST
         Response status codes:
         - 200: Schema comparison response.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -160,14 +165,15 @@
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def compare_schemas(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Compare branch schemas.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/schema/compare/branch_name#compare-branch-schemas.
         Path: /db/{db_branch_name}/schema/compare/{branch_name}
         Method: POST
         Response status codes:
         - 200: Schema comparison response.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -185,14 +191,15 @@
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def upadte_schema(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Update Branch schema
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/schema/update#update-branch-schema
         Path: /db/{db_branch_name}/schema/update
         Method: POST
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -210,14 +217,15 @@
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def preview(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Preview branch schema edits.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/schema/preview#preview-branch-schema-edits.
         Path: /db/{db_branch_name}/schema/preview
         Method: POST
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -236,14 +244,15 @@
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def apply(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Apply edit script.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/schema/apply#apply-edit-script.
         Path: /db/{db_branch_name}/schema/apply
         Method: POST
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -267,14 +276,15 @@
         list of applicable migrations can be fetched using the `schema/history` API from another
         branch or database.  The most recent migration must be part of the list or referenced (via
         `parentID`) by the first migration in the list of migrations to be pushed.  Each migration
         in the list has an `id`, `parentID`, and `checksum`. The checksum for migrations are
         generated and verified by xata.  The operation fails if any migration in the list has an
         invalid checksum.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/schema/push#push-migrations.
         Path: /db/{db_branch_name}/schema/push
         Method: POST
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
```

### Comparing `xata-1.0.0a3/xata/api/records.py` & `xata-1.0.0a4/xata/api/records.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,33 +19,35 @@
 
 # ------------------------------------------------------- #
 # Records
 # Record access API.
 # Specification: workspace:v1.0
 # ------------------------------------------------------- #
 
+from xata.api_request import ApiRequest
 from xata.api_response import ApiResponse
-from xata.namespace import Namespace
 
 
-class Records(Namespace):
+class Records(ApiRequest):
 
     scope = "workspace"
 
     def transaction(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Execute a transaction on a branch
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/transaction#execute-a-transaction-on-a-branch
         Path: /db/{db_branch_name}/transaction
         Method: POST
         Response status codes:
         - 200: Returns the results of a successful transaction.
         - 400: Returns errors from a failed transaction.
         - 401: Authentication Error
         - 404: Example response
+        - 429: Rate limit exceeded
         - 5XX: Unexpected Error
         - default: Unexpected Error
         Response: application/json
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
@@ -59,14 +61,15 @@
 
     def insert(
         self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None, columns: list = None
     ) -> ApiResponse:
         """
         Insert a new Record into the Table
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/data#insert-record
         Path: /db/{db_branch_name}/tables/{table_name}/data
         Method: POST
         Response status codes:
         - 201: Record ID and metadata
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -90,14 +93,15 @@
 
     def get(
         self, table_name: str, record_id: str, db_name: str = None, branch_name: str = None, columns: list = None
     ) -> ApiResponse:
         """
         Retrieve record by ID
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/data/record_id#get-record-by-id
         Path: /db/{db_branch_name}/tables/{table_name}/data/{record_id}
         Method: GET
         Response status codes:
         - 200: Table Record Reponse
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -130,14 +134,15 @@
         if_version: int = None,
     ) -> ApiResponse:
         """
         By default, IDs are auto-generated when data is insterted into Xata.  Sending a request to
         this endpoint allows us to insert a record with a pre-existing ID, bypassing the default
         automatic ID generation.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/data/record_id#insert-record-with-id
         Path: /db/{db_branch_name}/tables/{table_name}/data/{record_id}
         Method: PUT
         Response status codes:
         - 200: Record ID and metadata
         - 201: Record ID and metadata
         - 400: Bad Request
         - 401: Authentication Error
@@ -179,14 +184,15 @@
         branch_name: str = None,
         columns: list = None,
         if_version: int = None,
     ) -> ApiResponse:
         """
         Upsert record with ID
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/data/record_id#upsert-record-with-id
         Path: /db/{db_branch_name}/tables/{table_name}/data/{record_id}
         Method: POST
         Response status codes:
         - 200: Record ID and metadata
         - 201: Record ID and metadata
         - 400: Bad Request
         - 401: Authentication Error
@@ -218,14 +224,15 @@
 
     def delete(
         self, table_name: str, record_id: str, db_name: str = None, branch_name: str = None, columns: list = None
     ) -> ApiResponse:
         """
         Delete record from table
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/data/record_id#delete-record-from-table
         Path: /db/{db_branch_name}/tables/{table_name}/data/{record_id}
         Method: DELETE
         Response status codes:
         - 200: Table Record Reponse
         - 204: No Content
         - 400: Bad Request
         - 401: Authentication Error
@@ -255,14 +262,15 @@
         branch_name: str = None,
         columns: list = None,
         if_version: int = None,
     ) -> ApiResponse:
         """
         Update record with ID
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/data/record_id#update-record-with-id
         Path: /db/{db_branch_name}/tables/{table_name}/data/{record_id}
         Method: PATCH
         Response status codes:
         - 200: Record ID and metadata
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -293,16 +301,18 @@
 
     def bulk_insert(
         self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None, columns: list = None
     ) -> ApiResponse:
         """
         Bulk insert records
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/bulk#bulk-insert-records
         Path: /db/{db_branch_name}/tables/{table_name}/bulk
         Method: POST
+        Status: Experimental
         Response status codes:
         - 200: OK
         - 400: Response with multiple errors of the bulk execution
         - 401: Authentication Error
         - 404: Example response
         - 422: Example response
         - 5XX: Unexpected Error
```

### Comparing `xata-1.0.0a3/xata/api/search_and_filter.py` & `xata-1.0.0a4/xata/api/search_and_filter.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 
 # ------------------------------------------------------- #
 # SearchAndFilter
 # APIs for searching, querying, filtering, and aggregating records.
 # Specification: workspace:v1.0
 # ------------------------------------------------------- #
 
+from xata.api_request import ApiRequest
 from xata.api_response import ApiResponse
-from xata.namespace import Namespace
 
 
-class SearchAndFilter(Namespace):
+class SearchAndFilter(ApiRequest):
 
     scope = "workspace"
 
     def query(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         The Query Table API can be used to retrieve all records in a table.  The API support
         filtering, sorting, selecting a subset of columns, and pagination.  The overall structure
@@ -208,14 +208,15 @@
         can be more convenient at times as user code does not   need to remember the filter, sort,
         columns or page size configuration.  All   these information are read from the cursor.
         When using special cursors like `page.after="end"` or `page.before="end"`, we still allow
         `filter` and `sort` to be set.  Example of getting the last page:  ```json POST
         /db/demo:main/tables/table/query {   "page": {     "size": 10,     "before": "end"   } }
         ```
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/query#query-table
         Path: /db/{db_branch_name}/tables/{table_name}/query
         Method: POST
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -234,14 +235,15 @@
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def search_branch(self, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Run a free text search operation across the database branch.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/search#free-text-search
         Path: /db/{db_branch_name}/search
         Method: POST
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -265,14 +267,15 @@
         parameter that is used for the free text search and a set of structured filters (via the
         `filter` parameter) that are applied before the search.  The `filter` parameter uses the
         same syntax as the [query endpoint](/api-reference/db/db_branch_name/tables/table_name/)
         with the following exceptions: * filters `$contains`, `$startsWith`, `$endsWith` don't
         work on columns of type `text` * filtering on columns of type `multiple` is currently
         unsupported
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/search#free-text-search-in-a-table
         Path: /db/{db_branch_name}/tables/{table_name}/search
         Method: POST
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -295,14 +298,15 @@
     ) -> ApiResponse:
         """
         This endpoint can be used to perform vector-based similarity searches in a table.  It can
         be used for implementing semantic search and product recommendation.  To use this
         endpoint, you need a column of type vector.  The input vector must have the same dimension
         as the vector column.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/vectorSearch#vector-similarity-search-in-a-table
         Path: /db/{db_branch_name}/tables/{table_name}/vectorSearch
         Method: POST
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -319,83 +323,106 @@
         url_path = f"/db/{db_branch_name}/tables/{table_name}/vectorSearch"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def ask(
         self,
         table_name: str,
-        payload: dict,
+        question: str,
+        rules: list[str] = [],
+        options: dict = {},
+        streaming_results: bool = False,
         db_name: str = None,
         branch_name: str = None,
-        response_content_type: str = "application/json",
     ) -> ApiResponse:
         """
         Ask your table a question.  If the `Accept` header is set to `text/event-stream`, Xata
         will stream the results back as SSE's.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/ask#ask-your-table-a-question
         Path: /db/{db_branch_name}/tables/{table_name}/ask
         Method: POST
         Response status codes:
         - 200: Response to the question
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 429: Rate limit exceeded
-        - 503: Unexpected Error
+        - 503: ServiceUnavailable
         - 5XX: Unexpected Error
         Responses:
         - application/json
         - text/event-stream
 
         :param table_name: str The Table name
-        :param payload: dict content
+        :param question: str follow up question to ask
+        :param rules: list[str] specific rules you want to apply, default: []
+        :param options: dict more options to adjust the query, default: {}
+        :param streaming_results: bool get the results streamed, default: False
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
-        :param response_content_type: str = "application/json" Content type of the response. Default: application/json
 
         :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/ask"
+        payload = {
+            "question": question,
+        }
         headers = {
             "content-type": "application/json",
-            "accept": response_content_type,
+            "accept": "text/event-stream" if streaming_results else "application/json",
         }
         return self.request("POST", url_path, headers, payload)
 
-    def chat_session_message(
-        self, table_name: str, session_id: str, payload: dict, db_name: str = None, branch_name: str = None
+    def ask_follow_up(
+        self,
+        table_name: str,
+        session_id: str,
+        question: str,
+        streaming_results: bool = False,
+        db_name: str = None,
+        branch_name: str = None,
     ) -> ApiResponse:
         """
-        Ask a follow-up question.  If the `Accept` header is set to `text/event-stream`, Xata will
-        stream the results back as SSE's.
+        Ask a follow-up question.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/ask/session_id#continue-a-conversation-with-your-data
         Path: /db/{db_branch_name}/tables/{table_name}/ask/{session_id}
         Method: POST
         Response status codes:
         - 200: Response to the question
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 429: Rate limit exceeded
         - 503: ServiceUnavailable
         - 5XX: Unexpected Error
-        Response: application/json
+        Responses:
+        - application/json
+        - text/event-stream
 
         :param table_name: str The Table name
-        :param session_id: str
-        :param payload: dict content
+        :param session_id: str Session id from initial question
+        :param question: str follow up question to ask
+        :param streaming_results: bool get the results streamed, default: False
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/ask/{session_id}"
-        headers = {"content-type": "application/json"}
+        payload = {
+            "message": question,
+        }
+        headers = {
+            "content-type": "application/json",
+            "accept": "text/event-stream" if streaming_results else "application/json",
+        }
         return self.request("POST", url_path, headers, payload)
 
     def summarize(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         This endpoint allows you to (optionally) define groups, and then to run calculations on
         the values in each group.  This is most helpful when  you'd like to understand the data
         you have in your database.  A group is a combination of unique values.  If you create a
@@ -426,14 +453,15 @@
         of data being processed in order  to reduce impact on your limits.  `summariesFilter`:
         tells Xata how to filter the results of a summary.  It has the same syntax as `filter`,
         however, by using `summariesFilter` you may also filter on the results of a query.  note:
         This is a much slower to use than `filter`. We recommend using  `filter` wherever possible
         and `summariesFilter` when it's not  possible to use `filter`.  `page.size`: tells Xata
         how many records to return.  If unspecified, Xata will return the default size.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/summarize#summarize-table
         Path: /db/{db_branch_name}/tables/{table_name}/summarize
         Method: POST
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -457,14 +485,15 @@
         While the summary endpoint is served from a transactional store and the results are
         strongly  consistent, the aggregate endpoint is served from our columnar store and the
         results are  only eventually consistent.  On the other hand, the aggregate endpoint uses a
         store that is more appropiate for analytics, makes use of approximative algorithms  (e.g
         for cardinality), and is generally faster and can do more complex aggregations.  For
         usage, see the [API Guide](https://xata.io/docs/api-guide/aggregate).
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/aggregate#run-aggregations-over-a-table
         Path: /db/{db_branch_name}/tables/{table_name}/aggregate
         Method: POST
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
```

### Comparing `xata-1.0.0a3/xata/api/table.py` & `xata-1.0.0a4/xata/api/table.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,27 +19,28 @@
 
 # ------------------------------------------------------- #
 # Table
 # Table management.
 # Specification: workspace:v1.0
 # ------------------------------------------------------- #
 
+from xata.api_request import ApiRequest
 from xata.api_response import ApiResponse
-from xata.namespace import Namespace
 
 
-class Table(Namespace):
+class Table(ApiRequest):
 
     scope = "workspace"
 
     def create(self, table_name: str, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Creates a new table with the given name.  Returns 422 if a table with the same name
         already exists.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name#create-table
         Path: /db/{db_branch_name}/tables/{table_name}
         Method: PUT
         Response status codes:
         - 201: Created
         - 204: No Content
         - 400: Bad Request
         - 401: Authentication Error
@@ -59,14 +60,15 @@
         url_path = f"/db/{db_branch_name}/tables/{table_name}"
         return self.request("PUT", url_path)
 
     def delete(self, table_name: str, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Deletes the table with the given name.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name#delete-table
         Path: /db/{db_branch_name}/tables/{table_name}
         Method: DELETE
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Not Found
@@ -86,14 +88,15 @@
 
     def update(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Update table.  Currently there is only one update operation supported: renaming the table
         by providing a new name.  In the example below, we rename a table from “users” to
         “people”:  ```json // PATCH /db/test:main/tables/users  {   "name": "people" } ```
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name#update-table
         Path: /db/{db_branch_name}/tables/{table_name}
         Method: PATCH
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -113,14 +116,15 @@
         headers = {"content-type": "application/json"}
         return self.request("PATCH", url_path, headers, payload)
 
     def get_schema(self, table_name: str, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Get table schema
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/schema#get-table-schema
         Path: /db/{db_branch_name}/tables/{table_name}/schema
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -138,14 +142,15 @@
         url_path = f"/db/{db_branch_name}/tables/{table_name}/schema"
         return self.request("GET", url_path)
 
     def set_schema(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Update table schema
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/schema#update-table-schema
         Path: /db/{db_branch_name}/tables/{table_name}/schema
         Method: PUT
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 204: No Content
         - 400: Bad Request
         - 401: Authentication Error
@@ -168,14 +173,15 @@
 
     def get_columns(self, table_name: str, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Retrieves the list of table columns and their definition.  This endpoint returns the
         column list with object columns being reported with their full dot-separated path
         (flattened).
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/columns#list-table-columns
         Path: /db/{db_branch_name}/tables/{table_name}/columns
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -194,14 +200,15 @@
         return self.request("GET", url_path)
 
     def add_column(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         Adds a new column to the table.  The body of the request should contain the column
         definition.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/columns#create-new-column
         Path: /db/{db_branch_name}/tables/{table_name}/columns
         Method: POST
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -222,14 +229,15 @@
 
     def get_column(
         self, table_name: str, column_name: str, db_name: str = None, branch_name: str = None
     ) -> ApiResponse:
         """
         Get the definition of a single column.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/columns/column_name#get-column-information
         Path: /db/{db_branch_name}/tables/{table_name}/columns/{column_name}
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -250,14 +258,15 @@
 
     def delete_column(
         self, table_name: str, column_name: str, db_name: str = None, branch_name: str = None
     ) -> ApiResponse:
         """
         Deletes the specified column.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/columns/column_name#delete-column
         Path: /db/{db_branch_name}/tables/{table_name}/columns/{column_name}
         Method: DELETE
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -278,14 +287,15 @@
     def update_column(
         self, table_name: str, column_name: str, payload: dict, db_name: str = None, branch_name: str = None
     ) -> ApiResponse:
         """
         Update column with partial data.  Can be used for renaming the column by providing a new
         "name" field.
 
+        Reference: https://xata.io/docs/api-reference/db/db_branch_name/tables/table_name/columns/column_name#update-column
         Path: /db/{db_branch_name}/tables/{table_name}/columns/{column_name}
         Method: PATCH
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
```

### Comparing `xata-1.0.0a3/xata/api/users.py` & `xata-1.0.0a4/xata/api/authentication.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,80 +14,83 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 
 # ------------------------------------------------------- #
-# Users
-# Users management
+# Authentication
+# Authentication and API Key management.
 # Specification: core:v1.0
 # ------------------------------------------------------- #
 
+from xata.api_request import ApiRequest
 from xata.api_response import ApiResponse
-from xata.namespace import Namespace
 
 
-class Users(Namespace):
+class Authentication(ApiRequest):
 
     scope = "core"
 
-    def get(self) -> ApiResponse:
+    def get_user_api_keys(self) -> ApiResponse:
         """
-        Return details of the user making the request
+        Retrieve a list of existing user API keys
 
-        Path: /user
+        Reference: https://xata.io/docs/api-reference/user/keys#get-the-list-of-user-api-keys
+        Path: /user/keys
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
 
         :returns ApiResponse
         """
-        url_path = "/user"
+        url_path = "/user/keys"
         return self.request("GET", url_path)
 
-    def update(self, payload: dict) -> ApiResponse:
+    def create_user_api_keys(self, key_name: str) -> ApiResponse:
         """
-        Update user info
+        Create and return new API key
 
-        Path: /user
-        Method: PUT
+        Reference: https://xata.io/docs/api-reference/user/keys/key_name#create-and-return-new-api-key
+        Path: /user/keys/{key_name}
+        Method: POST
         Response status codes:
-        - 200: OK
+        - 201: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
-        :param payload: dict content
+        :param key_name: str API Key name
 
         :returns ApiResponse
         """
-        url_path = "/user"
-        headers = {"content-type": "application/json"}
-        return self.request("PUT", url_path, headers, payload)
+        url_path = f"/user/keys/{key_name}"
+        return self.request("POST", url_path)
 
-    def delete(self) -> ApiResponse:
+    def delete_user_api_keys(self, key_name: str) -> ApiResponse:
         """
-        Delete the user making the request
+        Delete an existing API key
 
-        Path: /user
+        Reference: https://xata.io/docs/api-reference/user/keys/key_name#delete-an-existing-api-key
+        Path: /user/keys/{key_name}
         Method: DELETE
         Response status codes:
         - 204: No Content
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
 
+        :param key_name: str API Key name
 
         :returns ApiResponse
         """
-        url_path = "/user"
+        url_path = f"/user/keys/{key_name}"
         return self.request("DELETE", url_path)
```

### Comparing `xata-1.0.0a3/xata/api/workspaces.py` & `xata-1.0.0a4/xata/api/workspaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,26 +19,27 @@
 
 # ------------------------------------------------------- #
 # Workspaces
 # Workspaces management
 # Specification: core:v1.0
 # ------------------------------------------------------- #
 
+from xata.api_request import ApiRequest
 from xata.api_response import ApiResponse
-from xata.namespace import Namespace
 
 
-class Workspaces(Namespace):
+class Workspaces(ApiRequest):
 
     scope = "core"
 
     def list(self) -> ApiResponse:
         """
         Retrieve the list of workspaces the user belongs to
 
+        Reference: https://xata.io/docs/api-reference/workspaces#get-list-of-workspaces
         Path: /workspaces
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
@@ -77,14 +78,15 @@
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def get(self, workspace_id: str = None) -> ApiResponse:
         """
         Retrieve workspace info from a workspace ID
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id#get-an-existing-workspace
         Path: /workspaces/{workspace_id}
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 403: Authentication Error
@@ -101,14 +103,15 @@
         url_path = f"/workspaces/{workspace_id}"
         return self.request("GET", url_path)
 
     def update(self, payload: dict, workspace_id: str = None) -> ApiResponse:
         """
         Update workspace info
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id#update-an-existing-workspace
         Path: /workspaces/{workspace_id}
         Method: PUT
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 403: Authentication Error
@@ -127,14 +130,15 @@
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
     def delete(self, workspace_id: str = None) -> ApiResponse:
         """
         Delete the workspace with the provided ID
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id#delete-an-existing-workspace
         Path: /workspaces/{workspace_id}
         Method: DELETE
         Response status codes:
         - 204: No Content
         - 400: Bad Request
         - 401: Authentication Error
         - 403: Authentication Error
@@ -150,14 +154,15 @@
         url_path = f"/workspaces/{workspace_id}"
         return self.request("DELETE", url_path)
 
     def get_members(self, workspace_id: str = None) -> ApiResponse:
         """
         Retrieve the list of members of the given workspace
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id/members#get-the-list-members-of-a-workspace
         Path: /workspaces/{workspace_id}/members
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 403: Authentication Error
@@ -175,14 +180,15 @@
         return self.request("GET", url_path)
 
     def update_member(self, user_id: str, payload: dict, workspace_id: str = None) -> ApiResponse:
         """
         Update a workspace member role.  Workspaces must always have at least one owner, so this
         operation will fail if trying to remove owner role from the last owner in the workspace.
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id/members/user_id#update-workspace-member-role
         Path: /workspaces/{workspace_id}/members/{user_id}
         Method: PUT
         Response status codes:
         - 204: No Content
         - 400: Bad Request
         - 401: Authentication Error
         - 403: Authentication Error
@@ -201,14 +207,15 @@
         headers = {"content-type": "application/json"}
         return self.request("PUT", url_path, headers, payload)
 
     def remove_member(self, user_id: str, workspace_id: str = None) -> ApiResponse:
         """
         Remove the member from the workspace
 
+        Reference: https://xata.io/docs/api-reference/workspaces/workspace_id/members/user_id#remove-a-member-from-the-workspace
         Path: /workspaces/{workspace_id}/members/{user_id}
         Method: DELETE
         Response status codes:
         - 204: No Content
         - 400: Bad Request
         - 401: Authentication Error
         - 403: Authentication Error
```

### Comparing `xata-1.0.0a3/xata/api_response.py` & `xata-1.0.0a4/xata/api_response.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a3/xata/client.py` & `xata-1.0.0a4/xata/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from .api.search_and_filter import SearchAndFilter
 from .api.table import Table
 from .api.users import Users
 from .api.workspaces import Workspaces
 
 # TODO this is a manual task, to keep in sync with pyproject.toml
 # could/should be automated to keep in sync
-__version__ = "1.0.0a3"
+__version__ = "1.0.0a4"
 
 PERSONAL_API_KEY_LOCATION = "~/.config/xata/key"
 DEFAULT_DATA_PLANE_DOMAIN = "xata.sh"
 DEFAULT_CONTROL_PLANE_DOMAIN = "api.xata.io"
 DEFAULT_REGION = "us-east-1"
 DEFAULT_BRANCH_NAME = "main"
 CONFIG_LOCATION = ".xatarc"
@@ -119,14 +119,15 @@
         self.domain_core = domain_core
         self.domain_workspace = domain_workspace
 
         # init default headers
         self.headers = {
             "authorization": f"Bearer {self.api_key}",
             "user-agent": f"xataio/xata-py:{__version__}",
+            "connection": "keep-alive",
             "x-xata-client-id": str(uuid.uuid4()),
             "x-xata-session-id": str(uuid.uuid4()),
             "x-xata-agent": f"client=PY_SDK;version={__version__};",
         }
 
         # init namespaces
         self._authentication = Authentication(self)
@@ -315,84 +316,77 @@
             # branch defined and not empty, return it!
             return host_parts[0], host_parts[1], db_branch_parts[0], db_branch_parts[1], domain
         # does not have a branch defined
         return host_parts[0], host_parts[1], db_branch_parts[0], DEFAULT_BRANCH_NAME, domain
 
     def authentication(self) -> Authentication:
         """
-        Authentication Namespace
         :returns Authentication
         """
         return self._authentication
 
     def databases(self) -> Databases:
         """
-        Databases Namespace
         :returns Databases
         """
         return self._databases
 
     def invites(self) -> Invites:
         """
-        Invites Namespace
         :returns Invites
         """
         return self._invites
 
     def users(self) -> Users:
         """
-        Users Namespace
         :returns Users
         """
         return self._users
 
     def workspaces(self) -> Workspaces:
         """
-        Workspaces Namespace
         :returns Workspaces
         """
         return self._workspaces
 
     def branch(self) -> Branch:
         """
-        Branch Namespace
         :returns Branch
         """
         return self._branch
 
     def migrations(self) -> Migrations:
         """
-        Migrations Namespace
         :returns Migrations
         """
         return self._migrations
 
     def records(self) -> Records:
         """
-        Records Namespace
         :returns Records
         """
         return self._records
 
     def search_and_filter(self) -> SearchAndFilter:
         """
-        Search_and_Filter Namespace
         :returns Search_and_filter
         """
         return self._search_and_filter
 
     def data(self) -> SearchAndFilter:
         """
         Shorter alias for Search_and_Filter
         :returns Search_and_filter
         """
         return self._search_and_filter
 
     def table(self) -> Table:
         """
-        Table Namespace
         :returns Table
         """
         return self._table
 
     def files(self) -> Files:
+        """
+        :returns Files
+        """
         return self._files
```

### Comparing `xata-1.0.0a3/xata/errors.py` & `xata-1.0.0a4/xata/errors.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a3/xata/helpers.py` & `xata-1.0.0a4/xata/helpers.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a3/xata/namespace.py` & `xata-1.0.0a4/xata/api_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 from requests import request
 
 from xata.api_response import ApiResponse
 
 from .errors import RateLimitError, UnauthorizedError, XataServerError
 
 
-class Namespace:
+class ApiRequest:
     """
-    Parent class for Namespaces
+    Parent class for API requests
     """
 
     def __init__(self, client):
         self.client = client
         self.logger = logging.getLogger(self.__class__.__name__)
 
     def get_scope(self) -> str:
```

### Comparing `xata-1.0.0a3/PKG-INFO` & `xata-1.0.0a4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xata
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Python client for Xata.io
 License: Apache-2.0
 Author: Xata
 Author-email: support@xata.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -15,16 +15,19 @@
 Requires-Dist: orjson (>=3.8.1,<4.0.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Documentation, https://xata-py.readthedocs.io
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <img width="200" src="https://raw.githubusercontent.com/xataio/company/main/logo/non-resizable/for-light-backgrounds/colored-with-text.png#gh-light-mode-only" />
-  <img width="200" src="https://raw.githubusercontent.com/xataio/company/main/logo/non-resizable/for-dark-backgrounds/colored-with-text.png#gh-dark-mode-only" />
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="./assets/logo_dark.svg">
+    <source media="(prefers-color-scheme: light)" srcset="./assets/logo_light.svg">
+    <img width="400" alt="Xata" src="./assets/logo_dark.svg">
+  </picture>
 </p>
 
 # Python SDK for Xata
 
 [![Documentation Status](https://readthedocs.org/projects/xata-py/badge/?version=latest)](https://xata-py.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/xata.svg)](https://badge.fury.io/py/xata)
 
 Simple Python client for xata.io databases. Currently work in progress.
```

