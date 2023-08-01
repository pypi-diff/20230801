# Comparing `tmp/SGtSNEpiPy-1.1.4.tar.gz` & `tmp/SGtSNEpiPy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SGtSNEpiPy-1.1.4.tar", last modified: Sun Jul 30 04:59:13 2023, max compression
+gzip compressed data, was "SGtSNEpiPy-1.1.5.tar", last modified: Tue Aug  1 00:42:39 2023, max compression
```

## Comparing `SGtSNEpiPy-1.1.4.tar` & `SGtSNEpiPy-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 04:59:13.987742 SGtSNEpiPy-1.1.4/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     9046 2023-07-30 04:59:13.987854 SGtSNEpiPy-1.1.4/PKG-INFO
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     8652 2023-07-30 04:58:55.000000 SGtSNEpiPy-1.1.4/README.md
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       38 2023-07-30 04:59:13.988199 SGtSNEpiPy-1.1.4/setup.cfg
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      808 2023-07-30 04:58:50.000000 SGtSNEpiPy-1.1.4/setup.py
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 04:59:13.985775 SGtSNEpiPy-1.1.4/src/
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 04:59:13.986801 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     2055 2023-07-28 17:34:50.000000 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy/SGtSNEpiPy.py
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy/__init__.py
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 04:59:13.987578 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy.egg-info/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     9046 2023-07-30 04:59:13.000000 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy.egg-info/PKG-INFO
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      273 2023-07-30 04:59:13.000000 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy.egg-info/SOURCES.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        1 2023-07-30 04:59:13.000000 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy.egg-info/dependency_links.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       18 2023-07-30 04:59:13.000000 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy.egg-info/requires.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       11 2023-07-30 04:59:13.000000 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy.egg-info/top_level.txt
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-08-01 00:42:39.818016 SGtSNEpiPy-1.1.5/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)    13061 2023-08-01 00:42:39.818146 SGtSNEpiPy-1.1.5/PKG-INFO
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)    12668 2023-08-01 00:40:47.000000 SGtSNEpiPy-1.1.5/README.md
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       38 2023-08-01 00:42:39.818524 SGtSNEpiPy-1.1.5/setup.cfg
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      808 2023-08-01 00:41:25.000000 SGtSNEpiPy-1.1.5/setup.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-08-01 00:42:39.815923 SGtSNEpiPy-1.1.5/src/
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-08-01 00:42:39.817046 SGtSNEpiPy-1.1.5/src/SGtSNEpiPy/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     2055 2023-07-28 17:34:50.000000 SGtSNEpiPy-1.1.5/src/SGtSNEpiPy/SGtSNEpiPy.py
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.1.5/src/SGtSNEpiPy/__init__.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-08-01 00:42:39.817860 SGtSNEpiPy-1.1.5/src/SGtSNEpiPy.egg-info/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)    13061 2023-08-01 00:42:39.000000 SGtSNEpiPy-1.1.5/src/SGtSNEpiPy.egg-info/PKG-INFO
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      273 2023-08-01 00:42:39.000000 SGtSNEpiPy-1.1.5/src/SGtSNEpiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        1 2023-08-01 00:42:39.000000 SGtSNEpiPy-1.1.5/src/SGtSNEpiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       18 2023-08-01 00:42:39.000000 SGtSNEpiPy-1.1.5/src/SGtSNEpiPy.egg-info/requires.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       11 2023-08-01 00:42:39.000000 SGtSNEpiPy-1.1.5/src/SGtSNEpiPy.egg-info/top_level.txt
```

### Comparing `SGtSNEpiPy-1.1.4/PKG-INFO` & `SGtSNEpiPy-1.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,78 @@
 Metadata-Version: 2.1
 Name: SGtSNEpiPy
-Version: 1.1.4
+Version: 1.1.5
 Summary: SGtSNEpiPy is a Python interface to SG-t-SNE-П, a powerful tool for visualizing large, sparse, stochastic graphs.
 Author: ['Chenshuhao Qin', 'Yihua Zhong']
 Author-email: cq27@duke.edu, yz737@duke.edu,
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 
 # SGtSNEpiPy
 
 ## Overview
 
