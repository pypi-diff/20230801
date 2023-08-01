# Comparing `tmp/SuperNeuroABM-0.1.0.tar.gz` & `tmp/SuperNeuroABM-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SuperNeuroABM-0.1.0.tar", last modified: Mon Jun 26 14:16:01 2023, max compression
+gzip compressed data, was "SuperNeuroABM-0.2.0.tar", last modified: Tue Aug  1 14:52:22 2023, max compression
```

## Comparing `SuperNeuroABM-0.1.0.tar` & `SuperNeuroABM-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 co1       (3116) users      (100)        0 2023-06-26 14:16:01.714932 SuperNeuroABM-0.1.0/
--rw-r--r--   0 co1       (3116) users      (100)      487 2023-06-26 14:16:01.714932 SuperNeuroABM-0.1.0/PKG-INFO
--rw-r--r--   0 co1       (3116) users      (100)      235 2023-06-26 14:15:31.000000 SuperNeuroABM-0.1.0/README.md
-drwxr-xr-x   0 co1       (3116) users      (100)        0 2023-06-26 14:16:01.714932 SuperNeuroABM-0.1.0/SuperNeuroABM.egg-info/
--rw-r--r--   0 co1       (3116) users      (100)      487 2023-06-26 14:16:01.000000 SuperNeuroABM-0.1.0/SuperNeuroABM.egg-info/PKG-INFO
--rw-r--r--   0 co1       (3116) users      (100)      389 2023-06-26 14:16:01.000000 SuperNeuroABM-0.1.0/SuperNeuroABM.egg-info/SOURCES.txt
--rw-r--r--   0 co1       (3116) users      (100)        1 2023-06-26 14:16:01.000000 SuperNeuroABM-0.1.0/SuperNeuroABM.egg-info/dependency_links.txt
--rw-r--r--   0 co1       (3116) users      (100)       41 2023-06-26 14:16:01.000000 SuperNeuroABM-0.1.0/SuperNeuroABM.egg-info/requires.txt
--rw-r--r--   0 co1       (3116) users      (100)       14 2023-06-26 14:16:01.000000 SuperNeuroABM-0.1.0/SuperNeuroABM.egg-info/top_level.txt
--rw-r--r--   0 co1       (3116) users      (100)       38 2023-06-26 14:16:01.714932 SuperNeuroABM-0.1.0/setup.cfg
--rwxr-xr-x   0 co1       (3116) users      (100)      766 2023-06-26 14:15:31.000000 SuperNeuroABM-0.1.0/setup.py
-drwxr-xr-x   0 co1       (3116) users      (100)        0 2023-06-26 14:16:01.714932 SuperNeuroABM-0.1.0/superneuroabm/
--rw-r--r--   0 co1       (3116) users      (100)        0 2023-06-15 01:52:35.000000 SuperNeuroABM-0.1.0/superneuroabm/__init__.py
-drwxr-xr-x   0 co1       (3116) users      (100)        0 2023-06-26 14:16:01.714932 SuperNeuroABM-0.1.0/superneuroabm/core/
--rwxr-xr-x   0 co1       (3116) users      (100)        0 2023-06-15 01:54:26.000000 SuperNeuroABM-0.1.0/superneuroabm/core/__init__.py
--rwxr-xr-x   0 co1       (3116) users      (100)     9920 2023-06-15 02:09:03.000000 SuperNeuroABM-0.1.0/superneuroabm/core/agent.py
--rwxr-xr-x   0 co1       (3116) users      (100)     7788 2023-06-15 02:07:18.000000 SuperNeuroABM-0.1.0/superneuroabm/core/model.py
--rw-r--r--   0 co1       (3116) users      (100)     1808 2023-06-15 01:54:26.000000 SuperNeuroABM-0.1.0/superneuroabm/core/util.py
--rwxr-xr-x   0 co1       (3116) users      (100)     6415 2023-06-15 01:55:53.000000 SuperNeuroABM-0.1.0/superneuroabm/model.py
--rwxr-xr-x   0 co1       (3116) users      (100)     3621 2023-06-15 01:52:35.000000 SuperNeuroABM-0.1.0/superneuroabm/neuron.py
+drwxr-xr-x   0 co1       (3116) users      (100)        0 2023-08-01 14:52:22.758588 SuperNeuroABM-0.2.0/
+-rw-r--r--   0 co1       (3116) users      (100)     1516 2023-07-23 18:25:19.000000 SuperNeuroABM-0.2.0/LICENSE
+-rw-r--r--   0 co1       (3116) users      (100)      509 2023-08-01 14:52:22.758588 SuperNeuroABM-0.2.0/PKG-INFO
+-rw-r--r--   0 co1       (3116) users      (100)      570 2023-07-23 18:21:21.000000 SuperNeuroABM-0.2.0/README.md
+drwxr-xr-x   0 co1       (3116) users      (100)        0 2023-08-01 14:52:22.758588 SuperNeuroABM-0.2.0/SuperNeuroABM.egg-info/
+-rw-r--r--   0 co1       (3116) users      (100)      509 2023-08-01 14:52:22.000000 SuperNeuroABM-0.2.0/SuperNeuroABM.egg-info/PKG-INFO
+-rw-r--r--   0 co1       (3116) users      (100)      397 2023-08-01 14:52:22.000000 SuperNeuroABM-0.2.0/SuperNeuroABM.egg-info/SOURCES.txt
+-rw-r--r--   0 co1       (3116) users      (100)        1 2023-08-01 14:52:22.000000 SuperNeuroABM-0.2.0/SuperNeuroABM.egg-info/dependency_links.txt
+-rw-r--r--   0 co1       (3116) users      (100)       41 2023-08-01 14:52:22.000000 SuperNeuroABM-0.2.0/SuperNeuroABM.egg-info/requires.txt
+-rw-r--r--   0 co1       (3116) users      (100)       14 2023-08-01 14:52:22.000000 SuperNeuroABM-0.2.0/SuperNeuroABM.egg-info/top_level.txt
+-rw-r--r--   0 co1       (3116) users      (100)       38 2023-08-01 14:52:22.758588 SuperNeuroABM-0.2.0/setup.cfg
+-rwxr-xr-x   0 co1       (3116) users      (100)      766 2023-08-01 14:48:28.000000 SuperNeuroABM-0.2.0/setup.py
+drwxr-xr-x   0 co1       (3116) users      (100)        0 2023-08-01 14:52:22.758588 SuperNeuroABM-0.2.0/superneuroabm/
+-rw-r--r--   0 co1       (3116) users      (100)        0 2023-06-15 01:52:35.000000 SuperNeuroABM-0.2.0/superneuroabm/__init__.py
+drwxr-xr-x   0 co1       (3116) users      (100)        0 2023-08-01 14:52:22.758588 SuperNeuroABM-0.2.0/superneuroabm/core/
+-rwxr-xr-x   0 co1       (3116) users      (100)        0 2023-06-15 01:54:26.000000 SuperNeuroABM-0.2.0/superneuroabm/core/__init__.py
+-rwxr-xr-x   0 co1       (3116) users      (100)     9824 2023-07-27 19:47:23.000000 SuperNeuroABM-0.2.0/superneuroabm/core/agent.py
+-rwxr-xr-x   0 co1       (3116) users      (100)     8340 2023-07-27 19:47:23.000000 SuperNeuroABM-0.2.0/superneuroabm/core/model.py
+-rw-r--r--   0 co1       (3116) users      (100)     1981 2023-07-27 19:47:23.000000 SuperNeuroABM-0.2.0/superneuroabm/core/util.py
+-rwxr-xr-x   0 co1       (3116) users      (100)     7414 2023-07-27 19:47:23.000000 SuperNeuroABM-0.2.0/superneuroabm/model.py
+-rwxr-xr-x   0 co1       (3116) users      (100)     6762 2023-07-31 20:02:07.000000 SuperNeuroABM-0.2.0/superneuroabm/neuron.py
```

### Comparing `SuperNeuroABM-0.1.0/setup.py` & `SuperNeuroABM-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="SuperNeuroABM",
-    version="0.1.0",
+    version="0.2.0",
     author="Chathika Gunaratne, Prasanna Date, Shruti Kulkarni, Xi Zhang",
     author_email="gunaratnecs@ornl.gov",
     packages=["superneuroabm", "superneuroabm.core"],
     include_package_data=True,
     url="https://code.ornl.gov/superneuro/superneuroabm",
     license="GPL",
     description="A GPU-based multi-agent simulation framework for neuromorphic computing.",
