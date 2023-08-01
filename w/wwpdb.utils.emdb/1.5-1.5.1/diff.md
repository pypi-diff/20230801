# Comparing `tmp/wwpdb.utils.emdb-1.5.tar.gz` & `tmp/wwpdb.utils.emdb-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.emdb-1.5.tar", last modified: Sat Jul 29 12:25:02 2023, max compression
+gzip compressed data, was "wwpdb.utils.emdb-1.5.1.tar", last modified: Tue Aug  1 13:37:43 2023, max compression
```

## Comparing `wwpdb.utils.emdb-1.5.tar` & `wwpdb.utils.emdb-1.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:25:02.639000 wwpdb.utils.emdb-1.5/
--rw-r--r--   0 vsts      (1001) docker     (123)      106 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-07-29 12:25:02.639000 wwpdb.utils.emdb-1.5/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       46 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-29 12:25:02.639000 wwpdb.utils.emdb-1.5/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2278 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:25:02.631000 wwpdb.utils.emdb-1.5/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:25:02.635000 wwpdb.utils.emdb-1.5/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:25:02.635000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/
--rw-r--r--   0 vsts      (1001) docker     (123)      322 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/EmdbSchema.py
--rw-r--r--   0 vsts      (1001) docker     (123)      143 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:25:02.635000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/atomcheck/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/atomcheck/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7031 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/atomcheck/atomcheck.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:25:02.639000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/
--rwxr-xr-x   0 vsts      (1001) docker     (123)      139 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)   676573 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1866 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (123)  2305255 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1196 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2490 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:25:02.639000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/data/
--rw-r--r--   0 vsts      (1001) docker     (123)   219087 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/data/emdb-v3.xsd
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:25:02.635000 wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-07-29 12:25:02.000000 wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      914 2023-07-29 12:25:02.000000 wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-29 12:25:02.000000 wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-07-29 12:25:02.000000 wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-29 12:24:44.000000 wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      101 2023-07-29 12:25:02.000000 wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-29 12:25:02.000000 wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 13:37:43.171410 wwpdb.utils.emdb-1.5.1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      106 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-08-01 13:37:43.171410 wwpdb.utils.emdb-1.5.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       46 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-08-01 13:37:43.171410 wwpdb.utils.emdb-1.5.1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2278 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 13:37:43.159410 wwpdb.utils.emdb-1.5.1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 13:37:43.163410 wwpdb.utils.emdb-1.5.1/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 13:37:43.163410 wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)      322 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/EmdbSchema.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      145 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 13:37:43.163410 wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/atomcheck/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/atomcheck/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7031 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/atomcheck/atomcheck.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 13:37:43.171410 wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/cif_emdb_translator/
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      139 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/cif_emdb_translator/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)   675611 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1866 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (123)  2299985 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1196 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2490 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 13:37:43.171410 wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)   218781 2023-08-01 13:36:53.000000 wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/data/emdb-v3.xsd
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 13:37:43.163410 wwpdb.utils.emdb-1.5.1/wwpdb.utils.emdb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-08-01 13:37:43.000000 wwpdb.utils.emdb-1.5.1/wwpdb.utils.emdb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      914 2023-08-01 13:37:43.000000 wwpdb.utils.emdb-1.5.1/wwpdb.utils.emdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-01 13:37:43.000000 wwpdb.utils.emdb-1.5.1/wwpdb.utils.emdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-08-01 13:37:43.000000 wwpdb.utils.emdb-1.5.1/wwpdb.utils.emdb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-01 13:37:25.000000 wwpdb.utils.emdb-1.5.1/wwpdb.utils.emdb.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      101 2023-08-01 13:37:43.000000 wwpdb.utils.emdb-1.5.1/wwpdb.utils.emdb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-08-01 13:37:43.000000 wwpdb.utils.emdb-1.5.1/wwpdb.utils.emdb.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.emdb-1.5/setup.py` & `wwpdb.utils.emdb-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/atomcheck/atomcheck.py` & `wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/atomcheck/atomcheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py` & `wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
         # Create a tree
         # print(dir(self.__block))
         # print self.__block.getObjNameList()
 
     def __getitem__(self, item):
         # Handle if abc in self.cif - key is an integer
