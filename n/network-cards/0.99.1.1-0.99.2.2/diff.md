# Comparing `tmp/network-cards-0.99.1.1.tar.gz` & `tmp/network_cards-0.99.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "network-cards-0.99.1.1.tar", max compression
+gzip compressed data, was "network_cards-0.99.2.2.tar", max compression
```

## Comparing `network-cards-0.99.1.1.tar` & `network_cards-0.99.2.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1521 2022-05-23 15:35:20.251503 network-cards-0.99.1.1/LICENSE
--rw-r--r--   0        0        0     6155 2022-05-27 15:06:03.714433 network-cards-0.99.1.1/README.md
--rw-r--r--   0        0        0      397 2022-05-27 18:32:55.802784 network-cards-0.99.1.1/pyproject.toml
--rw-r--r--   0        0        0      128 2022-05-27 18:25:29.069843 network-cards-0.99.1.1/src/network_cards/__init__.py
--rw-r--r--   0        0        0     7268 2022-05-16 20:05:30.829499 network-cards-0.99.1.1/src/network_cards/format_helpers.py
--rw-r--r--   0        0        0    32846 2022-05-27 18:21:26.136191 network-cards-0.99.1.1/src/network_cards/network_cards.py
--rw-r--r--   0        0        0     7046 2022-05-27 18:33:23.343776 network-cards-0.99.1.1/setup.py
--rw-r--r--   0        0        0     6711 2022-05-27 18:33:23.344663 network-cards-0.99.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1521 2022-05-23 15:35:20.251503 network_cards-0.99.2.2/LICENSE
+-rw-r--r--   0        0        0     6374 2023-08-01 16:44:29.430823 network_cards-0.99.2.2/README.md
+-rw-r--r--   0        0        0      397 2023-08-01 16:49:02.723420 network_cards-0.99.2.2/pyproject.toml
+-rw-r--r--   0        0        0      128 2022-05-27 18:25:29.069843 network_cards-0.99.2.2/src/network_cards/__init__.py
+-rw-r--r--   0        0        0     7268 2022-05-16 20:05:30.829499 network_cards-0.99.2.2/src/network_cards/format_helpers.py
+-rw-r--r--   0        0        0    32999 2022-09-27 19:06:59.077730 network_cards-0.99.2.2/src/network_cards/network_cards.py
+-rw-r--r--   0        0        0     6981 1970-01-01 00:00:00.000000 network_cards-0.99.2.2/PKG-INFO
```

### Comparing `network-cards-0.99.1.1/LICENSE` & `network_cards-0.99.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `network-cards-0.99.1.1/README.md` & `network_cards-0.99.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 # Network Cards
 
 A network card is a three-panel tabular summary of a network dataset:
 
 <p align='center'>
-<img src='network-card-example.png' alt='Example network card for the Zachary Karate Club' width='600'>
+<img src='https://raw.githubusercontent.com/network-cards/network-cards/main/network-card-example.png' alt='Example network card for the Zachary Karate Club' width='600'>
 </p>
 
 The first panel provides an overall summary of the network, the second summarizes the structure of the network (size, density, connectivity), and the third panel provides additional meta-information, what metadata are associated with nodes and links, how were the data gathered, and so forth.
 
 Network cards are intended to be _concise, readable and flexible_, allowing researchers across fields to quickly read and understand studies involving network datasets. 
 We believe that a standard representation is crucial to ensuring that key information associated with network data remains available.
 
 This repository provides [templates](templates/) and a [Python package](#install) to create, update, and export network cards.
 
+Interested in more? Check out [the paper][1].
+
 ## Table of Contents
 
-* [Example](#example)
 * [Install](#install)
 	- [Requirements](#requirements)
+* [Example](#example)
 * [Citation](#citation)
 * [License](#License)
 
 
+## Install
+
+`pip install network-cards`
+
+#### Requirements
+
+* Python 3.8+
+* Networkx
+* Pandas
+
+
 
 
 ## Example
 
 `Network Cards` provides [fill-in templates](templates/) but you can also generate and save a card programmatically. 
 Here's Python code where we load a network from a file and compute the basic card: 
 
@@ -118,29 +131,18 @@
 ```python
 card.to_latex("karate-card.tex")
 card.to_excel("karate-card.xlsx")
 ```
 
 
 
-## Install
-
-`pip install network-cards`
-
-#### Requirements
-
-* Python 3.8+
-* Networkx
-* Pandas
-
-
 
 ## Citation
 
-If you use a Network Card, please cite our paper:
+If you use a Network Card, please cite [our paper][1]:
 
 Bagrow, J., & Ahn, Y. (2022). Network Cards: concise, readable summaries of network data
 
 Here is a bibtex entry ([.bib file](references/citation.bib)):
 
 ```bibtex
 @unpublished{bagrow2022cards,
@@ -162,7 +164,9 @@
 ER  - 
 ```
 
 ## License
 
 [BSD-3-Clause](LICENSE) © James Bagrow
 
+
+[1]: https://arxiv.org/abs/2206.00026 "Network Cards: concise, readable summaries of network data"
```

### Comparing `network-cards-0.99.1.1/src/network_cards/format_helpers.py` & `network_cards-0.99.2.2/src/network_cards/format_helpers.py`

 * *Files identical despite different names*

### Comparing `network-cards-0.99.1.1/src/network_cards/network_cards.py` & `network_cards-0.99.2.2/src/network_cards/network_cards.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # network_cards.py
 # Jim Bagrow
-# Last Modified: 2022-05-27
+# Last Modified: 2022-09-27
 
 import json
 import random
 import pprint
 from collections import OrderedDict
 import numpy as np
 import pandas as pd
@@ -46,14 +46,15 @@
                Node metadata  Age, gender
                Link metadata  Communication medium (phone or email)
             Date of creation  N/A
      Data generating process  Field survey
                       Ethics  All participants gave informed consent
                      Funding  N/A
                     Citation  N/A
+                      Access  https://example.org/data
     """
     _null_string = ""
 
     def __init__(self, graph, initialize=True):
         """Initialize a network card for `graph`.
         """
         self.graph = graph
@@ -83,14 +84,15 @@
             self.update_metainfo("Node metadata")
             self.update_metainfo("Link metadata")
             self.update_metainfo("Date of creation")
             self.update_metainfo("Data generating process")
             self.update_metainfo("Ethics")
             self.update_metainfo("Funding")
             self.update_metainfo("Citation")
+            self.update_metainfo("Access")
 
         self._sizes()
 
     def _str_labeler(self, label, func):
         return {label: func(self.graph)}
 
     def label_name(self, unnamed=""):
@@ -155,15 +157,16 @@
     def label_links(self):
         """Get entry for network's number of links. Intended for card's
         structure panel.
         """
         nsl = nx.number_of_selfloops(self.graph)
         if nsl > 0:
             m = nx.number_of_edges(self.graph)
-            return {'Number of links': f"{m} ({nsl} self-loops)"}
+            lbl = 'self-loop' if nsl == 1 else 'self-loops'
+            return {'Number of links': f"{m} ({nsl} {lbl})"}
         return self._str_labeler("Number of links", nx.number_of_edges)
 
     def label_bidirectional_links(self):
         """Get entry for network's proportion (%) of bidirectional link.
         Intended for card's structure panel. Intended for directed networks.
 
         A bidirectional link is one where both (i,j) and (j,i) links exist.
```

### Comparing `network-cards-0.99.1.1/setup.py` & `network_cards-0.99.2.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,190 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: network-cards
+Version: 0.99.2.2
+Summary: Concise, readable summaries of network data
+License: BSD-3-Clause
+Author: James Bagrow
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: networkx (>=2.8.2,<3.0.0)
+Requires-Dist: pandas (>=1.4.2,<2.0.0)
+Description-Content-Type: text/markdown
+
+# Network Cards
+
+A network card is a three-panel tabular summary of a network dataset:
+
+<p align='center'>
+<img src='https://raw.githubusercontent.com/network-cards/network-cards/main/network-card-example.png' alt='Example network card for the Zachary Karate Club' width='600'>
+</p>
+
+The first panel provides an overall summary of the network, the second summarizes the structure of the network (size, density, connectivity), and the third panel provides additional meta-information, what metadata are associated with nodes and links, how were the data gathered, and so forth.
+
+Network cards are intended to be _concise, readable and flexible_, allowing researchers across fields to quickly read and understand studies involving network datasets. 
+We believe that a standard representation is crucial to ensuring that key information associated with network data remains available.
+
+This repository provides [templates](templates/) and a [Python package](#install) to create, update, and export network cards.
+
+Interested in more? Check out [the paper][1].
+
+## Table of Contents
+
+* [Install](#install)
+	- [Requirements](#requirements)
+* [Example](#example)
+* [Citation](#citation)
+* [License](#License)
+
+
+## Install
+
+`pip install network-cards`
+
+#### Requirements
+
+* Python 3.8+
+* Networkx
+* Pandas
+
+
+
+
+## Example
+
+`Network Cards` provides [fill-in templates](templates/) but you can also generate and save a card programmatically. 
+Here's Python code where we load a network from a file and compute the basic card: 
+
+```python
+import networkx as nx
+import network_cards as nc
+
+G = nx.read_edgelist("karate_club.edgelist")
+
+card = nc.NetworkCard(G)
+print(card)
+```
+This gives:
+
+```text
+                   Name                       
+                   Kind Undirected, unweighted
+              Nodes are                       
+              Links are                       
+         Considerations                       
+        Number of nodes                     34
+        Number of links                     78
+               Degree^1        4.58824 [1, 17]
+             Clustering                  0.571
+              Connected                    Yes
+               Diameter                      5
+ Assortativity (degree)                 -0.476
+          Node metadata                       
+          Link metadata                       
+       Date of creation                       
+Data generating process                       
+                 Ethics                       
+                Funding                       
+               Citation                       
+
+^1: Distributions summarized with average [min, max].
+```
+
+Unfortunately, few of the important definitions, details or meta-information are computable, so
+most of the fields outside the structure panel are blank.
+Let's use `update_*` methods to populate the remaining fields ourselves:
+
+```python
+card.update_overall("Name", "Zachary Karate Club")
+card.update_overall("Nodes are", "Members of club at US university")
+card.update_overall("Links are", "Members consistently interacted outside club")
+card.update_overall("Considerations", "Heavily used as an example network")
+
+card.update_metainfo({
+    "Node metadata":           "None",
+    "Link metadata":           "None (original study included eight interaction contexts)",
+    "Date of creation":        "1977",
+    "Data generating process": "Direct observation of club members during period 1970-72",
+    "Funding":                 "None",
+    "Citation":                "Zachary (1977)"
+    })
+```
+
+We used `card.update_overall()` and `card.update_metainfo()` to insert entries into the previous card. 
+Entries can be updated one at a time (like we did when updating the overall panel) or a dictionary can be passed to update multiple entries at once.
+
+Now, print the revised card with `print(card)`:
+
+```text
+                   Name                                       Zachary Karate Club
+                   Kind                                    Undirected, unweighted
+              Nodes are                          Members of club at US university
+              Links are              Members consistently interacted outside club
+         Considerations                        Heavily used as an example network
+        Number of nodes                                                        34
+        Number of links                                                        78
+               Degree^1                                           4.58824 [1, 17]
+             Clustering                                                     0.571
+              Connected                                                       Yes
+               Diameter                                                         5
+ Assortativity (degree)                                                    -0.476
+          Node metadata                                                      None
+          Link metadata None (original study included eight interaction contexts)
+       Date of creation                                                      1977
+Data generating process  Direct observation of club members during period 1970-72
+                 Ethics                                                          
+                Funding                                                      None
+               Citation                                            Zachary (1977)
+
+^1: Distributions summarized with average [min, max].
+```
+
+And we can save to a convenient file format:
+
+```python
+card.to_latex("karate-card.tex")
+card.to_excel("karate-card.xlsx")
+```
+
+
+
+
+## Citation
+
+If you use a Network Card, please cite [our paper][1]:
+
+Bagrow, J., & Ahn, Y. (2022). Network Cards: concise, readable summaries of network data
+
+Here is a bibtex entry ([.bib file](references/citation.bib)):
+
+```bibtex
+@unpublished{bagrow2022cards,
+	author = {Bagrow, James and Ahn, Yong-Yeol},
+	title  = {Network Cards: concise, readable summaries of network data},
+	year   = {2022},
+}
+```
 
-package_dir = \
-{'': 'src'}
+and a .ris entry ([.ris file](references/citation.ris)):
 
-packages = \
-['network_cards']
+```text
+TY  - UNPB
+AU  - Bagrow, James
+AU  - Ahn, Yong-Yeol
+TI  - Network Cards: concise, readable summaries of network data
+PY  - 2022
+DA  - 2022
+ER  - 
+```
+
+## License
+
+[BSD-3-Clause](LICENSE) © James Bagrow
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['networkx>=2.8.2,<3.0.0', 'pandas>=1.4.2,<2.0.0']
-
-setup_kwargs = {
-    'name': 'network-cards',
-    'version': '0.99.1.1',
-    'description': 'Concise, readable summaries of network data',
-    'long_description': '# Network Cards\n\nA network card is a three-panel tabular summary of a network dataset:\n\n<p align=\'center\'>\n<img src=\'network-card-example.png\' alt=\'Example network card for the Zachary Karate Club\' width=\'600\'>\n</p>\n\nThe first panel provides an overall summary of the network, the second summarizes the structure of the network (size, density, connectivity), and the third panel provides additional meta-information, what metadata are associated with nodes and links, how were the data gathered, and so forth.\n\nNetwork cards are intended to be _concise, readable and flexible_, allowing researchers across fields to quickly read and understand studies involving network datasets. \nWe believe that a standard representation is crucial to ensuring that key information associated with network data remains available.\n\nThis repository provides [templates](templates/) and a [Python package](#install) to create, update, and export network cards.\n\n## Table of Contents\n\n* [Example](#example)\n* [Install](#install)\n\t- [Requirements](#requirements)\n* [Citation](#citation)\n* [License](#License)\n\n\n\n\n## Example\n\n`Network Cards` provides [fill-in templates](templates/) but you can also generate and save a card programmatically. \nHere\'s Python code where we load a network from a file and compute the basic card: \n\n```python\nimport networkx as nx\nimport network_cards as nc\n\nG = nx.read_edgelist("karate_club.edgelist")\n\ncard = nc.NetworkCard(G)\nprint(card)\n```\nThis gives:\n\n```text\n                   Name                       \n                   Kind Undirected, unweighted\n              Nodes are                       \n              Links are                       \n         Considerations                       \n        Number of nodes                     34\n        Number of links                     78\n               Degree^1        4.58824 [1, 17]\n             Clustering                  0.571\n              Connected                    Yes\n               Diameter                      5\n Assortativity (degree)                 -0.476\n          Node metadata                       \n          Link metadata                       \n       Date of creation                       \nData generating process                       \n                 Ethics                       \n                Funding                       \n               Citation                       \n\n^1: Distributions summarized with average [min, max].\n```\n\nUnfortunately, few of the important definitions, details or meta-information are computable, so\nmost of the fields outside the structure panel are blank.\nLet\'s use `update_*` methods to populate the remaining fields ourselves:\n\n```python\ncard.update_overall("Name", "Zachary Karate Club")\ncard.update_overall("Nodes are", "Members of club at US university")\ncard.update_overall("Links are", "Members consistently interacted outside club")\ncard.update_overall("Considerations", "Heavily used as an example network")\n\ncard.update_metainfo({\n    "Node metadata":           "None",\n    "Link metadata":           "None (original study included eight interaction contexts)",\n    "Date of creation":        "1977",\n    "Data generating process": "Direct observation of club members during period 1970-72",\n    "Funding":                 "None",\n    "Citation":                "Zachary (1977)"\n    })\n```\n\nWe used `card.update_overall()` and `card.update_metainfo()` to insert entries into the previous card. \nEntries can be updated one at a time (like we did when updating the overall panel) or a dictionary can be passed to update multiple entries at once.\n\nNow, print the revised card with `print(card)`:\n\n```text\n                   Name                                       Zachary Karate Club\n                   Kind                                    Undirected, unweighted\n              Nodes are                          Members of club at US university\n              Links are              Members consistently interacted outside club\n         Considerations                        Heavily used as an example network\n        Number of nodes                                                        34\n        Number of links                                                        78\n               Degree^1                                           4.58824 [1, 17]\n             Clustering                                                     0.571\n              Connected                                                       Yes\n               Diameter                                                         5\n Assortativity (degree)                                                    -0.476\n          Node metadata                                                      None\n          Link metadata None (original study included eight interaction contexts)\n       Date of creation                                                      1977\nData generating process  Direct observation of club members during period 1970-72\n                 Ethics                                                          \n                Funding                                                      None\n               Citation                                            Zachary (1977)\n\n^1: Distributions summarized with average [min, max].\n```\n\nAnd we can save to a convenient file format:\n\n```python\ncard.to_latex("karate-card.tex")\ncard.to_excel("karate-card.xlsx")\n```\n\n\n\n## Install\n\n`pip install network-cards`\n\n#### Requirements\n\n* Python 3.8+\n* Networkx\n* Pandas\n\n\n\n## Citation\n\nIf you use a Network Card, please cite our paper:\n\nBagrow, J., & Ahn, Y. (2022). Network Cards: concise, readable summaries of network data\n\nHere is a bibtex entry ([.bib file](references/citation.bib)):\n\n```bibtex\n@unpublished{bagrow2022cards,\n\tauthor = {Bagrow, James and Ahn, Yong-Yeol},\n\ttitle  = {Network Cards: concise, readable summaries of network data},\n\tyear   = {2022},\n}\n```\n\nand a .ris entry ([.ris file](references/citation.ris)):\n\n```text\nTY  - UNPB\nAU  - Bagrow, James\nAU  - Ahn, Yong-Yeol\nTI  - Network Cards: concise, readable summaries of network data\nPY  - 2022\nDA  - 2022\nER  - \n```\n\n## License\n\n[BSD-3-Clause](LICENSE) © James Bagrow\n\n',
-    'author': 'James Bagrow',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
 
+[1]: https://arxiv.org/abs/2206.00026 "Network Cards: concise, readable summaries of network data"
 
-setup(**setup_kwargs)
```

