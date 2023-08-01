# Comparing `tmp/morphoaap-0.0.6.tar.gz` & `tmp/morphoaap-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphoaap-0.0.6.tar", last modified: Fri Jul 28 00:15:43 2023, max compression
+gzip compressed data, was "morphoaap-0.0.7.tar", last modified: Tue Aug  1 20:45:15 2023, max compression
```

## Comparing `morphoaap-0.0.6.tar` & `morphoaap-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-07-28 00:15:43.056587 morphoaap-0.0.6/
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     1160 2023-07-15 20:24:22.000000 morphoaap-0.0.6/CMakeLists.txt
--rw-r--r--   0 wonderalexandre   (501) staff       (20)    35149 2023-07-13 11:33:07.000000 morphoaap-0.0.6/LICENSE
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      111 2023-07-14 16:12:23.000000 morphoaap-0.0.6/MANIFEST.in
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      565 2023-07-28 00:15:43.056281 morphoaap-0.0.6/PKG-INFO
--rw-r--r--   0 wonderalexandre   (501) staff       (20)       33 2023-07-13 13:11:59.000000 morphoaap-0.0.6/README.md
-drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-07-28 00:15:43.050064 morphoaap-0.0.6/morphoaap/
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     1738 2023-07-16 00:45:25.000000 morphoaap-0.0.6/morphoaap/CMakeLists.txt
-drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-07-28 00:15:43.053968 morphoaap-0.0.6/morphoaap/include/
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     1687 2023-07-15 20:34:52.000000 morphoaap-0.0.6/morphoaap/include/AttributeComputedIncrementally.hpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     4402 2023-07-15 20:35:10.000000 morphoaap-0.0.6/morphoaap/include/AttributeFilters.hpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      523 2023-07-15 20:35:16.000000 morphoaap-0.0.6/morphoaap/include/AttributeProfile.hpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      954 2023-07-15 20:35:20.000000 morphoaap-0.0.6/morphoaap/include/ComponentTree.hpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      711 2023-07-15 20:35:27.000000 morphoaap-0.0.6/morphoaap/include/ComputerMSER.hpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      479 2023-07-11 21:03:13.000000 morphoaap-0.0.6/morphoaap/include/NodeCT.hpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     2390 2023-07-15 20:37:49.000000 morphoaap-0.0.6/morphoaap/morphoaap.cpp
-drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-07-28 00:15:43.055853 morphoaap-0.0.6/morphoaap/src/
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      559 2023-07-15 20:38:08.000000 morphoaap-0.0.6/morphoaap/src/AttributeComputedIncrementally.cpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     1774 2023-07-15 20:34:13.000000 morphoaap-0.0.6/morphoaap/src/AttributeFilters.cpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     2930 2023-07-15 20:34:27.000000 morphoaap-0.0.6/morphoaap/src/AttributeProfile.cpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     5350 2023-07-15 20:34:34.000000 morphoaap-0.0.6/morphoaap/src/ComponentTree.cpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     4199 2023-07-15 20:34:01.000000 morphoaap-0.0.6/morphoaap/src/ComputerMSER.cpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      699 2023-07-15 20:34:43.000000 morphoaap-0.0.6/morphoaap/src/NodeCT.cpp
-drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-07-28 00:15:43.051583 morphoaap-0.0.6/morphoaap.egg-info/
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      565 2023-07-28 00:15:42.000000 morphoaap-0.0.6/morphoaap.egg-info/PKG-INFO
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      719 2023-07-28 00:15:42.000000 morphoaap-0.0.6/morphoaap.egg-info/SOURCES.txt
--rw-r--r--   0 wonderalexandre   (501) staff       (20)        1 2023-07-28 00:15:42.000000 morphoaap-0.0.6/morphoaap.egg-info/dependency_links.txt
--rw-r--r--   0 wonderalexandre   (501) staff       (20)        1 2023-07-28 00:01:54.000000 morphoaap-0.0.6/morphoaap.egg-info/not-zip-safe
--rw-r--r--   0 wonderalexandre   (501) staff       (20)       10 2023-07-28 00:15:42.000000 morphoaap-0.0.6/morphoaap.egg-info/top_level.txt
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      338 2023-07-14 11:21:09.000000 morphoaap-0.0.6/pybind11.cmake
--rw-r--r--   0 wonderalexandre   (501) staff       (20)       38 2023-07-28 00:15:43.056701 morphoaap-0.0.6/setup.cfg
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     3309 2023-07-28 00:15:36.000000 morphoaap-0.0.6/setup.py
+drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-08-01 20:45:15.179665 morphoaap-0.0.7/
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     1160 2023-08-01 20:32:00.000000 morphoaap-0.0.7/CMakeLists.txt
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)    35149 2023-07-13 11:33:07.000000 morphoaap-0.0.7/LICENSE
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      111 2023-07-14 16:12:23.000000 morphoaap-0.0.7/MANIFEST.in
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      565 2023-08-01 20:45:15.179341 morphoaap-0.0.7/PKG-INFO
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)       33 2023-07-13 13:11:59.000000 morphoaap-0.0.7/README.md
+drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-08-01 20:45:15.172578 morphoaap-0.0.7/morphoaap/
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     1816 2023-08-01 20:38:15.000000 morphoaap-0.0.7/morphoaap/CMakeLists.txt
+drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-08-01 20:45:15.176864 morphoaap-0.0.7/morphoaap/include/
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     1494 2023-08-01 20:38:15.000000 morphoaap-0.0.7/morphoaap/include/Adjacency8.hpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     1678 2023-08-01 20:38:15.000000 morphoaap-0.0.7/morphoaap/include/AttributeComputedIncrementally.hpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     4385 2023-08-01 20:38:15.000000 morphoaap-0.0.7/morphoaap/include/AttributeFilters.hpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      613 2023-08-01 20:38:15.000000 morphoaap-0.0.7/morphoaap/include/AttributeProfile.hpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     1794 2023-08-01 20:38:15.000000 morphoaap-0.0.7/morphoaap/include/ComponentTree.hpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      790 2023-08-01 20:38:15.000000 morphoaap-0.0.7/morphoaap/include/ComputerMSER.hpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      479 2023-07-11 21:03:13.000000 morphoaap-0.0.7/morphoaap/include/NodeCT.hpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     3231 2023-08-01 20:38:15.000000 morphoaap-0.0.7/morphoaap/morphoaap.cpp
+drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-08-01 20:45:15.178933 morphoaap-0.0.7/morphoaap/src/
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      993 2023-08-01 20:38:15.000000 morphoaap-0.0.7/morphoaap/src/Adjacency8.cpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      561 2023-08-01 20:38:15.000000 morphoaap-0.0.7/morphoaap/src/AttributeComputedIncrementally.cpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     1774 2023-07-15 20:34:13.000000 morphoaap-0.0.7/morphoaap/src/AttributeFilters.cpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     5212 2023-08-01 20:38:15.000000 morphoaap-0.0.7/morphoaap/src/AttributeProfile.cpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     5770 2023-08-01 20:38:15.000000 morphoaap-0.0.7/morphoaap/src/ComponentTree.cpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     4021 2023-08-01 20:38:15.000000 morphoaap-0.0.7/morphoaap/src/ComputerMSER.cpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      699 2023-08-01 20:32:06.000000 morphoaap-0.0.7/morphoaap/src/NodeCT.cpp
+drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-08-01 20:45:15.174650 morphoaap-0.0.7/morphoaap.egg-info/
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      565 2023-08-01 20:45:15.000000 morphoaap-0.0.7/morphoaap.egg-info/PKG-INFO
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      781 2023-08-01 20:45:15.000000 morphoaap-0.0.7/morphoaap.egg-info/SOURCES.txt
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)        1 2023-08-01 20:45:15.000000 morphoaap-0.0.7/morphoaap.egg-info/dependency_links.txt
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)        1 2023-08-01 20:41:21.000000 morphoaap-0.0.7/morphoaap.egg-info/not-zip-safe
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)       10 2023-08-01 20:45:15.000000 morphoaap-0.0.7/morphoaap.egg-info/top_level.txt
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      338 2023-07-14 11:21:09.000000 morphoaap-0.0.7/pybind11.cmake
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)       38 2023-08-01 20:45:15.179774 morphoaap-0.0.7/setup.cfg
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     3309 2023-08-01 20:44:47.000000 morphoaap-0.0.7/setup.py
```

### Comparing `morphoaap-0.0.6/CMakeLists.txt` & `morphoaap-0.0.7/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.6/LICENSE` & `morphoaap-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.6/PKG-INFO` & `morphoaap-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: morphoaap
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple library for adative attribute profiles
 Home-page: https://github.com/wonderalexandre/aap
 Author: Wonder Alexandre Luz Alves
 Author-email: worderalexandre@gmail.com
 License: GPL-3.0
 Description: UNKNOWN
 Keywords: attribute profiles,mathematical morphology,morphological trees