-        if type(item) == int:
+        if type(item) == int:  # noqa: E721
             nl = self.__block.getObjNameList()
             if item >= len(nl):
                 raise StopIteration
             else:
                 return nl[item]
 
         return self.get(item)
@@ -105,15 +105,15 @@
 
     class Constants(object):
         """
         There are many constants in use for the translation.
         They have been collected here for ease of use.
         """
 
-        XML_OUT_VERSION = "3.0.7.2"
+        XML_OUT_VERSION = "3.0.8.0"
         XML_VERSION = XML_OUT_VERSION.replace('.', '_')
 
         # Cif categories
         CITATION = "citation"
         CITATION_AUTHOR = "citation_author"
         DATABASE_2 = "database_2"
         EM_ADMIN = "em_admin"
@@ -3465,15 +3465,15 @@
                             nat_src_id = get_cif_value("entity_assembly_id", const.EM_ENTITY_ASSEMBLY_NATURALSOURCE, src_in)
                             if assembly_id == nat_src_id:
                                 set_cif_value(src.set_synthetically_produced, cif_value=True)
 
                 def set_el_organism(src, tax_id_in, cif_category, src_in):
                     """
                     XSD: <xs:element name="organism" type="organism_type">
-                    CIF: _entity_src_nat.common_name
+                    CIF: _entity_src_nat.pdbx_organism_scientific
                     CIF: _entity_src_gen.pdbx_gene_src_scientific_name
                     CIF: _pdbx_entity_src_syn.organism_scientific
                     For some entries _entity_src_nat.common_name is not given but _entity_src_nat.pdbx_organism_scientific is
                     CIF: _entity_src_nat.pdbx_organism_scientific
                     CIF: _em_entity_assembly_naturalsource.organism
                     """
                     a_dict = {
@@ -11374,44 +11374,26 @@
                         for hf_map_in in hf_map_list_in:
                             hf_map = make_map(hf_map_in, get_canonical_map_name(hf_map_in, "HALFMAP"))
                             if hf_map.has__content():
                                 hf_map_list.add_half_map(hf_map)
                         if hf_map_list.has__content():
                             intrp.set_half_map_list(hf_map_list)
 
-                    def set_el_mask_list(intrp, map_dict_in):
-                        """
-                        XSD: <xs:element name="mask_list" minOccurs="0">
-                        """
-
-                        msk_map_list_in = map_dict_in[const.MAP_MASK] if const.MAP_MASK in map_dict_in else []
-                        msk_map_list = emdb.mask_listType()
-                        for msk_map_in in msk_map_list_in:
-                            msk_map = make_map(msk_map_in, get_canonical_map_name(msk_map_in, "MASK"))
-                            msk_file = msk_map.get_file()
-                            set_cif_value(msk_map.set_file, cif_value=msk_file)
-                            if msk_map.has__content():
-                                msk_map_list.add_mask(msk_map)
-                        if msk_map_list.has__content():
-                            intrp.set_mask_list(msk_map_list)
-
                     # element 1
                     set_el_modelling_list(intrp)
                     # element 2
                     set_el_figure_list()
                     # element 3
                     set_el_segmentation_list(intrp)
                     # element 4
                     set_el_slices_list()
                     # element 5
                     set_el_additional_map_list(intrp, map_dict_in)
                     # element 6
                     set_el_half_map_list(intrp, map_dict_in)
-                    # element 7
-                    set_el_mask_list(intrp, map_dict_in)
 
                 map_dict_in = make_list_of_dicts(const.EM_MAP, "type")
                 intrp = emdb.interpretation_type()
                 set_interpretation_type(intrp, map_dict_in)
                 if intrp.has__content():
                     self.xml_out.set_interpretation(intrp)
```

### Comparing `wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py` & `wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/emdb.py` & `wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/cif_emdb_translator/emdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #
-# Generated Mon Jul 17 15:20:35 2023 by generateDS.py version 2.41.5.
+# Generated Tue Aug  1 11:24:30 2023 by generateDS.py version 2.41.5.
 # Python 3.9.5 (default, May 18 2021, 12:31:01)  [Clang 10.0.0 ]
 #
 # Command line options:
 #   ('--root-element', 'emd')
 #   ('-f', '')
-#   ('-o', 'emdb-schemas/emdb_schemas/v3/v3_0_7_2/emdb.py')
+#   ('-o', 'emdb-schemas/emdb_schemas/v3/v3_0_8_0/emdb.py')
 #   ('--no-warnings', '')
 #   ('--external-encoding', 'utf-8')
 #
 # Command line arguments:
-#   emdb-schemas/emdb_schemas/v3/v3_0_7_2/emdb.xsd
+#   emdb-schemas/emdb_schemas/v3/v3_0_8_0/emdb.xsd
 #
 # Command line:
-#   /Users/amudha/project/generateDS-2.41.5/generateDS.py --root-element="emd" -f -o "emdb-schemas/emdb_schemas/v3/v3_0_7_2/emdb.py" --no-warnings --external-encoding="utf-8" emdb-schemas/emdb_schemas/v3/v3_0_7_2/emdb.xsd
+#   /Users/amudha/project/generateDS-2.41.5/generateDS.py --root-element="emd" -f -o "emdb-schemas/emdb_schemas/v3/v3_0_8_0/emdb.py" --no-warnings --external-encoding="utf-8" emdb-schemas/emdb_schemas/v3/v3_0_8_0/emdb.xsd
 #
 # Current working directory (os.getcwd()):
 #   IdeaProjects
 #
 
 import sys
 try:
@@ -1761,15 +1761,15 @@
     VIRUSLIKEPARTICLE='VIRUS-LIKE PARTICLE'
 
 
 class entry_type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, emdb_id=None, version='3.0.7.2', admin=None, crossreferences=None, sample=None, structure_determination_list=None, map=None, interpretation=None, validation=None, gds_collector_=None, **kwargs_):
