# Comparing `tmp/hilbert_modular_group-0.1.0.tar.gz` & `tmp/hilbert_modular_group-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hilbert_modular_group-0.1.0.tar", last modified: Thu Apr  7 17:36:36 2022, max compression
+gzip compressed data, was "hilbert_modular_group-0.1.1.tar", last modified: Tue Aug  1 15:24:31 2023, max compression
```

## Comparing `hilbert_modular_group-0.1.0.tar` & `hilbert_modular_group-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2022-04-07 17:36:36.694984 hilbert_modular_group-0.1.0/
-drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2022-04-07 17:36:36.652375 hilbert_modular_group-0.1.0/.github/
-drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2022-04-07 17:36:36.683169 hilbert_modular_group-0.1.0/.github/workflows/
--rw-r--r--   0 fredrik    (501) staff       (20)      612 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/.github/workflows/docker-image.yml
--rw-r--r--   0 fredrik    (501) staff       (20)      105 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/.gitignore
--rw-r--r--   0 fredrik    (501) staff       (20)      975 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/.relint.yaml
--rw-r--r--   0 fredrik    (501) staff       (20)      577 2022-04-07 17:31:27.000000 hilbert_modular_group-0.1.0/CHANGELOG.md
--rw-r--r--   0 fredrik    (501) staff       (20)      554 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/Dockerfile
--rw-r--r--   0 fredrik    (501) staff       (20)    35149 2021-11-16 23:58:10.000000 hilbert_modular_group-0.1.0/LICENSE
--rw-r--r--   0 fredrik    (501) staff       (20)      372 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/MANIFEST.in
--rw-r--r--   0 fredrik    (501) staff       (20)     2384 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/Makefile
--rw-r--r--   0 fredrik    (501) staff       (20)     9610 2022-04-07 17:36:36.695166 hilbert_modular_group-0.1.0/PKG-INFO
--rw-r--r--   0 fredrik    (501) staff       (20)     7331 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/README.md
--rwxr-xr-x   0 fredrik    (501) staff       (20)     1254 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/entrypoint.sh
-drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2022-04-07 17:36:36.686768 hilbert_modular_group-0.1.0/examples/
--rw-r--r--   0 fredrik    (501) staff       (20)    13515 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/examples/ExamplesK1.ipynb
--rw-r--r--   0 fredrik    (501) staff       (20)    21796 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/examples/ExamplesK2.ipynb
--rw-r--r--   0 fredrik    (501) staff       (20)    11813 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/examples/ExamplesK3.ipynb
--rw-r--r--   0 fredrik    (501) staff       (20)     5603 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/examples/ExamplesK4.ipynb
--rw-r--r--   0 fredrik    (501) staff       (20)     6090 2021-11-23 10:36:34.000000 hilbert_modular_group-0.1.0/examples/plot.py
-drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2022-04-07 17:36:36.688905 hilbert_modular_group-0.1.0/hilbert_modular_group.egg-info/
--rw-r--r--   0 fredrik    (501) staff       (20)     9610 2022-04-07 17:36:36.000000 hilbert_modular_group-0.1.0/hilbert_modular_group.egg-info/PKG-INFO
--rw-r--r--   0 fredrik    (501) staff       (20)      866 2022-04-07 17:36:36.000000 hilbert_modular_group-0.1.0/hilbert_modular_group.egg-info/SOURCES.txt
--rw-r--r--   0 fredrik    (501) staff       (20)        1 2022-04-07 17:36:36.000000 hilbert_modular_group-0.1.0/hilbert_modular_group.egg-info/dependency_links.txt
--rw-r--r--   0 fredrik    (501) staff       (20)       17 2022-04-07 17:36:36.000000 hilbert_modular_group-0.1.0/hilbert_modular_group.egg-info/top_level.txt
--rw-r--r--   0 fredrik    (501) staff       (20)      318 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/pyproject.toml
--rw-r--r--   0 fredrik    (501) staff       (20)     1133 2022-04-07 17:36:36.696035 hilbert_modular_group-0.1.0/setup.cfg
--rw-r--r--   0 fredrik    (501) staff       (20)     2036 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/setup.py
-drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2022-04-07 17:36:36.672699 hilbert_modular_group-0.1.0/src/
-drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2022-04-07 17:36:36.694652 hilbert_modular_group-0.1.0/src/hilbert_modgroup/
--rw-r--r--   0 fredrik    (501) staff       (20)       44 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/src/hilbert_modgroup/__init__.py
--rw-r--r--   0 fredrik    (501) staff       (20)      260 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/src/hilbert_modgroup/all.py
--rw-r--r--   0 fredrik    (501) staff       (20)    36910 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/src/hilbert_modgroup/hilbert_modular_group_class.py
--rw-r--r--   0 fredrik    (501) staff       (20)    20086 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/src/hilbert_modgroup/hilbert_modular_group_element.pyx
--rw-r--r--   0 fredrik    (501) staff       (20)    94167 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/src/hilbert_modgroup/pullback.py
--rw-r--r--   0 fredrik    (501) staff       (20)    17317 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/src/hilbert_modgroup/pullback_cython.pyx
--rw-r--r--   0 fredrik    (501) staff       (20)     1564 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/src/hilbert_modgroup/upper_half_plane.pxd
--rw-r--r--   0 fredrik    (501) staff       (20)    67245 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/src/hilbert_modgroup/upper_half_plane.pyx
--rw-r--r--   0 fredrik    (501) staff       (20)      786 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/src/hilbert_modgroup/utils.py
--rw-r--r--   0 fredrik    (501) staff       (20)      142 2022-04-07 17:36:36.000000 hilbert_modular_group-0.1.0/src/hilbert_modgroup/version.py
--rw-r--r--   0 fredrik    (501) staff       (20)     1868 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.0/tox.ini
+drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2023-08-01 15:24:31.965309 hilbert_modular_group-0.1.1/
+drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2023-08-01 15:24:31.953252 hilbert_modular_group-0.1.1/.github/
+drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2023-08-01 15:24:31.958261 hilbert_modular_group-0.1.1/.github/workflows/
+-rw-r--r--   0 fredrik    (501) staff       (20)      612 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.1/.github/workflows/docker-image.yml
+-rw-r--r--   0 fredrik    (501) staff       (20)      105 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.1/.gitignore
+-rw-r--r--   0 fredrik    (501) staff       (20)      975 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.1/.relint.yaml
+-rw-r--r--   0 fredrik    (501) staff       (20)      577 2022-04-07 17:31:27.000000 hilbert_modular_group-0.1.1/CHANGELOG.md
+-rw-r--r--   0 fredrik    (501) staff       (20)      556 2023-08-01 15:20:19.000000 hilbert_modular_group-0.1.1/Dockerfile
+-rw-r--r--   0 fredrik    (501) staff       (20)    35149 2021-11-16 23:58:10.000000 hilbert_modular_group-0.1.1/LICENSE
+-rw-r--r--   0 fredrik    (501) staff       (20)      372 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.1/MANIFEST.in
+-rw-r--r--   0 fredrik    (501) staff       (20)     2411 2023-08-01 15:20:19.000000 hilbert_modular_group-0.1.1/Makefile
+-rw-r--r--   0 fredrik    (501) staff       (20)     8469 2023-08-01 15:24:31.965409 hilbert_modular_group-0.1.1/PKG-INFO
+-rw-r--r--   0 fredrik    (501) staff       (20)     7493 2023-08-01 15:20:19.000000 hilbert_modular_group-0.1.1/README.md
+-rwxr-xr-x   0 fredrik    (501) staff       (20)     1254 2023-08-01 15:18:32.000000 hilbert_modular_group-0.1.1/entrypoint.sh
+drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2023-08-01 15:24:31.959982 hilbert_modular_group-0.1.1/examples/
+-rw-r--r--   0 fredrik    (501) staff       (20)    13560 2023-08-01 15:20:19.000000 hilbert_modular_group-0.1.1/examples/ExamplesK1.ipynb
+-rw-r--r--   0 fredrik    (501) staff       (20)    21918 2023-08-01 15:20:19.000000 hilbert_modular_group-0.1.1/examples/ExamplesK2.ipynb
+-rw-r--r--   0 fredrik    (501) staff       (20)    11814 2023-08-01 15:20:19.000000 hilbert_modular_group-0.1.1/examples/ExamplesK3.ipynb
+-rw-r--r--   0 fredrik    (501) staff       (20)     5615 2023-08-01 15:20:19.000000 hilbert_modular_group-0.1.1/examples/ExamplesK4.ipynb
+-rw-r--r--   0 fredrik    (501) staff       (20)     6090 2021-11-23 10:36:34.000000 hilbert_modular_group-0.1.1/examples/plot.py
+drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2023-08-01 15:24:31.961696 hilbert_modular_group-0.1.1/hilbert_modular_group.egg-info/
+-rw-r--r--   0 fredrik    (501) staff       (20)     8469 2023-08-01 15:24:31.000000 hilbert_modular_group-0.1.1/hilbert_modular_group.egg-info/PKG-INFO
+-rw-r--r--   0 fredrik    (501) staff       (20)      866 2023-08-01 15:24:31.000000 hilbert_modular_group-0.1.1/hilbert_modular_group.egg-info/SOURCES.txt
+-rw-r--r--   0 fredrik    (501) staff       (20)        1 2023-08-01 15:24:31.000000 hilbert_modular_group-0.1.1/hilbert_modular_group.egg-info/dependency_links.txt
+-rw-r--r--   0 fredrik    (501) staff       (20)       17 2023-08-01 15:24:31.000000 hilbert_modular_group-0.1.1/hilbert_modular_group.egg-info/top_level.txt
+-rw-r--r--   0 fredrik    (501) staff       (20)      318 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.1/pyproject.toml
+-rw-r--r--   0 fredrik    (501) staff       (20)     1133 2023-08-01 15:24:31.965808 hilbert_modular_group-0.1.1/setup.cfg
+-rw-r--r--   0 fredrik    (501) staff       (20)     2841 2023-08-01 15:20:19.000000 hilbert_modular_group-0.1.1/setup.py
+drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2023-08-01 15:24:31.953649 hilbert_modular_group-0.1.1/src/
+drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2023-08-01 15:24:31.964969 hilbert_modular_group-0.1.1/src/hilbert_modgroup/
+-rw-r--r--   0 fredrik    (501) staff       (20)       44 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.1/src/hilbert_modgroup/__init__.py
+-rw-r--r--   0 fredrik    (501) staff       (20)      260 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.1/src/hilbert_modgroup/all.py
+-rw-r--r--   0 fredrik    (501) staff       (20)    37207 2023-08-01 15:20:19.000000 hilbert_modular_group-0.1.1/src/hilbert_modgroup/hilbert_modular_group_class.py
+-rw-r--r--   0 fredrik    (501) staff       (20)    20086 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.1/src/hilbert_modgroup/hilbert_modular_group_element.pyx
+-rw-r--r--   0 fredrik    (501) staff       (20)    94350 2023-08-01 15:20:19.000000 hilbert_modular_group-0.1.1/src/hilbert_modgroup/pullback.py
+-rw-r--r--   0 fredrik    (501) staff       (20)    17328 2023-08-01 15:20:19.000000 hilbert_modular_group-0.1.1/src/hilbert_modgroup/pullback_cython.pyx
+-rw-r--r--   0 fredrik    (501) staff       (20)     1564 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.1/src/hilbert_modgroup/upper_half_plane.pxd
+-rw-r--r--   0 fredrik    (501) staff       (20)    67324 2023-08-01 15:20:19.000000 hilbert_modular_group-0.1.1/src/hilbert_modgroup/upper_half_plane.pyx
+-rw-r--r--   0 fredrik    (501) staff       (20)      786 2022-04-07 16:27:41.000000 hilbert_modular_group-0.1.1/src/hilbert_modgroup/utils.py
+-rw-r--r--   0 fredrik    (501) staff       (20)      176 2023-08-01 15:24:31.000000 hilbert_modular_group-0.1.1/src/hilbert_modgroup/version.py
+-rw-r--r--   0 fredrik    (501) staff       (20)     1893 2023-08-01 15:20:19.000000 hilbert_modular_group-0.1.1/tox.ini
```

### Comparing `hilbert_modular_group-0.1.0/.github/workflows/docker-image.yml` & `hilbert_modular_group-0.1.1/.github/workflows/docker-image.yml`

 * *Files identical despite different names*

### Comparing `hilbert_modular_group-0.1.0/.relint.yaml` & `hilbert_modular_group-0.1.1/.relint.yaml`

 * *Files identical despite different names*

### Comparing `hilbert_modular_group-0.1.0/CHANGELOG.md` & `hilbert_modular_group-0.1.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `hilbert_modular_group-0.1.0/Dockerfile` & `hilbert_modular_group-0.1.1/Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ARG REMOTE_SRC=1
 ARG GIT_BRANCH=develop
 
-FROM sagemath/sagemath:9.5 as base
+FROM sagemath/sagemath:9.7 as base
 RUN sudo apt-get update
 RUN sudo apt-get -y install git
 
 FROM base as use-git-1
 RUN git clone https://github.com/fredstro/hilbertmodgroup.git
 WORKDIR "hilbertmodgroup"
-RUN git config pull.rebase false && git checkout $GIT_BRANCH
+RUN git config pull.rebase false && git checkout ${GIT_BRANCH}
 
 FROM base as use-git-0
 ARG GIT_BRANCH=''
 COPY --chown=sage . hilbertmodgroup
 WORKDIR "hilbertmodgroup"
 
 FROM use-git-${REMOTE_SRC} AS final
```

