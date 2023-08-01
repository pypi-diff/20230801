# Comparing `tmp/cloudimg-1.6.2.tar.gz` & `tmp/cloudimg-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudimg-1.6.2.tar", last modified: Wed May 24 22:09:11 2023, max compression
+gzip compressed data, was "cloudimg-1.7.0.tar", last modified: Tue Aug  1 03:02:36 2023, max compression
```

## Comparing `cloudimg-1.6.2.tar` & `cloudimg-1.7.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:11.139413 cloudimg-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-24 22:08:56.000000 cloudimg-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-24 22:08:56.000000 cloudimg-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 22:09:11.139413 cloudimg-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-24 22:08:56.000000 cloudimg-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:11.139413 cloudimg-1.6.2/cloudimg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:08:56.000000 cloudimg-1.6.2/cloudimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25686 2023-05-24 22:08:56.000000 cloudimg-1.6.2/cloudimg/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-24 22:08:56.000000 cloudimg-1.6.2/cloudimg/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    19465 2023-05-24 22:08:56.000000 cloudimg-1.6.2/cloudimg/ms_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:11.139413 cloudimg-1.6.2/cloudimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 22:09:10.000000 cloudimg-1.6.2/cloudimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-24 22:09:11.000000 cloudimg-1.6.2/cloudimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:09:10.000000 cloudimg-1.6.2/cloudimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-24 22:09:10.000000 cloudimg-1.6.2/cloudimg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 22:09:10.000000 cloudimg-1.6.2/cloudimg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-24 22:08:56.000000 cloudimg-1.6.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-24 22:08:56.000000 cloudimg-1.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 22:09:11.139413 cloudimg-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-24 22:08:56.000000 cloudimg-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:11.139413 cloudimg-1.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    35840 2023-05-24 22:08:56.000000 cloudimg-1.6.2/tests/test_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    25204 2023-05-24 22:08:56.000000 cloudimg-1.6.2/tests/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-24 22:08:56.000000 cloudimg-1.6.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:02:36.557578 cloudimg-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-01 03:02:21.000000 cloudimg-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-01 03:02:21.000000 cloudimg-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-01 03:02:36.557578 cloudimg-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-01 03:02:21.000000 cloudimg-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:02:36.553578 cloudimg-1.7.0/cloudimg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 03:02:21.000000 cloudimg-1.7.0/cloudimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25686 2023-08-01 03:02:21.000000 cloudimg-1.7.0/cloudimg/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-08-01 03:02:21.000000 cloudimg-1.7.0/cloudimg/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21006 2023-08-01 03:02:21.000000 cloudimg-1.7.0/cloudimg/ms_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:02:36.557578 cloudimg-1.7.0/cloudimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-01 03:02:36.000000 cloudimg-1.7.0/cloudimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-01 03:02:36.000000 cloudimg-1.7.0/cloudimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 03:02:36.000000 cloudimg-1.7.0/cloudimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-01 03:02:36.000000 cloudimg-1.7.0/cloudimg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 03:02:36.000000 cloudimg-1.7.0/cloudimg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-01 03:02:21.000000 cloudimg-1.7.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-01 03:02:21.000000 cloudimg-1.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 03:02:36.557578 cloudimg-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-01 03:02:21.000000 cloudimg-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:02:36.557578 cloudimg-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    35840 2023-08-01 03:02:21.000000 cloudimg-1.7.0/tests/test_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27301 2023-08-01 03:02:21.000000 cloudimg-1.7.0/tests/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-01 03:02:21.000000 cloudimg-1.7.0/tox.ini
```

### Comparing `cloudimg-1.6.2/LICENSE` & `cloudimg-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudimg-1.6.2/PKG-INFO` & `cloudimg-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cloudimg
-Version: 1.6.2
+Version: 1.7.0
 Summary: Services for building and releasing products in cloud environments
 Home-page: https://github.com/release-engineering/cloudimg
 Author: Alex Misstear
 Author-email: amisstea@redhat.com
 License: GPLv3
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `cloudimg-1.6.2/README.md` & `cloudimg-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudimg-1.6.2/cloudimg/aws.py` & `cloudimg-1.7.0/cloudimg/aws.py`

 * *Files identical despite different names*

### Comparing `cloudimg-1.6.2/cloudimg/common.py` & `cloudimg-1.7.0/cloudimg/common.py`

 * *Files identical despite different names*

### Comparing `cloudimg-1.6.2/cloudimg/ms_azure.py` & `cloudimg-1.7.0/cloudimg/ms_azure.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     BlobSasPermissions,
     BlobType,
     generate_account_sas,
     generate_blob_sas,
     ResourceTypes,
 )
 
-from cloudimg.common import BaseService, PublishingMetadata
+from cloudimg.common import BaseService, DeleteMetadata, PublishingMetadata
 
 log = logging.getLogger(__name__)
 
 
 class BlobNotFoundError(Exception):
     """
     Raised when a required Blob is missing.
@@ -121,14 +121,28 @@
     def __init__(self, *args, **kwargs):
         super(AzurePublishingMetadata, self).__init__(*args, **kwargs)
 
         assert self.container, 'A container must be defined'
         assert self.tags, 'A tag must be defined'
 
 
+class AzureDeleteMetadata(DeleteMetadata):
+    """The required information to delete a blob on Azure."""
+
+    def __init__(self, container, *args, **kwargs):
+        # Set the image NAME as the ID for Azure as both are redundant
+        # for this marketplace.
+        if not kwargs.get("image_name"):
+            kwargs.update({"image_name": kwargs.get("image_id")})
+
+        super(AzureDeleteMetadata, self).__init__(*args, **kwargs)
+
+        self.container = container
+
+
 class AzureService(BaseService):
     """
     Azure cloud provider service.
     It's expected to be instantiated through one of its factories.
 
     Args:
         blob_service_client (BlobServiceClient): The blob service client to