```

### Comparing `SuperNeuroABM-0.1.0/superneuroabm/core/agent.py` & `SuperNeuroABM-0.2.0/superneuroabm/core/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,16 +246,14 @@
     def update_agents_properties(
         self, equal_side_agent_data_tensors=List[List[Any]], use_cuda=True
     ) -> None:
         property_names = list(self._property_name_2_agent_data_tensor.keys())
         for i, property_name in enumerate(property_names):
             if use_cuda:
                 dt = equal_side_agent_data_tensors[i]
-                if property_name == "output_spikes":
-                    dt = dt.copy_to_host()
             else:
                 dt = equal_side_agent_data_tensors[i]
                 # Free shared memory
                 shm = shared_memory.SharedMemory(
                     name=f"npshared{property_name}"
                 )
                 shm.close()
```

### Comparing `SuperNeuroABM-0.1.0/superneuroabm/core/model.py` & `SuperNeuroABM-0.2.0/superneuroabm/core/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,20 +39,34 @@
             )
         self._agent_factory.register_breed(breed)
 
     def create_agent_of_breed(self, breed: Breed, **kwargs) -> int:
         agent_id = self._agent_factory.create_agent(breed, **kwargs)
         return agent_id
 
-    def get_agent_info(self, breed: Breed, id: int) -> List[Any]:
+    def get_synapse_weight(
+        self, presynaptic_neuron_id: int, post_synaptic_neuron_id: int
+    ) -> float:
         """
-        Query agent from population by its breed and id
+        Return synaptic weight. This function is useful if STDP is
+        turned on as weights will be updated during simulation.
 
+        :param presynaptic_neuron_id: int
+        :param presynaptic_neuron_id: int
+        :returns: float, final weight of synapse
         """