### Comparing `hilbert_modular_group-0.1.0/LICENSE` & `hilbert_modular_group-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hilbert_modular_group-0.1.0/Makefile` & `hilbert_modular_group-0.1.1/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -41,25 +41,25 @@
 	sage -n jupyter --no-browser --ip='0.0.0.0' --port=$(NBPORT)\
                             --notebook-dir=examples\
                             --NotebookApp.custom_display_url=http://127.0.0.1:$(NBPORT)\
                             --NotebookApp.use_redirect_file=False\
                             --NotebookApp.browser=x-www-browser
 
 tox:
-	sage -pip install tox
+	sage -pip install tox meson
 	sage --python -m tox src -c tox.ini -e $(TOX_ARGS)
 
 docker:
 	docker build --build-arg GIT_BRANCH=$(GIT_BRANCH) --build-arg REMOTE_SRC=$(REMOTE_SRC) -t hilbertmodgroup-$(TAG) .
 
 docker-rebuild:
-	docker build --build-arg GIT_BRANCH=$(GIT_BRANCH) --build-arg REMOTE_SRC=$(REMOTE_SRC) --no-cache -t hilbertmodgroup=$(TAG) .
+	docker build --build-arg GIT_BRANCH=$(GIT_BRANCH) --build-arg REMOTE_SRC=$(REMOTE_SRC) --no-cache -t hilbertmodgroup-$(TAG) .
 
 docker-test: docker
-	docker run -it --init hilbertmodgroup-$(GIT_BRANCH) test
+	docker run -it -e GIT_BRANCH=$(GIT_BRANCH) --init hilbertmodgroup-$(TAG) test
 
 docker-examples: docker
 	docker run -p $(NBPORT):$(NBPORT) -it -e GIT_BRANCH=$(GIT_BRANCH) -e NBPORT=$(NBPORT) --init hilbertmodgroup-$(TAG) examples $(EXAMPLES_ARGS)
 
 docker-tox: docker
 	docker run -it -e GIT_BRANCH=$(GIT_BRANCH) -e TOX_ARGS=$(TOX_ARGS) --init hilbertmodgroup-$(TAG) tox
```

### Comparing `hilbert_modular_group-0.1.0/PKG-INFO` & `hilbert_modular_group-0.1.1/hilbert_modular_group.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,187 +1,193 @@
 Metadata-Version: 2.1
-Name: hilbert_modular_group
-Version: 0.1.0
+Name: hilbert-modular-group
+Version: 0.1.1
 Summary: Algorithms for Hilbert modular groups
 Home-page: https://github.com/fredstro/hilbertmodgroup
 Author: Fredrik Stromberg
 Author-email: fredrik314@gmail.com
 License: GPL v3+
 Project-URL: Bug Tracker, https://github.com/fredstro/hilbertmodgroup/issues
 Project-URL: Source Code, https://github.com/fredstro/hilbertmodgroup/
