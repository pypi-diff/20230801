# Comparing `tmp/robocat-0.0.2.tar.gz` & `tmp/robocat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocat-0.0.2.tar", last modified: Sun Jul  2 22:47:42 2023, max compression
+gzip compressed data, was "robocat-0.0.4.tar", last modified: Tue Aug  1 20:09:34 2023, max compression
```

## Comparing `robocat-0.0.2.tar` & `robocat-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:47:42.174958 robocat-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-02 22:47:32.000000 robocat-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-02 22:47:42.174958 robocat-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-07-02 22:47:32.000000 robocat-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:47:42.174958 robocat-0.0.2/roboCAT/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-02 22:47:32.000000 robocat-0.0.2/roboCAT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-02 22:47:32.000000 robocat-0.0.2/roboCAT/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-02 22:47:32.000000 robocat-0.0.2/roboCAT/model2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-02 22:47:32.000000 robocat-0.0.2/roboCAT/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)    23189 2023-07-02 22:47:32.000000 robocat-0.0.2/roboCAT/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:47:42.174958 robocat-0.0.2/robocat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-02 22:47:42.000000 robocat-0.0.2/robocat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-02 22:47:42.000000 robocat-0.0.2/robocat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 22:47:42.000000 robocat-0.0.2/robocat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-02 22:47:42.000000 robocat-0.0.2/robocat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 22:47:42.000000 robocat-0.0.2/robocat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 22:47:42.174958 robocat-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-02 22:47:32.000000 robocat-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:09:34.271448 robocat-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 20:09:24.000000 robocat-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-01 20:09:34.271448 robocat-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-08-01 20:09:24.000000 robocat-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:09:34.267448 robocat-0.0.4/robocat/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-01 20:09:24.000000 robocat-0.0.4/robocat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-08-01 20:09:24.000000 robocat-0.0.4/robocat/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24054 2023-08-01 20:09:24.000000 robocat-0.0.4/robocat/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:09:34.271448 robocat-0.0.4/robocat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:09:24.000000 robocat-0.0.4/robocat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-08-01 20:09:24.000000 robocat-0.0.4/robocat/utils/stabe_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-01 20:09:24.000000 robocat-0.0.4/robocat/utils/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:09:34.271448 robocat-0.0.4/robocat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-01 20:09:34.000000 robocat-0.0.4/robocat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-01 20:09:34.000000 robocat-0.0.4/robocat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:09:34.000000 robocat-0.0.4/robocat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-01 20:09:34.000000 robocat-0.0.4/robocat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 20:09:34.000000 robocat-0.0.4/robocat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:09:34.271448 robocat-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-01 20:09:24.000000 robocat-0.0.4/setup.py
```

### Comparing `robocat-0.0.2/LICENSE` & `robocat-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `robocat-0.0.2/PKG-INFO` & `robocat-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocat
-Version: 0.0.2
+Version: 0.0.4
 Summary: Robo CAT- Pytorch
 Home-page: https://github.com/kyegomez/RoboCAT
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,robotics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `robocat-0.0.2/README.md` & `robocat-0.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 # ROBOTCAT
+![ROBOCAT MODELS](robocat.png)
 
 RoboCAT is a self-improving foundation agent for robotic manipulation developed by DeepMind Robotics. The model architecture of RoboCAT is similar to the RT-1 model. It follows a tokenization approach where robotics images, proprioception, and future actions are tokenized. 
 
 