-        raise NotImplemented()
+        out_synapses = self.get_agent_property_value(
+            presynaptic_neuron_id, "output_synapses"
+        )
+        weight = math.nan
+        for out_synapse in out_synapses:
+            if out_synapse[0] == post_synaptic_neuron_id:
+                weight = out_synapse[1]
+                break
+        return weight
 
     def get_agent_property_value(self, id: int, property_name: str) -> Any:
         return self._agent_factory.get_agent_property_value(
             property_name=property_name, agent_id=id
         )
 
     def set_agent_property_value(
```

### Comparing `SuperNeuroABM-0.1.0/superneuroabm/core/util.py` & `SuperNeuroABM-0.2.0/superneuroabm/core/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,25 +39,29 @@
                 fill_arr(item, new_coord)
 
     start = time.time()
     fill_arr(tensor, [])
     return answer
 
 
-def compress_tensor(arr: Iterable, outer: bool = True):
+def compress_tensor(arr: Iterable, level: int = 0):
     if not hasattr(arr, "__iter__") and not hasattr(
         arr, "__cuda_array_interface__"
     ):
         if not np.isnan(arr):
             return arr
         else:
             return None
     else:
         new_arr = []
         for item in arr:
-            new_item = compress_tensor(item, False)
-            if new_item != None:
+            new_item = compress_tensor(item, level + 1)
+            if (
+                (not isinstance(new_item, Iterable) and new_item != None)
+                or (isinstance(new_item, Iterable) and len(new_item))
+                or level <= 0
+            ):
                 new_arr.append(new_item)
         if len(new_arr):
             return new_arr
         else:
-            return [] if outer else None
+            return [] if level else None
```

### Comparing `SuperNeuroABM-0.1.0/superneuroabm/model.py` & `SuperNeuroABM-0.2.0/superneuroabm/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,128 +1,133 @@
 """
 Model class for building an SNN
 """
+from typing import Dict, Callable, List
 
 import numpy as np
 
 from superneuroabm.core.model import Model
 from superneuroabm.core.agent import Breed
 from superneuroabm.neuron import (
     synapse_step_func,
     neuron_step_func,
+    synapse_with_stdp_step_func,
 )
 
 
 class NeuromorphicModel(Model):
-    def __init__(self, use_cuda: bool = False) -> None:
+    def __init__(
+        self,
+        use_cuda: bool = False,
+        neuron_breed_info: Dict[str, List[Callable]] = {
+            "Neuron": [neuron_step_func, synapse_step_func]
+        },
+    ) -> None:
         """
         Creates an SNN Model and provides methods to create, simulate,
         and monitor neurons and synapses.
 
-        :param use_cuda: True if the system supports CUDA GPU acceleration
+        :param use_cuda: True if the system supports CUDA GPU
+            acceleration.
+        :param neuron_breed_info: Dict of breed name to List of
+            Callable step functions. If specifed, will override
+            the default neuron breed and neuron and synapse step
+            functions, allowing for multi-breed simulations.
+            Step functions will be executed on the respective
+            breed every simulation step in the order specifed in the
+            list.
         """
         super().__init__(name="NeuromorphicModel", use_cuda=use_cuda)
-        # dictionary for datacollectors for each neuron to be tracked
-        """self._neuron_spike_collectors = {}"""
 
         axonal_delay = 1
         neuron_properties = {
             "threshold": 1,
             "reset_state": 0,
             "leak": 0,
-            "refactory_period": 0,
+            "refractory_period": 0,
             "output_synapses": [],
             "t_elapse": 0,
             "internal_state": 0,
             "neuron_delay_reg": [0 for _ in range(axonal_delay)],
             "input_spikes": [],
             "output_spikes": [],
         }
         max_dims = {
             "threshold": [],
             "reset_state": [],
             "leak": [],
-            "refactory_period": [],
-            "output_synapses": None,
+            "refractory_period": [],
+            "output_synapses": [],
             "t_elapse": [],
             "internal_state": [],
             "neuron_delay_reg": None,
             "input_spikes": None,
             "output_spikes": None,
         }
 
-        self._neuron_breed = Breed("Neuron")
-        for prop_name, default_val in neuron_properties.items():
-            self._neuron_breed.register_property(
-                prop_name, default_val, max_dims[prop_name]
-            )
-        self._neuron_breed.register_step_func(
-            step_func=neuron_step_func, priority=0
-        )
-        self._neuron_breed.register_step_func(
-            step_func=synapse_step_func, priority=1
-        )
+        self._neuron_breeds: Dict[str, Breed] = {}
+        for breed_name, step_funcs in neuron_breed_info.items():
+            neuron_breed = Breed(breed_name)
+            for prop_name, default_val in neuron_properties.items():
+                neuron_breed.register_property(
+                    prop_name, default_val, max_dims[prop_name]
+                )
+            for step_func_order, step_func in enumerate(step_funcs):
+                neuron_breed.register_step_func(
+                    step_func=step_func, priority=step_func_order
+                )
+            self.register_breed(neuron_breed)
+            self._neuron_breeds[breed_name] = neuron_breed
 
-        self.register_breed(self._neuron_breed)
-        self.register_breed(self._neuron_breed)
-        # self._output_synapsess = []
         self._output_synapsess_max_dim = [0, 2]
 
     def setup(self, output_buffer_len: int = 1000) -> None:
-        def get_neurons(breed: int, **kwargs):
-            return breed == 1
-
-        neuron_ids = self.get_agents_with(query=get_neurons)
-        for neuron_id in neuron_ids:
+        neuron_ids = self._agent_factory.num_agents
+        for neuron_id in range(neuron_ids):
             output_buffer = [0 for _ in range(output_buffer_len)]
             super().set_agent_property_value(
                 id=neuron_id,
                 property_name="output_spikes",
                 value=output_buffer,
                 dims=[output_buffer_len],
             )
-            """super().set_agent_property_value(
-                id=neuron_id,
-                property_name="output_synapses",
-                value=self._output_synapsess[neuron_id],
-                dims=
-            )"""
         super().setup()
 
     def simulate(
         self, ticks: int, update_data_ticks: int = 1, num_cpu_proc: int = 4
     ) -> None:
         """
         Override of superneuroabm.core.model mainly to register an
         AgentDataCollector to monitor marked output Neurons.
 
         """
         super().simulate(ticks, update_data_ticks, num_cpu_proc)
 
     def create_neuron(
         self,
+        breed: str = "Neuron",
         threshold: float = 1,
         reset_state: float = 0,
         leak: float = 0,
-        refactory_period: int = 0,
+        refractory_period: int = 0,
         axonal_delay: int = 1,
     ) -> int:
         """
         Creates and Neuron agent.
 
         :return: SAGESim agent id of neuron
 
         """
         delay_reg = [0 for _ in range(axonal_delay)]
         neuron_id = super().create_agent_of_breed(
-            breed=self._neuron_breed,
+            breed=self._neuron_breeds[breed],
             threshold=threshold,
             reset_state=reset_state,
             leak=leak,
-            refactory_period=refactory_period,
+            refractory_period=refractory_period,
         )
         self.set_agent_property_value(
             neuron_id, "neuron_delay_reg", delay_reg, [axonal_delay]
         )
         # synapse_infos = []
         # self._output_synapsess.append(synapse_infos)
         return neuron_id
@@ -190,13 +195,29 @@
 
     def summary(self) -> str:
         """
         Verbose summary of the network structure.
 
         :return: str information of netowkr struture
         """
-        # Function to print
-        # TODO: Have a better way to represent the network structure(?)
         summary = []
-        for k in range(len(self._agents)):
-            summary.append(f"Agent: {k} Type:{type(self.get_agent(k))}")
+        summary.append("Neuron information:")
+        for neuron_id in range(self._agent_factory.num_agents):
+            spikes = self.get_agent_property_value(neuron_id, "output_spikes")
+            summary.append(f"Neuron: {neuron_id} Spike Train: {str(spikes)}")
+
+        summary.append("\n\n\nSynapse information:")
+        for presynaptic_neuron_id in range(self._agent_factory.num_agents):
+            synapses = self.get_agent_property_value(
+                presynaptic_neuron_id, "output_synapses"
+            )
+            for synapse in synapses:
+                postsynaptic_neuron_id = synapse[0]
+                weight = synapse[1]
+                summary.append(
+                    (
+                        f"Neuron {presynaptic_neuron_id} -> {postsynaptic_neuron_id}"
+                        f": weight: {weight}"
+                    )
+                )
+
         return "\n".join(summary)
```

