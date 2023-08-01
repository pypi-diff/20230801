# Comparing `tmp/plateauutils-0.0.3.tar.gz` & `tmp/plateauutils-0.0.4.tar.gz`

## Comparing `plateauutils-0.0.3.tar` & `plateauutils-0.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 plateauutils-0.0.3/dev-requirements.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 plateauutils-0.0.3/requirements.txt
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 plateauutils-0.0.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 plateauutils-0.0.3/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/Makefile
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/conf.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/make.bat
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/modules.rst
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/plateauutils.mesh_geocorder.rst
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/plateauutils.parser.rst
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/plateauutils.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/plateauutils.tile_list.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/__init__.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/abc/__init__.py
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/abc/plateau_parser.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/abc/polygon_to_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/mesh_geocorder/__init__.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/mesh_geocorder/geo_to_mesh.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/mesh_geocorder/polygon_to_meshcode_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/mesh_geocorder/tests/__init__.py
--rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/mesh_geocorder/tests/test_geo_to_mesh.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/mesh_geocorder/tests/test_polygon_to_meshcode_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/parser/__init__.py
--rw-r--r--   0        0        0     8616 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/parser/city_gml_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/parser/tests/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/parser/tests/test_city_gml_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/tests/__init__.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/tests/test_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/tile_list/__init__.py
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/tile_list/geo_to_tile.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/tile_list/polygon_to_tile_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/tile_list/tests/__init__.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/tile_list/tests/test_geo_to_tile.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/tile_list/tests/test_polygon_to_tile_list.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 plateauutils-0.0.3/.gitignore
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 plateauutils-0.0.3/LICENSE
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 plateauutils-0.0.3/README.rst
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 plateauutils-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    15302 2020-02-02 00:00:00.000000 plateauutils-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 plateauutils-0.0.4/dev-requirements.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 plateauutils-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 plateauutils-0.0.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 plateauutils-0.0.4/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 plateauutils-0.0.4/doc/Makefile
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 plateauutils-0.0.4/doc/conf.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 plateauutils-0.0.4/doc/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 plateauutils-0.0.4/doc/make.bat
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 plateauutils-0.0.4/doc/modules.rst
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 plateauutils-0.0.4/doc/plateauutils.mesh_geocorder.rst
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 plateauutils-0.0.4/doc/plateauutils.parser.rst
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 plateauutils-0.0.4/doc/plateauutils.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 plateauutils-0.0.4/doc/plateauutils.tile_list.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/__init__.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/abc/__init__.py
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/abc/plateau_parser.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/abc/polygon_to_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/mesh_geocorder/__init__.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/mesh_geocorder/geo_to_mesh.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/mesh_geocorder/polygon_to_meshcode_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/mesh_geocorder/tests/__init__.py
+-rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/mesh_geocorder/tests/test_geo_to_mesh.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/mesh_geocorder/tests/test_polygon_to_meshcode_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/parser/__init__.py
+-rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/parser/city_gml_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/parser/tests/__init__.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/parser/tests/test_city_gml_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/tests/__init__.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/tests/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/tile_list/__init__.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/tile_list/geo_to_tile.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/tile_list/polygon_to_tile_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/tile_list/tests/__init__.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/tile_list/tests/test_geo_to_tile.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 plateauutils-0.0.4/plateauutils/tile_list/tests/test_polygon_to_tile_list.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 plateauutils-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 plateauutils-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 plateauutils-0.0.4/README.rst
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 plateauutils-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    15302 2020-02-02 00:00:00.000000 plateauutils-0.0.4/PKG-INFO
```

### Comparing `plateauutils-0.0.3/dev-requirements.txt` & `plateauutils-0.0.4/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/.github/workflows/ci.yml` & `plateauutils-0.0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/.github/workflows/documentation.yml` & `plateauutils-0.0.4/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/doc/Makefile` & `plateauutils-0.0.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/doc/conf.py` & `plateauutils-0.0.4/doc/conf.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/doc/index.rst` & `plateauutils-0.0.4/doc/index.rst`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/doc/make.bat` & `plateauutils-0.0.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/doc/plateauutils.mesh_geocorder.rst` & `plateauutils-0.0.4/doc/plateauutils.mesh_geocorder.rst`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/doc/plateauutils.tile_list.rst` & `plateauutils-0.0.4/doc/plateauutils.tile_list.rst`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/plateauutils/cli.py` & `plateauutils-0.0.4/plateauutils/cli.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/plateauutils/abc/plateau_parser.py` & `plateauutils-0.0.4/plateauutils/abc/plateau_parser.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/plateauutils/abc/polygon_to_list.py` & `plateauutils-0.0.4/plateauutils/abc/polygon_to_list.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/plateauutils/mesh_geocorder/geo_to_mesh.py` & `plateauutils-0.0.4/plateauutils/mesh_geocorder/geo_to_mesh.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/plateauutils/mesh_geocorder/polygon_to_meshcode_list.py` & `plateauutils-0.0.4/plateauutils/mesh_geocorder/polygon_to_meshcode_list.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/plateauutils/mesh_geocorder/tests/test_geo_to_mesh.py` & `plateauutils-0.0.4/plateauutils/mesh_geocorder/tests/test_geo_to_mesh.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/plateauutils/mesh_geocorder/tests/test_polygon_to_meshcode_list.py` & `plateauutils-0.0.4/plateauutils/mesh_geocorder/tests/test_polygon_to_meshcode_list.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/plateauutils/parser/city_gml_parser.py` & `plateauutils-0.0.4/plateauutils/parser/city_gml_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -65,16 +65,73 @@
                 unarchived_dir, "*", "udx", "bldg", target + "_bldg_*.gml"
             )
             # ファイルが二つ以上ある場合に対応させる
             for file_path in glob.glob(target_file_path):
                 # XMLのオブジェクトとして読み込む
                 tree = ET.parse(file_path)
                 root = tree.getroot()
+                # namespaceを作成
+                ns = {
+                    "core": "http://www.opengis.net/citygml/2.0",
+                    "bldg": "http://www.opengis.net/citygml/building/2.0",
+                    "gml": "http://www.opengis.net/gml",
+                    "uro": "",
+                }
+                # 処理の分岐のためのversion変数を作成
+                version = None
+                # uroのnamespaceとversionを取得
+                if (
+                    len(
+                        root.findall(
+                            ".//{https://www.geospatial.jp/iur/uro/2.0}buildingDetailAttribute"
+                        )
+                    )
+                    > 0
+                ):
+                    ns["uro"] = "https://www.geospatial.jp/iur/uro/2.0"
+                    version = 2
+                elif (
+                    len(
+                        root.findall(
+                            ".//{https://www.geospatial.jp/iur/uro/3.0}buildingDetailAttribute"
+                        )
+                    )
+                    > 0
+                ):
+                    ns["uro"] = "https://www.geospatial.jp/iur/uro/3.0"
+                    version = 3
+                elif (
+                    len(
+                        root.findall(
+                            ".//{http://www.kantei.go.jp/jp/singi/tiiki/toshisaisei/itoshisaisei/iur/uro/1.4}buildingDetails"
+                        )
+                    )
+                    > 0
+                ):
+                    ns[
+                        "uro"
+                    ] = "http://www.kantei.go.jp/jp/singi/tiiki/toshisaisei/itoshisaisei/iur/uro/1.4"
+                    version = 1
+                elif (
+                    len(
+                        root.findall(
+                            ".//{https://www.chisou.go.jp/tiiki/toshisaisei/itoshisaisei/iur/uro/1.5}buildingDetails"
+                        )
+                    )
+                    > 0
+                ):
+                    ns[
+                        "uro"
+                    ] = "https://www.chisou.go.jp/tiiki/toshisaisei/itoshisaisei/iur/uro/1.5"
+                    version = 1
+                # versionがNoneならエラーとする
+                if version is None:
+                    raise ValueError("version is None")
                 # パース処理を実施する
-                ret = self._parse(root, file_path)
+                ret = self._parse(root, file_path, ns, version)
                 # 返り値に追加
                 return_list.extend(ret)
         # 返り値を返却
         return return_list
 
     def download_and_parse(self, url: str = "", target_dir: str = "") -> list:
         """CityGMLファイルをダウンロードして、情報を返すメソッド
@@ -114,78 +171,71 @@
             polygon_to_mesh_code = PolygonToMeshCodeList(polygon, mesh)
             # 返り値に追加
             for j in polygon_to_mesh_code.output():
                 return_list.append(j)
         # 返り値を返す
         return return_list
 
-    def _parse(self, root: ET.Element, file_path: str) -> list:
+    def _parse(self, root: ET.Element, file_path: str, ns: dict, version: int) -> list:
         # 返り値を作成
         return_list = []
         # core:cityObjectMemberの一覧を取得
-        city_object_members = root.findall(
-            ".//{http://www.opengis.net/citygml/2.0}cityObjectMember"
-        )
+        city_object_members = root.findall(".//core:cityObjectMember", ns)
         # core:cityObjectMemberごとに処理
         for city_object_member in city_object_members:
             # bldg:Buildingを取得
-            building = city_object_member.find(
-                ".//{http://www.opengis.net/citygml/building/2.0}Building"
-            )
+            building = city_object_member.find(".//bldg:Building", ns)
             # gml:idを取得
-            gid = building.attrib["{http://www.opengis.net/gml}id"]
+            gid = building.get("{http://www.opengis.net/gml}id")
             # bldg:mesuredHeightを取得
             measured_height = float(
-                city_object_member.find(
-                    ".//{http://www.opengis.net/citygml/building/2.0}measuredHeight"
-                ).text
-            )
-            # uro:buildingDetailAttributeを取得
-            building_detail_attribute = city_object_member.find(
-                ".//{https://www.geospatial.jp/iur/uro/2.0}buildingDetailAttribute"
+                city_object_member.find(".//bldg:measuredHeight", ns).text
             )
+            # uro:BuildingDetails(v1) もしくは uro:buildingDetailAttribute(v2以降)を取得
+            if version == 1:
+                building_detail_attribute = city_object_member.find(
+                    ".//uro:BuildingDetails", ns
+                )
+            else:
+                building_detail_attribute = city_object_member.find(
+                    ".//uro:buildingDetailAttribute", ns
+                )
             # uro:buildingStructureTypeを取得
             building_structure_type = building_detail_attribute.find(
-                ".//{https://www.geospatial.jp/iur/uro/2.0}buildingStructureType"
+                ".//uro:buildingStructureType", ns
             )
             # uro:codeSpaceを取得
             code_space = building_structure_type.get("codeSpace")
             # codeSpaceから値を取得
             code_space_root = ET.parse(
                 os.path.abspath(os.path.join(file_path, "..", code_space))
             )
             code_space_root_root = code_space_root.getroot()
             building_structure_type_text = None
             for code_space_root_root_child in code_space_root_root.findall(
-                ".//{http://www.opengis.net/gml}dictionaryEntry"
+                ".//gml:dictionaryEntry", ns
             ):
-                gml_name = code_space_root_root_child.find(
-                    ".//{http://www.opengis.net/gml}name"
-                )
+                gml_name = code_space_root_root_child.find(".//gml:name", ns)
                 if str(gml_name.text) == str(building_structure_type.text):
                     building_structure_type_text = str(
-                        code_space_root_root_child.find(
-                            ".//{http://www.opengis.net/gml}description"
-                        ).text
+                        code_space_root_root_child.find(".//gml:description", ns).text
                     )
                     break
             # bldg:lod1Solidを取得
-            lod1_solid = city_object_member.find(
-                ".//{http://www.opengis.net/citygml/building/2.0}lod1Solid"
-            )
+            lod1_solid = city_object_member.find(".//bldg:lod1Solid", ns)
             # 返り値に入る値を作成
             return_value = {
                 "gid": gid,
                 "center": None,
                 "min_height": 10000,
                 "measured_height": measured_height,
                 "building_structure_type": building_structure_type_text,
             }
             # gml:posListを取得
-            pos_lists = lod1_solid.findall(".//{http://www.opengis.net/gml}posList")
+            pos_lists = lod1_solid.findall(".//gml:posList", ns)
             for poi_list in pos_lists:
                 # posListをパース
                 polygon, max_height = self._parse_poi_list(poi_list.text)
                 if max_height < return_value["min_height"]:
                     # 返り値に追加
                     return_value["center"] = [polygon.centroid.x, polygon.centroid.y]
                     return_value["min_height"] = max_height
```