-
 # Usage
 There are 2 methods one is by pip `pip install robotcat` and the other is `git clone`
 
 
 ## Method1
 * first `python3 -m pip install robocat`
 
 * Then:
 
 ```python
 import torch
-from roboCAT import robo_cat
+from robocat import PALME, Robocat
+
+model = Robocat(
+    palme=PALME(),
+    num_actions=11,
+    action_bins=256,
+    depth=6,
+    heads=8,
+    dim_head=64,
+    token_learner_ff_mult=2,
+    token_learner_num_layers=2,
+    token_learner_num_output_tokens=8,
+    cond_drop_prob=0.2,
+    use_attn_conditioner=False,
+    conditioner_kwargs=dict()
+)
+
+video = torch.rand((1, 3, 224, 224))
+texts = ["this is a text"]
+output = model(video, texts)
+print(output.shape)
+
+torch.save(model.state_dict(), 'rt3_model.pth')
 
-#example usage
-video = torch.randn(2, 3, 6, 224, 224)
-instructions = [
-    'Bring me tthat apple on the table',
-    'Please bring me the butter'
-]
-
-train_logits = robo_cat.forward(video, instructions)
-robo_cat.model.eval()
-eval_logits = robo_cat.forward(video, instructions, cond_scale=3.0)
 ```
 
 * Or train:
 
 ```python
-from roboCAT import RoboCat_Train
+from roboCAT import Train
 
-RoboCat_Train()
+Train()
 
 ```
 
 
 # Method 2
 
 * First `git clone` the repository: `git clone https://github.com/kyegomez/RoboCAT.git`
@@ -46,27 +58,38 @@
 * Then cd `cd RoboCAT` 
 
 * Then, pip install: `python3 -m pip install -r requirements.txt`
 
 * Then test with 
 ```python 
 import torch
-from roboCAT import robo_cat
+from robocat import PALME, Robocat
+
+model = Robocat(
+    palme=PALME(),
+    num_actions=11,
+    action_bins=256,
+    depth=6,
+    heads=8,
+    dim_head=64,
+    token_learner_ff_mult=2,
+    token_learner_num_layers=2,
+    token_learner_num_output_tokens=8,
+    cond_drop_prob=0.2,
+    use_attn_conditioner=False,
+    conditioner_kwargs=dict()
+)
+
+video = torch.rand((1, 3, 224, 224))
+texts = ["this is a text"]
+output = model(video, texts)
+print(output.shape)
 
+torch.save(model.state_dict(), 'rt3_model.pth')
 
-#example usage
-video = torch.randn(2, 3, 6, 224, 224)
-instructions = [
-    'Bring me tthat apple on the table',
-    'Please bring me the butter'
-]
-
-train_logits = robo_cat.forward(video, instructions)
-robo_cat.model.eval()
-eval_logits = robo_cat.forward(video, instructions, cond_scale=3.0)
 ```
 
 * Or run training on C4 `accelerate config`
 
 * Then, `accelerate launch roboCAT/train.py`
 
 ## Architecture
```

### Comparing `robocat-0.0.2/roboCAT/train.py` & `robocat-0.0.4/robocat/train.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from torch.distributed.fsdp import (
     FullyShardedDataParallel,
     MixedPrecision,
     BackwardPrefetch,
     ShardingStrategy,
 )
 from accelerate import Accelerator