-SGtSNEpiPy is a Python interface, i.e., a wrapper to 'SG-t-SNE-П (https://github.com/fcdimitr/SGtSNEpi.jl)', implemented using the 'JuliaCall (https://cjdoris.github.io/PythonCall.jl/stable/juliacall/)' from 'PythonCall & JuliaCall (https://cjdoris.github.io/PythonCall.jl/stable/)' package.
+`SGtSNEpiPy` is a `Python` interface, i.e., a wrapper to **['SG-t-SNE-П'](https://github.com/fcdimitr/SGtSNEpi.jl)** which is in `Julia`, implemented using the **[JuliaCall](https://cjdoris.github.io/PythonCall.jl/stable/juliacall/)** from **[PythonCall & JuliaCall](https://cjdoris.github.io/PythonCall.jl/stable/)** package.
 
 ### Introduction
 
-The algorithm SG-t-SNE and the software t-SNE-Π were first described in Reference **[(Nikos Pitsianis, Alexandros-Stavros Iliopoulos, Dimitris Floros, Xiaobai Sun (2019))](https://ieeexplore.ieee.org/document/8916505)** and released on **[GitHub](https://github.com/fcdimitr/sgtsnepi)** in June 2019 **[(Nikos Pitsianis, Dimitris Floros, Alexandros-Stavros Iliopoulos, Xiaobai Sun (2019))] (https://joss.theoj.org/papers/10.21105/joss.01577)**. SG-t-SNE-П is a nonlinear method that directly embeds large, sparse, stochastic graphs into low-dimensional spaces without requiring vertex features to reside in or be transformed into a metric space. The approach is inspired by and builds upon the core principle of t-SNE for nonlinear dimensionality reduction and data visualization. Our implementation provides high-performance software for 1D, 2D, and 3D embedding of large sparse graphs on shared memory multicore computers.
+The algorithm SG-t-SNE and the software t-SNE-Π were first described in Reference **[(Nikos Pitsianis, Alexandros-Stavros Iliopoulos, Dimitris Floros, Xiaobai Sun (2019))](https://ieeexplore.ieee.org/document/8916505)** [[1]](#1) and released on **[GitHub](https://github.com/fcdimitr/sgtsnepi)** in June 2019 **[(Nikos Pitsianis, Dimitris Floros, Alexandros-Stavros Iliopoulos, Xiaobai Sun (2019))](https://joss.theoj.org/papers/10.21105/joss.01577)** [[2]](#2). SG-t-SNE-П is a nonlinear method that directly embeds large, sparse, stochastic graphs into low-dimensional spaces without requiring vertex features to reside in or be transformed into a metric space. The approach is inspired by and builds upon the core principle of t-SNE for nonlinear dimensionality reduction and data visualization. Our implementation provides high-performance software for 1D, 2D, and 3D embedding of large sparse graphs on shared memory multicore computers.
 
 
-SGtSNEpi, a Julia interface, i.e., a wrapper to SG-t-SNE-Π was released on **[GitHub](https://github.com/fcdimitr/SGtSNEpi.jl)** in 2019. SGtSNEpiPy uses **[JuliaCall](https://cjdoris.github.io/PythonCall.jl/stable/juliacall/)** module to make this Julia interface SGtSNEpi readily deployable to the Python ecosystem.
+`SGtSNEpi`, a `Julia` interface, i.e., a wrapper to `SG-t-SNE-Π` was released on **[GitHub](https://github.com/fcdimitr/SGtSNEpi.jl)** in 2019. SGtSNEpiPy uses **[JuliaCall](https://cjdoris.github.io/PythonCall.jl/stable/juliacall/)** module to make this Julia interface `SGtSNEpi` readily deployable to the Python ecosystem.
 
 ## Installation
 
-From PyPi
+To install `SGtSNEpiPy` through `Python` from `PyPi`, issue
 
 ```
 $ pip install SGtSNEpiPy
 ```
 
-The installation is successful if you can import SGtSNEpiPy 
+The installation is successful if you can import `SGtSNEpiPy` 
 and run the command line tool:
 
-```
-$ python -c 'from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy'
+```python
+from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy
 ```
 
 **Warning:** 
-SGtSNEpiPy is currently not working on Windows and native M1 Macs: Either use WSL2 on Windows or use the package via rosetta2 on M1 Macs.
+`SGtSNEpiPy` is currently not working on Windows and native M1 Macs: Either use WSL2 on Windows or use the package via rosetta2 on M1 Macs.
 
 **Note**: The rest of the content remains unchanged as it does not contain any reST-specific elements.
 
 
 See **[the full documentation](https://fcdimitr.github.io/SGtSNEpi.jl/stable)** for moredetails.
 
 
 
 ## Parameters
 
 **SGtSNEpiPy.SGtSNEpiPy.sgtsnepipy**
 
 This package only has one method currently.
 
-
-```
-    sgtsnepi(A)
+```python
+   Y = sgtsnepi(A)
 ```
 
 
 ### A: the input CSR sparse matrix representing the data points' pairwise similarities. (Mandatory)
 
-<ul>
-<li>Data Type: **scipy.sparse.csr.csr_matrix** (The matrix includes row, value, value, whose type are all **numpy.ndarray** with three arrays of **numpy.int32, numpy.int32, numpy.int64**)</li>
-<li>A CSR sparse matrix generated by package scipy.</li>
-</ul>
+- Data Type: `scipy.sparse.csr.csr_matrix` (The matrix includes row, value, value, whose type are all `numpy.ndarray` with three arrays of `numpy.int32`, `numpy.int32`, `numpy.int64`), that is a CSR sparse matrix generated by package `scipy`.
+
+### Returns Y: array with the coordinates of the embedding of the graph nodes
+
+- Data Type: `numpy.ndarray`, a 2-dimensional array of `numpy.float64`.
+   - Number of rows: the number of rows or columns in the CSR matrix (the input).
+   - Number of columns: the number of dimensions of the embedding space.
+
+
+## Optional input parameters
 
 ### d: the number of dimensions of the embedding space. (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 2</li>
 </ul>
@@ -185,74 +190,145 @@
 <li>Options are:
 </ul>
 <li>SGtSNEpi.NUCONV_BL (default): band-limited, approximated via non-uniform convolution</li>
 <li>SGtSNEpi.NUCONV: approximated via non-uniform convolution (higher resolution than SGtSNEpi.NUCONV_BL, slower execution time)</li>
 <li>SGtSNEpi.EXACT: no approximation; quadratic complexity, use only with small datasets</li>
 </ul>
 
-## Returns
+## Examples
 
-- Data Type: **numpy.ndarray** with three arrays: **numpy.int32, numpy.int32, numpy.float4**
+### 2D SG-t-SNE-П Embedding of **[Zachary's Karate Club graph](https://networkx.org/documentation/stable/_modules/networkx/generators/social.html#karate_club_graph)**
 
-## Examples
-Here is an example to use function sgtsnepipy to generate a 2D embedding of an ER model.
-You have to use import networkx to generate a ER graph and matplotlib to visualize the embedding
+This example demonstrates the application of function `SGtSNEpiPy` using the **[SG-t-SNE-П](https://fcdimitr.github.io/SGtSNEpi.jl/stable/)** algorithm to visualize **[Zachary's Karate Club graph](https://networkx.org/documentation/stable/_modules/networkx/generators/social.html#karate_club_graph)** in `NetworkX`. The algorithm creates a low-dimensional embedding of the nodes in 2D while preserving their structural relationships. After the embedding, the example uses **[matplotlib.pyplot](https://matplotlib.org/3.5.3/api/_as_gen/matplotlib.pyplot.html)** to visualize 2D embedding. Nodes are colored based on their club membership ('Mr. Hi' or 'Officer'). The scatter plot helps understand the social network's structure and patterns based on club affiliations.
+
+
+```python
+   from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy
+   import networkx as nx
+   import numpy as np
+   import matplotlib.pyplot as plt
+
+   # 'G' is the Zachary's Karate Club graph with 'club' attribute for each node
+   
+   G = nx.karate_club_graph()
+   G_sparse_matrix = nx.to_scipy_sparse_matrix(G) 
+   y = sgtsnepipy(G_sparse_matrix,d=2)
+   
+   # Separate the X and Y coordinates from the embedding 'y'
+   X = y[:, 0]
+   Y = y[:, 1]
+   
+   # Get the color for each node based on the 'club' attribute
+   node_colors = ['red' if G.nodes[node]['club'] == 'Mr. Hi' else 'blue' for node in G.nodes]
+   
+   # Create a scatter plot to visualize the embedding and color the nodes
+   plt.scatter(X, Y, c=node_colors, alpha=0.7)
+   
+   # Label the nodes with their numbers (node names)
+   for node, (x, y) in enumerate(zip(X, Y)):
+       plt.text(x, y, str(node))
+   
+   plt.title("2D SG-t-SNE-П Embedding of Zachary's Karate Club")
+   plt.xlabel("Dimension 1")
+   plt.ylabel("Dimension 2")
+   plt.show()
+```
 
+<img width="599" alt="2D SG-t-SNE-Π Embedding of Zachary’s Karate CLub" src="https://github.com/CodyQin/SGtSNEpiPy/assets/125537769/7e299fc0-4162-4f0f-b39e-dfba6c6f59cc">
+
+### 3D SG-t-SNE-П Embedding of **[Zachary's Karate Club graph](https://networkx.org/documentation/stable/_modules/networkx/generators/social.html#karate_club_graph)**
+
+This example demonstrates the 3D embedding of same **[Zachary's Karate Club graph](https://networkx.org/documentation/stable/_modules/networkx/generators/social.html#karate_club_graph)** in `NetworkX`. 
+
+After useing **[matplotlib.pyplot](https://matplotlib.org/3.5.3/api/_as_gen/matplotlib.pyplot.html)** to generate a 3D graph, the example  refers to **[the website](https://sabopy.com/en/matplotlib-3d-14/)** that uses **[matplotlib.animation](https://matplotlib.org/stable/api/animation_api.html)** and **[mpl_toolkits.mplot3d.axes3d.Axes3D](https://matplotlib.org/3.5.1/api/_as_gen/mpl_toolkits.mplot3d.axes3d.Axes3D.html)** to generate a gif file to rotate the 3D graph.
+
+To save the animation to a gif file, you make sure you have **[Pillow](https://pillow.readthedocs.io/en/stable/)** in your python. 
+To install **[Pillow](https://pillow.readthedocs.io/en/stable/)** through Python from PyPi, issue
 
 ```
-    from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy
-    import networkx as nx
-    import matplotlib.pyplot as plt
-    import matplotlib.cm as cm
-    
-    # Generate ER Model graph
-    n = 1000  # Number of nodes
-    p = 0.2  # Probability of an edge between any two nodes
-    G = nx.erdos_renyi_graph(n=n, p=p, seed=170)
-
-    G_sparse_matrix = nx.to_scipy_sparse_matrix(G) 
-    y = sgtsnepipy(G_sparse_matrix)
-
-    # Now use the SGtSNEpi to show the visualization after embedding
-    # Get the degrees of the nodes in the graph
-    node_degrees = np.array([G.degree(node) for node in G.nodes])
-    # Normalize the degrees to the range [0, 1] for color mapping
-    node_degrees_normalized = node_degrees / np.max(node_degrees)
-    # Create a color map
-    color_map = cm.get_cmap('viridis')  # 'viridis' is just an example, you can use any color map you like
-    # Apply the color map to your normalized degrees
-    colors = color_map(node_degrees_normalized)
-
-    plt.scatter(y[:,0], y[:,1], c=colors)
-    plt.colorbar(label='Node degree')
-    plt.title("2D embedding of ER model (n = 1000, p = 0.2, seed = 170)")
+$ pip install SGtSNEpiPy
+```
+
+**The codes of 3D embedding**
 
-    plt.show()
+```python
+from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy
+import networkx as nx
+import numpy as np
+import matplotlib.pyplot as plt
+from matplotlib import animation
+from mpl_toolkits.mplot3d import axes3d
+
+G = nx.karate_club_graph()
+G_sparse_matrix = nx.to_scipy_sparse_matrix(G) 
+y = sgtsnepipy(G_sparse_matrix,d=3)
+
+# Get the color for each node based on the 'club' attribute
+node_colors = ['red' if G.nodes[node]['club'] == 'Mr. Hi' else 'blue' for node in G.nodes]
+
+# Separate the X, Y, and Z coordinates from the 3D embedding 'y'
+X = y[:, 0]
+Y = y[:, 1]
+Z = y[:, 2]
+
+# Create the 3D scatter plot to visualize the embedding
+fig = plt.figure()
+ax = fig.add_subplot(111, projection='3d')
+scatter = ax.scatter(X, Y, Z, c=node_colors, cmap='coolwarm')   # You can choose other colormaps too
+
+# Label the nodes with their numbers (node names)
+for node, (x, y, z) in zip(G.nodes, zip(X, Y, Z)):
+    ax.text(x, y, z, node)
+
+ax.set_title("3D SG-t-SNE-П Embedding of Zachary's Karate Club")
+ax.set_xlabel('X-axis')
+ax.set_ylabel('Y-axis')
+ax.set_zlabel('Z-axis')
+
+# Function to initialize the animation
+def init():
+    scatter.set_offsets(np.column_stack([X, Y, Z]))  # Update the scatter plot data
+    return scatter,
+
+# Function to update the plot for each frame of the animation
+def animate(i):
+    ax.view_init(elev=30., azim=3.6*i)
+    return scatter,
+
+# Create the animation
+ani = animation.FuncAnimation(fig, animate, init_func=init,
+                              frames=100, interval=100, blit=True)
+
+# Save the animation to a gif file
+ani.save('3d_karate_club_animation.gif', writer='pillow')
 ```
 
+![3d_karate_club_animation](https://github.com/CodyQin/SGtSNEpiPy/assets/125537769/998d13a8-7d2d-4fa3-b435-095783f1bdc0)
+
+
+
 
 ## Contact
 
 Chenshuhao(Cody) Qin: chenshuhao.qin@duke.edu
 
 Yihua(Aaron) Zhong: yihua.zhong@duke.edu
 
 
 ## Citation
 
-- Nikos Pitsianis, Alexandros-Stavros Iliopoulos, Dimitris Floros, Xiaobai Sun, **[Spaceland Embedding of Sparse Stochastic Graphs](https://doi.org/10.1109/HPEC.2019.8916505)**, In IEEE High Performance Extreme Computing Conference, 2019.
-- Nikos Pitsianis, Dimitris Floros, Alexandros-Stavros Iliopoulos, Xiaobai Sun, **[SG-t-SNE-Π: Swift Neighbor Embedding of Sparse Stochastic Graphs](https://doi.org/10.21105/joss.01577)**, Journal of Open Source Software, 4(39), 1577, 2019.
+<a id="1">[1]</a > Nikos Pitsianis, Alexandros-Stavros Iliopoulos, Dimitris Floros, Xiaobai Sun, **[Spaceland Embedding of Sparse Stochastic Graphs](https://doi.org/10.1109/HPEC.2019.8916505)**, In IEEE High Performance Extreme Computing Conference, 2019.
+
+<a id="2">[2]</a > Nikos Pitsianis, Dimitris Floros, Alexandros-Stavros Iliopoulos, Xiaobai Sun, **[SG-t-SNE-Π: Swift Neighbor Embedding of Sparse Stochastic Graphs](https://doi.org/10.21105/joss.01577)**, Journal of Open Source Software, 4(39), 1577, 2019.
 
 If you use this software, please cite the following paper.
 
 ```
-
-    @inproceedings{pitsianis2019sgtsnepi,
-    author = {Pitsianis, Nikos and Iliopoulos, Alexandros-Stavros and Floros, Dimitris and Sun, Xiaobai},
-    doi = {10.1109/HPEC.2019.8916505},
-    booktitle = {IEEE High Performance Extreme Computing Conference},
-    month = {11},
-    title = {{Spaceland Embedding of Sparse Stochastic Graphs}},
-    year = {2019}
-    }
-
+@inproceedings{pitsianis2019sgtsnepi,
+   author = {Pitsianis, Nikos and Iliopoulos, Alexandros-Stavros and Floros, Dimitris and Sun, Xiaobai},
+   doi = {10.1109/HPEC.2019.8916505},
+   booktitle = {IEEE High Performance Extreme Computing Conference},
+   month = {11},
+   title = {{Spaceland Embedding of Sparse Stochastic Graphs}},
+   year = {2019}
+}
 ```
```

### Comparing `SGtSNEpiPy-1.1.4/README.md` & `SGtSNEpiPy-1.1.5/src/SGtSNEpiPy.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,78 @@
+Metadata-Version: 2.1
+Name: SGtSNEpiPy
+Version: 1.1.5
+Summary: SGtSNEpiPy is a Python interface to SG-t-SNE-П, a powerful tool for visualizing large, sparse, stochastic graphs.
+Author: ['Chenshuhao Qin', 'Yihua Zhong']
+Author-email: cq27@duke.edu, yz737@duke.edu,
+Classifier: Programming Language :: Python
+Classifier: Intended Audience :: Developers
+Description-Content-Type: text/markdown
+
 # SGtSNEpiPy
 
 ## Overview
 
-SGtSNEpiPy is a Python interface, i.e., a wrapper to 'SG-t-SNE-П (https://github.com/fcdimitr/SGtSNEpi.jl)', implemented using the 'JuliaCall (https://cjdoris.github.io/PythonCall.jl/stable/juliacall/)' from 'PythonCall & JuliaCall (https://cjdoris.github.io/PythonCall.jl/stable/)' package.
+`SGtSNEpiPy` is a `Python` interface, i.e., a wrapper to **['SG-t-SNE-П'](https://github.com/fcdimitr/SGtSNEpi.jl)** which is in `Julia`, implemented using the **[JuliaCall](https://cjdoris.github.io/PythonCall.jl/stable/juliacall/)** from **[PythonCall & JuliaCall](https://cjdoris.github.io/PythonCall.jl/stable/)** package.
 
 ### Introduction
 
-The algorithm SG-t-SNE and the software t-SNE-Π were first described in Reference **[(Nikos Pitsianis, Alexandros-Stavros Iliopoulos, Dimitris Floros, Xiaobai Sun (2019))](https://ieeexplore.ieee.org/document/8916505)** and released on **[GitHub](https://github.com/fcdimitr/sgtsnepi)** in June 2019 **[(Nikos Pitsianis, Dimitris Floros, Alexandros-Stavros Iliopoulos, Xiaobai Sun (2019))] (https://joss.theoj.org/papers/10.21105/joss.01577)**. SG-t-SNE-П is a nonlinear method that directly embeds large, sparse, stochastic graphs into low-dimensional spaces without requiring vertex features to reside in or be transformed into a metric space. The approach is inspired by and builds upon the core principle of t-SNE for nonlinear dimensionality reduction and data visualization. Our implementation provides high-performance software for 1D, 2D, and 3D embedding of large sparse graphs on shared memory multicore computers.
+The algorithm SG-t-SNE and the software t-SNE-Π were first described in Reference **[(Nikos Pitsianis, Alexandros-Stavros Iliopoulos, Dimitris Floros, Xiaobai Sun (2019))](https://ieeexplore.ieee.org/document/8916505)** [[1]](#1) and released on **[GitHub](https://github.com/fcdimitr/sgtsnepi)** in June 2019 **[(Nikos Pitsianis, Dimitris Floros, Alexandros-Stavros Iliopoulos, Xiaobai Sun (2019))](https://joss.theoj.org/papers/10.21105/joss.01577)** [[2]](#2). SG-t-SNE-П is a nonlinear method that directly embeds large, sparse, stochastic graphs into low-dimensional spaces without requiring vertex features to reside in or be transformed into a metric space. The approach is inspired by and builds upon the core principle of t-SNE for nonlinear dimensionality reduction and data visualization. Our implementation provides high-performance software for 1D, 2D, and 3D embedding of large sparse graphs on shared memory multicore computers.
 
 
-SGtSNEpi, a Julia interface, i.e., a wrapper to SG-t-SNE-Π was released on **[GitHub](https://github.com/fcdimitr/SGtSNEpi.jl)** in 2019. SGtSNEpiPy uses **[JuliaCall](https://cjdoris.github.io/PythonCall.jl/stable/juliacall/)** module to make this Julia interface SGtSNEpi readily deployable to the Python ecosystem.
+`SGtSNEpi`, a `Julia` interface, i.e., a wrapper to `SG-t-SNE-Π` was released on **[GitHub](https://github.com/fcdimitr/SGtSNEpi.jl)** in 2019. SGtSNEpiPy uses **[JuliaCall](https://cjdoris.github.io/PythonCall.jl/stable/juliacall/)** module to make this Julia interface `SGtSNEpi` readily deployable to the Python ecosystem.
 
 ## Installation
 
-From PyPi
+To install `SGtSNEpiPy` through `Python` from `PyPi`, issue
 
 ```
 $ pip install SGtSNEpiPy
 ```
 
-The installation is successful if you can import SGtSNEpiPy 
+The installation is successful if you can import `SGtSNEpiPy` 
 and run the command line tool:
 
-```
-$ python -c 'from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy'
+```python
+from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy
 ```
 
 **Warning:** 
-SGtSNEpiPy is currently not working on Windows and native M1 Macs: Either use WSL2 on Windows or use the package via rosetta2 on M1 Macs.
+`SGtSNEpiPy` is currently not working on Windows and native M1 Macs: Either use WSL2 on Windows or use the package via rosetta2 on M1 Macs.
 
 **Note**: The rest of the content remains unchanged as it does not contain any reST-specific elements.
 
 
 See **[the full documentation](https://fcdimitr.github.io/SGtSNEpi.jl/stable)** for moredetails.
 
 
 
 ## Parameters
 
 **SGtSNEpiPy.SGtSNEpiPy.sgtsnepipy**
 
 This package only has one method currently.
 
-
-```
-    sgtsnepi(A)
+```python
+   Y = sgtsnepi(A)
 ```
 
 
 ### A: the input CSR sparse matrix representing the data points' pairwise similarities. (Mandatory)
 
-<ul>
-<li>Data Type: **scipy.sparse.csr.csr_matrix** (The matrix includes row, value, value, whose type are all **numpy.ndarray** with three arrays of **numpy.int32, numpy.int32, numpy.int64**)</li>
-<li>A CSR sparse matrix generated by package scipy.</li>
-</ul>
+- Data Type: `scipy.sparse.csr.csr_matrix` (The matrix includes row, value, value, whose type are all `numpy.ndarray` with three arrays of `numpy.int32`, `numpy.int32`, `numpy.int64`), that is a CSR sparse matrix generated by package `scipy`.
+
+### Returns Y: array with the coordinates of the embedding of the graph nodes
+
+- Data Type: `numpy.ndarray`, a 2-dimensional array of `numpy.float64`.
+   - Number of rows: the number of rows or columns in the CSR matrix (the input).
+   - Number of columns: the number of dimensions of the embedding space.
+
+
+## Optional input parameters
 
 ### d: the number of dimensions of the embedding space. (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 2</li>
 </ul>
@@ -175,74 +190,145 @@
 <li>Options are:
 </ul>
 <li>SGtSNEpi.NUCONV_BL (default): band-limited, approximated via non-uniform convolution</li>
 <li>SGtSNEpi.NUCONV: approximated via non-uniform convolution (higher resolution than SGtSNEpi.NUCONV_BL, slower execution time)</li>
 <li>SGtSNEpi.EXACT: no approximation; quadratic complexity, use only with small datasets</li>
 </ul>
 
-## Returns
+## Examples
 
-- Data Type: **numpy.ndarray** with three arrays: **numpy.int32, numpy.int32, numpy.float4**
+### 2D SG-t-SNE-П Embedding of **[Zachary's Karate Club graph](https://networkx.org/documentation/stable/_modules/networkx/generators/social.html#karate_club_graph)**
 
-## Examples
-Here is an example to use function sgtsnepipy to generate a 2D embedding of an ER model.
-You have to use import networkx to generate a ER graph and matplotlib to visualize the embedding
+This example demonstrates the application of function `SGtSNEpiPy` using the **[SG-t-SNE-П](https://fcdimitr.github.io/SGtSNEpi.jl/stable/)** algorithm to visualize **[Zachary's Karate Club graph](https://networkx.org/documentation/stable/_modules/networkx/generators/social.html#karate_club_graph)** in `NetworkX`. The algorithm creates a low-dimensional embedding of the nodes in 2D while preserving their structural relationships. After the embedding, the example uses **[matplotlib.pyplot](https://matplotlib.org/3.5.3/api/_as_gen/matplotlib.pyplot.html)** to visualize 2D embedding. Nodes are colored based on their club membership ('Mr. Hi' or 'Officer'). The scatter plot helps understand the social network's structure and patterns based on club affiliations.
+
+
+```python
+   from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy
+   import networkx as nx
+   import numpy as np
+   import matplotlib.pyplot as plt
+
+   # 'G' is the Zachary's Karate Club graph with 'club' attribute for each node
+   
+   G = nx.karate_club_graph()
+   G_sparse_matrix = nx.to_scipy_sparse_matrix(G) 
+   y = sgtsnepipy(G_sparse_matrix,d=2)
+   
+   # Separate the X and Y coordinates from the embedding 'y'
+   X = y[:, 0]
+   Y = y[:, 1]
+   
+   # Get the color for each node based on the 'club' attribute
+   node_colors = ['red' if G.nodes[node]['club'] == 'Mr. Hi' else 'blue' for node in G.nodes]
+   
+   # Create a scatter plot to visualize the embedding and color the nodes
+   plt.scatter(X, Y, c=node_colors, alpha=0.7)
+   
+   # Label the nodes with their numbers (node names)
+   for node, (x, y) in enumerate(zip(X, Y)):
+       plt.text(x, y, str(node))
+   
+   plt.title("2D SG-t-SNE-П Embedding of Zachary's Karate Club")
+   plt.xlabel("Dimension 1")
+   plt.ylabel("Dimension 2")
+   plt.show()
+```
 
+<img width="599" alt="2D SG-t-SNE-Π Embedding of Zachary’s Karate CLub" src="https://github.com/CodyQin/SGtSNEpiPy/assets/125537769/7e299fc0-4162-4f0f-b39e-dfba6c6f59cc">
+
+### 3D SG-t-SNE-П Embedding of **[Zachary's Karate Club graph](https://networkx.org/documentation/stable/_modules/networkx/generators/social.html#karate_club_graph)**
+
+This example demonstrates the 3D embedding of same **[Zachary's Karate Club graph](https://networkx.org/documentation/stable/_modules/networkx/generators/social.html#karate_club_graph)** in `NetworkX`. 
+
+After useing **[matplotlib.pyplot](https://matplotlib.org/3.5.3/api/_as_gen/matplotlib.pyplot.html)** to generate a 3D graph, the example  refers to **[the website](https://sabopy.com/en/matplotlib-3d-14/)** that uses **[matplotlib.animation](https://matplotlib.org/stable/api/animation_api.html)** and **[mpl_toolkits.mplot3d.axes3d.Axes3D](https://matplotlib.org/3.5.1/api/_as_gen/mpl_toolkits.mplot3d.axes3d.Axes3D.html)** to generate a gif file to rotate the 3D graph.
+
+To save the animation to a gif file, you make sure you have **[Pillow](https://pillow.readthedocs.io/en/stable/)** in your python. 
+To install **[Pillow](https://pillow.readthedocs.io/en/stable/)** through Python from PyPi, issue
 
 ```
-    from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy
-    import networkx as nx
-    import matplotlib.pyplot as plt
-    import matplotlib.cm as cm
-    
-    # Generate ER Model graph
-    n = 1000  # Number of nodes
-    p = 0.2  # Probability of an edge between any two nodes
-    G = nx.erdos_renyi_graph(n=n, p=p, seed=170)
-
-    G_sparse_matrix = nx.to_scipy_sparse_matrix(G) 
-    y = sgtsnepipy(G_sparse_matrix)
-
-    # Now use the SGtSNEpi to show the visualization after embedding
-    # Get the degrees of the nodes in the graph
-    node_degrees = np.array([G.degree(node) for node in G.nodes])
-    # Normalize the degrees to the range [0, 1] for color mapping
-    node_degrees_normalized = node_degrees / np.max(node_degrees)
-    # Create a color map
-    color_map = cm.get_cmap('viridis')  # 'viridis' is just an example, you can use any color map you like
-    # Apply the color map to your normalized degrees
-    colors = color_map(node_degrees_normalized)
-
-    plt.scatter(y[:,0], y[:,1], c=colors)
-    plt.colorbar(label='Node degree')
-    plt.title("2D embedding of ER model (n = 1000, p = 0.2, seed = 170)")
+$ pip install SGtSNEpiPy
+```
+
+**The codes of 3D embedding**
+
+```python
+from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy
+import networkx as nx
+import numpy as np
+import matplotlib.pyplot as plt
+from matplotlib import animation
+from mpl_toolkits.mplot3d import axes3d
+
+G = nx.karate_club_graph()
+G_sparse_matrix = nx.to_scipy_sparse_matrix(G) 
+y = sgtsnepipy(G_sparse_matrix,d=3)
+
+# Get the color for each node based on the 'club' attribute
+node_colors = ['red' if G.nodes[node]['club'] == 'Mr. Hi' else 'blue' for node in G.nodes]
+
+# Separate the X, Y, and Z coordinates from the 3D embedding 'y'
+X = y[:, 0]
+Y = y[:, 1]
+Z = y[:, 2]
+
+# Create the 3D scatter plot to visualize the embedding
+fig = plt.figure()
+ax = fig.add_subplot(111, projection='3d')
+scatter = ax.scatter(X, Y, Z, c=node_colors, cmap='coolwarm')   # You can choose other colormaps too
+
+# Label the nodes with their numbers (node names)
+for node, (x, y, z) in zip(G.nodes, zip(X, Y, Z)):
+    ax.text(x, y, z, node)
+
+ax.set_title("3D SG-t-SNE-П Embedding of Zachary's Karate Club")
+ax.set_xlabel('X-axis')
+ax.set_ylabel('Y-axis')
+ax.set_zlabel('Z-axis')
+
+# Function to initialize the animation
+def init():
+    scatter.set_offsets(np.column_stack([X, Y, Z]))  # Update the scatter plot data
+    return scatter,
+
+# Function to update the plot for each frame of the animation
+def animate(i):
+    ax.view_init(elev=30., azim=3.6*i)
+    return scatter,
+
+# Create the animation
+ani = animation.FuncAnimation(fig, animate, init_func=init,
+                              frames=100, interval=100, blit=True)
 
-    plt.show()
+# Save the animation to a gif file
+ani.save('3d_karate_club_animation.gif', writer='pillow')
 ```
 
+![3d_karate_club_animation](https://github.com/CodyQin/SGtSNEpiPy/assets/125537769/998d13a8-7d2d-4fa3-b435-095783f1bdc0)
+
+
+
 
 ## Contact
 
 Chenshuhao(Cody) Qin: chenshuhao.qin@duke.edu
 
 Yihua(Aaron) Zhong: yihua.zhong@duke.edu
 
 
 ## Citation
 
-- Nikos Pitsianis, Alexandros-Stavros Iliopoulos, Dimitris Floros, Xiaobai Sun, **[Spaceland Embedding of Sparse Stochastic Graphs](https://doi.org/10.1109/HPEC.2019.8916505)**, In IEEE High Performance Extreme Computing Conference, 2019.
-- Nikos Pitsianis, Dimitris Floros, Alexandros-Stavros Iliopoulos, Xiaobai Sun, **[SG-t-SNE-Π: Swift Neighbor Embedding of Sparse Stochastic Graphs](https://doi.org/10.21105/joss.01577)**, Journal of Open Source Software, 4(39), 1577, 2019.
+<a id="1">[1]</a > Nikos Pitsianis, Alexandros-Stavros Iliopoulos, Dimitris Floros, Xiaobai Sun, **[Spaceland Embedding of Sparse Stochastic Graphs](https://doi.org/10.1109/HPEC.2019.8916505)**, In IEEE High Performance Extreme Computing Conference, 2019.
+
+<a id="2">[2]</a > Nikos Pitsianis, Dimitris Floros, Alexandros-Stavros Iliopoulos, Xiaobai Sun, **[SG-t-SNE-Π: Swift Neighbor Embedding of Sparse Stochastic Graphs](https://doi.org/10.21105/joss.01577)**, Journal of Open Source Software, 4(39), 1577, 2019.
 
 If you use this software, please cite the following paper.
 
 ```
-
-    @inproceedings{pitsianis2019sgtsnepi,
-    author = {Pitsianis, Nikos and Iliopoulos, Alexandros-Stavros and Floros, Dimitris and Sun, Xiaobai},
-    doi = {10.1109/HPEC.2019.8916505},
-    booktitle = {IEEE High Performance Extreme Computing Conference},
-    month = {11},
-    title = {{Spaceland Embedding of Sparse Stochastic Graphs}},
-    year = {2019}
-    }
-
-```
+@inproceedings{pitsianis2019sgtsnepi,
+   author = {Pitsianis, Nikos and Iliopoulos, Alexandros-Stavros and Floros, Dimitris and Sun, Xiaobai},
+   doi = {10.1109/HPEC.2019.8916505},
+   booktitle = {IEEE High Performance Extreme Computing Conference},
+   month = {11},
+   title = {{Spaceland Embedding of Sparse Stochastic Graphs}},
+   year = {2019}
+}
+```
```

### Comparing `SGtSNEpiPy-1.1.4/setup.py` & `SGtSNEpiPy-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 with open("readme.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='SGtSNEpiPy',
-    version='1.1.4',
+    version='1.1.5',
     description='SGtSNEpiPy is a Python interface to SG-t-SNE-П, a powerful tool for visualizing large, sparse, stochastic graphs.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author=['Chenshuhao Qin','Yihua Zhong'],
     author_email="cq27@duke.edu, yz737@duke.edu,",
     classifiers=[
                 'Programming Language :: Python',
```

### Comparing `SGtSNEpiPy-1.1.4/src/SGtSNEpiPy/SGtSNEpiPy.py` & `SGtSNEpiPy-1.1.5/src/SGtSNEpiPy/SGtSNEpiPy.py`

 * *Files identical despite different names*

### Comparing `SGtSNEpiPy-1.1.4/src/SGtSNEpiPy.egg-info/PKG-INFO` & `SGtSNEpiPy-1.1.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,68 @@
-Metadata-Version: 2.1
-Name: SGtSNEpiPy
-Version: 1.1.4
-Summary: SGtSNEpiPy is a Python interface to SG-t-SNE-П, a powerful tool for visualizing large, sparse, stochastic graphs.
-Author: ['Chenshuhao Qin', 'Yihua Zhong']
-Author-email: cq27@duke.edu, yz737@duke.edu,
-Classifier: Programming Language :: Python
-Classifier: Intended Audience :: Developers
-Description-Content-Type: text/markdown
-
 # SGtSNEpiPy
 
 ## Overview
 
-SGtSNEpiPy is a Python interface, i.e., a wrapper to 'SG-t-SNE-П (https://github.com/fcdimitr/SGtSNEpi.jl)', implemented using the 'JuliaCall (https://cjdoris.github.io/PythonCall.jl/stable/juliacall/)' from 'PythonCall & JuliaCall (https://cjdoris.github.io/PythonCall.jl/stable/)' package.
+`SGtSNEpiPy` is a `Python` interface, i.e., a wrapper to **['SG-t-SNE-П'](https://github.com/fcdimitr/SGtSNEpi.jl)** which is in `Julia`, implemented using the **[JuliaCall](https://cjdoris.github.io/PythonCall.jl/stable/juliacall/)** from **[PythonCall & JuliaCall](https://cjdoris.github.io/PythonCall.jl/stable/)** package.
 
 ### Introduction
 
-The algorithm SG-t-SNE and the software t-SNE-Π were first described in Reference **[(Nikos Pitsianis, Alexandros-Stavros Iliopoulos, Dimitris Floros, Xiaobai Sun (2019))](https://ieeexplore.ieee.org/document/8916505)** and released on **[GitHub](https://github.com/fcdimitr/sgtsnepi)** in June 2019 **[(Nikos Pitsianis, Dimitris Floros, Alexandros-Stavros Iliopoulos, Xiaobai Sun (2019))] (https://joss.theoj.org/papers/10.21105/joss.01577)**. SG-t-SNE-П is a nonlinear method that directly embeds large, sparse, stochastic graphs into low-dimensional spaces without requiring vertex features to reside in or be transformed into a metric space. The approach is inspired by and builds upon the core principle of t-SNE for nonlinear dimensionality reduction and data visualization. Our implementation provides high-performance software for 1D, 2D, and 3D embedding of large sparse graphs on shared memory multicore computers.
+The algorithm SG-t-SNE and the software t-SNE-Π were first described in Reference **[(Nikos Pitsianis, Alexandros-Stavros Iliopoulos, Dimitris Floros, Xiaobai Sun (2019))](https://ieeexplore.ieee.org/document/8916505)** [[1]](#1) and released on **[GitHub](https://github.com/fcdimitr/sgtsnepi)** in June 2019 **[(Nikos Pitsianis, Dimitris Floros, Alexandros-Stavros Iliopoulos, Xiaobai Sun (2019))](https://joss.theoj.org/papers/10.21105/joss.01577)** [[2]](#2). SG-t-SNE-П is a nonlinear method that directly embeds large, sparse, stochastic graphs into low-dimensional spaces without requiring vertex features to reside in or be transformed into a metric space. The approach is inspired by and builds upon the core principle of t-SNE for nonlinear dimensionality reduction and data visualization. Our implementation provides high-performance software for 1D, 2D, and 3D embedding of large sparse graphs on shared memory multicore computers.
 
 
-SGtSNEpi, a Julia interface, i.e., a wrapper to SG-t-SNE-Π was released on **[GitHub](https://github.com/fcdimitr/SGtSNEpi.jl)** in 2019. SGtSNEpiPy uses **[JuliaCall](https://cjdoris.github.io/PythonCall.jl/stable/juliacall/)** module to make this Julia interface SGtSNEpi readily deployable to the Python ecosystem.
+`SGtSNEpi`, a `Julia` interface, i.e., a wrapper to `SG-t-SNE-Π` was released on **[GitHub](https://github.com/fcdimitr/SGtSNEpi.jl)** in 2019. SGtSNEpiPy uses **[JuliaCall](https://cjdoris.github.io/PythonCall.jl/stable/juliacall/)** module to make this Julia interface `SGtSNEpi` readily deployable to the Python ecosystem.
 
 ## Installation
 
-From PyPi
+To install `SGtSNEpiPy` through `Python` from `PyPi`, issue
 
 ```
 $ pip install SGtSNEpiPy
 ```
 
-The installation is successful if you can import SGtSNEpiPy 
+The installation is successful if you can import `SGtSNEpiPy` 
 and run the command line tool:
 
-```
-$ python -c 'from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy'
+```python
+from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy
 ```
 
 **Warning:** 
-SGtSNEpiPy is currently not working on Windows and native M1 Macs: Either use WSL2 on Windows or use the package via rosetta2 on M1 Macs.
+`SGtSNEpiPy` is currently not working on Windows and native M1 Macs: Either use WSL2 on Windows or use the package via rosetta2 on M1 Macs.
 
 **Note**: The rest of the content remains unchanged as it does not contain any reST-specific elements.
 
 
 See **[the full documentation](https://fcdimitr.github.io/SGtSNEpi.jl/stable)** for moredetails.
 
 
 
 ## Parameters
 
 **SGtSNEpiPy.SGtSNEpiPy.sgtsnepipy**
 
 This package only has one method currently.
 
-
-```
-    sgtsnepi(A)
+```python
+   Y = sgtsnepi(A)
 ```
 
 
 ### A: the input CSR sparse matrix representing the data points' pairwise similarities. (Mandatory)
 
-<ul>
-<li>Data Type: **scipy.sparse.csr.csr_matrix** (The matrix includes row, value, value, whose type are all **numpy.ndarray** with three arrays of **numpy.int32, numpy.int32, numpy.int64**)</li>
-<li>A CSR sparse matrix generated by package scipy.</li>
-</ul>
+- Data Type: `scipy.sparse.csr.csr_matrix` (The matrix includes row, value, value, whose type are all `numpy.ndarray` with three arrays of `numpy.int32`, `numpy.int32`, `numpy.int64`), that is a CSR sparse matrix generated by package `scipy`.
+
+### Returns Y: array with the coordinates of the embedding of the graph nodes
+
+- Data Type: `numpy.ndarray`, a 2-dimensional array of `numpy.float64`.
+   - Number of rows: the number of rows or columns in the CSR matrix (the input).
+   - Number of columns: the number of dimensions of the embedding space.
+
+
+## Optional input parameters
 
 ### d: the number of dimensions of the embedding space. (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 2</li>
 </ul>
@@ -185,74 +180,145 @@
 <li>Options are:
 </ul>
 <li>SGtSNEpi.NUCONV_BL (default): band-limited, approximated via non-uniform convolution</li>
 <li>SGtSNEpi.NUCONV: approximated via non-uniform convolution (higher resolution than SGtSNEpi.NUCONV_BL, slower execution time)</li>
 <li>SGtSNEpi.EXACT: no approximation; quadratic complexity, use only with small datasets</li>
 </ul>
 
-## Returns
+## Examples
 
-- Data Type: **numpy.ndarray** with three arrays: **numpy.int32, numpy.int32, numpy.float4**
+### 2D SG-t-SNE-П Embedding of **[Zachary's Karate Club graph](https://networkx.org/documentation/stable/_modules/networkx/generators/social.html#karate_club_graph)**
 
-## Examples
-Here is an example to use function sgtsnepipy to generate a 2D embedding of an ER model.
-You have to use import networkx to generate a ER graph and matplotlib to visualize the embedding
+This example demonstrates the application of function `SGtSNEpiPy` using the **[SG-t-SNE-П](https://fcdimitr.github.io/SGtSNEpi.jl/stable/)** algorithm to visualize **[Zachary's Karate Club graph](https://networkx.org/documentation/stable/_modules/networkx/generators/social.html#karate_club_graph)** in `NetworkX`. The algorithm creates a low-dimensional embedding of the nodes in 2D while preserving their structural relationships. After the embedding, the example uses **[matplotlib.pyplot](https://matplotlib.org/3.5.3/api/_as_gen/matplotlib.pyplot.html)** to visualize 2D embedding. Nodes are colored based on their club membership ('Mr. Hi' or 'Officer'). The scatter plot helps understand the social network's structure and patterns based on club affiliations.
 
 
+```python
+   from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy
+   import networkx as nx
+   import numpy as np
+   import matplotlib.pyplot as plt
+
+   # 'G' is the Zachary's Karate Club graph with 'club' attribute for each node
+   
+   G = nx.karate_club_graph()
+   G_sparse_matrix = nx.to_scipy_sparse_matrix(G) 
+   y = sgtsnepipy(G_sparse_matrix,d=2)
+   
+   # Separate the X and Y coordinates from the embedding 'y'
+   X = y[:, 0]
+   Y = y[:, 1]
+   
+   # Get the color for each node based on the 'club' attribute
+   node_colors = ['red' if G.nodes[node]['club'] == 'Mr. Hi' else 'blue' for node in G.nodes]
+   
+   # Create a scatter plot to visualize the embedding and color the nodes
+   plt.scatter(X, Y, c=node_colors, alpha=0.7)
+   
+   # Label the nodes with their numbers (node names)
+   for node, (x, y) in enumerate(zip(X, Y)):
+       plt.text(x, y, str(node))
+   
+   plt.title("2D SG-t-SNE-П Embedding of Zachary's Karate Club")
+   plt.xlabel("Dimension 1")
+   plt.ylabel("Dimension 2")
+   plt.show()
 ```
-    from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy
-    import networkx as nx
-    import matplotlib.pyplot as plt
-    import matplotlib.cm as cm
-    
-    # Generate ER Model graph
-    n = 1000  # Number of nodes
-    p = 0.2  # Probability of an edge between any two nodes
-    G = nx.erdos_renyi_graph(n=n, p=p, seed=170)
-
-    G_sparse_matrix = nx.to_scipy_sparse_matrix(G) 
-    y = sgtsnepipy(G_sparse_matrix)
-
-    # Now use the SGtSNEpi to show the visualization after embedding
-    # Get the degrees of the nodes in the graph
-    node_degrees = np.array([G.degree(node) for node in G.nodes])
-    # Normalize the degrees to the range [0, 1] for color mapping
-    node_degrees_normalized = node_degrees / np.max(node_degrees)
-    # Create a color map
-    color_map = cm.get_cmap('viridis')  # 'viridis' is just an example, you can use any color map you like
-    # Apply the color map to your normalized degrees
-    colors = color_map(node_degrees_normalized)
-
-    plt.scatter(y[:,0], y[:,1], c=colors)
-    plt.colorbar(label='Node degree')
-    plt.title("2D embedding of ER model (n = 1000, p = 0.2, seed = 170)")
 
-    plt.show()
+<img width="599" alt="2D SG-t-SNE-Π Embedding of Zachary’s Karate CLub" src="https://github.com/CodyQin/SGtSNEpiPy/assets/125537769/7e299fc0-4162-4f0f-b39e-dfba6c6f59cc">
+
+### 3D SG-t-SNE-П Embedding of **[Zachary's Karate Club graph](https://networkx.org/documentation/stable/_modules/networkx/generators/social.html#karate_club_graph)**
+
+This example demonstrates the 3D embedding of same **[Zachary's Karate Club graph](https://networkx.org/documentation/stable/_modules/networkx/generators/social.html#karate_club_graph)** in `NetworkX`. 
+
+After useing **[matplotlib.pyplot](https://matplotlib.org/3.5.3/api/_as_gen/matplotlib.pyplot.html)** to generate a 3D graph, the example  refers to **[the website](https://sabopy.com/en/matplotlib-3d-14/)** that uses **[matplotlib.animation](https://matplotlib.org/stable/api/animation_api.html)** and **[mpl_toolkits.mplot3d.axes3d.Axes3D](https://matplotlib.org/3.5.1/api/_as_gen/mpl_toolkits.mplot3d.axes3d.Axes3D.html)** to generate a gif file to rotate the 3D graph.
+
+To save the animation to a gif file, you make sure you have **[Pillow](https://pillow.readthedocs.io/en/stable/)** in your python. 
+To install **[Pillow](https://pillow.readthedocs.io/en/stable/)** through Python from PyPi, issue
+
+```
+$ pip install SGtSNEpiPy
+```
+
+**The codes of 3D embedding**
+
+```python
+from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy
+import networkx as nx
+import numpy as np
+import matplotlib.pyplot as plt
+from matplotlib import animation
+from mpl_toolkits.mplot3d import axes3d
+
+G = nx.karate_club_graph()
+G_sparse_matrix = nx.to_scipy_sparse_matrix(G) 
+y = sgtsnepipy(G_sparse_matrix,d=3)
+
+# Get the color for each node based on the 'club' attribute
+node_colors = ['red' if G.nodes[node]['club'] == 'Mr. Hi' else 'blue' for node in G.nodes]
+
+# Separate the X, Y, and Z coordinates from the 3D embedding 'y'
+X = y[:, 0]
+Y = y[:, 1]
+Z = y[:, 2]
+
+# Create the 3D scatter plot to visualize the embedding
+fig = plt.figure()
+ax = fig.add_subplot(111, projection='3d')
+scatter = ax.scatter(X, Y, Z, c=node_colors, cmap='coolwarm')   # You can choose other colormaps too
+
+# Label the nodes with their numbers (node names)
+for node, (x, y, z) in zip(G.nodes, zip(X, Y, Z)):
+    ax.text(x, y, z, node)
+
+ax.set_title("3D SG-t-SNE-П Embedding of Zachary's Karate Club")
+ax.set_xlabel('X-axis')
+ax.set_ylabel('Y-axis')
+ax.set_zlabel('Z-axis')
+
+# Function to initialize the animation
+def init():
+    scatter.set_offsets(np.column_stack([X, Y, Z]))  # Update the scatter plot data
+    return scatter,
+
+# Function to update the plot for each frame of the animation
+def animate(i):
+    ax.view_init(elev=30., azim=3.6*i)
+    return scatter,
+
+# Create the animation
+ani = animation.FuncAnimation(fig, animate, init_func=init,
+                              frames=100, interval=100, blit=True)
+
+# Save the animation to a gif file
+ani.save('3d_karate_club_animation.gif', writer='pillow')
 ```
 
+![3d_karate_club_animation](https://github.com/CodyQin/SGtSNEpiPy/assets/125537769/998d13a8-7d2d-4fa3-b435-095783f1bdc0)
+
+
+
 
 ## Contact
 
 Chenshuhao(Cody) Qin: chenshuhao.qin@duke.edu
 
 Yihua(Aaron) Zhong: yihua.zhong@duke.edu
 
 
 ## Citation
 
-- Nikos Pitsianis, Alexandros-Stavros Iliopoulos, Dimitris Floros, Xiaobai Sun, **[Spaceland Embedding of Sparse Stochastic Graphs](https://doi.org/10.1109/HPEC.2019.8916505)**, In IEEE High Performance Extreme Computing Conference, 2019.
-- Nikos Pitsianis, Dimitris Floros, Alexandros-Stavros Iliopoulos, Xiaobai Sun, **[SG-t-SNE-Π: Swift Neighbor Embedding of Sparse Stochastic Graphs](https://doi.org/10.21105/joss.01577)**, Journal of Open Source Software, 4(39), 1577, 2019.
+<a id="1">[1]</a > Nikos Pitsianis, Alexandros-Stavros Iliopoulos, Dimitris Floros, Xiaobai Sun, **[Spaceland Embedding of Sparse Stochastic Graphs](https://doi.org/10.1109/HPEC.2019.8916505)**, In IEEE High Performance Extreme Computing Conference, 2019.
+
+<a id="2">[2]</a > Nikos Pitsianis, Dimitris Floros, Alexandros-Stavros Iliopoulos, Xiaobai Sun, **[SG-t-SNE-Π: Swift Neighbor Embedding of Sparse Stochastic Graphs](https://doi.org/10.21105/joss.01577)**, Journal of Open Source Software, 4(39), 1577, 2019.
 
 If you use this software, please cite the following paper.
 
 ```
-
-    @inproceedings{pitsianis2019sgtsnepi,
-    author = {Pitsianis, Nikos and Iliopoulos, Alexandros-Stavros and Floros, Dimitris and Sun, Xiaobai},
-    doi = {10.1109/HPEC.2019.8916505},
-    booktitle = {IEEE High Performance Extreme Computing Conference},
-    month = {11},
-    title = {{Spaceland Embedding of Sparse Stochastic Graphs}},
-    year = {2019}
-    }
-
+@inproceedings{pitsianis2019sgtsnepi,
+   author = {Pitsianis, Nikos and Iliopoulos, Alexandros-Stavros and Floros, Dimitris and Sun, Xiaobai},
+   doi = {10.1109/HPEC.2019.8916505},
+   booktitle = {IEEE High Performance Extreme Computing Conference},
+   month = {11},
+   title = {{Spaceland Embedding of Sparse Stochastic Graphs}},
+   year = {2019}
+}
 ```
```