@@ -554,7 +568,37 @@
                       blob_props.container,
                       blob_props.name
                   )
             log.error(err)
             raise BlobNotFoundError(err)
 
         return blob.set_blob_tags(tags)
+
+    def delete(self, metadata):
+        """
+        Delete VHD images for given metadata.
+
+        Args:
+            metadata(AzureDeleteMetadata): Metadata about the image
+
+        Returns:
+            tuple (image_name[Str], image_path[Str]) of removed objects.
+        """
+        image_name = metadata.image_name
+
+        log.info('Searching for image: %s', image_name)
+        blob = self.get_object_by_name(
+            container=metadata.container,
+            name=image_name
+        )
+
+        if not blob:
+            log.info('Image does not exist: %s', image_name)
+            return None, None
+
+        image_path = "%s/%s" % (blob.container_name, blob.blob_name)
+        log.info("Deleting the image from %s", image_path)
+        # https://learn.microsoft.com/en-us/python/api/azure-storage-blob/azure.storage.blob.blobclient?view=azure-python#azure-storage-blob-blobclient-delete-blob
+        blob.delete_blob(delete_snapshots="include")
+
+        log.info("Deleted the image from %s", image_path)
+        return image_name, image_path
```

### Comparing `cloudimg-1.6.2/cloudimg.egg-info/PKG-INFO` & `cloudimg-1.7.0/cloudimg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cloudimg
-Version: 1.6.2
+Version: 1.7.0
 Summary: Services for building and releasing products in cloud environments
 Home-page: https://github.com/release-engineering/cloudimg
 Author: Alex Misstear
 Author-email: amisstea@redhat.com
 License: GPLv3
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `cloudimg-1.6.2/setup.py` & `cloudimg-1.7.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cloudimg',
-    version='1.6.2',
+    version='1.7.0',
     author='Alex Misstear',
     author_email='amisstea@redhat.com',
     description=('Services for building and releasing products in cloud '
                  'environments'),
     license='GPLv3',
     url='https://github.com/release-engineering/cloudimg',
     packages=find_packages(),
```

### Comparing `cloudimg-1.6.2/tests/test_aws.py` & `cloudimg-1.7.0/tests/test_aws.py`

 * *Files identical despite different names*

### Comparing `cloudimg-1.6.2/tests/test_azure.py` & `cloudimg-1.7.0/tests/test_azure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from tempfile import NamedTemporaryFile
 import unittest
 
 from unittest.mock import MagicMock, patch, call, ANY
 
 from cloudimg.ms_azure import (
+    AzureDeleteMetadata,
     AzurePublishingMetadata,
     AzureService,
     BlobNotFoundError,
     BlobServiceClient,
     BlobType,
     UploadProgress,
 )
@@ -641,10 +642,70 @@
                           tags=tags)
 
         mock_get_obj.assert_called_once_with(
             container='foo',
             name='bar',
         )
 
+    @patch("cloudimg.ms_azure.AzureService.get_object_by_name")
+    def test_delete_image_exists(self, mock_get_obj):
+        image_name = "fake_image_name"
+        container_name = "fake_container_name"
+        mock_blob = MagicMock()
+        mock_blob.container_name = container_name
+        mock_blob.blob_name = image_name
+        mock_get_obj.return_value = mock_blob
+
+        delete_meta = AzureDeleteMetadata(
+            image_id=image_name,
+            container=container_name,
+        )
+
+        # run delete
+        deleted_img_name, deleted_img_path = self.svc.delete(delete_meta)
+
+        # Ensure the metadata's `image_name` and `image_id` are the same
+        assert delete_meta.image_id == delete_meta.image_name
+
+        # Ensure the calls were properly made
+        mock_get_obj.assert_called_once_with(
+            container=container_name,
+            name=image_name,
+        )
+        mock_blob.delete_blob.assert_called_once_with(
+            delete_snapshots="include",
+        )
+
+        # Ensure the return is the expected ones
+        assert deleted_img_name == image_name
+        assert deleted_img_path == "%s/%s" % (container_name, image_name)
+
+    @patch("cloudimg.ms_azure.AzureService.get_object_by_name")
+    def test_delete_image_missing(self, mock_get_obj):
+        image_name = "fake_image_name"
+        container_name = "fake_container_name"
+        mock_get_obj.return_value = None
+
+        delete_meta = AzureDeleteMetadata(
+            image_id=image_name,
+            container=container_name,
+        )
+
+        # run delete
+        deleted_img_name, deleted_img_path = self.svc.delete(delete_meta)
+
+        # Ensure the metadata's `image_name` and `image_id` are the same
+        assert delete_meta.image_id == delete_meta.image_name
+
+        # Ensure the calls were properly made
+        mock_get_obj.assert_called_once_with(
+            container=container_name,
+            name=image_name,
+        )
+
+        # Ensure the return is the expected ones
+        assert not deleted_img_name
+        assert not deleted_img_path
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cloudimg-1.6.2/tox.ini` & `cloudimg-1.7.0/tox.ini`

 * *Files identical despite different names*

