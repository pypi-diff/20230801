# Comparing `tmp/SPCEj9bbotw-0.0.4.tar.gz` & `tmp/SPCEj9bbotw-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPCEj9bbotw-0.0.4.tar", last modified: Sat Jul 29 11:24:44 2023, max compression
+gzip compressed data, was "SPCEj9bbotw-0.0.5.tar", last modified: Tue Aug  1 06:36:35 2023, max compression
```

## Comparing `SPCEj9bbotw-0.0.4.tar` & `SPCEj9bbotw-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 11:24:44.748187 SPCEj9bbotw-0.0.4/
--rw-rw-rw-   0        0        0       58 2023-07-29 11:24:44.748187 SPCEj9bbotw-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 11:24:44.736184 SPCEj9bbotw-0.0.4/SPCEj9bbotw/
--rw-rw-rw-   0        0        0     3028 2023-06-14 07:31:18.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw/_.py
--rw-rw-rw-   0        0        0       21 2023-07-29 11:24:02.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw/__init__.py
--rw-rw-rw-   0        0        0     1094 2023-07-29 11:24:24.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw/_main.py
--rw-rw-rw-   0        0        0     8306 2023-07-29 08:22:02.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw/kernels.py
--rw-rw-rw-   0        0        0    14654 2023-07-29 11:24:26.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw/optimizer.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:24:44.746187 SPCEj9bbotw-0.0.4/SPCEj9bbotw.egg-info/
--rw-rw-rw-   0        0        0       58 2023-07-29 11:24:44.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-29 11:24:44.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 11:24:44.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-29 11:24:44.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 11:24:44.748187 SPCEj9bbotw-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      134 2023-07-29 11:24:22.000000 SPCEj9bbotw-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 06:36:35.639975 SPCEj9bbotw-0.0.5/
+-rw-rw-rw-   0        0        0       58 2023-08-01 06:36:35.639975 SPCEj9bbotw-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 06:36:35.625971 SPCEj9bbotw-0.0.5/SPCEj9bbotw/
+-rw-rw-rw-   0        0        0     3028 2023-06-14 07:31:18.000000 SPCEj9bbotw-0.0.5/SPCEj9bbotw/_.py
+-rw-rw-rw-   0        0        0       25 2023-08-01 06:36:10.000000 SPCEj9bbotw-0.0.5/SPCEj9bbotw/__init__.py
+-rw-rw-rw-   0        0        0     4650 2023-08-01 06:32:47.000000 SPCEj9bbotw-0.0.5/SPCEj9bbotw/_main.py
+-rw-rw-rw-   0        0        0     8720 2023-08-01 06:04:33.000000 SPCEj9bbotw-0.0.5/SPCEj9bbotw/kernels.py
+-rw-rw-rw-   0        0        0     6533 2023-08-01 06:04:14.000000 SPCEj9bbotw-0.0.5/SPCEj9bbotw/optimizer.py
+drwxrwxrwx   0        0        0        0 2023-08-01 06:36:35.637975 SPCEj9bbotw-0.0.5/SPCEj9bbotw.egg-info/
+-rw-rw-rw-   0        0        0       58 2023-08-01 06:36:35.000000 SPCEj9bbotw-0.0.5/SPCEj9bbotw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-08-01 06:36:35.000000 SPCEj9bbotw-0.0.5/SPCEj9bbotw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 06:36:35.000000 SPCEj9bbotw-0.0.5/SPCEj9bbotw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-01 06:36:35.000000 SPCEj9bbotw-0.0.5/SPCEj9bbotw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 06:36:35.639975 SPCEj9bbotw-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      134 2023-08-01 06:36:06.000000 SPCEj9bbotw-0.0.5/setup.py
```

### Comparing `SPCEj9bbotw-0.0.4/SPCEj9bbotw/_.py` & `SPCEj9bbotw-0.0.5/SPCEj9bbotw/_.py`

 * *Files identical despite different names*

### Comparing `SPCEj9bbotw-0.0.4/SPCEj9bbotw/kernels.py` & `SPCEj9bbotw-0.0.5/SPCEj9bbotw/kernels.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,26 +17,27 @@
     } IDXS;
     
     typedef struct {
         float rho1;
         float rho2;
     } COND;
     
