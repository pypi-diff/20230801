# Comparing `tmp/fileformats_medimage_extras-0.1.1.tar.gz` & `tmp/fileformats_medimage_extras-0.1.2.tar.gz`

## Comparing `fileformats_medimage_extras-0.1.1.tar` & `fileformats_medimage_extras-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/.codespell-ignorewords
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/.flake8
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/conftest.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/pytest.ini
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/_version.py
--rw-r--r--   0        0        0     6922 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/converters.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/dicom.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/diffusion.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/mrtrix3.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/nifti.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/tests/test_neuro_converters.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/LICENSE
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/README.rst
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    18991 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/.codespell-ignorewords
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/.flake8
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/conftest.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/pytest.ini
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/_version.py
+-rw-r--r--   0        0        0     6922 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/converters.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/dicom.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/diffusion.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/mrtrix3.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/nifti.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/tests/test_neuro_converters.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/README.rst
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    18991 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/PKG-INFO
```

### Comparing `fileformats_medimage_extras-0.1.1/.pre-commit-config.yaml` & `fileformats_medimage_extras-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.1/conftest.py` & `fileformats_medimage_extras-0.1.2/conftest.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.1/.github/workflows/publish.yml` & `fileformats_medimage_extras-0.1.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.1/.github/workflows/tests.yml` & `fileformats_medimage_extras-0.1.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/converters.py` & `fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/dicom.py` & `fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/dicom.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,19 +42,19 @@
 
 
 @DicomCollection.series_number.register
 def dicom_series_number(collection: DicomCollection):
     return int(collection.read_metadata(specific_tags=[SERIES_NUMBER_TAG])[0])
 
 
-@FileSet.generate_test_data.register
-def dicom_dir_generate_test_data(dcmdir: DicomDir, dest_dir: Path):
+@FileSet.generate_sample_data.register
+def dicom_dir_generate_sample_data(dcmdir: DicomDir, dest_dir: Path):
     return medimages4tests.dummy.dicom.mri.t1w.siemens.skyra.syngo_d13c.get_image(dest_dir / "dicom_dir")
 
 
-@FileSet.generate_test_data.register
-def dicom_set_generate_test_data(dcmdir: DicomSet, dest_dir: Path):
-    dicom_dir = dicom_dir_generate_test_data(dest_dir)
+@FileSet.generate_sample_data.register
+def dicom_set_generate_sample_data(dcmdir: DicomSet, dest_dir: Path):
+    dicom_dir = dicom_dir_generate_sample_data(dest_dir)
     return list(dicom_dir.iterdir())
 
 
 SERIES_NUMBER_TAG = ("0020", "0011")
```

### Comparing `fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/diffusion.py` & `fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/diffusion.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/nifti.py` & `fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/nifti.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,28 +23,28 @@
 
 @MedicalImage.dims.register
 def nifti_dims(nifti: Nifti):
     # FIXME: This won't work for 4-D files
     return nifti.metadata["dim"][1:4]
 
 
-@FileSet.generate_test_data.register
-def nifti_generate_test_data(nifti: Nifti1, dest_dir: Path):
+@FileSet.generate_sample_data.register
+def nifti_generate_sample_data(nifti: Nifti1, dest_dir: Path):
     return medimages4tests.dummy.nifti.get_image(out_file=dest_dir / "nifti.nii")
 
 
-@FileSet.generate_test_data.register
-def nifti_gz_generate_test_data(nifti: NiftiGz, dest_dir: Path):
+@FileSet.generate_sample_data.register
+def nifti_gz_generate_sample_data(nifti: NiftiGz, dest_dir: Path):
     return medimages4tests.dummy.nifti.get_image(
         out_file=dest_dir / "nifti.nii.gz", compressed=True
     )
 
 
-@FileSet.generate_test_data.register
-def nifti_gz_x_generate_test_data(nifti: NiftiGzX, dest_dir: Path):
+@FileSet.generate_sample_data.register
+def nifti_gz_x_generate_sample_data(nifti: NiftiGzX, dest_dir: Path):
     return medimages4tests.mri.neuro.t1w.get_image()
 
 
-@FileSet.generate_test_data.register
-def nifti_x_generate_test_data(nifti: NiftiX, dest_dir: Path):
+@FileSet.generate_sample_data.register
+def nifti_x_generate_sample_data(nifti: NiftiX, dest_dir: Path):
     nifti_gz_x = NiftiGzX(medimages4tests.mri.neuro.t1w.get_image())
     return NiftiX.convert(nifti_gz_x)
```

### Comparing `fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/tests/test_neuro_converters.py` & `fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/tests/test_neuro_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.1/LICENSE` & `fileformats_medimage_extras-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.1/README.rst` & `fileformats_medimage_extras-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.1/pyproject.toml` & `fileformats_medimage_extras-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.1/PKG-INFO` & `fileformats_medimage_extras-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats-medimage-extras
-Version: 0.1.1
+Version: 0.1.2
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats-medimage-extras
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