```

### Comparing `morphoaap-0.0.6/morphoaap/CMakeLists.txt` & `morphoaap-0.0.7/morphoaap/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -44,15 +44,16 @@
     ${PROJECT_SOURCE_DIR}/ComponentTree.cpp
     ${PROJECT_INCLUDE_DIR}/ComputerMSER.hpp
     ${PROJECT_SOURCE_DIR}/ComputerMSER.cpp
     ${PROJECT_INCLUDE_DIR}/AttributeProfile.hpp
     ${PROJECT_SOURCE_DIR}/AttributeProfile.cpp
     ${PROJECT_INCLUDE_DIR}/AttributeFilters.hpp
     ${PROJECT_SOURCE_DIR}/AttributeFilters.cpp
-    
+    ${PROJECT_INCLUDE_DIR}/Adjacency8.hpp
+    ${PROJECT_SOURCE_DIR}/Adjacency8.cpp
 )
 
 # Set up such that XCode organizes the files correctly
 source_group(TREE ${CMAKE_CURRENT_SOURCE_DIR} FILES ${SOURCE_FILES})
 
 # Add library
 add_library(morphoaap SHARED ${SOURCE_FILES})
```

### Comparing `morphoaap-0.0.6/morphoaap/include/AttributeComputedIncrementally.hpp` & `morphoaap-0.0.7/morphoaap/include/AttributeComputedIncrementally.hpp`

 * *Files 17% similar despite different names*

```diff
@@ -10,34 +10,35 @@
 class AttributeComputedIncrementally{
 
 public:
     virtual void preProcessing(NodeCT *v);
 
     virtual void mergeChildren(NodeCT *parent, NodeCT *child);
 
-    virtual void posProcessing(NodeCT *parent);
+    virtual void postProcessing(NodeCT *parent);
 
     void computerAttribute(NodeCT *root);
 
 	static void computerAttribute(NodeCT* root, 
 										std::function<void(NodeCT*)> preProcessing,
 										std::function<void(NodeCT*, NodeCT*)> mergeChildren,
-										std::function<void(NodeCT*)> posProcessing ){
+										std::function<void(NodeCT*)> postProcessing ){
 		
 		preProcessing(root);
 			
 		for(NodeCT *child: root->getChildren()){
-			AttributeComputedIncrementally::computerAttribute(child, preProcessing, mergeChildren, posProcessing);
+			AttributeComputedIncrementally::computerAttribute(child, preProcessing, mergeChildren, postProcessing);
 			mergeChildren(root, child);
 		}
-		posProcessing(root);
+
+		postProcessing(root);
 	}
 
     static py::array_t<double> computerArea(ComponentTree *tree){
-	    double* attribute = new double[tree->getNumNodes()];
+	    double attribute[tree->getNumNodes()];
 		
 	    AttributeComputedIncrementally::computerAttribute(tree->getRoot(),
 						[&attribute](NodeCT* node) -> void {
 							attribute[node->getIndex()] = node->getCNPs().size();
 						},
 						[&attribute](NodeCT* root, NodeCT* child) -> void {
 							attribute[root->getIndex()] += attribute[child->getIndex()];
```

### Comparing `morphoaap-0.0.6/morphoaap/include/AttributeFilters.hpp` & `morphoaap-0.0.7/morphoaap/include/AttributeFilters.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 #include "../include/NodeCT.hpp"
 #include "../include/ComponentTree.hpp"
 #include "../include/ComputerMSER.hpp"
 
 #include <stack>
+#include <vector>
 #include <limits.h>
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 #include <pybind11/numpy.h>
 
 #ifndef ATTRIBUTE_FILTERS_H
 #define ATTRIBUTE_FILTERS_H
@@ -30,15 +31,15 @@
         s.push(tree->getRoot());
         while(!s.empty()){
             NodeCT *node = s.top(); s.pop();
             for (int p : node->getCNPs()){
                 imgOutput[p] = node->getLevel();
             }
             for (NodeCT *child: node->getChildren()){
-                if(attribute[child->getIndex()] > threshold){
+                if(attribute[child->getIndex()] >= threshold){
                     s.push(child);
                 }else{
                     std::stack<NodeCT*> stackSubtree;
                     stackSubtree.push(child);
                     while(!stackSubtree.empty()){
                         NodeCT *childChild = stackSubtree.top(); stackSubtree.pop();
                         for (int p : childChild->getCNPs()){
@@ -52,35 +53,34 @@
             }
         }
     }
 
 
     
     static void prunningMinByAdaptativeThreshold(ComponentTree *tree, double *attribute, double threshold, int delta, int *imgOutput){
-		bool* selectedPruned = new bool[tree->getNumNodes()]; //nodes pruned
+		std::vector<bool> selectedPruned(tree->getNumNodes(), false); //nodes pruned
 		for(NodeCT *node: tree->getListNodes()){
 			if(node->getParent() != nullptr && attribute[node->getIndex()] <= threshold){
 				if ( attribute[node->getParent()->getIndex()] != attribute[node->getIndex()] ) {
 					selectedPruned[node->getIndex()] = true;
 				}
 			}
 		}
 		
-        ComputerMSER *mser = new ComputerMSER(tree);
-		mser->computerMSER(delta);
+        ComputerMSER mser(tree);
+		mser.computerMSER(delta);
 
-		double *stability = mser->getStabilities();
-		bool *isPruned = new bool[tree->getNumNodes()];
+		std::vector<double> stability = mser.getStabilities();
+		std::vector<bool> isPruned(tree->getNumNodes(), false);
 		for(NodeCT *node: tree->getListNodes()){
-            isPruned[node->getIndex()] = false;
-			if(selectedPruned[node->getIndex()] && stability[node->getIndex()] != INT_MAX && attribute[node->getIndex()] <= threshold){ //node pruned
+            if(selectedPruned[node->getIndex()] && stability[node->getIndex()] != INT_MAX && attribute[node->getIndex()] < threshold){ //node pruned
 				double min = stability[node->getIndex()];
 				
-				int indexDescMinStabilityDesc = mser->descendantNodeWithMinStability(node);
-				int indexAncMinStabilityAsc = mser->ascendantNodeWithMinStability(node);
+				int indexDescMinStabilityDesc = mser.descendantNodeWithMinStability(node);
+				int indexAncMinStabilityAsc = mser.ascendantNodeWithMinStability(node);
 				double minDesc = INT_MIN;
 				double minAnc =  INT_MIN;
 				if(indexDescMinStabilityDesc != -1) {
 					minDesc = stability[indexDescMinStabilityDesc];
 				}
 				if(indexAncMinStabilityAsc != -1) {
 					minAnc = stability[indexAncMinStabilityAsc];
```

### Comparing `morphoaap-0.0.6/morphoaap/include/AttributeProfile.hpp` & `morphoaap-0.0.7/morphoaap/include/AttributeProfile.hpp`

 * *Files 21% similar despite different names*

```diff
@@ -22,10 +22,12 @@
 	
 
 public:
 	AttributeProfile(py::array_t<int> &input, int numRows, int numCols);
 
 	py::array_t<double> getAP(std::list<double> thresholds, int attributeType);
 
+	py::array_t<double> getAAP(std::list<double> thresholds, int attributeType, int delta);
+
 };
 
 #endif
```

### Comparing `morphoaap-0.0.6/morphoaap/morphoaap.cpp` & `morphoaap-0.0.7/morphoaap/morphoaap.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,80 @@
 
 #include "include/NodeCT.hpp"
 #include "include/ComponentTree.hpp"
 #include "include/AttributeProfile.hpp"
 #include "include/AttributeComputedIncrementally.hpp"
 #include "include/AttributeFilters.hpp"
+#include "include/ComputerMSER.hpp"
 
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 #include <pybind11/numpy.h>
 
 namespace py = pybind11;
 
 
 void init_NodeCT(py::module &m){
     py::class_<NodeCT>(m, "NodeCT")
 		.def(py::init<>())
-		.def_property_readonly("rep", &NodeCT::getRep )
+		.def_property_readonly("id", &NodeCT::getIndex )
+        .def_property_readonly("rep", &NodeCT::getRep )
 		.def_property_readonly("cnps", &NodeCT::getCNPs )
 		.def_property_readonly("level", &NodeCT::getLevel )
 		.def_property_readonly("children", &NodeCT::getChildren )
 		.def_property_readonly("parent", &NodeCT::getParent );
 }
 void init_ComponentTree(py::module &m){
       py::class_<ComponentTree>(m, "ComponentTree")
         .def(py::init<py::array_t<int> &, int,int, bool>())
         .def("reconstructionImage", &ComponentTree::reconstructionImage )
-		.def_property_readonly("root", &ComponentTree::getRoot )
-		.def_property_readonly("parent", &ComponentTree::getParent );
+		.def_property_readonly("numNodes", &ComponentTree::getNumNodes )
+        .def_property_readonly("listNodes", &ComponentTree::getListNodes )
+        .def_property_readonly("root", &ComponentTree::getRoot )
+        .def_static("computerParent", &ComponentTree::computerParent);
 
+		//.def_property_readonly("parent", &ComponentTree::getParent );
         //.def("prunningMin", py::overload_cast<py::array_t<double> &, double>(&ComponentTree::prunningMin))
         //.def("prunningMin", &ComponentTree::prunningMin)
         //.def("computerArea", &ComponentTree::computerArea)
         //.def("prunningMin", py::overload_cast<py::array_t<double> &, double>(&ComponentTree::prunningMin))
 }
 
 void init_AttributeProfile(py::module &m){
     	py::class_<AttributeProfile>(m, "AttributeProfile")
         .def(py::init<py::array_t<int> &, int,int>())
-        .def("getAP", &AttributeProfile::getAP );
+        .def("getAP", &AttributeProfile::getAP )
+        .def("getAAP", &AttributeProfile::getAAP );
 }
 
 void init_AttributeComputedIncrementally(py::module &m){
     	py::class_<AttributeComputedIncrementally>(m, "Attribute")
         //.def_static("computerAttribute", &AttributeComputedIncrementally::computerAttribute)
         .def_static("computerArea", &AttributeComputedIncrementally::computerArea);
 }
 
 void init_AttributeFilters(py::module &m){
     py::class_<AttributeFilters>(m, "AttributeFilters")
     .def(py::init<ComponentTree *>())
-    .def("prunningMin", py::overload_cast<py::array_t<double> &, double>(&AttributeFilters::prunningMin));
+    .def("prunningMin", py::overload_cast<py::array_t<double> &, double>(&AttributeFilters::prunningMin))
+    .def("prunningMinByAdaptativeThreshold", py::overload_cast<py::array_t<double> &, double, int>(&AttributeFilters::prunningMinByAdaptativeThreshold));
 }
 
+void init_ComputerMSER(py::module &m){
+    py::class_<ComputerMSER>(m, "ComputerMSER")
+    .def(py::init<ComponentTree *>())
+    .def("computerMSER", &ComputerMSER::computerMSER )
+    .def("getStabilities", &ComputerMSER::getStabilities )
+    .def("getStability", &ComputerMSER::getStability );
+}
 
 PYBIND11_MODULE(morphoaap, m) {
     // Optional docstring
     m.doc() = "Adative attribute profiles";
     
     init_NodeCT(m);
     init_ComponentTree(m);
     init_AttributeProfile(m);
     init_AttributeComputedIncrementally(m);
     init_AttributeFilters(m);
+    init_ComputerMSER(m);
 }
```

### Comparing `morphoaap-0.0.6/morphoaap/src/AttributeComputedIncrementally.cpp` & `morphoaap-0.0.7/morphoaap/src/AttributeComputedIncrementally.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 #include "../include/AttributeComputedIncrementally.hpp"
 
 
 void AttributeComputedIncrementally::preProcessing(NodeCT *v){}
 
 void AttributeComputedIncrementally::mergeChildren(NodeCT *parent, NodeCT *child){}
 
-void AttributeComputedIncrementally::posProcessing(NodeCT *parent){}
+void AttributeComputedIncrementally::postProcessing(NodeCT *parent){}
 
 void AttributeComputedIncrementally::computerAttribute(NodeCT *root) {
         preProcessing(root);
         for (NodeCT *child : root->getChildren())
         {
             computerAttribute(child);
             mergeChildren(root, child);
         }
-        posProcessing(root);
+        postProcessing(root);
 }
```

### Comparing `morphoaap-0.0.6/morphoaap/src/AttributeFilters.cpp` & `morphoaap-0.0.7/morphoaap/src/AttributeFilters.cpp`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.6/morphoaap/src/AttributeProfile.cpp` & `morphoaap-0.0.7/morphoaap/src/AttributeProfile.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 			{ sizeof(int), sizeof(int) * n  }  /* Strides for each dimension */
 	));
 	if(attributeType != 0){
 		std::cout << "attribute type not implemented. At the moment only type (attributeType = 0) of area is available";
         return ap_numpy;
 	}
 
-	double *attributeMintree = new double[this->mintree->getNumNodes()];
-	double *attributeMaxtree = new double[this->maxtree->getNumNodes()]; 
+	double attributeMintree[this->mintree->getNumNodes()];
+	double attributeMaxtree[this->maxtree->getNumNodes()]; 
 	
 	AttributeComputedIncrementally::computerAttribute(this->mintree->getRoot(),
 						[&attributeMintree](NodeCT* node) -> void {
 							attributeMintree[node->getIndex()] = node->getCNPs().size();
 						},
 						[&attributeMintree](NodeCT* root, NodeCT* child) -> void {
 							attributeMintree[root->getIndex()] += attributeMintree[child->getIndex()];
@@ -81,7 +81,72 @@
 		mid_offset += n;
 		offset -= n;
 	}
 		
 	return ap_numpy;
 
 }
+
+
+py::array_t<double> AttributeProfile::getAAP(std::list<double> thresholds, int attributeType, int delta){
+		
+
+	int n = this->numRows * this->numCols;
+	int ap_size = (2*thresholds.size()+1);
+	auto ap_numpy = py::array(py::buffer_info(
+			nullptr,            /* Pointer to data (nullptr -> ask NumPy to allocate!) */
+			sizeof(int),     /* Size of one item */
+			py::format_descriptor<int>::value, /* Buffer format */
+			2,          /* How many dimensions? */
+			{ n, ap_size  },  /* Number of elements for each dimension */
+			{ sizeof(int), sizeof(int) * n  }  /* Strides for each dimension */
+	));
+	if(attributeType != 0){
+		std::cout << "attribute type not implemented. At the moment only type (attributeType = 0) of area is available";
+        return ap_numpy;
+	}
+
+	double attributeMintree[this->mintree->getNumNodes()];
+	double attributeMaxtree[this->maxtree->getNumNodes()]; 
+	
+	AttributeComputedIncrementally::computerAttribute(this->mintree->getRoot(),
+						[&attributeMintree](NodeCT* node) -> void {
+							attributeMintree[node->getIndex()] = node->getCNPs().size();
+						},
+						[&attributeMintree](NodeCT* root, NodeCT* child) -> void {
+							attributeMintree[root->getIndex()] += attributeMintree[child->getIndex()];
+						},
+						[](NodeCT* node) -> void { 							
+						});
+
+	AttributeComputedIncrementally::computerAttribute(this->maxtree->getRoot(),
+						[&attributeMaxtree](NodeCT* node) -> void {
+							attributeMaxtree[node->getIndex()] = node->getCNPs().size();
+						},
+						[&attributeMaxtree](NodeCT* root, NodeCT* child) -> void {
+							attributeMaxtree[root->getIndex()] += attributeMaxtree[child->getIndex()];
+						},
+						[](NodeCT* node) -> void { 							
+						});
+
+
+	auto buf_ap = ap_numpy.request();
+	int *ap = (int *) buf_ap.ptr;
+	int *img = this->mintree->getInputImage();
+	
+	int mid_offset = int(ap_size/2) * n;
+	for (int p=0; p < n; p++){	
+		ap[p + mid_offset] = img[p];	
+	}
+	int offset = mid_offset - n;
+	mid_offset += n;
+	
+	for(double threshold: thresholds){
+		AttributeFilters::prunningMinByAdaptativeThreshold(this->maxtree, attributeMaxtree, threshold, delta, &ap[mid_offset]);
+		AttributeFilters::prunningMinByAdaptativeThreshold(this->mintree, attributeMintree, threshold, delta, &ap[offset]);
+		mid_offset += n;
+		offset -= n;
+	}
+		
+	return ap_numpy;
+
+}
```

### Comparing `morphoaap-0.0.6/morphoaap/src/ComponentTree.cpp` & `morphoaap-0.0.7/morphoaap/src/ComponentTree.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 #include <list>
 #include <vector>
 #include <stack>
 #include <unordered_map>
 
 #include "../include/NodeCT.hpp"
 #include "../include/ComponentTree.hpp"
-
+#include "../include/Adjacency8.hpp"
 
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 #include <pybind11/numpy.h>
 
 
-int* ComponentTree::countingSort(){
+int* ComponentTree::countingSort(int* img){
 	int n = this->numRows * this->numCols;
-	int maxvalue = this->img[0];
+	int maxvalue = img[0];
 	for (int i = 1; i < n; i++)
 		if(maxvalue < img[i]) maxvalue = img[i];
 			
-	std::vector<int> counter(maxvalue + 1, 0);
+	std::vector<int> counter(maxvalue + 1, 0); 
 	int *orderedPixels = new int[n];
 		
 	if(this->isMaxtree()){
 		for (int i = 0; i < n; i++)
-			counter[maxvalue - this->img[i]]++;
+			counter[maxvalue - img[i]]++;
 
 		for (int i = 1; i < maxvalue; i++) 
 			counter[i] += counter[i - 1];
 		counter[maxvalue] += counter[maxvalue-1];
 
 		
 		for (int i = n - 1; i >= 0; --i)
 			orderedPixels[--counter[maxvalue - img[i]]] = i;
 	}else{
 		for (int i = 0; i < n; i++)
-			counter[this->img[i]]++;
+			counter[img[i]]++;
 
 		for (int i = 1; i < maxvalue; i++) 
 			counter[i] += counter[i - 1];
 		counter[maxvalue] += counter[maxvalue-1];
 
 		
 		for (int i = n - 1; i >= 0; --i)
@@ -53,136 +53,126 @@
 		return x;
 	else {
 		zPar[x] = findRoot(zPar, zPar[x]);
 		return zPar[x];
 	}
 }
 
-int ComponentTree::coord2Index(int row, int col) {
-	return (row * this->numCols) + col;
-}
-
-
-std::vector<int> ComponentTree::getAdjPixels(int index) {
-	int row = index / this->numCols;
-	int col = index % this->numCols;
-	std::vector<int> listAdj(8);
-	for (int l=row - 1; l <= row + 1; l++ )
-		for(int c=col -1; c <= col + 1; c++)
-			if (l >= 0 && c >= 0 && l < this->numRows && c < this->numCols) 
-				listAdj.push_back( coord2Index(l, c) );
-			
-		
-	return listAdj;
-}
-
-
-
-void ComponentTree::createTreeByUnionFind() {
+int* ComponentTree::createTreeByUnionFind(int* orderedPixels, int* img) {
 	const int n = this->numRows * this->numCols;
-
+	Adjacency8 adj(this->numRows, this->numCols);
 	int *zPar = new int[n];
+	int *parent = new int[n];
 		
 	for (int p = 0; p < n; p++) {
 		zPar[p] =  -1;
 	}
 		
 	for(int i=n-1; i >= 0; i--){
-		int p = this->orderedPixels[i];
-		this->parent[p] = p;
+		int p = orderedPixels[i];
+		parent[p] = p;
 		zPar[p] = p;
-		for (int n : this->getAdjPixels(p)) {
+		for (int n : adj.getAdjPixels(p)) {
 			if(zPar[n] != -1){
 				int r = this->findRoot(zPar, n);
 				if(p != r){
-					this->parent[r] = p;
+					parent[r] = p;
 					zPar[r] = p;
 				}
 			}
 		}
 	}
 			
 	// canonizacao da arvore
 	for (int i = 0; i < n; i++) {
-		int p = this->orderedPixels[i];
-		int q = this->parent[p];
+		int p = orderedPixels[i];
+		int q = parent[p];
 				
-		if(img[this->parent[q]] == img[q]){
-			this->parent[p] = this->parent[q];
+		if(img[parent[q]] == img[q]){
+			parent[p] = parent[q];
 		}
 	}
 		
-	delete[] zPar;		
+	delete[] zPar;
+	return parent;		
 }
 
-void ComponentTree::reconstruction(NodeCT* node, int* img){
+void ComponentTree::reconstruction(NodeCT* node, int* imgOut){
 	for (int p : node->getCNPs()){
-		img[p] = node->getLevel();
+		imgOut[p] = node->getLevel();
 	}
 	for(NodeCT* child: node->getChildren()){
-		reconstruction(child, img);
+		reconstruction(child, imgOut);
 	}
 }
 
+ComponentTree::ComponentTree(int numRows, int numCols, bool isMaxtree){
+	this->numRows = numRows;
+	this->numCols = numCols;
+	this->maxtreeTreeType = isMaxtree;
+ }
+
 ComponentTree::ComponentTree(py::array_t<int> &input, int numRows, int numCols, bool isMaxtree){
 	this->numRows = numRows;
 	this->numCols = numCols;
 	this->maxtreeTreeType = isMaxtree;
 		
 	auto buf_input = input.request();
 		
-	this->img = (int *) buf_input.ptr;
-
-	int n = n = this->numRows * this->numCols;
-	this->parent = new int[ n ];
-	this->orderedPixels = countingSort();
+	int* img = (int *) buf_input.ptr;
 
-	createTreeByUnionFind();
+	int n = this->numRows * this->numCols;
+	//this->parent = new int[ n ];
+	int* orderedPixels = countingSort(img);
+	int* parent = createTreeByUnionFind(orderedPixels, img);
 		
 	std::unordered_map<int, NodeCT*> nodes;
 	this->numNodes = 0;
 	for (int i = 0; i < n; i++) {
-		int p = this->orderedPixels[i];
-		if (p == this->parent[p]) { //representante do node raiz
-			this->root = nodes[p] = new NodeCT(this->numNodes++, p, nullptr, this->img[p]);
+		int p = orderedPixels[i];
+		if (p == parent[p]) { //representante do node raiz
+			this->root = nodes[p] = new NodeCT(this->numNodes++, p, nullptr, img[p]);
 			this->listNodes.push_back(nodes[p]);
 			nodes[p]->addCNPs(p);
 		}
-		else if (this->img[p] != this->img[this->parent[p]]) { //representante de um node
-			nodes[p] = new NodeCT(this->numNodes++, p, nodes[this->parent[p]], this->img[p]);
+		else if (img[p] != img[parent[p]]) { //representante de um node
+			nodes[p] = new NodeCT(this->numNodes++, p, nodes[parent[p]], img[p]);
 			this->listNodes.push_back(nodes[p]);
 			nodes[p]->addCNPs(p);
-			nodes[this->parent[p]]->addChild(nodes[p]);
+			nodes[parent[p]]->addChild(nodes[p]);
 		}
-		else if (this->img[p] == this->img[this->parent[p]]) {
-			nodes[this->parent[p]]->addCNPs(p);
+		else if (img[p] == img[parent[p]]) {
+			nodes[parent[p]]->addCNPs(p);
 		}
 	}
+
+	delete[] parent;
+	delete[] orderedPixels;
 }
 
+/*
 py::array_t<int> ComponentTree::getParent(){
 		
 	int n = this->numRows * this->numCols;
 		
 	auto parent_numpy = py::array(py::buffer_info(
-		this->parent,            /* Pointer to data (nullptr -> ask NumPy to allocate!) */
-		sizeof(int),     /* Size of one item */
-		py::format_descriptor<int>::value, /* Buffer format */
-		1,          /* How many dimensions? */
-		{ ( n ) },  /* Number of elements for each dimension */
-		{ sizeof(int) }  /* Strides for each dimension */
+		this->parent,            // Pointer to data (nullptr -> ask NumPy to allocate!) 
+		sizeof(int),     // Size of one item 
+		py::format_descriptor<int>::value, // Buffer format 
+		1,          // How many dimensions? 
+		{ ( n ) },  // Number of elements for each dimension 
+		{ sizeof(int) }  // Strides for each dimension 
 	));
-		
 
 	return parent_numpy;
 }
 
 int* ComponentTree::getInputImage(){
 	return this->img;
-}
+}*/
 	
 NodeCT* ComponentTree::getRoot() {
 	return this->root;
 }
 
 bool ComponentTree::isMaxtree(){
 	return this->maxtreeTreeType;
@@ -212,12 +202,38 @@
 			sizeof(int),     /* Size of one item */
 			py::format_descriptor<int>::value, /* Buffer format */
 			1,          /* How many dimensions? */
 			{ ( n ) },  /* Number of elements for each dimension */
 			{ sizeof(int) }  /* Strides for each dimension */
 	));
 	auto buf_img = img_numpy.request();
-	int *img = (int *) buf_img.ptr;
-	this->reconstruction(this->root, img);
+	int *imgOut = (int *) buf_img.ptr;
+	this->reconstruction(this->root, imgOut);
 	return img_numpy;
 
 }
+
+int* ComponentTree::getInputImage(){
+	int n = this->numRows * this->numCols;
+	int* img = new int[n];
+	this->reconstruction(this->root, img);
+	return img;
+}
+	
+/*
+int ComponentTree::coord2Index(int row, int col) {
+	return (row * this->numCols) + col;
+}
+
+
+std::vector<int> ComponentTree::getAdjPixels(int index) {
+	int row = index / this->numCols;
+	int col = index % this->numCols;
+	std::vector<int> listAdj(8);
+	for (int l=row - 1; l <= row + 1; l++ )
+		for(int c=col -1; c <= col + 1; c++)
+			if (l >= 0 && c >= 0 && l < this->numRows && c < this->numCols) 
+				listAdj.push_back( coord2Index(l, c) );
+			
+		
+	return listAdj;
+}*/
```

### Comparing `morphoaap-0.0.6/morphoaap/src/ComputerMSER.cpp` & `morphoaap-0.0.7/morphoaap/src/ComputerMSER.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 			if(this->tree->isMaxtree()){
 				if(node->getLevel() >= n->getLevel() + h)
 					return n;
 			}else{
 				if(node->getLevel() <= n->getLevel() - h)
 					return n;
 			}
-			if(n->getParent() != this->tree->getRoot())
+			if(n->getParent() != nullptr)
 				n = n->getParent();
 			else 
 				return n;
 		}
 		return n;
 	}
 
@@ -36,102 +36,97 @@
 		if( this->attribute[ this->descendants[nodeAsc->getIndex()] ] < this->attribute[ nodeDes->getIndex() ])
 			this->descendants[nodeAsc->getIndex()] = nodeDes->getIndex();
 		
 	}
 	
 	double ComputerMSER::getStability(NodeCT* node){
 		if(this->ascendant[node->getIndex()] != -1 && this->descendants[node->getIndex()] != -1){
-			return ( this->attribute[ascendant[node->getIndex()]] - this->attribute[this->descendants[node->getIndex()]]) / double(this->attribute[node->getIndex()]);
+			return (this->attribute[ascendant[node->getIndex()]] - this->attribute[this->descendants[node->getIndex()]]) / ( (double) this->attribute[node->getIndex()]);
 		}
 		else{
 			return INT_MAX;
 		}
 	}
 
 
 	ComputerMSER::ComputerMSER(ComponentTree* tree){
 		this->tree = tree;
 		this->maxVariation = 0.5;
 		this->minArea = 0;
+		this->maxArea = INT_MAX;
 
-		double *_attribute = new double[this->tree->getNumNodes()]; 
+		double _attribute[this->tree->getNumNodes()]; 
 		AttributeComputedIncrementally::computerAttribute(this->tree->getRoot(),
 						[&_attribute](NodeCT* node) -> void {
 							_attribute[node->getIndex()] = node->getCNPs().size();
 						},
 						[&_attribute](NodeCT* root, NodeCT* child) -> void {
 							_attribute[root->getIndex()] += _attribute[child->getIndex()];
 						},
 						[](NodeCT* node) -> void { 							
 						});
 
 		this->attribute = _attribute;
-		this->maxArea = attribute[tree->getRoot()->getIndex()];
+		
 	}
 
-	bool* ComputerMSER::computerMSER(int delta){
-		this->ascendant = new int[this->tree->getNumNodes()];
-		this->descendants = new int[this->tree->getNumNodes()];
-		bool *mser = new bool[this->tree->getNumNodes()];
-		this->num = 0;
-		for(int i=0; i < this->tree->getNumNodes(); i++){
-			this->ascendant[i] = -1;
-			this->descendants[i] = -1;
-			mser[i] = false;
-		}
+	std::vector<bool> ComputerMSER::computerMSER(int delta){
+
+		std::vector<int> tmp_asc (this->tree->getNumNodes(), -1);
+		this->ascendant = tmp_asc;
 
+		std::vector<int> tmp_des (this->tree->getNumNodes(), -1);
+		this->descendants = tmp_des;
+
+		std::vector<double> tmp_stab (this->tree->getNumNodes(), -1);
+		this->stability = tmp_stab;
+		
 		for(NodeCT *node: tree->getListNodes()){
 			NodeCT *nodeAsc = this->getNodeAscendant(node, delta);
 			this->maxAreaDescendants(nodeAsc, node);
 			this->ascendant[node->getIndex()] = nodeAsc->getIndex();
 		}
-
-		this->stability = new double[this->tree->getNumNodes()];
+		
 		for(NodeCT *node: tree->getListNodes()){
 			if(this->ascendant[node->getIndex()] != -1 && this->descendants[node->getIndex()] != -1){
 				this->stability[node->getIndex()] = this->getStability(node);
 			}else{
 				this->stability[node->getIndex()] = INT_MAX;
 			}
 			
 		}
-
-
+		
+		this->num = 0;
+		double minStabilityDesc, minStabilityAsc;
+		std::vector<bool> mser(this->tree->getNumNodes(), false);
 		for(NodeCT *node: tree->getListNodes()){
-			if(this->stability[node->getIndex()] != -1 && this->stability[this->ascendant[node->getIndex()] ] != -1 && this->stability[this->descendants[node->getIndex()]] != -1){
-				double minStabilityDesc = this->stability[this->descendants[node->getIndex()]];
-				double minStabilityAsc = this->stability[this->ascendant[node->getIndex()]];
+			if(this->stability[node->getIndex()] != INT_MAX && this->stability[this->ascendant[node->getIndex()] ] != INT_MAX && this->stability[this->descendants[node->getIndex()]] != INT_MAX){
+				minStabilityDesc = this->stability[this->descendants[node->getIndex()]];
+				minStabilityAsc = this->stability[this->ascendant[node->getIndex()]];
 				if(this->stability[node->getIndex()] < minStabilityDesc && this->stability[node->getIndex()] < minStabilityAsc){
 					if(stability[node->getIndex()] < maxVariation && this->attribute[node->getIndex()] >= minArea && this->attribute[node->getIndex()] <= maxArea){
 						mser[node->getIndex()] = true;
 						this->num++;
 					}
 				}
 			}
 		}
-
 		return mser;
 	}
 
 
 	int ComputerMSER::descendantNodeWithMinStability(NodeCT* node) {
-		if( this->stability[this->descendants[node->getIndex()] ] != -1)
-			return this->descendants[node->getIndex()];
-		else
-			return -1;
+		return this->descendants[node->getIndex()];
 	}
 	
-	double* ComputerMSER::getStabilities(){
+	std::vector<double> ComputerMSER::getStabilities(){
 		return this->stability;
 	}
 
     int ComputerMSER::ascendantNodeWithMinStability(NodeCT* node) {
-		if( this->stability[this->ascendant[node->getIndex()] ] != -1)
-			return this->ascendant[node->getIndex()];
-		else
-			return -1;
+		return this->ascendant[node->getIndex()];
 	}
 
 	int ComputerMSER::getNumNodes() {
 		return  num;
 	}
```

### Comparing `morphoaap-0.0.6/morphoaap/src/NodeCT.cpp` & `morphoaap-0.0.7/morphoaap/src/NodeCT.cpp`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.6/morphoaap.egg-info/PKG-INFO` & `morphoaap-0.0.7/morphoaap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: morphoaap
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple library for adative attribute profiles
 Home-page: https://github.com/wonderalexandre/aap
 Author: Wonder Alexandre Luz Alves
 Author-email: worderalexandre@gmail.com
 License: GPL-3.0
 Description: UNKNOWN
 Keywords: attribute profiles,mathematical morphology,morphological trees
```

### Comparing `morphoaap-0.0.6/morphoaap.egg-info/SOURCES.txt` & `morphoaap-0.0.7/morphoaap.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 morphoaap/CMakeLists.txt
 morphoaap/morphoaap.cpp
 morphoaap.egg-info/PKG-INFO
 morphoaap.egg-info/SOURCES.txt
 morphoaap.egg-info/dependency_links.txt
 morphoaap.egg-info/not-zip-safe
 morphoaap.egg-info/top_level.txt
+morphoaap/include/Adjacency8.hpp
 morphoaap/include/AttributeComputedIncrementally.hpp
 morphoaap/include/AttributeFilters.hpp
 morphoaap/include/AttributeProfile.hpp
 morphoaap/include/ComponentTree.hpp
 morphoaap/include/ComputerMSER.hpp
 morphoaap/include/NodeCT.hpp
+morphoaap/src/Adjacency8.cpp
 morphoaap/src/AttributeComputedIncrementally.cpp
 morphoaap/src/AttributeFilters.cpp
 morphoaap/src/AttributeProfile.cpp
 morphoaap/src/ComponentTree.cpp
 morphoaap/src/ComputerMSER.cpp
 morphoaap/src/NodeCT.cpp
```

### Comparing `morphoaap-0.0.6/setup.py` & `morphoaap-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     source_path = extdir / self.get_ext_filename(ext.name)
     dest_directory = dest_path.parents[0]
     dest_directory.mkdir(parents=True, exist_ok=True)
     self.copy_file(source_path, dest_path)
 
 setup(
   name="morphoaap",
-  version="0.0.6",
+  version="0.0.7",
   description="A simple library for adative attribute profiles",
   long_description="",
   author="Wonder Alexandre Luz Alves",
   author_email="worderalexandre@gmail.com",
   license="GPL-3.0",
   url= "https://github.com/wonderalexandre/aap",
   #packages=["morphoaap"],
```