### Comparing `plateauutils-0.0.3/plateauutils/parser/tests/test_city_gml_parser.py` & `plateauutils-0.0.4/plateauutils/parser/tests/test_city_gml_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,37 @@
 from plateauutils.parser.city_gml_parser import CityGMLParser
 from shapely import from_wkt
 import tempfile
 
 
-def test_citygml_parser():
+def test_citygml_parser_v2():
     target_polygon = from_wkt(
         "POLYGON ((130.41249721501615 33.224722548534864, 130.41249721501615 33.22506264293093, 130.41621606802997 33.22506264293093, 130.41621606802997 33.224722548534864, 130.41249721501615 33.224722548534864))"
     )
     parser = CityGMLParser(target_polygon)
     with tempfile.TemporaryDirectory() as tmpdir:
         result = parser.download_and_parse(
-            "https://file.smellman.org/test_citygml.zip", tmpdir
+            "https://file.smellman.org/test_citygml_v2.zip", tmpdir
         )
         assert len(result) == 3
         assert result[0]["gid"] == "bldg_383f1804-aa34-4634-949f-f769e09fa92d"
         assert result[0]["center"] == [130.41263587199947, 33.22489181671553]
         assert result[0]["min_height"] == 3.805999994277954
         assert result[0]["measured_height"] == 9.3
         assert result[0]["building_structure_type"] == "非木造"
