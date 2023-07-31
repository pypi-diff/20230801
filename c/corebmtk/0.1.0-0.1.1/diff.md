# Comparing `tmp/corebmtk-0.1.0.tar.gz` & `tmp/corebmtk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corebmtk-0.1.0.tar", last modified: Wed Feb  1 19:15:00 2023, max compression
+gzip compressed data, was "corebmtk-0.1.1.tar", last modified: Mon Jul 31 23:13:57 2023, max compression
```

## Comparing `corebmtk-0.1.0.tar` & `corebmtk-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-02-01 19:15:00.735065 corebmtk-0.1.0/
--rw-rw-rw-   0        0        0     1526 2023-01-31 21:04:10.000000 corebmtk-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3022 2023-02-01 19:15:00.734068 corebmtk-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2273 2023-01-31 21:11:20.000000 corebmtk-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-01 19:15:00.706100 corebmtk-0.1.0/corebmtk/
--rw-rw-rw-   0        0        0    14324 2023-02-01 19:14:38.000000 corebmtk-0.1.0/corebmtk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-01 19:15:00.732066 corebmtk-0.1.0/corebmtk.egg-info/
--rw-rw-rw-   0        0        0     3022 2023-02-01 19:15:00.000000 corebmtk-0.1.0/corebmtk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-02-01 19:15:00.000000 corebmtk-0.1.0/corebmtk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-01 19:15:00.000000 corebmtk-0.1.0/corebmtk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-02-01 19:15:00.000000 corebmtk-0.1.0/corebmtk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-01 19:15:00.000000 corebmtk-0.1.0/corebmtk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-01 19:15:00.735065 corebmtk-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1120 2023-02-01 19:14:38.000000 corebmtk-0.1.0/setup.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-31 23:13:57.668733 corebmtk-0.1.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1498 2023-07-31 23:13:16.000000 corebmtk-0.1.1/LICENSE
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2928 2023-07-31 23:13:57.668733 corebmtk-0.1.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2200 2023-07-31 23:13:16.000000 corebmtk-0.1.1/README.md
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-31 23:13:57.664734 corebmtk-0.1.1/corebmtk/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    14145 2023-07-31 23:13:16.000000 corebmtk-0.1.1/corebmtk/__init__.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-31 23:13:57.668733 corebmtk-0.1.1/corebmtk.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2928 2023-07-31 23:13:57.000000 corebmtk-0.1.1/corebmtk.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      206 2023-07-31 23:13:57.000000 corebmtk-0.1.1/corebmtk.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-07-31 23:13:57.000000 corebmtk-0.1.1/corebmtk.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       16 2023-07-31 23:13:57.000000 corebmtk-0.1.1/corebmtk.egg-info/requires.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        9 2023-07-31 23:13:57.000000 corebmtk-0.1.1/corebmtk.egg-info/top_level.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       38 2023-07-31 23:13:57.668733 corebmtk-0.1.1/setup.cfg
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1085 2023-07-31 23:13:32.000000 corebmtk-0.1.1/setup.py
```

### Comparing `corebmtk-0.1.0/LICENSE` & `corebmtk-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-BSD 3-Clause License
-
-Copyright (c) 2023, Tyler Banks
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2023, Tyler Banks
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `corebmtk-0.1.0/PKG-INFO` & `corebmtk-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-Metadata-Version: 2.1
-Name: corebmtk
-Version: 0.1.0
-Summary: corebmtk
-Home-page: https://github.com/tjbanks/corebmtk
-Download-URL: 
-Author: Tyler Banks
-Author-email: tbanks@mail.missouri.edu
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# corebmtk
-A module to allow [BMTK](https://github.com/AllenInstitute/bmtk/) to function with [Core Neuron](https://github.com/BlueBrain/CoreNeuron/) before official support.
-
-Currently, BMTK uses `h.run` and `extracellular` NEURON mechanisms, which are both incompatible with CoreNeuron.
-
-`corebmtk` uses `pc.psolve` and takes an alternate approach to recording and storing output. The goal of this project
-was to maintain all of BMTK's functionality while allowing for the use of CoreNeuron. 
-Recording modules remove the `step` phase and integrate into `initialize` and `finalize` to be compatilbe with `pc.psolve`.
-
-### Installation
-
-```
-pip install --upgrade corebmtk
-```
-
-### Usage
-
-In your `run_network.py` `BMTK` script replace your BioSimulator with a CoreBioSimulator.
-
-```
-import corebmtk
-
-# sim = bionet.BioSimulator.from_config(conf, network=graph)
-sim = corebmtk.CoreBioSimulator.from_config(conf, network=graph)
-```
-
-When using MPI you'll have to replace your config as well. This wrapper prevents loading of mechanisms prior to running with `x86_64/special`.
-
-```
-# conf = bionet.Config.from_json(config_file, validate=True)
-conf = corebmtk.Config.from_json(config_file, validate=True)
-```
-
-### Limitations
-
-Some recoring mechanisms are not yet implemented. See run output for more info.
-
-Implemented recording modules:
-
-1. `reports.SpikesReport`
-1. `netcon_report`
-1. `reports.MembraneReport (report.params['sections'] == 'soma')`
-1. `reports.ECPReport`
-
-Modules NOT implemented
-
-1. `mods.MembraneReport` (general)
-1. `reports.ClampReport`
-1. `save_synapses`
-
-### Troubleshooting
-
-When using ECP recording: 
-```CoreNEURON cannot simulate a model that contains the extracellular mechanism```
-
-Change your `ecp report` to use `"module": "ecp"` instead of `"module": "extracellular"`
-
-```
-    "ecp": {
-      "cells": "all",
-      "variable_name": "v",
-      "module": "ecp",
-      "electrode_positions": "./components/recXelectrodes/linear_electrode.csv",
-      "file_name": "ecp.h5",
-      "electrode_channels": "all"
-    }
-```
-
-### Acknowledgments
-
-Thanks [@gregglickert](https://github.com/gregglickert) for kicking this project off.
-
-[BMTK](https://github.com/AllenInstitute/bmtk/)
+Metadata-Version: 2.1
+Name: corebmtk
+Version: 0.1.1
+Summary: corebmtk
+Home-page: https://github.com/tjbanks/corebmtk
+Download-URL: 
+Author: Tyler Banks
+Author-email: tbanks@mail.missouri.edu
+License: MIT
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# corebmtk
+A module to allow [BMTK](https://github.com/AllenInstitute/bmtk/) to function with [Core Neuron](https://github.com/BlueBrain/CoreNeuron/) before official support.
+
+Currently, BMTK uses `h.run` and `extracellular` NEURON mechanisms, which are both incompatible with CoreNeuron.
+
+`corebmtk` uses `pc.psolve` and takes an alternate approach to recording and storing output. The goal of this project
+was to maintain all of BMTK's functionality while allowing for the use of CoreNeuron. 
+Recording modules remove the `step` phase and integrate into `initialize` and `finalize` to be compatilbe with `pc.psolve`.
+
+### Installation
+
+```
+pip install --upgrade corebmtk
+```
+
+### Usage
+
+In your `run_network.py` `BMTK` script replace your BioSimulator with a CoreBioSimulator.
+
+```
+import corebmtk
+
+# sim = bionet.BioSimulator.from_config(conf, network=graph)
+sim = corebmtk.CoreBioSimulator.from_config(conf, network=graph)
+```
+
+When using MPI you'll have to replace your config as well. This wrapper prevents loading of mechanisms prior to running with `x86_64/special`.
+
+```
+# conf = bionet.Config.from_json(config_file, validate=True)
+conf = corebmtk.Config.from_json(config_file, validate=True)
+```
+
+### Limitations
+
+Some recoring mechanisms are not yet implemented. See run output for more info.
+
+Implemented recording modules:
+
+1. `reports.SpikesReport`
+1. `netcon_report`
+1. `reports.MembraneReport (report.params['sections'] == 'soma')`
+1. `reports.ECPReport`
+
+Modules NOT implemented
+
+1. `mods.MembraneReport` (general)
+1. `reports.ClampReport`
+1. `save_synapses`
+
+### Troubleshooting
+
+When using ECP recording: 
+```CoreNEURON cannot simulate a model that contains the extracellular mechanism```
+
+Change your `ecp report` to use `"module": "ecp"` instead of `"module": "extracellular"`
+
+```
+    "ecp": {
+      "cells": "all",
+      "variable_name": "v",
+      "module": "ecp",
+      "electrode_positions": "./components/recXelectrodes/linear_electrode.csv",
+      "file_name": "ecp.h5",
+      "electrode_channels": "all"
+    }
+```
+
+### Acknowledgments
+
+Thanks [@gregglickert](https://github.com/gregglickert) for kicking this project off.
+
+[BMTK](https://github.com/AllenInstitute/bmtk/)
```