-Description: # Hilbert Modular Groups
-        
-        This repository contains a python package `hilbert_modgroup` that implements algorithms 
-        for Hilbert modular groups, in particular a reduction algorithm. The implementation is written in Python 
-        and is dependent on SageMath.
-        
-        ## Requirements
-        - SageMath v9.4+ (https://www.sagemath.org/)
-        
-        ## Installation
-        ### Using sage pip
-        This package needs to be installed in the virtual environment provided by SageMath, and it is therefore necessary 
-        to run the following command 
-        ```console
-        $ sage -pip install --no-build-isolation hilbert-modular-group
-        ```
-        **Note**: The `--no-build-isolation` is necessary as the compiler needs access 
-        to certain library files from the sage installation and SageMath itself is 
-        too large to be required as a build dependency. 
-        As an alternative to this flag you can also specify the environment variable 
-        SAGE_LIB explicitly.
-        
-        ### From git source
-        If the SageMath executable `sage` is in the current path you can install from source using the Makefile
-        
-        ```console
-        $ git clone https://github.com/fredstro/hilbertmodgroup.git
-        $ cd hilbertmodgrup
-        $ make install
-        ```
-        
-        ### Docker
-        If you do not have SageMath installed, but you have docker you can use install this package
-        in a docker container built and executed using e.g. `make docker-sage` or `make docker-examples`
-        
-        
-        ## Usage
-        The package can be imported and used as any other package. 
-        For example, to find the reduction of the point given by [1+i,1+i] in H^2 
-        with respect to the Hilbert modular group of Q joint by square-root of 5 write: 
-        
-        ```
-        sage: from hilbert_modgroup.all import *
-        sage: H1=HilbertModularGroup(5)
-        sage: P1=HilbertPullback(H1)
-        sage: z = UpperHalfPlaneProductElement([1+I,1+I])
-        sage: P1.reduce(z)
-        [1.00000000000000*I, 1.00000000000000*I]
-        sage: z = UpperHalfPlaneProductElement([0.25+I/2,1+I])
-        sage: P1.reduce(z) # abs tol 1e-10
-        [0.694427190999916 + 0.611145618000168*I, -0.309016994374947 + 1.30901699437495*I]
-        sage: P1.reduce(z, return_map=True)[1]
-        [-1/2*a + 1/2  1/2*a + 1/2]
-        [-1/2*a + 1/2            0]
-        
-        ```
-        For more examples see the embedded doctests (search for `EXAMPLES`) as well as
-        the `/examples` directory which contains Jupyter notebook with more extensive 
-        examples corresponding to the paper
-        "Reduction Algorithms for Hilbert Modular Groups" by F. Stromberg. (Reference to appear)
-        
-        ## Examples
-        
-        The directory `/examples` contains Jupyter notebooks with example code to illustrate the interface and functionality of this package. 
-        You can either open them manually from SageMath or run one of the following commands:
-        `make examples`
-        `make docker-examples`
-        which will start up a Jupyter notebook server from sagemath either locally or in a docker container. 
-        
-        ## Community Guidelines
-        
-        ### How to Contribute?
-        - Open an issue on GitHub and create a pull / merge request against the `develop` branch.
-        ### How to report an issue or a problem? 
-        - First check if the issue is resolved in the `develop` branch. If not, open an issue on GitHub. 
-        ### How to seek help and support?
-        - Contact the maintainer, Fredrik Stromberg, at: fredrik314@gmail.com (alternatively at fredrik.stromberg@nottingham.ac.uk)
-        
-        ## Development and testing
-        
-        The make file `Makefile` contains a number of useful commands that you can run using 
-        ```console
-        $ make <command>
-        ```
-        The following commands are run in your local SagMath environment:
-        1. `build` -- builds the package in place (sometimes useful for development).
-        2. `sdist` -- create a source distribution in /sdist (can be installed using `sage -pip install sdist/<dist name>`)
-        3. `install` -- build and install the package in the currently active sage environment
-        4. `clean` -- remove all build and temporary files
-        5. `test` -- run sage's doctests (same as `sage -t src/*`)
-        6. `examples` -- run a Jupyter notebook with the SageMath kernel initialised at the `/examples` directory.
-        7. `tox` -- run `sage -tox` with all environments: `doctest`, `coverage`, `pycodestyle`, `relint`, `codespell`
-           Note: If your local SageMath installation does not contain tox this will run `sage -pip install tox`.
-        
-        The following commands are run in an isolated docker container 
-        and requires docker to be installed and running:
-        1. `docker` -- build a docker container with the tag `hilbertmodgroup-{GIT_BRANCH}`
-        2. `docker-rebuild` -- rebuild the docker container without cache
-        3. `docker-test` -- run SageMath's doctests in the docker container
-        4. `docker-examples` -- run a Jupyter notebook with the SageMath kernel initialised at the `/examples` directory 
-          and exposing the notebook at http://127.0.0.1:8888. The port used can be modified by 
-        5. `docker-tox` -- run tox with all environments: `doctest`, `coverage`, `pycodestyle`, `relint`, `codespell`. 
-        6. `docker-shell` -- run a shell in a docker container
-        7. `docker-sage` -- run a sage interactive shell in a docker container
-        
-        The following command-line parameters are available 
-        - `NBPORT` -- set the port of the notebook for `examples` and `docker-examples`  (default is 8888)
-        - `TOX_ARGS` -- can be used to select one or more of the tox environments (default is all)
-        - `REMOTE_SRC` -- set to 0 if you want to use the local source instead of pulling from gitHub (default 1)
-        - `GIT_BRANCH` -- the branch to pull from gitHub (used if REMOTE_SRC=1)
-        
-        ### Example usage
-        Run tox coverage on the branch `main` from gitHub:
-        
-        `make docker-tox REMOTE_SRC=1 GIT_BRANCH=main TOX_ARGS=coverage`
-        
-        Run doctests on the local source with local version of sage:
-        
-        `make tox TOX_ARGS=doctest`
-        
-        Run relint on the local source with docker version of sage:
-        
-        `make docker-tox REMOTE_SRC=0 TOX_ARGS=relint`
-        
-        ## Development
-        
-        ### GitHub Workflow
-        
-        - There are two long-lived branches `main` and `develop`.
-        - The `develop` branch is used for development and can contain new / experimental features.  
-        - Pull-requests should be based on `develop`.
-        - Releases should be based on `main`.
-        - The `main` branch should always be as stable and functional as possible. In particular, merges should always happen from `develop` into `main`. 
-        - Git-Flow is enabled (and encouraged) with feature branches based on `develop` and hotfixes based on `main`. 
-        
-        ### GitHub Actions
-        
-        Each commit is tested and checked using gitHub actions with tox running:
-        - `doctest` -- run all doctests
-        - `coverage` -- ensure that all functions and classes are documented 
-        - `pycodestyle-minimal` -- ensure PEP8 style guide is followed (except we allow max line length 99)
-        - `relint` -- relint against some patterns taken from the SageMath source (config file .relint.yaml)
-        - `codespell` -- spellchecker
-        
-        To make sure that your commit passes all tests you should `make tox` or `make docker-tox REMOTE_SRC=0` on the command line.
-        
-        ### Versions
-        
-        Versioning of this project is managed by setuptools_scm.
-        To bump the version create a git tag `x.y.z` and the file 
-         `src/hilbert_modgroup/version.py` will then be automatically updated to contain 
-        ```
-        version = 'x.y.z.???'
-        version_tuple = (x, y, z, '???')
-        ```
-        where ??? depends on the state of the current directory. 
-        If you are creating a new version to release the source directory should be clean.
-        
-        ### PyPi
-        
-        To upload new versions to PyPi: 
-        1. `make sdist` -- creates a source distribution `dist/hilbert_modular_group-x.y.z`
-        2. `twine check dist/hilbert_modular_group-x.y.z`
-        3. `twine upload --repository pypi dist/hilbert_modular_group-z.y.z`
-        
 Keywords: "hilbert modular groups,reduction algorithms"
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Cython
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Hilbert Modular Groups
+
+This repository contains a python package `hilbert_modgroup` that implements algorithms 
+for Hilbert modular groups, in particular a reduction algorithm. The implementation is written in Python 
+and is dependent on SageMath.
+
+## Requirements
+- SageMath v9.6+ (https://www.sagemath.org/)
+  (Tested on v9.6, v9.7 and v10.0)
+
+## Installation
+### Using sage pip
+This package needs to be installed in the virtual environment provided by SageMath, and it is therefore necessary 
+to run the following command 
+```console
+$ sage -pip install --no-build-isolation hilbert-modular-group
+```
+**Note**: The `--no-build-isolation` is necessary as the compiler needs access 
+to certain library files from the sage installation and SageMath itself is 
+too large to be required as a build dependency. 
+As an alternative to this flag you can also specify the environment variable 
+SAGE_LIB explicitly.
+
+### From git source
+If the SageMath executable `sage` is in the current path you can install from source using the Makefile
+
+```console
+$ git clone https://github.com/fredstro/hilbertmodgroup.git
+$ cd hilbertmodgrup
+$ make install
+```
+
+### Docker
+If you do not have SageMath installed, but you have docker you can use install this package
+in a docker container built and executed using e.g. `make docker-sage` or `make docker-examples`
+
+
+## Usage
+The package can be imported and used as any other package. 
+For example, to find the reduction of the point given by [1+i,1+i] in H^2 
+with respect to the Hilbert modular group of Q joint by square-root of 5 write: 
+
+```
+sage: from hilbert_modgroup.all import *
+sage: H1=HilbertModularGroup(5)
+sage: P1=HilbertPullback(H1)
+sage: z = UpperHalfPlaneProductElement([1+I,1+I])
+sage: P1.reduce(z)
+[1.00000000000000*I, 1.00000000000000*I]
+sage: z = UpperHalfPlaneProductElement([0.25+I/2,1+I])
+sage: P1.reduce(z) # abs tol 1e-10
+[0.694427190999916 + 0.611145618000168*I, -0.309016994374947 + 1.30901699437495*I]
+sage: P1.reduce(z, return_map=True)[1]
+[-1/2*a + 1/2  1/2*a + 1/2]
+[-1/2*a + 1/2            0]
+
+```
+For more examples see the embedded doctests (search for `EXAMPLES`) as well as
+the `/examples` directory which contains Jupyter notebook with more extensive 
+examples corresponding to the paper
+"Reduction Algorithms for Hilbert Modular Groups" by F. Stromberg. (Reference to appear)
+
+## Examples
+
+The directory `/examples` contains Jupyter notebooks with example code to illustrate the interface and functionality of this package. 
+You can either open them manually from SageMath or run one of the following commands:
+`make examples`
+`make docker-examples`
+which will start up a Jupyter notebook server from sagemath either locally or in a docker container. 
+
+## Community Guidelines
+
+### How to Contribute?
+- Open an issue on GitHub and create a pull / merge request against the `develop` branch.
+### How to report an issue or a problem? 
+- First check if the issue is resolved in the `develop` branch. If not, open an issue on GitHub. 
+### How to seek help and support?
+- Contact the maintainer, Fredrik Stromberg, at: fredrik314@gmail.com (alternatively at fredrik.stromberg@nottingham.ac.uk)
+
+## Development and testing
+
+The make file `Makefile` contains a number of useful commands that you can run using 
+```console
+$ make <command>
+```
+The following commands are run in your local SagMath environment:
+1. `build` -- builds the package in place (sometimes useful for development).
+2. `sdist` -- create a source distribution in /sdist (can be installed using `sage -pip install sdist/<dist name>`)
+3. `install` -- build and install the package in the currently active sage environment
+4. `clean` -- remove all build and temporary files
+5. `test` -- run sage's doctests (same as `sage -t src/*`)
+6. `examples` -- run a Jupyter notebook with the SageMath kernel initialised at the `/examples` directory.
+7. `tox` -- run `sage -tox` with all environments: `doctest`, `coverage`, `pycodestyle`, `relint`, `codespell`
+   Note: If your local SageMath installation does not contain tox this will run `sage -pip install tox`.
+
+The following commands are run in an isolated docker container 
+and requires docker to be installed and running:
+1. `docker` -- build a docker container with the tag `hilbertmodgroup-{GIT_BRANCH}`
+2. `docker-rebuild` -- rebuild the docker container without cache
+3. `docker-test` -- run SageMath's doctests in the docker container
+4. `docker-examples` -- run a Jupyter notebook with the SageMath kernel initialised at the `/examples` directory 
+  and exposing the notebook at http://127.0.0.1:8888. The port used can be modified by 
+5. `docker-tox` -- run tox with all environments: `doctest`, `coverage`, `pycodestyle`, `relint`, `codespell`. 
+6. `docker-shell` -- run a shell in a docker container
+7. `docker-sage` -- run a sage interactive shell in a docker container
+
+The following command-line parameters are available 
+- `NBPORT` -- set the port of the notebook for `examples` and `docker-examples`  (default is 8888)
+- `TOX_ARGS` -- can be used to select one or more of the tox environments (default is all)
+- `REMOTE_SRC` -- set to 0 if you want to use the local source instead of pulling from gitHub (default 1)
+- `GIT_BRANCH` -- the branch to pull from gitHub (used if REMOTE_SRC=1)
+
+### Example usage
+Run tox coverage on the branch `main` from gitHub:
+
+`make docker-tox REMOTE_SRC=1 GIT_BRANCH=main TOX_ARGS=coverage`
+
+Run doctests on the local source with local version of sage:
+
+`make tox TOX_ARGS=doctest`
+
+Run relint on the local source with docker version of sage:
+
+`make docker-tox REMOTE_SRC=0 TOX_ARGS=relint`
+
+## Development
+
+### GitHub Workflow
+
+- There are two long-lived branches `main` and `develop`.
+- The `develop` branch is used for development and can contain new / experimental features.  
+- Pull-requests should be based on `develop`.
+- Releases should be based on `main`.
+- The `main` branch should always be as stable and functional as possible. In particular, merges should always happen from `develop` into `main`. 
+- Git-Flow is enabled (and encouraged) with feature branches based on `develop` and hotfixes based on `main`. 
+
+### GitHub Actions
+
+Each commit is tested and checked using gitHub actions with tox running:
+- `doctest` -- run all doctests
+- `coverage` -- ensure that all functions and classes are documented 
+- `pycodestyle-minimal` -- ensure PEP8 style guide is followed (except we allow max line length 99)
+- `relint` -- relint against some patterns taken from the SageMath source (config file .relint.yaml)
+- `codespell` -- spellchecker
+
+To make sure that your commit passes all tests you should `make tox` or `make docker-tox REMOTE_SRC=0` on the command line.
+
+### Versions
+
+Versioning of this project is managed by setuptools_scm.
+To bump the version create a git tag `x.y.z` and the file 
+ `src/hilbert_modgroup/version.py` will then be automatically updated to contain 
+```
+version = 'x.y.z.???'
+version_tuple = (x, y, z, '???')
+```
+where ??? depends on the state of the current directory. 
+If you are creating a new version to release the source directory should be clean.
+
+### PyPi
+
+To upload new versions to PyPi: 
+1. `make sdist` -- creates a source distribution `dist/hilbert_modular_group-x.y.z`
+2. `twine check dist/hilbert_modular_group-x.y.z`
+3. `twine upload --repository pypi dist/hilbert_modular_group-z.y.z`
+
+## References:
+
+- [![DOI](https://joss.theoj.org/papers/10.21105/joss.03996/status.svg)](https://doi.org/10.21105/joss.03996)
```

### Comparing `hilbert_modular_group-0.1.0/README.md` & `hilbert_modular_group-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Hilbert Modular Groups
 
 This repository contains a python package `hilbert_modgroup` that implements algorithms 
 for Hilbert modular groups, in particular a reduction algorithm. The implementation is written in Python 
 and is dependent on SageMath.
 
 ## Requirements
-- SageMath v9.4+ (https://www.sagemath.org/)
+- SageMath v9.6+ (https://www.sagemath.org/)
+  (Tested on v9.6, v9.7 and v10.0)
 
 ## Installation
 ### Using sage pip
 This package needs to be installed in the virtual environment provided by SageMath, and it is therefore necessary 
 to run the following command 
 ```console
 $ sage -pip install --no-build-isolation hilbert-modular-group
@@ -158,7 +159,11 @@
 
 ### PyPi
 
 To upload new versions to PyPi: 
 1. `make sdist` -- creates a source distribution `dist/hilbert_modular_group-x.y.z`
 2. `twine check dist/hilbert_modular_group-x.y.z`
 3. `twine upload --repository pypi dist/hilbert_modular_group-z.y.z`
+
+## References:
+
+- [![DOI](https://joss.theoj.org/papers/10.21105/joss.03996/status.svg)](https://doi.org/10.21105/joss.03996)
```

### Comparing `hilbert_modular_group-0.1.0/entrypoint.sh` & `hilbert_modular_group-0.1.1/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `hilbert_modular_group-0.1.0/examples/ExamplesK1.ipynb` & `hilbert_modular_group-0.1.1/examples/ExamplesK1.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9918081576893052%*

 * *Differences: {"'cells'": "{25: {'source': "*

 * *            '["plot_polygon(p,K1.fractional_ideal(1).integral_basis(),action=\'show\',**norm_args)"]}, '*

 * *            "27: {'source': "*

 * *            '["plot_polygon(p,K1.fractional_ideal(1).integral_basis(),action=\'save\',filename=\'K1.z1.domain1.pgf\',**norm_args)"]}, '*

 * *            "51: {'source': ['basis=K1.fractional_ideal(1).integral_basis(); basis']}, 54: "*

 * *            "{'source': {insert: [(0, "*

 * *            '"plot_polygon(p1,K1.fractional_ideal(1).integral_basis(),action= […]*

```diff
@@ -236,15 +236,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_polygon(p,K1.ideal(1).integral_basis(),action='show',**norm_args)"
+                "plot_polygon(p,K1.fractional_ideal(1).integral_basis(),action='show',**norm_args)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We observe here that of course the points $1$ and $-1$ lie on the norm bound curves. "
@@ -252,15 +252,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_polygon(p,K1.ideal(1).integral_basis(),action='save',filename='K1.z1.domain1.pgf',**norm_args)"
+                "plot_polygon(p,K1.fractional_ideal(1).integral_basis(),action='save',filename='K1.z1.domain1.pgf',**norm_args)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -457,15 +457,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "basis=K1.ideal(1).integral_basis(); basis"
+                "basis=K1.fractional_ideal(1).integral_basis(); basis"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -486,15 +486,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_polygon(p1,K1.ideal(1).integral_basis(),action='save',filename='K1.z2.domain1.pgf',xmin=-3,xmax=3,ymin=-3,ymax=3,\n",
+                "plot_polygon(p1,K1.fractional_ideal(1).integral_basis(),action='save',filename='K1.z2.domain1.pgf',xmin=-3,xmax=3,ymin=-3,ymax=3,\n",
                 "             ticks=[2,2],**norm_args)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -546,27 +546,27 @@
             "source": [
                 "P1._candidate_closest_cusps(z,use_initial_bd_d=False,as_cusps=True)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "SageMath 9.5",
+            "display_name": "SageMath 10.0",
             "language": "sage",
             "name": "sagemath"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.2"
+            "version": "3.11.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `hilbert_modular_group-0.1.0/examples/ExamplesK2.ipynb` & `hilbert_modular_group-0.1.1/examples/ExamplesK2.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9913507326007326%*

 * *Differences: {"'cells'": "{25: {'source': {insert: [(1, "*

 * *            '"plot_polygon(p,K2.fractional_ideal(1).integral_basis(),action=\'show\',xmin=-5,xmax=5,ymin=-4.5,ymax=4.5,**norm_args)")], '*

 * *            "delete: [1]}}, 26: {'source': "*

 * *            '["plot_polygon(p,K2.fractional_ideal(1).integral_basis(),action=\'save\',xmin=-5,xmax=5,ymin=-4.5,ymax=4.5,filename=\'K2.z1.domain1.pgf\',**norm_args)"]}, '*

 * *            '41: {\'source\': {insert: [(1, "norm_args = '*

 * *            '{\'norm_bound\':P2._bound_for_sigma_norm(z […]*

```diff
@@ -248,24 +248,24 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "p=P2._candidate_integers_sigma(z,domain='preimage',return_polyhedron=True)\n",
-                "plot_polygon(p,K2.ideal(1).integral_basis(),action='show',xmin=-5,xmax=5,ymin=-4.5,ymax=4.5,**norm_args)"
+                "plot_polygon(p,K2.fractional_ideal(1).integral_basis(),action='show',xmin=-5,xmax=5,ymin=-4.5,ymax=4.5,**norm_args)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_polygon(p,K2.ideal(1).integral_basis(),action='save',xmin=-5,xmax=5,ymin=-4.5,ymax=4.5,filename='K2.z1.domain1.pgf',**norm_args)"
+                "plot_polygon(p,K2.fractional_ideal(1).integral_basis(),action='save',xmin=-5,xmax=5,ymin=-4.5,ymax=4.5,filename='K2.z1.domain1.pgf',**norm_args)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -391,45 +391,46 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "p=P2._candidate_integers_sigma(z,domain='preimage',return_polyhedron=True)\n",
-                "norm_args = {'norm_bound':P2._bound_for_sigma_norm(z,dist=0.5)}\n",
-                "plot_polygon(p,K2.ideal(1).integral_basis(),action='show',**norm_args)"
+                "norm_args = {'norm_bound':P2._bound_for_sigma_norm(z,dist=0.5),'xmin':-35,'xmax':35}\n",
+                "plot_polygon(p,K2.fractional_ideal(1).integral_basis(),action='show',**norm_args)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_polygon(p,K2.ideal(1).integral_basis(),action='save',filename='K2.z2.domain1.pgf',**norm_args)"
+                "plot_polygon(p,K2.fractional_ideal(1).integral_basis(),action='save',filename='K2.z2.domain1.png',**norm_args)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "p=P2._candidate_integers_sigma(z,domain='polytope',return_polyhedron=True)\n",
-                "norm_args = {'norm_bound':P2._bound_for_sigma_norm(z,dist=0.5),'curve_map':P2.basis_matrix_ideal().inverse(),'norm_plot_factor':1.5}\n",
-                "plot_polygon(p,[1,1],action='show',ymax=4,ymin=-4,**norm_args)"
+                "norm_args = {'norm_bound':P2._bound_for_sigma_norm(z,dist=0.5),'curve_map':P2.basis_matrix_ideal().inverse(),\n",
+                "             'norm_plot_factor':1.5,'ymin':-7,'ymax':7}\n",
+                "plot_polygon(p,[1,1],action='show',**norm_args)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_polygon(p,[1,1],action='save',ymax=4,ymin=-4,filename='K2.z2.domain2.pgf',**norm_args)"
+                "plot_polygon(p,[1,1],action='save',filename='K2.z2.domain2.png',**norm_args)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "It is clear from these images that we again have only $\\sigma = 0, -1, 1$ and the potential cusps are also precisely $0$, $1$ and $-1$"
@@ -546,24 +547,24 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "p=P2._candidate_integers_sigma(z,domain='preimage',return_polyhedron=True)\n",
                 "norm_args = {'norm_bound':P2._bound_for_sigma_norm(z,dist=1.59731464318420)}\n",
-                "plot_polygon(p,K2.ideal(1).integral_basis(),action='show',ticks=[5,5],**norm_args)"
+                "plot_polygon(p,K2.fractional_ideal(1).integral_basis(),action='show',ticks=[5,5],**norm_args)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_polygon(p,K2.ideal(1).integral_basis(),action='save',ticks=[5,5],filename='K2.z3.domain1.pgf',**norm_args)"
+                "plot_polygon(p,K2.fractional_ideal(1).integral_basis(),action='save',ticks=[5,5],filename='K2.z3.domain1.pgf',**norm_args)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -655,24 +656,24 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "c.is_Gamma0_equivalent(H2.cusps()[0],K2.ideal(1)) # Not equivalent to infinity"
+                "c.is_Gamma0_equivalent(H2.cusps()[0],K2.fractional_ideal(1)) # Not equivalent to infinity"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "c.is_Gamma0_equivalent(H2.cusps()[1],K2.ideal(1),True) #Is equivalent to the other cusp."
+                "c.is_Gamma0_equivalent(H2.cusps()[1],K2.fractional_ideal(1),True) #Is equivalent to the other cusp."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -850,27 +851,27 @@
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "SageMath 9.5",
+            "display_name": "SageMath 10.0",
             "language": "sage",
             "name": "sagemath"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.2"
+            "version": "3.11.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `hilbert_modular_group-0.1.0/examples/ExamplesK3.ipynb` & `hilbert_modular_group-0.1.1/examples/ExamplesK3.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9925595238095238%*

 * *Differences: {"'metadata'": "{'kernelspec': {'display_name': 'SageMath 10.0'}, 'language_info': {'version': "*

 * *               "'3.11.3'}}"}*

```diff
@@ -486,27 +486,27 @@
             "source": [
                 "So 0 is the unique closest cusp."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "SageMath 9.5",
+            "display_name": "SageMath 10.0",
             "language": "sage",
             "name": "sagemath"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.2"
+            "version": "3.11.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `hilbert_modular_group-0.1.0/examples/ExamplesK4.ipynb` & `hilbert_modular_group-0.1.1/examples/ExamplesK4.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9920160455486542%*

 * *Differences: {"'cells'": "{10: {'source': ['K4.fractional_ideal(1).basis()']}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'SageMath 10.0'}, 'language_info': {'version': "*

 * *               "'3.11.3'}}"}*

```diff
@@ -108,15 +108,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "K4.ideal(1).basis()"
+                "K4.fractional_ideal(1).basis()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -226,27 +226,27 @@
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "SageMath 9.5",
+            "display_name": "SageMath 10.0",
             "language": "sage",
             "name": "sagemath"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.2"
+            "version": "3.11.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `hilbert_modular_group-0.1.0/examples/plot.py` & `hilbert_modular_group-0.1.1/examples/plot.py`

 * *Files identical despite different names*

### Comparing `hilbert_modular_group-0.1.0/hilbert_modular_group.egg-info/PKG-INFO` & `hilbert_modular_group-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,187 +1,193 @@
 Metadata-Version: 2.1
-Name: hilbert-modular-group
-Version: 0.1.0
+Name: hilbert_modular_group
+Version: 0.1.1
 Summary: Algorithms for Hilbert modular groups
 Home-page: https://github.com/fredstro/hilbertmodgroup
 Author: Fredrik Stromberg
 Author-email: fredrik314@gmail.com
 License: GPL v3+
 Project-URL: Bug Tracker, https://github.com/fredstro/hilbertmodgroup/issues
 Project-URL: Source Code, https://github.com/fredstro/hilbertmodgroup/
-Description: # Hilbert Modular Groups
-        
-        This repository contains a python package `hilbert_modgroup` that implements algorithms 
-        for Hilbert modular groups, in particular a reduction algorithm. The implementation is written in Python 
-        and is dependent on SageMath.
-        
-        ## Requirements
-        - SageMath v9.4+ (https://www.sagemath.org/)
-        
-        ## Installation
-        ### Using sage pip
-        This package needs to be installed in the virtual environment provided by SageMath, and it is therefore necessary 
-        to run the following command 
-        ```console
-        $ sage -pip install --no-build-isolation hilbert-modular-group
-        ```
-        **Note**: The `--no-build-isolation` is necessary as the compiler needs access 
-        to certain library files from the sage installation and SageMath itself is 
-        too large to be required as a build dependency. 
-        As an alternative to this flag you can also specify the environment variable 
-        SAGE_LIB explicitly.
-        
-        ### From git source
-        If the SageMath executable `sage` is in the current path you can install from source using the Makefile
-        
-        ```console
-        $ git clone https://github.com/fredstro/hilbertmodgroup.git
-        $ cd hilbertmodgrup
-        $ make install
-        ```
-        
-        ### Docker
-        If you do not have SageMath installed, but you have docker you can use install this package
-        in a docker container built and executed using e.g. `make docker-sage` or `make docker-examples`
-        
-        
-        ## Usage
-        The package can be imported and used as any other package. 
-        For example, to find the reduction of the point given by [1+i,1+i] in H^2 
-        with respect to the Hilbert modular group of Q joint by square-root of 5 write: 
-        
-        ```
-        sage: from hilbert_modgroup.all import *
-        sage: H1=HilbertModularGroup(5)
-        sage: P1=HilbertPullback(H1)
-        sage: z = UpperHalfPlaneProductElement([1+I,1+I])
-        sage: P1.reduce(z)
-        [1.00000000000000*I, 1.00000000000000*I]
-        sage: z = UpperHalfPlaneProductElement([0.25+I/2,1+I])
-        sage: P1.reduce(z) # abs tol 1e-10
-        [0.694427190999916 + 0.611145618000168*I, -0.309016994374947 + 1.30901699437495*I]
-        sage: P1.reduce(z, return_map=True)[1]
-        [-1/2*a + 1/2  1/2*a + 1/2]
-        [-1/2*a + 1/2            0]
-        
-        ```
-        For more examples see the embedded doctests (search for `EXAMPLES`) as well as
-        the `/examples` directory which contains Jupyter notebook with more extensive 
-        examples corresponding to the paper
-        "Reduction Algorithms for Hilbert Modular Groups" by F. Stromberg. (Reference to appear)
-        
-        ## Examples
-        
-        The directory `/examples` contains Jupyter notebooks with example code to illustrate the interface and functionality of this package. 
-        You can either open them manually from SageMath or run one of the following commands:
-        `make examples`
-        `make docker-examples`
-        which will start up a Jupyter notebook server from sagemath either locally or in a docker container. 
-        
-        ## Community Guidelines
-        
-        ### How to Contribute?
-        - Open an issue on GitHub and create a pull / merge request against the `develop` branch.
-        ### How to report an issue or a problem? 
-        - First check if the issue is resolved in the `develop` branch. If not, open an issue on GitHub. 
-        ### How to seek help and support?
-        - Contact the maintainer, Fredrik Stromberg, at: fredrik314@gmail.com (alternatively at fredrik.stromberg@nottingham.ac.uk)
-        
-        ## Development and testing
-        
-        The make file `Makefile` contains a number of useful commands that you can run using 
-        ```console
-        $ make <command>
-        ```
-        The following commands are run in your local SagMath environment:
-        1. `build` -- builds the package in place (sometimes useful for development).
-        2. `sdist` -- create a source distribution in /sdist (can be installed using `sage -pip install sdist/<dist name>`)
-        3. `install` -- build and install the package in the currently active sage environment
-        4. `clean` -- remove all build and temporary files
-        5. `test` -- run sage's doctests (same as `sage -t src/*`)
-        6. `examples` -- run a Jupyter notebook with the SageMath kernel initialised at the `/examples` directory.
-        7. `tox` -- run `sage -tox` with all environments: `doctest`, `coverage`, `pycodestyle`, `relint`, `codespell`
-           Note: If your local SageMath installation does not contain tox this will run `sage -pip install tox`.
-        
-        The following commands are run in an isolated docker container 
-        and requires docker to be installed and running:
-        1. `docker` -- build a docker container with the tag `hilbertmodgroup-{GIT_BRANCH}`
-        2. `docker-rebuild` -- rebuild the docker container without cache
-        3. `docker-test` -- run SageMath's doctests in the docker container
-        4. `docker-examples` -- run a Jupyter notebook with the SageMath kernel initialised at the `/examples` directory 
-          and exposing the notebook at http://127.0.0.1:8888. The port used can be modified by 
-        5. `docker-tox` -- run tox with all environments: `doctest`, `coverage`, `pycodestyle`, `relint`, `codespell`. 
-        6. `docker-shell` -- run a shell in a docker container
-        7. `docker-sage` -- run a sage interactive shell in a docker container
-        
-        The following command-line parameters are available 
-        - `NBPORT` -- set the port of the notebook for `examples` and `docker-examples`  (default is 8888)
-        - `TOX_ARGS` -- can be used to select one or more of the tox environments (default is all)
-        - `REMOTE_SRC` -- set to 0 if you want to use the local source instead of pulling from gitHub (default 1)
-        - `GIT_BRANCH` -- the branch to pull from gitHub (used if REMOTE_SRC=1)
-        
-        ### Example usage
-        Run tox coverage on the branch `main` from gitHub:
-        
-        `make docker-tox REMOTE_SRC=1 GIT_BRANCH=main TOX_ARGS=coverage`
-        
-        Run doctests on the local source with local version of sage:
-        
-        `make tox TOX_ARGS=doctest`
-        
-        Run relint on the local source with docker version of sage:
-        
-        `make docker-tox REMOTE_SRC=0 TOX_ARGS=relint`
-        
-        ## Development
-        
-        ### GitHub Workflow
-        
-        - There are two long-lived branches `main` and `develop`.
-        - The `develop` branch is used for development and can contain new / experimental features.  
-        - Pull-requests should be based on `develop`.
-        - Releases should be based on `main`.
-        - The `main` branch should always be as stable and functional as possible. In particular, merges should always happen from `develop` into `main`. 
-        - Git-Flow is enabled (and encouraged) with feature branches based on `develop` and hotfixes based on `main`. 
-        
-        ### GitHub Actions
-        
-        Each commit is tested and checked using gitHub actions with tox running:
-        - `doctest` -- run all doctests
-        - `coverage` -- ensure that all functions and classes are documented 
-        - `pycodestyle-minimal` -- ensure PEP8 style guide is followed (except we allow max line length 99)
-        - `relint` -- relint against some patterns taken from the SageMath source (config file .relint.yaml)
-        - `codespell` -- spellchecker
-        
-        To make sure that your commit passes all tests you should `make tox` or `make docker-tox REMOTE_SRC=0` on the command line.
-        
-        ### Versions
-        
-        Versioning of this project is managed by setuptools_scm.
-        To bump the version create a git tag `x.y.z` and the file 
-         `src/hilbert_modgroup/version.py` will then be automatically updated to contain 
-        ```
-        version = 'x.y.z.???'
-        version_tuple = (x, y, z, '???')
-        ```
-        where ??? depends on the state of the current directory. 
-        If you are creating a new version to release the source directory should be clean.
-        
-        ### PyPi
-        
-        To upload new versions to PyPi: 
-        1. `make sdist` -- creates a source distribution `dist/hilbert_modular_group-x.y.z`
-        2. `twine check dist/hilbert_modular_group-x.y.z`
-        3. `twine upload --repository pypi dist/hilbert_modular_group-z.y.z`
-        
 Keywords: "hilbert modular groups,reduction algorithms"
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Cython
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Hilbert Modular Groups
+
+This repository contains a python package `hilbert_modgroup` that implements algorithms 
+for Hilbert modular groups, in particular a reduction algorithm. The implementation is written in Python 
+and is dependent on SageMath.
+
+## Requirements
+- SageMath v9.6+ (https://www.sagemath.org/)
+  (Tested on v9.6, v9.7 and v10.0)
+
+## Installation
+### Using sage pip
+This package needs to be installed in the virtual environment provided by SageMath, and it is therefore necessary 
+to run the following command 
+```console
+$ sage -pip install --no-build-isolation hilbert-modular-group
+```
+**Note**: The `--no-build-isolation` is necessary as the compiler needs access 
+to certain library files from the sage installation and SageMath itself is 
+too large to be required as a build dependency. 
+As an alternative to this flag you can also specify the environment variable 
+SAGE_LIB explicitly.
+
+### From git source
+If the SageMath executable `sage` is in the current path you can install from source using the Makefile
+
+```console
+$ git clone https://github.com/fredstro/hilbertmodgroup.git
+$ cd hilbertmodgrup
+$ make install
+```
+
+### Docker
+If you do not have SageMath installed, but you have docker you can use install this package
+in a docker container built and executed using e.g. `make docker-sage` or `make docker-examples`
+
+
+## Usage
+The package can be imported and used as any other package. 
+For example, to find the reduction of the point given by [1+i,1+i] in H^2 
+with respect to the Hilbert modular group of Q joint by square-root of 5 write: 
+
+```
+sage: from hilbert_modgroup.all import *
+sage: H1=HilbertModularGroup(5)
+sage: P1=HilbertPullback(H1)
+sage: z = UpperHalfPlaneProductElement([1+I,1+I])
+sage: P1.reduce(z)
+[1.00000000000000*I, 1.00000000000000*I]
+sage: z = UpperHalfPlaneProductElement([0.25+I/2,1+I])
+sage: P1.reduce(z) # abs tol 1e-10
+[0.694427190999916 + 0.611145618000168*I, -0.309016994374947 + 1.30901699437495*I]
+sage: P1.reduce(z, return_map=True)[1]
+[-1/2*a + 1/2  1/2*a + 1/2]
+[-1/2*a + 1/2            0]
+
+```
+For more examples see the embedded doctests (search for `EXAMPLES`) as well as
+the `/examples` directory which contains Jupyter notebook with more extensive 
+examples corresponding to the paper
+"Reduction Algorithms for Hilbert Modular Groups" by F. Stromberg. (Reference to appear)
+
+## Examples
+
+The directory `/examples` contains Jupyter notebooks with example code to illustrate the interface and functionality of this package. 
+You can either open them manually from SageMath or run one of the following commands:
+`make examples`
+`make docker-examples`
+which will start up a Jupyter notebook server from sagemath either locally or in a docker container. 
+
+## Community Guidelines
+
+### How to Contribute?
+- Open an issue on GitHub and create a pull / merge request against the `develop` branch.
+### How to report an issue or a problem? 
+- First check if the issue is resolved in the `develop` branch. If not, open an issue on GitHub. 
+### How to seek help and support?
+- Contact the maintainer, Fredrik Stromberg, at: fredrik314@gmail.com (alternatively at fredrik.stromberg@nottingham.ac.uk)
+
+## Development and testing
+
+The make file `Makefile` contains a number of useful commands that you can run using 
+```console
+$ make <command>
+```
+The following commands are run in your local SagMath environment:
+1. `build` -- builds the package in place (sometimes useful for development).
+2. `sdist` -- create a source distribution in /sdist (can be installed using `sage -pip install sdist/<dist name>`)
+3. `install` -- build and install the package in the currently active sage environment
+4. `clean` -- remove all build and temporary files
+5. `test` -- run sage's doctests (same as `sage -t src/*`)
+6. `examples` -- run a Jupyter notebook with the SageMath kernel initialised at the `/examples` directory.
+7. `tox` -- run `sage -tox` with all environments: `doctest`, `coverage`, `pycodestyle`, `relint`, `codespell`
+   Note: If your local SageMath installation does not contain tox this will run `sage -pip install tox`.
+
+The following commands are run in an isolated docker container 
+and requires docker to be installed and running:
+1. `docker` -- build a docker container with the tag `hilbertmodgroup-{GIT_BRANCH}`
+2. `docker-rebuild` -- rebuild the docker container without cache
+3. `docker-test` -- run SageMath's doctests in the docker container
+4. `docker-examples` -- run a Jupyter notebook with the SageMath kernel initialised at the `/examples` directory 
+  and exposing the notebook at http://127.0.0.1:8888. The port used can be modified by 
+5. `docker-tox` -- run tox with all environments: `doctest`, `coverage`, `pycodestyle`, `relint`, `codespell`. 
+6. `docker-shell` -- run a shell in a docker container
+7. `docker-sage` -- run a sage interactive shell in a docker container
+
+The following command-line parameters are available 
+- `NBPORT` -- set the port of the notebook for `examples` and `docker-examples`  (default is 8888)
+- `TOX_ARGS` -- can be used to select one or more of the tox environments (default is all)
+- `REMOTE_SRC` -- set to 0 if you want to use the local source instead of pulling from gitHub (default 1)
+- `GIT_BRANCH` -- the branch to pull from gitHub (used if REMOTE_SRC=1)
+
+### Example usage
+Run tox coverage on the branch `main` from gitHub:
+
+`make docker-tox REMOTE_SRC=1 GIT_BRANCH=main TOX_ARGS=coverage`
+
+Run doctests on the local source with local version of sage:
+
+`make tox TOX_ARGS=doctest`
+
+Run relint on the local source with docker version of sage:
+
+`make docker-tox REMOTE_SRC=0 TOX_ARGS=relint`
+
+## Development
+
+### GitHub Workflow
+
+- There are two long-lived branches `main` and `develop`.
+- The `develop` branch is used for development and can contain new / experimental features.  
+- Pull-requests should be based on `develop`.
+- Releases should be based on `main`.
+- The `main` branch should always be as stable and functional as possible. In particular, merges should always happen from `develop` into `main`. 
+- Git-Flow is enabled (and encouraged) with feature branches based on `develop` and hotfixes based on `main`. 
+
+### GitHub Actions
+
+Each commit is tested and checked using gitHub actions with tox running:
+- `doctest` -- run all doctests
+- `coverage` -- ensure that all functions and classes are documented 
+- `pycodestyle-minimal` -- ensure PEP8 style guide is followed (except we allow max line length 99)
+- `relint` -- relint against some patterns taken from the SageMath source (config file .relint.yaml)
+- `codespell` -- spellchecker
+
+To make sure that your commit passes all tests you should `make tox` or `make docker-tox REMOTE_SRC=0` on the command line.
+
+### Versions
+
+Versioning of this project is managed by setuptools_scm.
+To bump the version create a git tag `x.y.z` and the file 
+ `src/hilbert_modgroup/version.py` will then be automatically updated to contain 
+```
+version = 'x.y.z.???'
+version_tuple = (x, y, z, '???')
+```
+where ??? depends on the state of the current directory. 
+If you are creating a new version to release the source directory should be clean.
+
+### PyPi
+
+To upload new versions to PyPi: 
+1. `make sdist` -- creates a source distribution `dist/hilbert_modular_group-x.y.z`
+2. `twine check dist/hilbert_modular_group-x.y.z`
+3. `twine upload --repository pypi dist/hilbert_modular_group-z.y.z`
+
+## References:
+
+- [![DOI](https://joss.theoj.org/papers/10.21105/joss.03996/status.svg)](https://doi.org/10.21105/joss.03996)
```

### Comparing `hilbert_modular_group-0.1.0/hilbert_modular_group.egg-info/SOURCES.txt` & `hilbert_modular_group-0.1.1/hilbert_modular_group.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hilbert_modular_group-0.1.0/setup.cfg` & `hilbert_modular_group-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hilbert_modular_group-0.1.0/src/hilbert_modgroup/hilbert_modular_group_class.py` & `hilbert_modular_group-0.1.1/src/hilbert_modgroup/hilbert_modular_group_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 
 
 AUTHORS:
 - Fredrik Stromberg (2021)
 
 
 """
+import sage
 from sage.categories.groups import Groups
 from sage.groups.matrix_gps.linear import LinearMatrixGroup_generic
 from sage.modular.cusps_nf import NFCusp
 from sage.rings.infinity import infinity
-from sage.rings.number_field.number_field import is_NumberField, QuadraticField, CyclotomicField
+from sage.rings.number_field.number_field import QuadraticField, CyclotomicField
 from sage.all import latex, Integer, Matrix, matrix
 from sage.misc.cachefunc import cached_method
 from sage.rings.number_field.order import is_NumberFieldOrder
 
 # from .upper_half_plane import ComplexPlaneOtimesK
 from hilbert_modgroup.upper_half_plane import ComplexPlaneProductElement__class
 from .hilbert_modular_group_element import HilbertModularGroupElement
@@ -88,15 +89,16 @@
             sage: HilbertModularGroup(QuadraticField(5))
             Hilbert Modular Group ... x^2 - 5 with a = 2.236067977499790?
 
 
     """
     if isinstance(number_field, (int, Integer)) and number_field > 0:
         ring = QuadraticField(number_field).ring_of_integers()
-    elif is_NumberField(number_field) and number_field.is_totally_real():
+    elif isinstance(number_field, sage.rings.number_field.number_field_base.NumberField) \
+            and number_field.is_totally_real():
         ring = number_field.ring_of_integers()
     else:
         raise ValueError("The input must be a totally real Number Field or a positive integer")
     if not projective:
         raise NotImplementedError("Only PSL2 is implemented at the moment.")
     degree = Integer(2)
     name = f'Hilbert Modular Group PSL({degree}) over {ring}'
@@ -159,15 +161,15 @@
         # Instance data related to cusps
         self._ncusps = None
         self._cusps = []
         self._ideal_cusp_representatives = []
         self._cusp_normalizing_maps = {}
         self._cusp_normalizing_maps_inverse = {}
         # At the moment we only deal with full level (1)
-        self._level = base_ring.ideal(1)
+        self._level = base_ring.fractional_ideal(1)
         super(HilbertModularGroup_class, self).__init__(degree=Integer(2), base_ring=base_ring,
                                                         special=True,
                                                         sage_name=sage_name,
                                                         latex_string=latex_string,
                                                         category=Groups().Infinite(),
                                                         invariant_form=None)
 
@@ -249,15 +251,15 @@
             sage: H.T()
             [1 1]
             [0 1]
             sage: u0,u1=H.base_ring().number_field().unit_group().gens()
             sage: H.T(u0)
             [ 1 -1]
             [ 0  1]
-            sage: H.T(u1)
+            sage: H.T(u0*u1)
             [          1 1/2*a - 1/2]
             [          0           1]
         """
         return self([1, a, 0, 1])
 
     @cached_method
     def L(self, a):
@@ -274,15 +276,15 @@
             sage: H.L(1)
             [1 0]
             [1 1]
             sage: u0,u1=H.base_ring().number_field().unit_group().gens()
             sage: H.L(u0)
             [ 1 0]
             [-1 1]
-            sage: H.L(u1)
+            sage: H.L(u0*u1)
             [          1           0]
             [1/2*a - 1/2           1]
 
         """
         return self([1, 0, a, 1])
 
     @cached_method
@@ -300,15 +302,15 @@
             sage: H.E(1)
             [1 0]
             [0 1]
             sage: u0,u1=H.base_ring().number_field().unit_group().gens()
             sage: H.E(u0)
             [-1  0]
             [ 0 -1]
-            sage: H.E(u1)
+            sage: H.E(u0*u1)
             [1/2*a - 1/2           0]
             [          0 1/2*a + 1/2]
 
         """
         return self([u, 0, 0, u ** -1])
 
     def gens(self, algorithm='standard'):
@@ -462,15 +464,15 @@
              Cusp [2: 1/3*a^2 + 1/3*a - 23/3] of Number Field ... polynomial x^3 - 36*x - 1,
              Cusp [6: 1/3*a^2 + 1/3*a - 26/3] of Number Field ... polynomial x^3 - 36*x - 1]
 
             sage: K4 = NumberField(x**4 - 17*x**2 + 36,names='a'); a=K4.gen()
             sage: H4=HilbertModularGroup(NumberField(x**4 - 17*x**2 + 36,names='a'))
             sage: H4.cusps()
             [Cusp Infinity of Number Field in a with defining polynomial x^4 - 17*x^2 + 36,
-             Cusp [2: a] of Number Field in a with defining polynomial x^4 - 17*x^2 + 36]
+             Cusp [2: a + 1] of Number Field in a with defining polynomial x^4 - 17*x^2 + 36]
 
 
         """
         for a in self.ideal_cusp_representatives():
             logger.debug("Set cusp info for ideal a={0}".format(a))
             if a.is_trivial():
                 ca = NFCusp(self.base_ring().number_field(),
@@ -487,15 +489,16 @@
         return self._cusps
 
     def ideal_cusp_representatives(self):
         r"""
         Return a list of ideals corresponding to cusp representatives, i.e.
         ideal representatives of ideal classes.
 
-        Note: We choose the ideal of smallest norm in each class.
+        Note: We choose an ideal of smallest norm in each class.
+            If the ideal given by sage is already minimal we return this.
 
         EXAMPLES::
 
             sage: from hilbert_modgroup.all import HilbertModularGroup
             sage: H1=HilbertModularGroup(5)
             sage: H1.ideal_cusp_representatives()
             [Fractional ideal (1)]
@@ -512,25 +515,27 @@
              Fractional ideal (2, a + 1),
              Fractional ideal (3, 1/3*a^2 + 1/3*a - 26/3),
              Fractional ideal (2, 1/3*a^2 + 1/3*a - 23/3),
              Fractional ideal (6, 1/3*a^2 + 1/3*a - 26/3)]
             sage: K4 = NumberField(x**4 - 17*x**2 + 36,names='a'); a=K4.gen()
             sage: H4=HilbertModularGroup(NumberField(x**4 - 17*x**2 + 36,names='a'))
             sage: H4.ideal_cusp_representatives()
-            [Fractional ideal (1), Fractional ideal (2, a)]
+            [Fractional ideal (1), Fractional ideal (2, a + 1)]
 
 
         """
         if not self._ideal_cusp_representatives:
             self._ideal_cusp_representatives = []
 
             def _find_equivalent_ideal_of_minimal_norm(c):
                 for a in self.base_ring().number_field().ideals_of_bdd_norm(c.norm() - 1).items():
                     for ideala in a[1]:
                         if (ideala * c ** -1).is_principal():
+                            if c.norm() <= ideala.norm():
+                                return c
                             return ideala
                 return c
 
             for ideal_class in self.base_ring().class_group():
                 c = ideal_class.ideal().reduce_equiv()
                 # NOTE: Even though we use 'reduce_equiv' we are not guaranteed a representative
                 #       with minimal **norm**
@@ -863,16 +868,16 @@
             sage: H3.cusp_normalizing_map(H3.cusps()[3])
             [                     2                      1]
             [1/3*a^2 + 1/3*a - 23/3 1/6*a^2 + 1/6*a - 10/3]
 
             sage: K4 = NumberField(x**4 - 17*x**2 + 36,names='a'); a=K4.gen()
             sage: H4=HilbertModularGroup(K4)
             sage: H4.cusp_normalizing_map(H4.cusps()[1])
-            [                 2 1/12*a^3 - 17/12*a]
-            [                 a                 -1]
+            [                          2 1/4*a^3 - 1/4*a^2 - 4*a + 4]
+            [                      a + 1                          -2]
 
         """
         base_nf = self.base_ring().number_field()
         if not isinstance(cusp, NFCusp) or cusp.number_field() != base_nf:
             raise ValueError(f"Input should be a NF cusp defined over {base_nf}!")
         ca, cb = (cusp.numerator(), cusp.denominator())
         if not (ca, cb) in self._cusp_normalizing_maps:
```

### Comparing `hilbert_modular_group-0.1.0/src/hilbert_modgroup/hilbert_modular_group_element.pyx` & `hilbert_modular_group-0.1.1/src/hilbert_modgroup/hilbert_modular_group_element.pyx`

 * *Files identical despite different names*

### Comparing `hilbert_modular_group-0.1.0/src/hilbert_modgroup/pullback.py` & `hilbert_modular_group-0.1.1/src/hilbert_modgroup/pullback.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,20 +215,20 @@
 
         EXAMPLES::
 
             sage: from hilbert_modgroup.all import *
             sage: H1 = HilbertModularGroup(5)
             sage: P1 = HilbertPullback(H1)
             sage: P1.fundamental_units()
-            [1/2*a - 1/2]
+            [-1/2*a + 1/2]
             sage: x = ZZ['x'].gen()
             sage: H3=HilbertModularGroup(NumberField(x^3-36*x-1, names='a'))
             sage: P3=HilbertPullback(H3)
             sage: P3.fundamental_units()
-            [-a, -a - 6]
+            [a, -a - 6]
 
         """
         nf = self.group().base_ring().number_field()
         return nf.unit_group().fundamental_units()
 
     def Y(self, z, return_error_estimate=False):
         r"""
@@ -268,23 +268,23 @@
             (2.42129586908836)
 
             # The precision gets worse when the imaginary parts have large
             # differences.
             sage: H3=HilbertModularGroup(NumberField(x^3-36*x-1, names='a'))
             sage: P3=HilbertPullback(H3)
             sage: z=UpperHalfPlaneProductElement([CC(0,1),CC(0,2),CC(0,1)])
-            sage: P3.Y(z,return_error_estimate=True)
+            sage: P3.Y(z,return_error_estimate=True) # abs tol 1e-10
             ((-0.128907673154173, 0.0000882959672881647), 2.220446049250313e-16)
             sage: z=UpperHalfPlaneProductElement([CC(0,100),CC(0,200),CC(0,100)])
-            sage: P3.Y(z,return_error_estimate=True)
+            sage: P3.Y(z,return_error_estimate=True) # abs tol 1e-10
             ((-0.128907673154173, 0.0000882959672880335), 6.38378239159465e-16)
             sage: z=UpperHalfPlaneProductElement([CC(0,1),CC(0,2),CC(0,100)])
             sage: P3.Y(z)
             (0.638975592292095, 0.680877344221728)
-            sage: P3.Y(z,return_error_estimate=True)
+            sage: P3.Y(z,return_error_estimate=True) # abs tol 1e-10
             ((0.638975592292095, 0.680877344221728), 1.1546319456101628e-14)
             sage: CF=ComplexField(106)
             sage: z=UpperHalfPlaneProductElement([CF(0,1),CF(0,2),CF(0,100)])
             sage: P3.Y(z,return_error_estimate=True)
             ((0.6389755922920966140584010614944, 0.6808773442217317886140786738603),
              2.0214560696288428e-30)
 
@@ -348,16 +348,16 @@
             )
 
             sage: z=UpperHalfPlaneProductElement([CC(0,0.0001),CC(0,0.1),CC(0,100)])
             sage: P3.reduce_by_units(z,return_map=True)
             (
             [0.0143665696311556*I, 3.63341121163000*I, 0.0191572146738068*I],
             <BLANKLINE>
-            [    a - 6         0]
-            [        0 a^2 + 6*a]
+            [   -a + 6          0]
+            [        0 -a^2 - 6*a]
             )
 
         """
         K = self.group().base_ring().number_field()
         units = K.unit_group().gens()[1:]  # Only include the units != -1
         # To avoid overflow it is more efficient to apply the map,
         # e.g. compute (z*u**-k)/u**k instead of z*u**-(2k)
@@ -531,30 +531,30 @@
         - ``a`` -- ideal or number field element.
 
         EXAMPLES::
 
             sage: from hilbert_modgroup.all import *
             sage: H1 = HilbertModularGroup(5)
             sage: P1 = HilbertPullback(H1)
-            sage: b1,b2=P1.number_field().ideal(1).basis()
+            sage: b1,b2=P1.number_field().fractional_ideal(1).basis()
             sage: P1.coordinates_in_number_field_ideal(b1)
             (1, 0)
             sage: P1.coordinates_in_number_field_ideal(b2)
             (0, 1)
             sage: H2=HilbertModularGroup(10)
             sage: P2 = HilbertPullback(H2)
-            sage: b1,b2=P2.number_field().ideal(1).basis()
+            sage: b1,b2=P2.number_field().fractional_ideal(1).basis()
             sage: P2.coordinates_in_number_field_ideal(b1)
             (1, 0)
             sage: P2.coordinates_in_number_field_ideal(b2)
             (0, 1)
             sage: x=var('x')
             sage: H3=HilbertModularGroup(NumberField(x^3-36*x-1, names='a'))
             sage: P3=HilbertPullback(H3)
-            sage: b1,b2,b3=P3.number_field().ideal(1).basis()
+            sage: b1,b2,b3=P3.number_field().fractional_ideal(1).basis()
             sage: P3.coordinates_in_number_field_ideal(b1)
             (1, 0, 0)
             sage: P3.coordinates_in_number_field_ideal(b2)
             (0, 1, 0)
             sage: P3.coordinates_in_number_field_ideal(b3)
             (0, 0, 1)
 
@@ -658,15 +658,15 @@
             [   23.3400000000000  0.0200000000000000  0.0100000000000000  0.0300000000000000]
             [  -73.8075605883300  0.0632455532033676 -0.0316227766016838  0.0948683298050514]
             sage: x = ZZ['x'].gen()
             sage: H3=HilbertModularGroup(NumberField(x^3-36*x-1, names='a'))
             sage: P3=HilbertPullback(H3)
             sage: K3=P3.number_field()
             sage: z = UpperHalfPlaneProductElement([0+0.02*I,10+0.2*I,1+0.2*I])
-            sage: P3.basis_matrix_ideal_plusz(z,K3.ideal(1))
+            sage: P3.basis_matrix_ideal_plusz(z,K3.fractional_ideal(1))
             [    1.00000000000000     1.00000000000000     1.00000000000000    0.000000000000000...
             [   -5.98606258583498  -0.0277783731902446     6.01384095902523    0.000000000000000...
             [    2.28229423189948    -7.67566891172438     6.39337467982490    0.000000000000000...
             [   0.000000000000000     10.0000000000000     1.00000000000000   0.0200000000000000...
             [  -0.000000000000000   -0.277783731902446     6.01384095902523   -0.119721251716700...
             [   0.000000000000000    -76.7566891172438     6.39337467982490   0.0456458846379896...
 
@@ -738,15 +738,15 @@
             [ 212  -67  -15    1]
             [ 348 -110  -14    5]
             sage: x = ZZ['x'].gen()
             sage: H3=HilbertModularGroup(NumberField(x^3-36*x-1, names='a'))
             sage: P3=HilbertPullback(H3)
             sage: K3=P3.number_field()
             sage: z = UpperHalfPlaneProductElement([0+0.02*I,10+0.2*I,1+0.2*I])
-            sage: P3._shortest_vectors_ideal_plusz(z,K3.ideal(1))
+            sage: P3._shortest_vectors_ideal_plusz(z,K3.fractional_ideal(1))
             [  2   0  -1  -1   1   0]
             [ 15   1  -4   3  -1   1]
             [-28  -2   7   8  -2   0]
             [ 36   3  -8  -2  -1   1]
             [ 18   1  -5   2   0   1]
             [ 21   2  -4 -13   2  -1]
 
@@ -785,15 +785,15 @@
         return U
 
     def get_heuristic_closest_cusp(self, z, a=None, as_cusp=False):
         """
         Try to find a heuristic closest cusp using LLL.
 
         INPUT:
-        - ``z`` -- point in the uper half-plane
+        - ``z`` -- point in the upper half-plane
         - ``a`` -- ideal or number field element (default = None)
                     If None then this is set to the entire ring of integers.
         - ``as_cusp`` -- boolean (default: False)
                     If True we return an element of type NFCusp
         EXAMPLES::
 
             sage: from hilbert_modgroup.all import *
@@ -860,27 +860,27 @@
 
         EXAMPLES::
 
         sage: from hilbert_modgroup.all import *
         sage: P1=HilbertPullback(HilbertModularGroup(5))
         sage: P1._construct_ideal(1)
         Fractional ideal (1)
-        sage: P1._construct_ideal(P1.number_field().ideal(1))
+        sage: P1._construct_ideal(P1.number_field().fractional_ideal(1))
         Fractional ideal (1)
 
 
         """
         if a is None:
-            ideala = self.group().base_ring().ideal(1)
+            ideala = self.group().base_ring().fractional_ideal(1)
         elif is_NumberFieldIdeal(a):
             ideala = a
         elif a in self.group().base_ring() and not b:
-            ideala = self.group().base_ring().ideal(a)
+            ideala = self.group().base_ring().fractional_ideal(a)
         elif a in self.group().base_ring() and b in self.group().base_ring():
-            ideala = self.group().base_ring().ideal(a, b)
+            ideala = self.group().base_ring().fractional_ideal(a, b)
         else:
             raise ValueError(f"Could not construct a number field ideal from a={a} and b={b}")
         return ideala
 
     def _construct_cusp(self, c, d=None):
         r"""
         Return an instance of NFCusp for the number field of self from input c and optional d
@@ -920,15 +920,15 @@
             sage: from hilbert_modgroup.all import *
             sage: from hilbert_modgroup.upper_half_plane import UpperHalfPlaneProductElement
             sage: H1 = HilbertModularGroup(5)
             sage: P1 = HilbertPullback(H1)
             sage: z=UpperHalfPlaneProductElement([CC(1,1),CC(1,1)])
             sage: P1.X(z)
             (1.00000000000000, 0.000000000000000)
-            sage: b1,b2 = H1.base_ring().ideal(1).integral_basis(); b1,b2
+            sage: b1,b2 = H1.base_ring().fractional_ideal(1).integral_basis(); b1,b2
             (1, 1/2*a - 1/2)
             sage: P1.X(z+b1)
             (2.00000000000000, 0.000000000000000)
             sage: P1.X(z-b1)
             (0.000000000000000, 0.000000000000000)
             sage: P1.X(z+b2)
             (0.999999999999999, 1.00000000000000)
@@ -1078,16 +1078,16 @@
             sage: z = UpperHalfPlaneProductElement([1+I,1+I])
             sage: P1.reduce(z)
             [1.00000000000000*I, 1.00000000000000*I]
             sage: z = UpperHalfPlaneProductElement([0.25+I/2,1+I])
             sage: P1.reduce(z) # abs tol 1e-10
             [0.694427190999916 + 0.611145618000168*I, -0.309016994374947 + 1.30901699437495*I]
             sage: P1.reduce(z, return_map=True)[1]
-            [-1/2*a + 1/2  1/2*a + 1/2]
-            [-1/2*a + 1/2            0]
+            [ 1/2*a - 1/2  -1/2*a - 1/2]
+            [ 1/2*a - 1/2             0]
 
         """
         c = self.find_closest_cusp(z, return_multiple=False, as_cusp=True)
         c_rep, Umu = self.group().cusp_representative(c, return_map=True)
         A = self._group.cusp_normalizing_map(c_rep)
         # Move to the cusp representative
         w = z.apply(A.inverse()*Umu)
@@ -1529,19 +1529,19 @@
             3.510634603648856
             sage: x = ZZ['x'].gen()
             sage: K3.<a> = NumberField(x^3-x^2-2*x+1)
             sage: P3 = HilbertPullback(HilbertModularGroup(K3))
             sage: P3.Di() # abs tol 1e-10
             5.04891733952231
             sage: P3.Di(0) # abs tol 1e-10
-            2.01219217261232
+            1.67389896224499
             sage: P3.Di(1) # abs tol 1e-10
-            1.49899286313093
+            2.01219217261232
             sage: P3.Di(2) # abs tol 1e-10
-            1.67389896224499
+            1.49899286313093
         """
         n = self.group().base_ring().number_field().degree()
         return float(self.max_ideal_norm()**(1/n)*self._exp_matrix_BLambda_row_sum(i).sqrt())
 
     @cached_method()
     def D(self):
         r"""
@@ -1557,15 +1557,15 @@
             sage: P2 = HilbertPullback(HilbertModularGroup(10))
             sage: P2.D() # abs tol 1e-10
             [3.510634603648856, 3.510634603648856]
             sage: x = ZZ['x'].gen()
             sage: K3.<a> = NumberField(x^3-x^2-2*x+1)
             sage: P3 = HilbertPullback(HilbertModularGroup(K3))
             sage: P3.D() # abs tol 1e-10
-            [2.0121921726123237, 1.4989928631309313, 1.6738989622449851]
+            [1.673898962244985, 2.012192172612324, 1.4989928631309313]
         """
         n = self.group().base_ring().number_field().degree()
         return [self.Di(i) for i in range(n)]
 
     #
     # A collection of bounds necessary for finding the closest cusp.
     #
@@ -2056,23 +2056,23 @@
             sage: from hilbert_modgroup.all import *
             sage: H1 = HilbertModularGroup(5)
             sage: P1 = HilbertPullback(H1)
             sage: P1._get_lattice_and_ideal_basis()
             ([[1.00000000000000, -1.61803398874989],
               [1.00000000000000, 0.618033988749895]],
              [1, 1/2*a - 1/2])
-            sage: P1._get_lattice_and_ideal_basis(H1.base_ring().ideal(2))
+            sage: P1._get_lattice_and_ideal_basis(H1.base_ring().fractional_ideal(2))
             ([[2.00000000000000, -3.23606797749979], [2.00000000000000, 1.23606797749979]],
             [2, a - 1])
             sage: H2=HilbertModularGroup(10)
             sage: P2 = HilbertPullback(H2)
             sage: P2._get_lattice_and_ideal_basis()
              ([[1.00000000000000, -3.16227766016838], [1.00000000000000, 3.16227766016838]],
               [1, a])
-            sage: a=H2.base_ring().ideal(H2.base_ring().gen(1)+1)
+            sage: a=H2.base_ring().fractional_ideal(H2.base_ring().gen(1)+1)
             sage: P2._get_lattice_and_ideal_basis(a)
              ([[9.00000000000000, -2.16227766016838], [9.00000000000000, 4.16227766016838]],
               [9, a + 1])
             sage: x = ZZ['x'].gen()
             sage: H3=HilbertModularGroup(NumberField(x^3-36*x-1, names='a'))
             sage: P3=HilbertPullback(H3)
             sage: P3._get_lattice_and_ideal_basis()
```

### Comparing `hilbert_modular_group-0.1.0/src/hilbert_modgroup/pullback_cython.pyx` & `hilbert_modular_group-0.1.1/src/hilbert_modgroup/pullback_cython.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,15 @@
         sage: z=UpperHalfPlaneProductElement([CC(-2.58,0.5),CC(0.5,0.5)])
         sage: a = K.gen()
         sage: distance_to_cusp(P2,a-5,-a,z) # abs tol 1e-10
         1.01308408502928
  
     """
     cdef list rlist,slist
-    ideal_rs = r.parent().ideal(r,s)
+    ideal_rs = r.parent().fractional_ideal(r,s)
     rlist = r.complex_embeddings()
     slist = s.complex_embeddings()
     n = len(slist)
     d = 1
     for i in range(n):
         d = d* ((-z._x[i] * slist[i] + rlist[i]) ** 2 * z._y[i] ** -1 + slist[i] ** 2 * z._y[i])
     d = ideal_rs.norm()**-1*d.sqrt()
```

### Comparing `hilbert_modular_group-0.1.0/src/hilbert_modgroup/upper_half_plane.pxd` & `hilbert_modular_group-0.1.1/src/hilbert_modgroup/upper_half_plane.pxd`

 * *Files identical despite different names*

### Comparing `hilbert_modular_group-0.1.0/src/hilbert_modgroup/upper_half_plane.pyx` & `hilbert_modular_group-0.1.1/src/hilbert_modgroup/upper_half_plane.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,27 @@
 r"""
 
 Elements in the upper half plane of degree n
 
 Note: The structure of this class is based on ArithmeticSubgroupElement from sage/modular/arithgroup/arithgroup_element.pyx
 
 """
+import sage
 from sage.groups.perm_gps.permgroup_element import is_PermutationGroupElement
-from sage.rings.number_field.number_field import is_NumberField
 from sage.rings.real_mpfr import RealField
 from sage.structure.element cimport Element
 from sage.rings.all import Integer, CC
 from sage.rings.infinity import Infinity
 from sage.structure.parent import Parent
 from sage.structure.element cimport parent
 
 from sage.rings.complex_mpfr cimport ComplexNumber
 from sage.rings.complex_mpc cimport MPComplexNumber, MPComplexField_class
 from sage.rings.complex_mpc import MPComplexField
 from cpython.object cimport Py_EQ, Py_NE
-from sage.rings.number_field.number_field_element import is_NumberFieldElement
 from sage.modules.free_module_element import vector
 
 
 # Constructors for products Complex planes and upper half-planes
 def ComplexPlaneProduct(degree, **kwds):
     r"""
     Construct a product of complex planes.
@@ -38,15 +37,15 @@
         sage: from hilbert_modgroup.upper_half_plane import ComplexPlaneProduct
         sage: ComplexPlaneProduct(2)
         Product of complex planes of degree 2
         sage: ComplexPlaneProduct(3)
         Product of complex planes of degree 3
 
     """
-    if is_NumberField(degree):
+    if isinstance(degree, sage.rings.number_field.number_field_base.NumberField):
         degree = degree.absolute_degree()
     return ComplexPlaneProduct__class(degree, **kwds)
 
 def UpperHalfPlaneProduct(degree, **kwds):
     r"""
     Construct a product of complex planes.
 
@@ -59,15 +58,15 @@
         sage: from hilbert_modgroup.upper_half_plane import UpperHalfPlaneProduct
         sage: UpperHalfPlaneProduct(2)
         Product of upper half-planes of degree 2
         sage: UpperHalfPlaneProduct(3)
         Product of upper half-planes of degree 3
 
     """
-    if is_NumberField(degree):
+    if isinstance(degree, sage.rings.number_field.number_field_base.NumberField):
         degree = degree.absolute_degree()
     return UpperHalfPlaneProduct__class(degree, **kwds)
 
 ## Constructors for elements of products of complex planes and upper half-planes
 def UpperHalfPlaneProductElement(z, **kwds):
     """
     Construct an element in the product of upper half planes.
@@ -102,15 +101,15 @@
             return z
         if parent:
             return UpperHalfPlaneProductElement__class(list(z), parent=parent)
         return z
     prec = kwds.get('prec',getattr(z,'prec',lambda : 53)())
     if hasattr(z,'value'):
         z = z.value()
-    if is_NumberFieldElement(z):
+    if isinstance(z, sage.rings.number_field.number_field_element.NumberFieldElement):
         z = z.complex_embeddings(prec)
     if isinstance(z,list) and not isinstance(z[0], (ComplexNumber, MPComplexNumber)):
        z  = [MPComplexField(prec)(x) for x in z]
     elif not isinstance(z,list) and kwds.get('degree',0)>0:
         z = [MPComplexField(prec)(z)]*kwds.get('degree')
     if 'parent' not in kwds:
         kwds['parent'] = UpperHalfPlaneProduct(degree=len(z))
@@ -137,27 +136,27 @@
         sage: a=QuadraticField(5).gen()
         sage: ComplexPlaneProductElement(a)
         [-2.23606797749979, 2.23606797749979]
         sage: u0,u1=QuadraticField(5).unit_group().gens()
         sage: ComplexPlaneProductElement(u0)
         [-1.00000000000000, -1.00000000000000]
         sage: ComplexPlaneProductElement(u1)
-        [-1.61803398874989, 0.618033988749895]
+        [1.61803398874989, -0.618033988749895]
 
     """
     if isinstance(z,ComplexPlaneProductElement__class):
         parent = kwds.get('parent')
         if parent is z.parent():
             return z
         if parent:
             return ComplexPlaneProductElement__class(list(z), parent=parent)
         return z
     # Get precision in the first hand from kwds, second from z and third set default to 53 bits
     prec = kwds.get('prec',getattr(z,'prec',lambda : 53)())
-    if is_NumberFieldElement(z):
+    if isinstance(z, sage.rings.number_field.number_field_element.NumberFieldElement):
         z = z.complex_embeddings(prec)
     if hasattr(z,'value'):
         z = z.value().complex_embeddings(prec)
     if isinstance(z,list) and not isinstance(z[0],(ComplexNumber,MPComplexNumber)):
         z = [MPComplexField(prec)(x) for x in z]
     elif not isinstance(z,list) and kwds.get('degree',0)>0:
         z = [MPComplexField(prec)(z)]*kwds.get('degree')
@@ -524,15 +523,15 @@
         [-2.23606797749979, 2.23606797749979]
         sage: u0,u1=QuadraticField(5).unit_group().gens()
         sage: u0 = QuadraticField(5)(u0)
         sage: u1 = QuadraticField(5)(u1)
         sage: ComplexPlaneProductElement__class(u0.complex_embeddings())
         [-1.00000000000000, -1.00000000000000]
         sage: ComplexPlaneProductElement__class(u1.complex_embeddings())
-        [-1.61803398874989, 0.618033988749895]
+        [1.61803398874989, -0.618033988749895]
 
     TODO: Inherit from Ring or something? (for speed probably NO!)
 
     """
 
     Parent = ComplexPlaneProduct__class
 
@@ -1313,15 +1312,15 @@
             [-2.23606797749979 - 2.23606797749979*I, 4.47213595499958 - 2.23606797749979*I]
             sage: z*CC(1,3)
             [-2.00000000000000 + 4.00000000000000*I, 5.00000000000000 + 5.00000000000000*I]
             sage: z*5
             [5.00000000000000 + 5.00000000000000*I, 10.0000000000000 - 5.00000000000000*I]
             sage: u0,u1=K.unit_group().gens()
             sage: z*u1
-            [-1.61803398874989 - 1.61803398874989*I, 1.23606797749979 - 0.618033988749895*I]
+            [1.61803398874989 + 1.61803398874989*I, -1.23606797749979 + 0.618033988749895*I]
 
             # check Upper half plane elements
             sage: from hilbert_modgroup.all import UpperHalfPlaneProduct
             sage: z=UpperHalfPlaneProduct(degree=2)([1+I,1+2*I]); z
             [1.00000000000000 + 1.00000000000000*I, 1.00000000000000 + 2.00000000000000*I]
             sage: z*2
             [2.00000000000000 + 2.00000000000000*I, 2.00000000000000 + 4.00000000000000*I]
```

### Comparing `hilbert_modular_group-0.1.0/src/hilbert_modgroup/utils.py` & `hilbert_modular_group-0.1.1/src/hilbert_modgroup/utils.py`

 * *Files identical despite different names*

### Comparing `hilbert_modular_group-0.1.0/tox.ini` & `hilbert_modular_group-0.1.1/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 ###
 ### tox.ini with parts taken from the sagemath source
 ###
 [tox]
 envlist = doctest, coverage, pycodestyle, relint, codespell, flake8
 skipsdist = true
+requires =
+     tox>=3.18
 
 [testenv]
 setenv =
     SAGE=sage
     HOME={toxinidir}
-whitelist_externals =
+commands = tox -c {toxinidir}/tox.ini -e {envname} -- {posargs}
+allowlist_externals =
     {env:SAGE}
     tox
 
-commands = tox -c {toxinidir}/tox.ini -e {envname} -- {posargs}
-
 [testenv:doctest]
 description =
    run Sage the Sage doctester (same as "sage -t")
 commands =
     {env:SAGE} -t -p 0 {posargs:{toxinidir}/src/}
 
 [testenv:coverage]
@@ -34,25 +35,25 @@
 count = True
 
 # Not really PEP8 length but this is good enough here.
 [testenv:pycodestyle]
 description =
     Check against PEP8 style conventions.
 deps = pycodestyle
-whitelist_externals = pycodestyle
+allowlist_externals = pycodestyle
 commands = pycodestyle {posargs:{toxinidir}/src/}
 
 [testenv:relint]
 description =
     check whether some forbidden patterns appear
     (includes all patchbot pattern-exclusion plugins)
 # https://github.com/codingjoe/relint
 # The patterns are in .relint.yaml
 deps = relint
-whitelist_externals = find
+allowlist_externals = find
 commands = find {posargs:{toxinidir}/src/} -exec relint -c {toxinidir}/.relint.yaml \{\} +
 
 [testenv:codespell]
 description =
     check for misspelled words in source code
 # https://pypi.org/project/codespell/
 deps = codespell
```