+
+
+def test_citygml_parser_v1_4():
+    target_polygon = from_wkt(
+        "POLYGON ((130.41249721501615 33.224722548534864, 130.41249721501615 33.22506264293093, 130.41621606802997 33.22506264293093, 130.41621606802997 33.224722548534864, 130.41249721501615 33.224722548534864))"
+    )
+    parser = CityGMLParser(target_polygon)
+    with tempfile.TemporaryDirectory() as tmpdir:
+        result = parser.download_and_parse(
+            "https://file.smellman.org/test_citygml_v1.4.zip", tmpdir
+        )
+        assert len(result) == 2
+        assert result[0]["gid"] == "uuid_877DEA60-35D0-4FD9-8B02-852E39C75D81"
+        assert result[0]["center"] == [130.41619367090038, 33.22492719812357]
+        assert result[0]["min_height"] == 4.454999923706055
+        assert result[0]["measured_height"] == 3.0
+        assert result[0]["building_structure_type"] == "非木造"
```

### Comparing `plateauutils-0.0.3/plateauutils/tests/test_cli.py` & `plateauutils-0.0.4/plateauutils/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/plateauutils/tile_list/geo_to_tile.py` & `plateauutils-0.0.4/plateauutils/tile_list/geo_to_tile.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/plateauutils/tile_list/polygon_to_tile_list.py` & `plateauutils-0.0.4/plateauutils/tile_list/polygon_to_tile_list.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/plateauutils/tile_list/tests/test_geo_to_tile.py` & `plateauutils-0.0.4/plateauutils/tile_list/tests/test_geo_to_tile.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/plateauutils/tile_list/tests/test_polygon_to_tile_list.py` & `plateauutils-0.0.4/plateauutils/tile_list/tests/test_polygon_to_tile_list.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/.gitignore` & `plateauutils-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/LICENSE` & `plateauutils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/README.rst` & `plateauutils-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.3/pyproject.toml` & `plateauutils-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = "A collection of utilities for the Plateau project"
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3",
 ]
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
     "click",
     "numpy",
     "requests",
     "shapely",
     "tqdm",
 ]
```

### Comparing `plateauutils-0.0.3/PKG-INFO` & `plateauutils-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plateauutils
-Version: 0.0.3
+Version: 0.0.4
 Summary: A collection of utilities for the Plateau project
 Project-URL: Homepage, https://eukarya-inc.github.io/plateauutils/
 Project-URL: Bug Reports, https://github.com/eukarya-inc/plateauutils/issues
 Project-URL: Source, https://github.com/eukarya-inc/plateauutils
 Author: Eukarya Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
```