### Comparing `corebmtk-0.1.0/README.md` & `corebmtk-0.1.1/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-# corebmtk
-A module to allow [BMTK](https://github.com/AllenInstitute/bmtk/) to function with [Core Neuron](https://github.com/BlueBrain/CoreNeuron/) before official support.
-
-Currently, BMTK uses `h.run` and `extracellular` NEURON mechanisms, which are both incompatible with CoreNeuron.
-
-`corebmtk` uses `pc.psolve` and takes an alternate approach to recording and storing output. The goal of this project
-was to maintain all of BMTK's functionality while allowing for the use of CoreNeuron. 
-Recording modules remove the `step` phase and integrate into `initialize` and `finalize` to be compatilbe with `pc.psolve`.
-
-### Installation
-
-```
-pip install --upgrade corebmtk
-```
-
-### Usage
-
-In your `run_network.py` `BMTK` script replace your BioSimulator with a CoreBioSimulator.
-
-```
-import corebmtk
-
-# sim = bionet.BioSimulator.from_config(conf, network=graph)
-sim = corebmtk.CoreBioSimulator.from_config(conf, network=graph)
-```
-
-When using MPI you'll have to replace your config as well. This wrapper prevents loading of mechanisms prior to running with `x86_64/special`.
-
-```
-# conf = bionet.Config.from_json(config_file, validate=True)
-conf = corebmtk.Config.from_json(config_file, validate=True)
-```
-
-### Limitations
-
-Some recoring mechanisms are not yet implemented. See run output for more info.
-
-Implemented recording modules:
-
-1. `reports.SpikesReport`
-1. `netcon_report`
-1. `reports.MembraneReport (report.params['sections'] == 'soma')`
-1. `reports.ECPReport`
-
-Modules NOT implemented
-
-1. `mods.MembraneReport` (general)
-1. `reports.ClampReport`
-1. `save_synapses`
-
-### Troubleshooting
-
-When using ECP recording: 
-```CoreNEURON cannot simulate a model that contains the extracellular mechanism```
-
-Change your `ecp report` to use `"module": "ecp"` instead of `"module": "extracellular"`
-
-```
-    "ecp": {
-      "cells": "all",
-      "variable_name": "v",
-      "module": "ecp",
-      "electrode_positions": "./components/recXelectrodes/linear_electrode.csv",
-      "file_name": "ecp.h5",
-      "electrode_channels": "all"
-    }
-```
-
-### Acknowledgments
-
-Thanks [@gregglickert](https://github.com/gregglickert) for kicking this project off.
-
-[BMTK](https://github.com/AllenInstitute/bmtk/)
+# corebmtk
+A module to allow [BMTK](https://github.com/AllenInstitute/bmtk/) to function with [Core Neuron](https://github.com/BlueBrain/CoreNeuron/) before official support.
+
+Currently, BMTK uses `h.run` and `extracellular` NEURON mechanisms, which are both incompatible with CoreNeuron.
+
+`corebmtk` uses `pc.psolve` and takes an alternate approach to recording and storing output. The goal of this project
+was to maintain all of BMTK's functionality while allowing for the use of CoreNeuron. 
+Recording modules remove the `step` phase and integrate into `initialize` and `finalize` to be compatilbe with `pc.psolve`.
+
+### Installation
+
+```
+pip install --upgrade corebmtk
+```
+
+### Usage
+
+In your `run_network.py` `BMTK` script replace your BioSimulator with a CoreBioSimulator.
+
+```
+import corebmtk
+
+# sim = bionet.BioSimulator.from_config(conf, network=graph)
+sim = corebmtk.CoreBioSimulator.from_config(conf, network=graph)
+```
+
+When using MPI you'll have to replace your config as well. This wrapper prevents loading of mechanisms prior to running with `x86_64/special`.
+
+```
+# conf = bionet.Config.from_json(config_file, validate=True)
+conf = corebmtk.Config.from_json(config_file, validate=True)
+```
+
+### Limitations
+
+Some recoring mechanisms are not yet implemented. See run output for more info.
+
+Implemented recording modules:
+
+1. `reports.SpikesReport`
+1. `netcon_report`
+1. `reports.MembraneReport (report.params['sections'] == 'soma')`
+1. `reports.ECPReport`
+
+Modules NOT implemented
+
+1. `mods.MembraneReport` (general)
+1. `reports.ClampReport`
+1. `save_synapses`
+
+### Troubleshooting
+
+When using ECP recording: 
+```CoreNEURON cannot simulate a model that contains the extracellular mechanism```
+
+Change your `ecp report` to use `"module": "ecp"` instead of `"module": "extracellular"`
+
+```
+    "ecp": {
+      "cells": "all",
+      "variable_name": "v",
+      "module": "ecp",
+      "electrode_positions": "./components/recXelectrodes/linear_electrode.csv",
+      "file_name": "ecp.h5",
+      "electrode_channels": "all"
+    }
+```
+
+### Acknowledgments
+
+Thanks [@gregglickert](https://github.com/gregglickert) for kicking this project off.
+
+[BMTK](https://github.com/AllenInstitute/bmtk/)
```

### Comparing `corebmtk-0.1.0/corebmtk.egg-info/PKG-INFO` & `corebmtk-0.1.1/corebmtk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-Metadata-Version: 2.1
-Name: corebmtk
-Version: 0.1.0
-Summary: corebmtk
-Home-page: https://github.com/tjbanks/corebmtk
-Download-URL: 
-Author: Tyler Banks
-Author-email: tbanks@mail.missouri.edu
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# corebmtk
-A module to allow [BMTK](https://github.com/AllenInstitute/bmtk/) to function with [Core Neuron](https://github.com/BlueBrain/CoreNeuron/) before official support.
-
-Currently, BMTK uses `h.run` and `extracellular` NEURON mechanisms, which are both incompatible with CoreNeuron.
-
-`corebmtk` uses `pc.psolve` and takes an alternate approach to recording and storing output. The goal of this project
-was to maintain all of BMTK's functionality while allowing for the use of CoreNeuron. 
-Recording modules remove the `step` phase and integrate into `initialize` and `finalize` to be compatilbe with `pc.psolve`.
-
-### Installation
-
-```
-pip install --upgrade corebmtk
-```
-
-### Usage
-
-In your `run_network.py` `BMTK` script replace your BioSimulator with a CoreBioSimulator.
-
-```
-import corebmtk
-
-# sim = bionet.BioSimulator.from_config(conf, network=graph)
-sim = corebmtk.CoreBioSimulator.from_config(conf, network=graph)
-```
-
-When using MPI you'll have to replace your config as well. This wrapper prevents loading of mechanisms prior to running with `x86_64/special`.
-
-```
-# conf = bionet.Config.from_json(config_file, validate=True)
-conf = corebmtk.Config.from_json(config_file, validate=True)
-```
-
-### Limitations
-
-Some recoring mechanisms are not yet implemented. See run output for more info.
-
-Implemented recording modules:
-
-1. `reports.SpikesReport`
-1. `netcon_report`
-1. `reports.MembraneReport (report.params['sections'] == 'soma')`
-1. `reports.ECPReport`
-
-Modules NOT implemented
-
-1. `mods.MembraneReport` (general)
-1. `reports.ClampReport`
-1. `save_synapses`
-
-### Troubleshooting
-
-When using ECP recording: 
-```CoreNEURON cannot simulate a model that contains the extracellular mechanism```
-
-Change your `ecp report` to use `"module": "ecp"` instead of `"module": "extracellular"`
-
-```
-    "ecp": {
-      "cells": "all",
-      "variable_name": "v",
-      "module": "ecp",
-      "electrode_positions": "./components/recXelectrodes/linear_electrode.csv",
-      "file_name": "ecp.h5",
-      "electrode_channels": "all"
-    }
-```
-
-### Acknowledgments
-
-Thanks [@gregglickert](https://github.com/gregglickert) for kicking this project off.
-
-[BMTK](https://github.com/AllenInstitute/bmtk/)
+Metadata-Version: 2.1
+Name: corebmtk
+Version: 0.1.1
+Summary: corebmtk
+Home-page: https://github.com/tjbanks/corebmtk
+Download-URL: 
+Author: Tyler Banks
+Author-email: tbanks@mail.missouri.edu
+License: MIT
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# corebmtk
+A module to allow [BMTK](https://github.com/AllenInstitute/bmtk/) to function with [Core Neuron](https://github.com/BlueBrain/CoreNeuron/) before official support.
+
+Currently, BMTK uses `h.run` and `extracellular` NEURON mechanisms, which are both incompatible with CoreNeuron.
+
+`corebmtk` uses `pc.psolve` and takes an alternate approach to recording and storing output. The goal of this project
+was to maintain all of BMTK's functionality while allowing for the use of CoreNeuron. 
+Recording modules remove the `step` phase and integrate into `initialize` and `finalize` to be compatilbe with `pc.psolve`.
+
+### Installation
+
+```
+pip install --upgrade corebmtk
+```
+
+### Usage
+
+In your `run_network.py` `BMTK` script replace your BioSimulator with a CoreBioSimulator.
+
+```
+import corebmtk
+
+# sim = bionet.BioSimulator.from_config(conf, network=graph)
+sim = corebmtk.CoreBioSimulator.from_config(conf, network=graph)
+```
+
+When using MPI you'll have to replace your config as well. This wrapper prevents loading of mechanisms prior to running with `x86_64/special`.
+
+```
+# conf = bionet.Config.from_json(config_file, validate=True)
+conf = corebmtk.Config.from_json(config_file, validate=True)
+```
+
+### Limitations
+
+Some recoring mechanisms are not yet implemented. See run output for more info.
+
+Implemented recording modules:
+
+1. `reports.SpikesReport`
+1. `netcon_report`
+1. `reports.MembraneReport (report.params['sections'] == 'soma')`
+1. `reports.ECPReport`
+
+Modules NOT implemented
+
+1. `mods.MembraneReport` (general)
+1. `reports.ClampReport`
+1. `save_synapses`
+
+### Troubleshooting
+
+When using ECP recording: 
+```CoreNEURON cannot simulate a model that contains the extracellular mechanism```
+
+Change your `ecp report` to use `"module": "ecp"` instead of `"module": "extracellular"`
+
+```
+    "ecp": {
+      "cells": "all",
+      "variable_name": "v",
+      "module": "ecp",
+      "electrode_positions": "./components/recXelectrodes/linear_electrode.csv",
+      "file_name": "ecp.h5",
+      "electrode_channels": "all"
+    }
+```
+
+### Acknowledgments
+
+Thanks [@gregglickert](https://github.com/gregglickert) for kicking this project off.
+
+[BMTK](https://github.com/AllenInstitute/bmtk/)
```

### Comparing `corebmtk-0.1.0/setup.py` & `corebmtk-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from setuptools import setup
-from setuptools import find_packages
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setup(
-    name="corebmtk",
-    version="0.1.0",
-    author="Tyler Banks",
-    author_email="tbanks@mail.missouri.edu",
-    description="corebmtk",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/tjbanks/corebmtk",
-    download_url='',
-    license='MIT',
-    install_requires=[
-        'bmtk',
-        'h5py',
-        'numpy',
-    ],
-    classifiers=[
-        'Intended Audience :: Developers',
-        'Intended Audience :: Education',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: MIT License',
-        "Programming Language :: Python :: 3",
-        'Programming Language :: Python :: 3.6',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        "Operating System :: OS Independent",
-    ],
-    packages=find_packages(exclude=['tests']),
-    entry_points={}
+from setuptools import setup
+from setuptools import find_packages
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setup(
+    name="corebmtk",
+    version="0.1.1",
+    author="Tyler Banks",
+    author_email="tbanks@mail.missouri.edu",
+    description="corebmtk",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/tjbanks/corebmtk",
+    download_url='',
+    license='MIT',
+    install_requires=[
+        'bmtk',
+        'h5py',
+        'numpy',
+    ],
+    classifiers=[
+        'Intended Audience :: Developers',
+        'Intended Audience :: Education',
+        'Intended Audience :: Science/Research',
+        'License :: OSI Approved :: MIT License',
+        "Programming Language :: Python :: 3",
+        'Programming Language :: Python :: 3.6',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        "Operating System :: OS Independent",
+    ],
+    packages=find_packages(exclude=['tests']),
+    entry_points={}
 )
```