+    def __init__(self, emdb_id=None, version='3.0.8.0', admin=None, crossreferences=None, sample=None, structure_determination_list=None, map=None, interpretation=None, validation=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.emdb_id = _cast(None, emdb_id)
         self.emdb_id_nsprefix_ = None
@@ -1887,15 +1887,15 @@
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='entry_type'):
         if self.emdb_id is not None and 'emdb_id' not in already_processed:
             already_processed.add('emdb_id')
             outfile.write(' emdb_id=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.emdb_id), input_name='emdb_id')), ))
-        if self.version != "3.0.7.2" and 'version' not in already_processed:
+        if self.version != "3.0.8.0" and 'version' not in already_processed:
             already_processed.add('version')
             outfile.write(' version=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.version), input_name='version')), ))
     def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='entry_type', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
@@ -21682,15 +21682,15 @@
 # end class pixel_spacing_type
 
 
 class interpretation_type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, modelling_list=None, figure_list=None, segmentation_list=None, slices_list=None, additional_map_list=None, half_map_list=None, mask_list=None, gds_collector_=None, **kwargs_):
+    def __init__(self, modelling_list=None, figure_list=None, segmentation_list=None, slices_list=None, additional_map_list=None, half_map_list=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.modelling_list = modelling_list
         self.modelling_list_nsprefix_ = None
@@ -21700,16 +21700,14 @@
         self.segmentation_list_nsprefix_ = None
         self.slices_list = slices_list
         self.slices_list_nsprefix_ = None
         self.additional_map_list = additional_map_list
         self.additional_map_list_nsprefix_ = None
         self.half_map_list = half_map_list
         self.half_map_list_nsprefix_ = None
-        self.mask_list = mask_list
-        self.mask_list_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
                 CurrentSubclassModule_, interpretation_type)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if interpretation_type.subclass:
@@ -21741,27 +21739,22 @@
         return self.additional_map_list
     def set_additional_map_list(self, additional_map_list):
         self.additional_map_list = additional_map_list
     def get_half_map_list(self):
         return self.half_map_list
     def set_half_map_list(self, half_map_list):
         self.half_map_list = half_map_list
-    def get_mask_list(self):
-        return self.mask_list
-    def set_mask_list(self, mask_list):
-        self.mask_list = mask_list
     def has__content(self):
         if (
             self.modelling_list is not None or
             self.figure_list is not None or
             self.segmentation_list is not None or
             self.slices_list is not None or
             self.additional_map_list is not None or
-            self.half_map_list is not None or
-            self.mask_list is not None
+            self.half_map_list is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='interpretation_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('interpretation_type')
         if imported_ns_def_ is not None:
@@ -21806,17 +21799,14 @@
             self.slices_list.export(outfile, level, namespaceprefix_, namespacedef_='', name_='slices_list', pretty_print=pretty_print)
         if self.additional_map_list is not None:
             namespaceprefix_ = self.additional_map_list_nsprefix_ + ':' if (UseCapturedNS_ and self.additional_map_list_nsprefix_) else ''
             self.additional_map_list.export(outfile, level, namespaceprefix_, namespacedef_='', name_='additional_map_list', pretty_print=pretty_print)
         if self.half_map_list is not None:
             namespaceprefix_ = self.half_map_list_nsprefix_ + ':' if (UseCapturedNS_ and self.half_map_list_nsprefix_) else ''
             self.half_map_list.export(outfile, level, namespaceprefix_, namespacedef_='', name_='half_map_list', pretty_print=pretty_print)
-        if self.mask_list is not None:
-            namespaceprefix_ = self.mask_list_nsprefix_ + ':' if (UseCapturedNS_ and self.mask_list_nsprefix_) else ''
-            self.mask_list.export(outfile, level, namespaceprefix_, namespacedef_='', name_='mask_list', pretty_print=pretty_print)
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
         self._buildAttributes(node, node.attrib, already_processed)
@@ -21853,19 +21843,14 @@
             self.additional_map_list = obj_
             obj_.original_tagname_ = 'additional_map_list'
         elif nodeName_ == 'half_map_list':
             obj_ = half_map_listType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.half_map_list = obj_
             obj_.original_tagname_ = 'half_map_list'
-        elif nodeName_ == 'mask_list':
-            obj_ = mask_listType.factory(parent_object_=self)
-            obj_.build(child_, gds_collector_=gds_collector_)
-            self.mask_list = obj_
-            obj_.original_tagname_ = 'mask_list'
 # end class interpretation_type
 
 
 class modelling_type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
@@ -43406,116 +43391,14 @@
             obj_ = map_type.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.half_map.append(obj_)
             obj_.original_tagname_ = 'half_map'
 # end class half_map_listType
 
 
-class mask_listType(GeneratedsSuper):
-    __hash__ = GeneratedsSuper.__hash__
-    subclass = None
-    superclass = None
-    def __init__(self, mask=None, gds_collector_=None, **kwargs_):
-        self.gds_collector_ = gds_collector_
-        self.gds_elementtree_node_ = None
-        self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
-        self.ns_prefix_ = None
-        if mask is None:
-            self.mask = []
-        else:
-            self.mask = mask
-        self.mask_nsprefix_ = None
-    def factory(*args_, **kwargs_):
-        if CurrentSubclassModule_ is not None:
-            subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, mask_listType)
-            if subclass is not None:
-                return subclass(*args_, **kwargs_)
-        if mask_listType.subclass:
-            return mask_listType.subclass(*args_, **kwargs_)
-        else:
-            return mask_listType(*args_, **kwargs_)
-    factory = staticmethod(factory)
-    def get_ns_prefix_(self):
-        return self.ns_prefix_
-    def set_ns_prefix_(self, ns_prefix):
-        self.ns_prefix_ = ns_prefix
-    def get_mask(self):
-        return self.mask
-    def set_mask(self, mask):
-        self.mask = mask
-    def add_mask(self, value):
-        self.mask.append(value)
-    def insert_mask_at(self, index, value):
-        self.mask.insert(index, value)
-    def replace_mask_at(self, index, value):
-        self.mask[index] = value
-    def has__content(self):
-        if (
-            self.mask
-        ):
-            return True
-        else:
-            return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='mask_listType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('mask_listType')
-        if imported_ns_def_ is not None:
-            namespacedef_ = imported_ns_def_
-        if pretty_print:
-            eol_ = '\n'
-        else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'mask_listType':
-            name_ = self.original_tagname_
-        if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
-        showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='mask_listType')
-        if self.has__content():
-            outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='mask_listType', pretty_print=pretty_print)
-            showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
-        else:
-            outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='mask_listType'):
-        pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='mask_listType', fromsubclass_=False, pretty_print=True):
-        if pretty_print:
-            eol_ = '\n'
-        else:
-            eol_ = ''
-        for mask_ in self.mask:
-            namespaceprefix_ = self.mask_nsprefix_ + ':' if (UseCapturedNS_ and self.mask_nsprefix_) else ''
-            mask_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='mask', pretty_print=pretty_print)
-    def build(self, node, gds_collector_=None):
-        self.gds_collector_ = gds_collector_
-        if SaveElementTreeNode:
-            self.gds_elementtree_node_ = node
-        already_processed = set()
-        self.ns_prefix_ = node.prefix
-        self._buildAttributes(node, node.attrib, already_processed)
-        for child in node:
-            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
-        return self
-    def _buildAttributes(self, node, attrs, already_processed):
-        pass
-    def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'mask':
-            obj_ = map_type.factory(parent_object_=self)
-            obj_.build(child_, gds_collector_=gds_collector_)
-            self.mask.append(obj_)
-            obj_.original_tagname_ = 'mask'
-# end class mask_listType
-
-
 class initial_modelType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, access_code=None, chain=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