-from accelerate.utils import (DummyOptim, DummyScheduler,
+from accelerate.utils import (DummyOptim,
                               InitProcessGroupKwargs)
-from datasets import concatenate_datasets, load_dataset
+from datasets import load_dataset
 from lion_pytorch import Lion
 from torch.nn import LayerNorm
 
 from torch.nn import LayerNorm
 
 from torch.distributed.algorithms._checkpoint.checkpoint_wrapper import (
     CheckpointImpl, apply_activation_checkpointing, checkpoint_wrapper)
@@ -34,50 +34,56 @@
 from tqdm import tqdm
 from transformers import (AutoTokenizer, default_data_collator,
                           get_cosine_schedule_with_warmup,
                           get_linear_schedule_with_warmup, set_seed)
 
 
 # from utils.stable_adamw import StableAdamWUnfused
-from transformers import AutoModelForCausalLM, BitsAndBytesConfig
 
+from accelerate.logging import get_logger
 
-from robocat.models.MechaZilla.models.rt1.robotic_transformer import TransformerAttention
-from robocat.model import robo_cat
+
+from robocat.model import RoboCAT
 from robocat.utils.stabe_adam import StableAdamWUnfused
 
-############ SETUP CONFIG
-# import torch.distributed as dist
+########### SETUP CONFIG
+import torch.distributed as dist
+
+
+from accelerate.state import AcceleratorState
+
+# state = AcceleratorState()
 
-# dist.init_process_group(backend='nccl', init_method="env://")
 
-################
+logger = get_logger(__name__, log_level="INFO")
 
 class CFG:
-    BATCH_SIZE: int = 3
+    BATCH_SIZE = 1
     GRADIENT_ACCUMULATE_EVERY: int = 1
     SEED: int = 42
-    LEARNING_RATE: float = 3e-4
+    LEARNING_RATE: float = 1e-4 #3e-4 # 1e-4 for lion
     WEIGHT_DECAY: float = 0.1
     SEQ_LEN: int = 8192
     NUM_CPU: int = multiprocessing.cpu_count()
     USE_DEEPSPEED: bool = True
     USE_FSDP: bool = True
     USE_PRETOKENIZED: bool = True
-    USE_ACTIVATION_CHECKPOINTING: bool = False
-    RESUME_FROM_CHECKPOINT: str = None
+    USE_ACTIVATION_CHECKPOINTING: bool = True
+    RESUME_FROM_CHECKPOINT: str = False
     CHECKPOINTING_STEPS: int = 1000
-    OUTPUT_DIR: str = "YOUR_OUTPUT_DIR"
-    ENTITY_NAME: str = "YOUR_ENTITY_NAME" #wandb
+    OUTPUT_DIR: str = 'checkpoints/' # Folder
+    ENTITY_NAME: str = "Andromeda"
+    LOGGING_STEPS: int = 100
 
 
 # helpers
 
 
 def print_num_params(model, accelerator: Accelerator):
+    # n_params = sum(p.numel() for p in model.parameters() if p.requires_grad)
     n_params = sum(p.numel() for p in model.parameters() if p.requires_grad)
     accelerator.print(f"Number of parameters in model: {n_params}")
 
 
 # activation checkpointing
 
 
@@ -91,17 +97,17 @@
 
     Args:
         model (Module): The model to which to apply activation checkpointing.
         offload_to_cpu (bool, optional): Whether to offload the activations to CPU. Defaults to False.
         accelerator (Accelerator, optional): The Accelerate library accelerator. Defaults to None.
     """
     if accelerator is not None:
-        accelerator.print(f"Using activation checkpointing")
-    #maybe error here in TransformerAttention, use parallel transformer block
-    check_fn = lambda submodule: isinstance(submodule, TransformerAttention)
+        accelerator.print("Using activation checkpointing")
+    def check_fn(submodule):
+        return isinstance(submodule, RoboCAT)
     non_reentrant_wrapper = partial(
         checkpoint_wrapper,
         offload_to_cpu=offload_to_cpu,
         checkpoint_impl=CheckpointImpl.NO_REENTRANT,
     )
     apply_activation_checkpointing(
         model, checkpoint_wrapper_fn=non_reentrant_wrapper, check_fn=check_fn
@@ -130,22 +136,22 @@
         ValueError: If the provided mp (mixed precision mode) is not 'bf16', 'fp16' or 'fp32'.
         ValueError: If the provided shard_strat (sharding strategy) is not 'SHARD_GRAD', 'FULL_SHARD' or 'NO_SHARD'.
 
     Returns:
         torch.nn.Module: The input model wrapped with FSDP.
     """
     if auto_wrap:
-        robo_cat_auto_wrap_policy = partial(
+        Andromeda_auto_wrap_policy = partial(
             transformer_auto_wrap_policy,
             transformer_layer_cls={
-                TransformerAttention,
+                RoboCAT,
             },
         )
     else:
-        robo_cat_auto_wrap_policy = None
+        Andromeda_auto_wrap_policy = None
 
     if mp == "bf16":
         mp_fsdp = MixedPrecision(
             param_dtype=torch.bfloat16,
             # Gradient communication precision.
             reduce_dtype=torch.bfloat16,
             # Buffer precision.
@@ -185,15 +191,15 @@
             "Invalid scheduler_type. Expected 'SHARD_GRAD', 'FULL_SHARD' or 'NO_SHARD', got: {}".format(
                 shard_strat
             )
         )
 
     model = FullyShardedDataParallel(
         model,
-        auto_wrap_policy=robo_cat_auto_wrap_policy,
+        auto_wrap_policy=Andromeda_auto_wrap_policy,
         mixed_precision=mp_fsdp,
         backward_prefetch=BackwardPrefetch.BACKWARD_PRE,
         sharding_strategy=sharding_strat_fsdp,
         forward_prefetch=True,
         use_orig_params=True,
     )
 
@@ -353,16 +359,21 @@
             decay_param.append(param_dict[param])
 
     # Create an empty list called no_decay_param to store the parameters without weight decay.
     no_decay_param = []
 
     # Iterate over the no_decay list, which contains the names of the parameters without weight decay.
     for param in no_decay:
-        # Append the corresponding parameter from param_dict to the no_decay_param list.
-        no_decay_param.append(param_dict[param])
+        try:
+                
+            # Append the corresponding parameter from param_dict to the no_decay_param list.
+            no_decay_param.append(param_dict[param])
+        except KeyError:
+            # print(f"Parameter {param_name} does not exist in the model")
+            pass
 
     # Create a list called grouped_params that contains two dictionaries.
     # The first dictionary has the decay_param list and the corresponding weight_decay value.
     # The second dictionary has the no_decay_param list and a weight_decay value of 0.0.
     grouped_params = [
         {"params": decay_param, "weight_decay": weight_decay},
         {"params": no_decay_param, "weight_decay": 0.0},
@@ -375,14 +386,18 @@
         optimizer = AdamW(grouped_params, lr=learning_rate, betas=(beta_1, beta_2),)
     elif optimizer_type == "deepspeed":
         optimizer = DummyOptim(grouped_params, lr=learning_rate, betas=(beta_1, beta_2),)
     elif optimizer_type == "stable_adamw":
         optimizer = StableAdamWUnfused(
             grouped_params, lr=learning_rate, betas=(beta_1, beta_2),
         )
+    # elif optimizer_type=="Adam8bit":
+    #     optimizer = bnb.optim.Adam8bit(grouped_params, lr=learning_rate, betas=(beta_1, beta_2))
+    # elif optimizer_type=="Lion8Bit":
+    #     optimizer = bnb.optim.Lion8bit(grouped_params, lr=learning_rate, betas=(beta_1, beta_2))
     else:
         raise ValueError(
             "Invalid optimizer_type. Expected 'lion', 'adamw', 'deepspeed' or 'stable_adamw', got: {}".format(
                 optimizer_type
             )
         )
 
@@ -438,60 +453,58 @@
         group_texts, batched=True, num_proc=CFG.NUM_CPU,
     )
 
     return train_dataset
 
 #switch to falconwebdataset
 def build_pre_tokenized():
-    d0 = load_dataset("conceptofmind/c4_0-to-20_neox_with_eos_8k", split="train")
-    d1 = load_dataset("conceptofmind/c4_21-to-40_neox_with_eos_8k", split="train")
-    d2 = load_dataset("conceptofmind/c4_41-to-60_neox_with_eos_8k", split="train")
-    d3 = load_dataset("conceptofmind/c4_61-to-80_neox_with_eos_8k", split="train")
-    d4 = load_dataset("conceptofmind/c4_81-to-100_neox_with_eos_8k", split="train")
-    train_dataset = concatenate_datasets([d0, d1, d2, d3, d4])
-    return train_dataset
+    d0 = load_dataset("conceptofmind/c4_0-to-20_neox_with_eos_8k", split="train[:10]")
+    # d1 = load_dataset("conceptofmind/c4_21-to-40_neox_with_eos_8k", split="train")
+    # d2 = load_dataset("conceptofmind/c4_41-to-60_neox_with_eos_8k", split="train")
+    # d3 = load_dataset("conceptofmind/c4_61-to-80_neox_with_eos_8k", split="train")
+    # d4 = load_dataset("conceptofmind/c4_81-to-100_neox_with_eos_8k", split="train")
+    # train_dataset = concatenate_datasets([d0, d1, d2, d3, d4])
+    return d0
 
 
 
-def RoboCat_Train():
+def Train():
     # accelerator
 
     timeout = InitProcessGroupKwargs(timeout=timedelta(seconds=1_000_000))
 
     accelerator = Accelerator(
         gradient_accumulation_steps=CFG.GRADIENT_ACCUMULATE_EVERY,
         mixed_precision="fp16",
         log_with="wandb",
         kwargs_handlers=[timeout],
     )
-    # AcceleratorState().deepspeed_plugin.deepspeed_config['train_micro_batch_size_per_gpu'] = 4 #??????
 
+    state = AcceleratorState()
+    
+    state.deepspeed_plugin.deepspeed_config['train_micro_batch_size_per_gpu'] = CFG.BATCH_SIZE #??????
 
     accelerator.init_trackers(
-        project_name="robo_cat",
+        project_name="Andromeda",
         config={
             "batch_size": CFG.BATCH_SIZE,
             "gradient_accumulate_every": CFG.GRADIENT_ACCUMULATE_EVERY,
             "learning_rate": CFG.LEARNING_RATE,
             "seq_len": CFG.SEQ_LEN,
         },
-        init_kwargs={"wandb": {"entity": CFG.ENTITY_NAME}},
+        # init_kwargs={"wandb": {"entity": CFG.ENTITY_NAME}},
     )
 
     accelerator.print(f"Total GPUS: {accelerator.num_processes}")
 
     # set seed
 
     set_seed(CFG.SEED)
 
-
-    # model = robo_cat.to(accelerator.device)
-    # model = AutoModelForCausalLM.from_pretrained("YOUR MODEL", load_in_4bit=True, device_map="auto").to(accelerator.device)
-
-    model = robo_cat.to(accelerator.device)
+    model = RoboCAT()
 
     print_num_params(model, accelerator)
 
     if CFG.USE_FSDP:
         model = fsdp(
             model,
             mp="fp16",
@@ -510,51 +523,51 @@
     else:
         train_dataset = build_dataloaders()
 
     train_loader = DataLoader(
         train_dataset, batch_size=CFG.BATCH_SIZE, collate_fn=default_data_collator,
     )
 
-    # optimizer
 
+    # optimizer
     optim = decoupled_optimizer(
         model=model,
         learning_rate=CFG.LEARNING_RATE, 
         weight_decay=CFG.WEIGHT_DECAY, 
         beta_1=0.90, 
         beta_2=0.95, 
-        optimizer_type='deepspeed',  
+        optimizer_type='lion',  
         use_fsdp=True,
         accelerator=accelerator
     )
 
     # Determine number of training steps
 
     max_train_steps = math.ceil(len(train_loader) / CFG.GRADIENT_ACCUMULATE_EVERY)
     accelerator.print(f"Max train steps: {max_train_steps}")
 
     # lr scheduler
 
     NUM_WARMUP_STEPS = int(max_train_steps * 0.01)
     accelerator.print(f"Num warmup steps: {NUM_WARMUP_STEPS}")
 
-    if CFG.USE_DEEPSPEED:
-        lr_scheduler = DummyScheduler(
-            optim, 
-            total_num_steps=max_train_steps * accelerator.num_processes, 
-            warmup_num_steps=NUM_WARMUP_STEPS
-        )
-    else:
-        lr_scheduler = get_lr_scheduler_with_warmup(
-            optimizer=optim,
-            scheduler_type="cosine",
-            num_warmup_steps=NUM_WARMUP_STEPS,
-            max_train_steps=max_train_steps,
-            grad_accumulate_every=CFG.GRADIENT_ACCUMULATE_EVERY,
-        )
+    # if False: # if CFG.USE_DEEPSPEED:
+    #     lr_scheduler = DummyScheduler(
+    #         optim, 
+    #         total_num_steps=max_train_steps * accelerator.num_processes, 
+    #         warmup_num_steps=NUM_WARMUP_STEPS
+    #     )
+    # else:
+    lr_scheduler = get_lr_scheduler_with_warmup(
+        optimizer=optim,
+        scheduler_type="cosine",
+        num_warmup_steps=NUM_WARMUP_STEPS,
+        max_train_steps=max_train_steps,
+        grad_accumulate_every=CFG.GRADIENT_ACCUMULATE_EVERY,
+    )
 
     # prepare
 
     optim, train_loader, lr_scheduler = accelerator.prepare(
         optim, train_loader, lr_scheduler
     )
 
@@ -627,14 +640,20 @@
                 if CFG.OUTPUT_DIR is not None:
                     output_dir = os.path.join(CFG.OUTPUT_DIR, output_dir)
                 accelerator.save_state(output_dir)
 
         if completed_steps >= max_train_steps:
             break
 
+        #logging every CFG.LOGGING STEPS
+        if CFG.LOGGING_STEPS > 0 and step % CFG.LOGGING_STEPS == 0:
+            logger.info(
+                f"Step: {completed_steps}/{max_train_steps}, Loss: {loss.item():.5f}"
+            )
+
     # end training
 
     # accelerator.print(f"Training Finished")
     accelerator.end_training()
 
     # save final model
 
@@ -644,9 +663,24 @@
         unwrapped_model = accelerator.unwrap_model(model)
         with accelerator.main_process_first():
             accelerator.save(
                 unwrapped_model.state_dict(), f"{CFG.OUTPUT_DIR}/final/final_model.pt"
             )
 
 
-if __name__ == "__main__":
-    RoboCat_Train()
+def main():
+    os.environ['MASTER_ADDR'] #'localhost'
+    os.environ['MASTER_PORT'] #= '9994'
+    
+    # # [CRITICAL] Pay attention to this when scaling to multiple GPUs and clusters
+    
+    # # Pay attention to this, use "accelerate config"
+
+    os.environ['RANK']       #= str(0) # Number of nodes (servers)
+    os.environ['WORLD_SIZE'] # = str(torch.cuda.device_count())
+
+    dist.init_process_group(backend='nccl') #init_method="env://")
+    
+    Train()
+
+if __name__ == '__main__':
+    main()
```

### Comparing `robocat-0.0.2/robocat.egg-info/PKG-INFO` & `robocat-0.0.4/robocat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocat
-Version: 0.0.2
+Version: 0.0.4
 Summary: Robo CAT- Pytorch
 Home-page: https://github.com/kyegomez/RoboCAT
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,robotics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `robocat-0.0.2/setup.py` & `robocat-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'robocat',
   packages = find_packages(exclude=[]),
-  version = '0.0.2',
+  version = '0.0.4',
   license='MIT',
   description = 'Robo CAT- Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/RoboCAT',
   keywords = [
     'artificial intelligence',
     'deep learning',
     'transformers',
     'attention mechanism',
     'robotics'
   ],
   install_requires=[
-    'classifier-free-guidance-pytorch>=0.1.4',
-    'einops>=0.6',
-    'torch>=1.6',
-    ''
+      'transformers',
+      'torch',
+      'einops',
+      'beartype',
+      'palme',
+      'transformers',
+      'palm-rlhf-pytorch',
+      'tokenizers',
+      'wandb',
+      'classifier-free-guidance-pytorch'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

