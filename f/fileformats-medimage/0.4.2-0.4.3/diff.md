# Comparing `tmp/fileformats_medimage-0.4.2.tar.gz` & `tmp/fileformats_medimage-0.4.3.tar.gz`

## Comparing `fileformats_medimage-0.4.2.tar` & `fileformats_medimage-0.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/.codespell-ignorewords
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/.coveragerc
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/.flake8
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/conftest.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/pytest.ini
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/fileformats/medimage/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/fileformats/medimage/_version.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/fileformats/medimage/base.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/fileformats/medimage/dicom.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/fileformats/medimage/diffusion.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/fileformats/medimage/misc.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/fileformats/medimage/mrtrix3.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/fileformats/medimage/nifti.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/fileformats/medimage/raw.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/fileformats/medimage/tests/test_dicom.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/fileformats/medimage/tests/test_nifti.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/LICENSE
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/README.rst
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    18977 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/.codespell-ignorewords
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/.coveragerc
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/.flake8
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/conftest.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/pytest.ini
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/fileformats/medimage/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/fileformats/medimage/_version.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/fileformats/medimage/base.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/fileformats/medimage/dicom.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/fileformats/medimage/diffusion.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/fileformats/medimage/misc.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/fileformats/medimage/mrtrix3.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/fileformats/medimage/nifti.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/fileformats/medimage/raw.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/fileformats/medimage/tests/test_dicom.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/fileformats/medimage/tests/test_nifti.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/README.rst
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    18977 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.3/PKG-INFO
```

### Comparing `fileformats_medimage-0.4.2/.pre-commit-config.yaml` & `fileformats_medimage-0.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.2/conftest.py` & `fileformats_medimage-0.4.3/conftest.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.2/.github/workflows/publish.yml` & `fileformats_medimage-0.4.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.2/.github/workflows/tests.yml` & `fileformats_medimage-0.4.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.2/fileformats/medimage/__init__.py` & `fileformats_medimage-0.4.3/fileformats/medimage/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ._version import __version__
 from .base import MedicalImage
+from fileformats.misc import Dicom  # imported to alias it here as well
 from .misc import (  # noqa: F401
     Analyze,
 )
 from .nifti import (
     Nifti,
     Nifti1,
     Nifti2,
@@ -12,14 +13,15 @@
     NiftiGzX,
 )
 from .mrtrix3 import MrtrixImage, MrtrixImageHeader
 from .diffusion import (
     DwiEncoding,
     MrtrixTrack,
     Bvec,
+    Bval,
     Bfile,
     NiftiBvec,
     NiftiGzBvec,
     NiftiXBvec,
     NiftiGzXBvec,
     NiftiB,
     NiftiGzB,
```

### Comparing `fileformats_medimage-0.4.2/fileformats/medimage/base.py` & `fileformats_medimage-0.4.3/fileformats/medimage/base.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.2/fileformats/medimage/dicom.py` & `fileformats_medimage-0.4.3/fileformats/medimage/dicom.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.2/fileformats/medimage/diffusion.py` & `fileformats_medimage-0.4.3/fileformats/medimage/diffusion.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.2/fileformats/medimage/mrtrix3.py` & `fileformats_medimage-0.4.3/fileformats/medimage/mrtrix3.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from pathlib import Path
 from fileformats.core import mark
 from fileformats.generic import File
 from fileformats.core.mixin import WithMagicNumber
-from fileformats.numeric import DataFile
 from fileformats.core.exceptions import FormatMismatchError
 from .misc import MedicalImage
 
 
 class BaseMrtrixImage(WithMagicNumber, MedicalImage, File):
 
     magic_number = b"mrtrix image\n"
@@ -86,14 +85,19 @@
 class MrtrixImageHeader(BaseMrtrixImage):
 
     ext = ".mih"
 
     @mark.required
     @property
     def data_file(self):
-        return DataFile(self.data_fspath)
+        return MrtrixDataFile(self.data_fspath)
 
     def __attrs_post_init__(self):
         if len(self.fspaths) == 1:
             # add in data file if only header file is provided
             self.fspaths |= set([BaseMrtrixImage(self.fspath).data_fspath])
         super().__attrs_post_init__()
+
+
+class MrtrixDataFile(BaseMrtrixImage):
+
+    ext = ".dat"
```

### Comparing `fileformats_medimage-0.4.2/fileformats/medimage/nifti.py` & `fileformats_medimage-0.4.3/fileformats/medimage/nifti.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.2/fileformats/medimage/raw.py` & `fileformats_medimage-0.4.3/fileformats/medimage/raw.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.2/LICENSE` & `fileformats_medimage-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.2/README.rst` & `fileformats_medimage-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.2/pyproject.toml` & `fileformats_medimage-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.2/PKG-INFO` & `fileformats_medimage-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats-medimage
-Version: 0.4.2
+Version: 0.4.3
 Summary: Classes for representing various medical imaging file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats-medimage
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