-    typedef struct {
+    /*typedef struct {
         float theta;
         float sig;
         float u;
         float z;
         float pos ;
         float vel ;
         float socb;
         float exp1;
         float exp2;
-    } SCALE;
+    } SCALE;*/
 
+    //__device__ float y[""" + repr(num_thread) + r"""] ={0.0} ;
 
     __device__ float buff_y[""" + repr(num_thread) + r"""] ={0.0} ;
 
     __device__ float w["""+ repr(num_thread) +r"""]={0.0}  ;
 
     __device__ float buff_w["""+ repr(num_thread) +r"""]={0.0} ;
 
@@ -44,25 +45,25 @@
 
     __device__ float ys["""+ repr(num_thread) +r"""] ={0.0};
 
     __device__ int NR_epoch = 1000;
 
     __device__ int NR_eps = 0.001;
     
-    __device__ SCALE scale ={0, 10, 1, 1, 100, 10, 0.1, 0.1*0.2*24000, 0.1*0.8*24000};
+    //__device__ SCALE scale ={0, 10, 1, 1, 100, 10, 0.1, 0.1*0.2*24000, 0.1*0.8*24000};
     
 
-    __device__ float NR_f(float x, float a, float b, float rho){
+    __device__ float NR_f(float x, float a, float b, float rho, float c){
 
-        return expf(x)*(x - a) - powf(rho, 2)*expf(-x) + rho*(b);
+        return expf(c*x)*(x - a) - powf(rho, 2)*c*expf(-c*x) + rho*(b)*c;
     }
 
-    __device__ float NR_fdot(float x, float a, float b, float rho){
+    __device__ float NR_fdot(float x, float a, float b, float rho, float c){
 
-        return expf(x)*(x - a + 1) + powf(rho, 2)*expf(-x);
+        return expf(c*x)*(c*x - c*a + 1) + powf(rho, 2)*expf(-c*x)*powf(c,2);
     }
 
     __device__ float func_matmulvec(float* x, float* y, int act_len){
 
         float result = 0;
 
         for(int i=0; i < act_len; i++){
@@ -110,57 +111,59 @@
             }
         }
 
     }
     
     
     
-    __device__ float NR(float* a, float* b, float rho){
+    __device__ float NR(float* a, float* b, float rho, float c){
 
         float x = *a;
         
         for(int i=0; i < NR_epoch; i++){
-            x = x - NR_f(x, *a, *b, rho)/NR_fdot(x, *a, *b, rho);
-            if(fabsf(NR_f(x, *a, *b, rho)) <= NR_eps){
+            x = x - NR_f(x, *a, *b, rho, c)/NR_fdot(x, *a, *b, rho, c);
+            if(fabsf(NR_f(x, *a, *b, rho, c)) <= NR_eps){
                 return x;
             }
         }
 
         return x;
     }
 
-    __device__ void itv_exp(float* sig, float* z, float rho1, float rho2){
-
-        if(*sig < rho1*expf(- *z)){
-            *z = NR(z, sig, rho1);
-            *sig = rho1*expf(- *z);
-
+    __device__ void itv_exp(float* sig, float* z, float rho1, float rho2, float scl_z){
 
+        if(*sig < rho1*expf(- scl_z*(*z))){
+            *z = NR(z, sig, rho1, scl_z);
+            *sig = rho1*expf(- scl_z*(*z));
 
         }
-        else if(*sig > rho2*expf(- *z)){
-            *z = NR(z, sig, rho2);
-            *sig = rho2*expf(- *z);
+        else if(*sig > rho2*expf(- scl_z*(*z))){
+            *z = NR(z, sig, rho2, scl_z);
+            *sig = rho2*expf(- scl_z*(*z));
 
             
         }
 
     }
 
 
     extern "C"
-    __global__ void main_(float* y, float* y_fix, float* tilde_C, float* z_lb, float* z_ub, int N, int epoch, float* acc_cmd){
+    __global__ void main_(float* y, float* y_fix, float* tilde_C, float* z_lb, float* z_ub, int N, int epoch, float* acc_cmd, float* scales){
 
         int idx = _Coor;
         int len_var = 11*N;
         int len_dual = 9*N;
         int shr_idx = idx % 11;
         int res_idx = idx % N;
         
-        SCALE scale;
+        //SCALE scale;
+        
+        float scl_z = scales[0];
+        float scl_coeff_exp_lb = scales[1];
+        float scl_coeff_exp_ub = scales[2];
 
         IDXS idxs;
         idxs.u = 11*idx; idxs.x = 11*idx+3; idxs.sig = 11*idx+9; idxs.z = 11*idx+10;
 
         IDXS res_idxs;
         res_idxs.u = 11*res_idx; res_idxs.x = 11*res_idx+3; res_idxs.sig = 11*res_idx+9; res_idxs.z = 11*res_idx+10;
         
@@ -229,15 +232,15 @@
             /*-----------------socbp----------------------------------*/
             else if(3*N <= idx && idx < 4*N){
                 for(int i=0; i < 3; i++){
                     th_proj1[i] = buff_y[res_idxs.u+i] + th_ys[i];
                 }
                 *th_proj2 = buff_y[res_idxs.sig] + th_ys[3];
                 //Gcone_(th_proj1, th_proj2, scale.socb);
-                Gcone_(th_proj1, th_proj2, 0.1);
+                Gcone_(th_proj1, th_proj2, 0.1);  //
                 
                 for(int i=0; i < 3; i++){
                     th_ys[i] = th_ys[i] + buff_y[res_idxs.u+i] - th_proj1[i];
                 }
                 th_ys[3] = th_ys[3] + buff_y[res_idxs.sig] - *th_proj2;
                 
 
@@ -250,15 +253,15 @@
        
                 }
                 else{
                     *th_proj1 = buff_y[res_idxs.sig] + th_ys[0];
                     *th_proj2 = buff_y[res_idxs.z-11] + th_ys[1];
      
                 }
-                itv_exp(th_proj1, th_proj2, 480, 1920);
+                itv_exp(th_proj1, th_proj2, scl_coeff_exp_lb, scl_coeff_exp_ub, scl_z);    //
                 
                 
                 if(res_idx == 0){
                     th_ys[0] = th_ys[0] + buff_y[res_idxs.sig] - *th_proj1;
                     th_ys[1] = th_ys[1] + z_lb[0] - *th_proj2;
         
                 }
@@ -277,14 +280,15 @@
         }
         //y[idx] = buff_w[idx];
         sync(grid);
         if(idx == 0){
             for(int i=0; i < 3; i++){
                 acc_cmd[i] = y[i];
             }
+            acc_cmd[3] = y[9];
         }
 
         sync(grid);
     }
     """
     SM_main_ = cp.RawKernel(str_, 'main_', enable_cooperative_groups=True)
     return SM_main_
```