@@ -44778,15 +44661,14 @@
     "macromoleculeType",
     "macromolecule_listType",
     "macromolecule_list_type",
     "macromolecule_source_type",
     "macromolecules_and_complexes_type",
     "map_statistics_type",
     "map_type",
-    "mask_listType",
     "max",
     "max_angleType",
     "microscopy_centerType",
     "microscopy_listType",
     "min",
     "min_angleType",
     "modelling_listType",
```

### Comparing `wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py` & `wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py` & `wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/data/emdb-v3.xsd`

 * *Files 1% similar despite different names*

#### Comparing `wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb.utils.emdb-1.5.1/wwpdb/utils/emdb/data/emdb-v3.xsd`

```diff
@@ -20,15 +20,15 @@
           <xs:sequence>
             <xs:element ref="validation_method" maxOccurs="unbounded"/>
           </xs:sequence>
         </xs:complexType>
       </xs:element>
     </xs:sequence>
     <xs:attribute name="emdb_id" type="emdb_id_type" use="required"/>
-    <xs:attribute name="version" type="xs:token" default="3.0.7.2"/>
+    <xs:attribute name="version" type="xs:token" default="3.0.8.0"/>
     <!-- <xs:attribute name="composite_structure" type="xs:boolean"/> -->
   </xs:complexType>
   <xs:complexType name="admin_type">
     <xs:sequence>
       <xs:element name="status_history_list" type="version_list_type" minOccurs="0"/>
       <xs:element name="current_status" type="version_type"/>
       <xs:element name="sites">
@@ -3814,21 +3814,14 @@
                 <xs:complexType>
                     <xs:sequence>
                         <xs:element name="ref_map" minOccurs="0" type="map_type"/>
                     </xs:sequence>
                 </xs:complexType>
             </xs:element>
             -->
-      <xs:element minOccurs="0" name="mask_list">
-        <xs:complexType>
-          <xs:sequence>
-            <xs:element maxOccurs="unbounded" name="mask" type="map_type"/>
-          </xs:sequence>
-        </xs:complexType>
-      </xs:element>
     </xs:sequence>
   </xs:complexType>
   <xs:complexType name="modelling_type">
     <xs:sequence>
       <xs:element name="initial_model" minOccurs="0" maxOccurs="unbounded">
         <xs:complexType>
           <xs:sequence>
```

### Comparing `wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/SOURCES.txt` & `wwpdb.utils.emdb-1.5.1/wwpdb.utils.emdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

