# Comparing `tmp/rego-1.5.2.tar.gz` & `tmp/rego-1.6.1.tar.gz`

## Comparing `rego-1.5.2.tar` & `rego-1.6.1.tar`

### file list

```diff
@@ -1,700 +1,699 @@
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:52.000000 rego-1.5.2/
--rwxrwxr-x   0 davide    (1000) davide    (1000)      142 2022-05-26 15:35:19.000000 rego-1.5.2/MANIFEST.in
--rw-rw-r--   0 davide    (1000) davide    (1000)     2555 2022-05-26 15:35:52.000000 rego-1.5.2/PKG-INFO
--rwxrwxr-x   0 davide    (1000) davide    (1000)      115 2022-05-26 15:35:19.000000 rego-1.5.2/pyproject.toml
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1127 2022-05-26 15:35:19.000000 rego-1.5.2/LICENSE
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:52.000000 rego-1.5.2/src/
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/
--rwxrwxr-x   0 davide    (1000) davide    (1000)      208 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/NOTICE.txt
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11357 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/LICENSE
--rwxrwxr-x   0 davide    (1000) davide    (1000)    12666 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/README.md
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/line_search/
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11032 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/line_search/more_thuente.hpp
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/
--rwxrwxr-x   0 davide    (1000) davide    (1000)    10573 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/pso_dv.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8051 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/gd.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7453 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/gd.ipp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9955 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/lbfgs.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    15780 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/de_prmm.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     6505 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/newton.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11427 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/cg.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11188 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/pso.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    12830 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/nm.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9507 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/bfgs.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    10693 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/de.hpp
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/zeros/
--rwxrwxr-x   0 davide    (1000) davide    (1000)    16983 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/zeros/broyden_df.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    13567 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/zeros/broyden.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1876 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/optim.hpp
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/constrained/
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7773 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/constrained/sumt.hpp
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/
--rwxrwxr-x   0 davide    (1000) davide    (1000)    38092 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/optim_trace.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2155 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/numerical_gradient.hpp
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1477 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/reset_negative_values.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1513 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/max.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1140 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/dot.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1792 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/randi.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1112 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/exp.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1139 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/size.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1609 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/access.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1112 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/cos.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1656 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/abs_max.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1143 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/array_add.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1219 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/accu.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1421 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/array_div.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1269 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/transpose.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1337 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/get_sort_index.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1553 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/randu.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1111 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/cout.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1459 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/min.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1119 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/pow.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1146 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/array_mult.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1137 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/inv.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1162 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/diagmat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1924 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/randn.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1088 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/eval.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1467 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/sum.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1097 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/ncol.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1117 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/sqrt.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1140 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/abs.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1169 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/solve.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1399 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/zeros.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1275 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/set_size.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1112 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/log.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1230 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/index_min.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1116 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/endl.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1121 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/as_scalar.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1145 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/eye.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1167 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/hadamard.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1227 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/is_finite.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1700 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/norm.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1389 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/ones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1171 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/diagvec.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2007 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/jacobian_adjust.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3024 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/optim_options.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3024 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/error_reporting.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3958 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/transform_vals.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1102 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/misc.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1048 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/unit_vec.ipp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5491 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/optim_structs.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7261 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/error_reporting.ipp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1073 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/unit_vec.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1919 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/determine_bounds_type.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3856 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/numerical_hessian.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2166 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/optim-master/header_only_version/misc/optim_matdefs.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8785 2022-05-26 15:35:19.000000 rego-1.5.2/src/cypack/rego.pyx
--rwxrwxr-x   0 davide    (1000) davide    (1000)    56664 2022-05-26 15:35:19.000000 rego-1.5.2/src/cypack/functions.cpp
--rw-rw-r--   0 davide    (1000) davide    (1000)   326752 2022-05-26 15:35:27.000000 rego-1.5.2/src/cypack/rego.cpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1759 2022-05-26 15:35:19.000000 rego-1.5.2/src/cypack/functions.h
--rwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:19.000000 rego-1.5.2/src/cypack/__init__.py
--rwxrwxr-x   0 davide    (1000) davide    (1000)      912 2022-05-26 15:35:19.000000 rego-1.5.2/src/cypack/generate_doc.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/
--rwxrwxr-x   0 davide    (1000) davide    (1000)    30011 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11803 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_cube_slices_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1294 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/CubeToMatOp_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4113 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_hypot_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    18630 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/auxlib_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1114 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cor_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    14153 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_mean_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2062 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_shift.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1788 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_min_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1600 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_static_check.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2628 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/hdf5_name.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1650 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/span.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1216 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_cov_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9041 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/def_atlas.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2635 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_join_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4094 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_kron_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1994 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_hist.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3543 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_elem2_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8483 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_div.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2622 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_strans.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1581 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_find_unique.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3546 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_resize_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3971 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_chi2rnd_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7031 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/podarray_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1313 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_normalise_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11433 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_all_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7440 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/BaseCube_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    21305 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_elem.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1951 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_polyval_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1331 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_nonzeros_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1273 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_prod_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4704 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_svd.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2250 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/unwrap_cube.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5212 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_SortEigenvalue.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1437 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/GlueCube_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    97754 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1184 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_range_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1554 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_kmeans.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)      815 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/compiler_setup_post.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2792 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cond_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1132 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_trimat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4833 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_cube_each_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    14171 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_approx_equal.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3717 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_chi2rnd.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2354 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_reverse_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1923 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_stddev.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1288 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cumsum_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    18866 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_ostream_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1752 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_index_max_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1458 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_chi2rnd_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11193 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/config.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1537 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtGlueCube_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11016 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fft_engine.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9571 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/band_helper.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1479 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SizeMat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4068 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/def_superlu.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1106 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_hist_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    20201 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_norm_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1216 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_cor_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11768 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_SymEigsSolver_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2442 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_inplace_trans.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3041 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_eig_pair.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2896 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_var.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    14416 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/running_stat_vec_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    18533 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_times_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    10585 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_diagmat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1739 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_quantile.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1574 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_trapz_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    15000 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpBase_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1104 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_resize_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8959 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpRow_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3990 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_reverse_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4436 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_inv_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1194 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/compiler_extra.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2768 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_rel_comparators.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2763 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_sum.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3247 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_mean_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)   106690 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/def_lapack.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1359 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_diagvec_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2133 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Op_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1292 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/distr_param.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1704 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sort_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1525 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_cov.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2500 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_schur.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2617 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Op_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3643 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_hess.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2648 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_stddev_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1478 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_version.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2037 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11396 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_as_scalar.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4433 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpBase_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    19223 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_elem2_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2902 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eOpCube_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1493 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_hypot_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9043 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_schur.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2547 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1046 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_stddev_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5282 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_powmat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1724 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtGlue_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2539 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_var_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5410 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_randi.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1511 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_polyfit_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1743 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_affmul_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    24709 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpProxy.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    30357 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_each_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    13014 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mul_gemv.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1349 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_SparseGenMatProd_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1175 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_pinv_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1899 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mp_misc.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1474 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_strans_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3520 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_eigs_gen.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2836 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_join_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3161 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_randperm.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2304 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_expmat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1684 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_histc.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    13212 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_cmath.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1562 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_range.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1016 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_toeplitz_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1149 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_repmat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3349 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_norm_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3407 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_trimat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    10296 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_join_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2287 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eGlue_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    12332 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cx_scalar_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    27214 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_max_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1296 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_polyval_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    12134 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_plus.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    16131 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpSubview_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3844 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/csv_name.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1323 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_unique.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1509 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_hist_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     6523 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_min_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3143 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_elem_helper_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1237 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_reverse_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2428 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Gen_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)   151041 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpMat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1870 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtSpOp_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1620 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtSpGlue_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2704 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtOpCube_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1421 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/include_hdf5.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3783 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_dotext_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5550 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_shift_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    19411 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arrayops_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2174 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_trimat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1139 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_chol_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2320 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/GenCube_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3854 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_relational_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2752 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_mean.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4787 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sort_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1674 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpOp_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3516 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_symmat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1541 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SizeCube_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1869 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_all.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1453 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_intersect_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    23212 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_accu.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2125 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/access.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1426 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_trapz.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2961 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_fft.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2114 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/xvec_htrans_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5402 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_solve_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3493 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_relational_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1565 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_htrans_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2816 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_sprandu.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3176 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_cube_schur.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)   122818 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Cube_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    21615 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spdiagview_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5512 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_expmat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4054 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_eig_gen.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1295 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/cond_rel_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4176 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_config.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3299 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SizeCube_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    34646 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_times_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3272 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_field_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1723 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_inv_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     6523 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_max_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7793 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/MapMat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2344 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_max_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4214 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_wishrnd.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1991 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_schur_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     6978 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/gmm_full_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2231 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_eps.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1433 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtSpGlue_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4191 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8197 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_interp2.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4867 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_rng_cxx11.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1906 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_toeplitz_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2455 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_sum_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2134 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/typedef_elem_check.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    12978 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_affmul_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11286 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/config.hpp.cmake
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1244 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_nonzeros.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3959 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_min_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    10732 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/def_arpack.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1799 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_TridiagEigen_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1882 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_reverse.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2005 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_chol.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1632 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_vectorise_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3156 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_fft2.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    65539 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/gmm_diag_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2828 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_times_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1998 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_wishrnd_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3129 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/gmm_misc_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1687 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_diff.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1989 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_trans.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5617 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_quantile_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1377 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/include_atlas.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2508 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_DoubleShiftQR_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3486 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_logmat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4322 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_reshape.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1647 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sp_plus_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1493 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_atan2_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9582 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_var_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9985 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_index_min_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9700 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/translate_arpack.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    81970 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/translate_lapack.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3297 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_roots_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4559 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_histc_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2841 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/OpCube_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2517 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/OpCube_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1345 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_DenseGenMatProd_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1134 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_normalise_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    13647 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mul_herk.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1346 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_spones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2554 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_vectorise_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3575 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_dot_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    10728 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mul_gemm_mixed.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11090 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_join.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    12376 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_field_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    14274 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_htrans_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4694 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_size.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5279 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_max.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2110 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_speye.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1496 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_htrans_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    47137 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eglue_core_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1651 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_reshape_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1650 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_shuffle.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1083 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cond_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    15762 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/diagmat_proxy.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3372 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_polyfit_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11062 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sqrtmat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3395 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_intersect_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5866 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/memory.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1450 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_diagvec.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11776 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_GenEigsSolver_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3275 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_ostream_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1904 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_trunc_exp.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    44133 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Mat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3420 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_normalise_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     6528 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/sympd_helper.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2399 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/podarray_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1989 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/xtrans_mat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2444 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_resize.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1602 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_flip_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3966 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/typedef_mat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8945 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_misc_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11139 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/constants.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1839 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_clamp_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3710 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_sort_index.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    12603 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_logmat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2521 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtOp_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1293 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_diff_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    25327 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpMat_iterators_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1505 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_orth_null_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1768 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_plus_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1168 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_cross_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    16312 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_trace.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5465 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_max_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7405 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3257 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sort_index_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1293 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cumprod_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11543 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_rng.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3786 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eGlue_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2013 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_var_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9015 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_reshape_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4995 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_diff_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3110 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_strans_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    10351 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/translate_blas.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2278 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpToDOp_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2132 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_any_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     6062 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_flip_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1321 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_merge_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2739 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpCol_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     6993 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/constants_old.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1594 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpGlue_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5203 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_misc_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    64647 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_cube_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2570 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sp_minus_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    61755 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/field_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2729 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_mvnrnd.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2344 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_min_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    10441 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Row_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1114 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cov_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    16374 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_min_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)      989 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_sum_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11190 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_forward.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9829 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_solve.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9154 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_svds.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    34942 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Row_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2637 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cov_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2371 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/wall_clock_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4538 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_eig_sym.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2746 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_clamp.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    13125 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/translate_atlas.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7523 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_cube_relational.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11015 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/injector_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2132 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_all_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1473 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtGlueCube_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    72198 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/unwrap.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11453 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_misc_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4420 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sort_index_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2566 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/injector_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3156 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_index_min.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7012 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_dot.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3156 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_index_max.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7304 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_find.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1747 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_cumprod.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    17717 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/compiler_setup.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2071 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eGlueCube_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     6262 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_hist_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1226 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_cross.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     6065 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Base_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3610 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_det.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5430 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_shuffle_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3504 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_kron_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3111 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_ostream.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2782 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_eye.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3112 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_TridiagEigen_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2382 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_symmat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2736 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpRow_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7185 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Gen_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2725 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_toeplitz_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1633 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/CubeToMatOp_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1656 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_kron_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11121 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_str.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1734 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_quantile_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3869 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_strans_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4273 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/translate_superlu.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5925 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_each_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    14147 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_merge_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    22905 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_elem1_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2563 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_powmat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3035 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_find_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9455 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_DoubleShiftQR_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1191 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_symmat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1323 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_repmat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    21404 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2234 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_range_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    10419 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_diagmat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1266 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpToDOp_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4834 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_cube_plus.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4772 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_cube_minus.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    31865 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/debug.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3543 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spdiagview_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2002 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_fft_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1788 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_max_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1333 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_powmat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8023 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_relational_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    67945 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/gmm_full_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1736 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_cumsum.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5492 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_spsolve.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3034 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eOp_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2815 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_cube_times.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1742 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_polyfit.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2604 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_syl_lyap.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    13320 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/diskio_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7365 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_wishrnd_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3165 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_log_det.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1458 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_expmat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1345 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_cx_attrib.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5327 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/GenCube_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    33981 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpSubview_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3830 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_ones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1533 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_toeplitz.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2113 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtSpOp_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    15573 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_find_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1506 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_histc_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    10494 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_any_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3377 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_cube_slices_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2365 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtOpCube_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2285 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_cross_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    12570 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_minus.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)   112626 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/diskio_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1527 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_cor.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1181 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_reverse_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    32307 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpSubview_iterators_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    12770 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mul_gemm.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4444 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/sp_auxlib_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    17558 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_conv_to.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2221 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_pinv.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4316 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_prod_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7051 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_relational_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8752 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_trig.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1329 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_roots_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5525 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_log_normpdf.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    35544 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpMat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2356 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sum_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2103 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_prod.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1723 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/GenSpecialiser.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3020 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eglue_core_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    20647 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/hdf5_misc.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3695 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cumsum_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2691 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/BaseCube_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9903 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/include_superlu.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1691 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_min_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2257 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_mean_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2054 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_cov_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1330 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_repelem.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5103 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/upgrade_val.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4850 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_mvnrnd_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3019 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_mixed_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    12428 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sum_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4533 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_cube_div.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2704 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SizeMat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1673 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/xtrans_mat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9148 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_schur_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1328 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_kron_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1914 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpOp_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1976 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_minus_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     6611 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_randg.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4160 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eGlueCube_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2197 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_diagmat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2097 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_diagmat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4150 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_orth_null_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3334 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_repmat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5681 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_atan2_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3035 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cor_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8593 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_fft_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2923 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/strip.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1825 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_unique_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    15975 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/field_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9985 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_index_max_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9996 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/restrictors.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5705 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_regspace.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2491 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_chol_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2523 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_normalise.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8241 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpCol_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2409 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_kron.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5459 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_min_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)   200436 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Mat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1211 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_DenseGenMatProd_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1606 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_conv_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3030 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_find_unique_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5293 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_times_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    12474 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_misc.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1774 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_diagmat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5937 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_normcdf.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)   178262 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/auxlib_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8610 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_mean_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    26376 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/traits.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    10452 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Col_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5655 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/running_stat_vec_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8867 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_cube_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1605 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_intersect.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11241 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_median_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2269 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_lu.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2186 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Glue_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    22986 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/ProxyCube.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    27217 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_min_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3856 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_rng_cxx98.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7250 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_plus_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3963 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/unwrap_spmat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7192 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eop_core_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1691 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_max_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3733 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_trapz_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2002 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/cond_rel_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    35001 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Col_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5112 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/typedef_elem.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11657 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_join_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1248 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_polyval.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     6009 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_clamp_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7737 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_inv.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1162 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_elem_helper_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2651 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpValProxy_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2352 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sqrtmat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2790 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_hist_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1445 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtGlue_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1780 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_numel.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3005 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/running_stat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    10234 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_relational_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3957 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_max_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4329 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_randu.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3860 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_SymEigsSolver_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1359 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Glue_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5233 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_symmat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7223 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_norm.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3586 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_unique_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    12651 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mul_syrk.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2850 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_sprandn.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2410 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_orth_null.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2390 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtOp_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3915 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_elem1_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2706 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_repelem_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4355 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_randn.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    49167 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/sp_auxlib_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2162 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_conv.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1219 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_SparseGenMatProd_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1181 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_toeplitz_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2356 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_vectorise_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    13170 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_dot_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8194 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_princomp_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3707 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/diagview_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    19380 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Base_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    26690 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Cube_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3452 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_trimat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4450 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_princomp.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4103 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_htrans_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1869 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_any.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9932 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_trimat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4025 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_GenEigsSolver_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8559 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/running_stat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    34555 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/MapMat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1225 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/GlueCube_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8897 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_conv_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7196 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_var_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1752 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_index_min_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     6739 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sp_minus_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2152 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_cor_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2047 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_princomp_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4648 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_repmat_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3374 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_diagvec_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     7179 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/gmm_diag_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1579 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_shift_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    15254 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_mixed_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8408 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_minus_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2473 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/trimat_helper.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    10257 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/def_blas.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     9947 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/typedef_mat_fixed.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    20246 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eop_aux.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2358 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_vectorise.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1363 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_cond.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3320 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_eigs_sym.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1364 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/wall_clock_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2925 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_nonzeros_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3858 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eOpCube_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2027 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_trunc_log.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    10985 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_times.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2195 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_misc_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3747 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sp_plus_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8852 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_vectorise_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2229 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_EigsSelect.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3291 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_n_unique.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1528 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_dotext_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    15656 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_max_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     6638 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/def_hdf5.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2524 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eOp_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1697 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpGlue_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4487 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_sort.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    22436 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_cube_each_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4137 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_pinv_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1173 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_symmat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1566 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/xvec_htrans_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1497 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_relational_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3638 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/gmm_misc_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3365 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_sqrtmat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     3706 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cumprod_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    89635 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Proxy.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1783 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_rank.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4051 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cx_scalar_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    21581 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/diagview_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5360 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_normalise_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2040 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_qr.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1138 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_repmat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5279 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_min.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     4705 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_zeros.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1698 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_median.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5912 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arrayops_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     6557 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpValProxy_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1152 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_repelem_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     5455 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_normpdf.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1691 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_flip.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    20110 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_strans_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1287 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_shuffle_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2555 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_logmat_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     2595 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_inplace_strans.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1868 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_qz.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8822 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_interp1.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     8602 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_relational.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1860 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_find_unique_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    14914 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/promote_type.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1978 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_median_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1718 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_mvnrnd_bones.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1616 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_roots.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    31181 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eop_core_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)    17293 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_solve_meat.hpp
--rwxrwxr-x   0 davide    (1000) davide    (1000)      526 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/NOTICE.txt
--rwxrwxr-x   0 davide    (1000) davide    (1000)    11560 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/LICENSE.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        8 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/VERSION.txt
--rwxrwxr-x   0 davide    (1000) davide    (1000)    19070 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/armadillo/README.md
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/dll/
--rw-rw-r--   0 davide    (1000) davide    (1000)   526747 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/dll/libblas.dll
--rw-rw-r--   0 davide    (1000) davide    (1000)    25130 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/dll/libblas.lib
--rw-rw-r--   0 davide    (1000) davide    (1000)  7635918 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/dll/liblapack.dll
--rw-rw-r--   0 davide    (1000) davide    (1000)   302302 2022-05-26 15:35:52.000000 rego-1.5.2/src/cypack/dll/liblapack.lib
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2022-05-26 15:35:52.000000 rego-1.5.2/src/rego.egg-info/
--rw-rw-r--   0 davide    (1000) davide    (1000)        1 2022-05-26 15:35:52.000000 rego-1.5.2/src/rego.egg-info/dependency_links.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        1 2022-05-26 15:35:50.000000 rego-1.5.2/src/rego.egg-info/not-zip-safe
--rw-rw-r--   0 davide    (1000) davide    (1000)     2555 2022-05-26 15:35:52.000000 rego-1.5.2/src/rego.egg-info/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      391 2022-05-26 15:35:52.000000 rego-1.5.2/src/rego.egg-info/SOURCES.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       13 2022-05-26 15:35:52.000000 rego-1.5.2/src/rego.egg-info/requires.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       12 2022-05-26 15:35:52.000000 rego-1.5.2/src/rego.egg-info/top_level.txt
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1517 2022-05-26 15:35:19.000000 rego-1.5.2/setup.py
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1142 2022-05-26 15:35:19.000000 rego-1.5.2/README.md
--rwxrwxr-x   0 davide    (1000) davide    (1000)     1485 2022-05-26 15:35:52.000000 rego-1.5.2/setup.cfg
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:28:02.000000 rego-1.6.1/
+-rwxrwxr-x   0 davide    (1000) davide    (1000)      142 2023-08-01 10:27:25.000000 rego-1.6.1/MANIFEST.in
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2545 2023-08-01 10:28:02.000000 rego-1.6.1/PKG-INFO
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1127 2023-08-01 10:27:25.000000 rego-1.6.1/LICENSE
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:28:02.000000 rego-1.6.1/src/
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1795 2023-08-01 10:27:25.000000 rego-1.6.1/src/cypack/functions.h
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/
+-rwxrwxr-x   0 davide    (1000) davide    (1000)      526 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/NOTICE.txt
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5203 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_misc_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3297 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_roots_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1991 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_schur_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2358 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_vectorise.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8023 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_relational_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4834 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_cube_plus.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2455 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_sum_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    89635 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Proxy.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    17293 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_solve_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1226 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_cross.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9700 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/translate_arpack.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1505 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_orth_null_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3291 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_n_unique.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2356 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sum_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1237 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_reverse_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1509 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_hist_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2320 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/GenCube_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4533 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_cube_div.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1211 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_DenseGenMatProd_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1606 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_conv_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1083 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cond_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4273 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/translate_superlu.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11768 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_SymEigsSolver_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1349 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_SparseGenMatProd_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    27214 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_max_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3520 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_eigs_gen.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2114 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/xvec_htrans_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1493 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_atan2_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1168 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_cross_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7185 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Gen_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9582 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_var_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2287 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eGlue_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2500 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_schur.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2902 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eOpCube_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1594 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpGlue_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2566 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/injector_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2524 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eOp_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2071 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eGlueCube_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7523 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_cube_relational.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8408 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_minus_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1574 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_trapz_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1453 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_intersect_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5681 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_atan2_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3156 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_fft2.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3638 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/gmm_misc_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4025 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_GenEigsSolver_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2221 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_pinv.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2134 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/typedef_elem_check.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4103 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_htrans_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    10732 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/def_arpack.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    47137 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eglue_core_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1134 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_normalise_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4176 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_config.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1345 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_cx_attrib.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3783 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_dotext_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2103 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_prod.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    26690 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Cube_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    34646 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_times_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5465 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_max_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3005 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/running_stat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3695 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cumsum_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    14274 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_htrans_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    65539 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/gmm_diag_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    24709 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpProxy.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7192 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eop_core_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    12770 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mul_gemm.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    49167 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/sp_auxlib_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1194 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/compiler_extra.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3320 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_eigs_sym.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1248 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_polyval.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    97754 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4094 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_kron_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    26376 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/traits.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3858 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eOpCube_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4538 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_eig_sym.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11190 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_forward.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1266 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpToDOp_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2399 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/podarray_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4705 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_zeros.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2285 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_cross_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    15975 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/field_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2595 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_inplace_strans.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2002 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/cond_rel_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    61755 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/field_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2704 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtOpCube_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5430 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_shuffle_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2062 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_shift.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4833 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_cube_each_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    13125 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/translate_atlas.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2691 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/BaseCube_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2850 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_sprandn.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)      989 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_sum_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4329 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_randu.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2382 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_symmat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4051 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cx_scalar_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5492 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_spsolve.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7365 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_wishrnd_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2278 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpToDOp_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1951 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_polyval_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2816 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_sprandu.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1346 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_spones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    20201 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_norm_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    12474 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_misc.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1566 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/xvec_htrans_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4322 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_reshape.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    35544 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpMat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1870 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtSpOp_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1162 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_elem_helper_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    14147 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_merge_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7405 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    25327 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpMat_iterators_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    10985 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_times.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2763 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_sum.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    10296 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_join_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3643 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_hess.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2027 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_trunc_log.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5866 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/memory.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3161 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_randperm.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2836 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_join_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3786 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eGlue_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4487 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_sort.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    19223 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_elem2_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2442 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_inplace_trans.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1114 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cov_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1426 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_trapz.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3129 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/gmm_misc_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    14914 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/promote_type.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1329 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_roots_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1345 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_DenseGenMatProd_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    13014 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mul_gemv.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    15762 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/diagmat_proxy.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     6009 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_clamp_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2047 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_princomp_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)   106690 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/def_lapack.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5103 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/upgrade_val.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    32307 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpSubview_iterators_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11803 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_cube_slices_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    19411 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arrayops_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4160 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eGlueCube_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    16131 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpSubview_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1225 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/GlueCube_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2628 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/hdf5_name.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    16312 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_trace.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3856 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_rng_cxx98.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9148 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_schur_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1458 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_chi2rnd_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1533 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_toeplitz.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2197 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_diagmat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1184 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_range_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1994 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_hist.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    18533 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_times_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3165 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_log_det.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4450 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_princomp.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2704 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SizeMat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9154 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_svds.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1656 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_kron_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7223 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_norm.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1723 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/GenSpecialiser.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1799 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_TridiagEigen_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3860 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_SymEigsSolver_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    30357 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_each_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2815 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_cube_times.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1478 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_version.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5550 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_shift_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1632 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_vectorise_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    31865 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/debug.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2729 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_mvnrnd.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2491 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_chol_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2352 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sqrtmat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3854 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_relational_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1323 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_unique.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4648 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_repmat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5655 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/running_stat_vec_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3959 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_min_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    35001 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Col_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1323 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_repmat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3971 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_chi2rnd_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1868 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_qz.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2040 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_qr.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3717 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_chi2rnd.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4433 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpBase_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4054 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_eig_gen.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3543 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_elem2_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    12603 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_logmat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    10257 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/def_blas.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2521 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtOp_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1046 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_stddev_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1139 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_chol_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1016 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_toeplitz_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5912 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arrayops_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1602 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_flip_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1328 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_kron_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2110 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_speye.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8897 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_conv_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1581 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_find_unique.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1132 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_trimat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3516 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_symmat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1293 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cumprod_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2365 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtOpCube_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5293 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_times_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2555 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_logmat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1433 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtSpGlue_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     6978 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/gmm_full_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3486 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_logmat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4694 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_size.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3710 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_sort_index.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    23212 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_accu.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1473 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtGlueCube_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2152 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_cor_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11453 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_misc_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1363 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_cond.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3504 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_kron_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2554 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_vectorise_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2162 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_conv.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3020 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eglue_core_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3112 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_TridiagEigen_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1191 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_symmat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1839 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_clamp_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2961 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_fft.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    12134 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_plus.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1149 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_repmat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4995 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_diff_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1780 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_numel.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2539 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_var_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    15254 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_mixed_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3395 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_intersect_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2622 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_strans.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7012 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_dot.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1768 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_plus_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3869 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_strans_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    12332 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cx_scalar_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3407 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_trimat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2473 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/trimat_helper.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    22436 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_cube_each_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2125 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/access.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)   178262 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/auxlib_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1684 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_histc.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1528 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_dotext_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    15000 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpBase_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3844 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/csv_name.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11015 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/injector_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1698 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_median.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2269 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_lu.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5410 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_randi.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2354 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_reverse_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3452 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_trimat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3586 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_unique_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1882 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_reverse.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4150 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_orth_null_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    81970 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/translate_lapack.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4420 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sort_index_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3035 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_find_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    67945 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/gmm_full_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3275 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_ostream_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7051 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_relational_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1752 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_index_max_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5279 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_max.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    17717 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/compiler_setup.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2444 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_resize.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1216 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_cov_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1377 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/include_atlas.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5360 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_normalise_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3493 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_relational_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    19380 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Base_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    21404 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    20246 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eop_aux.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2508 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_DoubleShiftQR_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5279 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_min.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1450 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_diagvec.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1333 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_powmat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1788 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_max_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2841 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/OpCube_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1616 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_roots.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9985 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_index_max_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3156 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_index_min.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1998 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_wishrnd_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11286 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/config.hpp.cmake
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7196 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_var_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11543 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_rng.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    12428 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sum_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1825 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_unique_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1650 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_shuffle.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)   112626 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/diskio_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3963 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/unwrap_spmat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9015 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_reshape_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4316 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_prod_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1216 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_cor_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2409 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_kron.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1554 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_kmeans.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3176 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_cube_schur.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3733 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_trapz_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2523 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_normalise.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9932 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_trimat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3143 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_elem_helper_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     6523 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_max_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1181 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_toeplitz_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3966 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/typedef_mat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1152 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_repelem_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4867 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_rng_cxx11.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1359 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_diagvec_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2132 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_any_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1718 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_mvnrnd_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8610 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_mean_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11433 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_all_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5512 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_expmat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    31181 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eop_core_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    14416 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/running_stat_vec_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1445 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtGlue_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2923 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/strip.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4214 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_wishrnd.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2304 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_expmat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1181 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_reverse_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3543 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spdiagview_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2234 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_range_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1359 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Glue_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1321 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_merge_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1173 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_symmat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2113 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtSpOp_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1331 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_nonzeros_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8194 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_princomp_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7304 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_find.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1527 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_cor.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2768 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_rel_comparators.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8559 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/running_stat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1723 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_inv_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4137 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_pinv_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    34555 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/MapMat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3299 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SizeCube_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1313 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_normalise_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3334 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_repmat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    18630 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/auxlib_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2005 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_chol.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1600 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_static_check.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2037 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3957 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_max_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1869 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_all.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1691 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_flip.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8241 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpCol_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     6993 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/constants_old.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5112 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/typedef_elem.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2186 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Glue_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2097 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_diagmat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1736 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_cumsum.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1541 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SizeCube_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    21615 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spdiagview_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8959 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpRow_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1525 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_cov.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    17558 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_conv_to.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2651 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpValProxy_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1914 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpOp_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5233 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_symmat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    13170 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_dot_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1899 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mp_misc.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    10585 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_diagmat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1633 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/CubeToMatOp_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1437 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/GlueCube_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1273 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_prod_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2231 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_eps.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1114 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cor_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11090 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_join.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1860 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_find_unique_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2356 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_vectorise_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3915 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_elem1_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3035 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cor_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     6523 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_min_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1691 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_min_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3546 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_resize_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    34942 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Row_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    21305 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_elem.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    44133 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Mat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1869 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_any.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3372 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_polyfit_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2637 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cov_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1565 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_htrans_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1244 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_nonzeros.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     6557 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpValProxy_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7031 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/podarray_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1175 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_pinv_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    14171 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_approx_equal.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    64647 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_cube_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2002 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_fft_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1697 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpGlue_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4787 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sort_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2344 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_max_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2132 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_all_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3257 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sort_index_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1783 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_rank.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2792 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cond_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4444 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/sp_auxlib_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5925 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_each_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3707 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/diagview_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1493 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_hypot_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2725 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_toeplitz_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11062 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sqrtmat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    15573 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_find_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4355 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_randn.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1923 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_stddev.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1295 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/cond_rel_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1294 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/CubeToMatOp_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2896 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_var.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    72198 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/unwrap.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    14153 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_mean_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3374 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_diagvec_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3990 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_reverse_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11396 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_as_scalar.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3377 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_cube_slices_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    22986 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/ProxyCube.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2828 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_times_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    10234 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_relational_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1904 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_trunc_exp.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2706 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_repelem_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9571 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/band_helper.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7793 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/MapMat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2617 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Op_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1496 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_htrans_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2390 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtOp_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2746 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_clamp.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3019 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_mixed_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1691 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_max_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1537 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtGlueCube_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1138 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_repmat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1106 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_hist_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1976 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_minus_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1287 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_shuffle_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    33981 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpSubview_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3365 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_sqrtmat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5402 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_solve_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1747 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_cumprod.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8867 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_cube_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1742 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_polyfit.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3111 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_ostream.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)      815 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/compiler_setup_post.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8197 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_interp2.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4850 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_mvnrnd_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1511 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_polyfit_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5459 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_min_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1978 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_median_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)   122818 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Cube_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4436 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_inv_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2174 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_trimat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1673 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/xtrans_mat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    10351 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/translate_blas.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)   151041 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpMat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1296 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_polyval_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2229 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_EigsSelect.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    18866 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_ostream_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3041 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_eig_pair.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     6065 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Base_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1906 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_toeplitz_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4559 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_histc_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1497 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_relational_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1674 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpOp_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5525 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_log_normpdf.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1293 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_diff_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2195 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_misc_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1704 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sort_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    20110 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_strans_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7179 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/gmm_diag_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1687 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_diff.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3610 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_det.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2570 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sp_minus_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    10494 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_any_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9043 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_schur.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     6262 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_hist_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1724 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtGlue_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1734 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_quantile_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     6739 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sp_minus_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9829 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_solve.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3830 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_ones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2790 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_hist_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3247 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_mean_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    21581 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/diagview_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9996 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/restrictors.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11121 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_str.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3747 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sp_plus_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1330 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_repelem.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4113 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_hypot_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5212 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_SortEigenvalue.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2925 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_nonzeros_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    12376 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_field_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1651 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_reshape_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1620 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtSpGlue_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2517 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/OpCube_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1774 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_diagmat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3272 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_field_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4704 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_svd.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2054 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_cov_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    22905 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_elem1_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5937 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_normcdf.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5327 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/GenCube_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     6528 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/sympd_helper.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1605 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_intersect.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4191 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2739 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpCol_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11139 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/constants.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1739 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_quantile.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1989 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_trans.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1292 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/distr_param.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3030 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_find_unique_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)   200436 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Mat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2013 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_var_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1562 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_range.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3575 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_dot_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9947 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/typedef_mat_fixed.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9455 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_DoubleShiftQR_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3156 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_index_max.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    10728 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mul_gemm_mixed.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1421 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/include_hdf5.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     6638 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/def_hdf5.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2604 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_syl_lyap.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2371 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/wall_clock_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1752 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_index_min_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1104 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_resize_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3349 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_norm_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2344 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_min_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    12651 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mul_syrk.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8822 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_interp1.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5705 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_regspace.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1743 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_affmul_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1579 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_shift_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2133 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Op_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5617 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_quantile_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9985 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_index_min_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4068 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/def_superlu.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11657 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_join_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1219 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_SparseGenMatProd_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    16374 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_min_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1506 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_histc_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1474 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_strans_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    10419 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_diagmat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    13320 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/diskio_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     6611 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_randg.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7440 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/BaseCube_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2428 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Gen_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3034 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eOp_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1364 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/wall_clock_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    10452 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Col_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    15656 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_max_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2410 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_orth_null.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9041 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/def_atlas.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1647 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sp_plus_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1788 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_min_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11016 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fft_engine.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8852 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_vectorise_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8945 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_misc_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2635 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_join_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2752 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_mean.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3420 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_normalise_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8602 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_relational.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    20647 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/hdf5_misc.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9903 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/include_superlu.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2648 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_stddev_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1458 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_expmat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11776 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_GenEigsSolver_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2250 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/unwrap_cube.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2547 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    12570 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_minus.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2782 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_eye.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8752 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_trig.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     6062 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_flip_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    13647 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mul_herk.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3706 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cumprod_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8483 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_div.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5455 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_normpdf.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8593 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_fft_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     4772 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_cube_minus.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1288 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cumsum_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11241 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_median_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1989 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/xtrans_mat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    12978 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_affmul_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1650 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/span.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3110 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_strans_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    10441 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Row_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    13212 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_cmath.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11193 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/config.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7737 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_inv.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2563 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_powmat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7250 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_plus_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    27217 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_min_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1479 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SizeMat_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2736 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpRow_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5282 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_powmat_meat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2257 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_mean_bones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    30011 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/include/armadillo
+-rwxrwxr-x   0 davide    (1000) davide    (1000)        8 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/VERSION.txt
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11560 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/LICENSE.txt
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    19070 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/armadillo/README.md
+-rwxrwxr-x   0 davide    (1000) davide    (1000)      912 2023-08-01 10:27:25.000000 rego-1.6.1/src/cypack/generate_doc.py
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8756 2023-08-01 10:27:25.000000 rego-1.6.1/src/cypack/rego.pyx
+-rwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:27:25.000000 rego-1.6.1/src/cypack/__init__.py
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    56819 2023-08-01 10:27:25.000000 rego-1.6.1/src/cypack/functions.cpp
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/
+-rwxrwxr-x   0 davide    (1000) davide    (1000)      208 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/NOTICE.txt
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11357 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/LICENSE
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11427 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/cg.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11188 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/pso.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9507 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/bfgs.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     8051 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/gd.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     9955 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/lbfgs.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    12830 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/nm.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    10573 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/pso_dv.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    10693 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/de.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     6505 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/newton.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    15780 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/de_prmm.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7453 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/gd.ipp
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7261 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/error_reporting.ipp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3024 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/optim_options.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1073 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/unit_vec.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1048 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/unit_vec.ipp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2155 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/numerical_gradient.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1102 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/misc.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2166 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/optim_matdefs.hpp
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1137 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/inv.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1553 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/randu.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1924 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/randn.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1477 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/reset_negative_values.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1112 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/exp.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1275 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/set_size.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1513 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/max.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1167 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/hadamard.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1119 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/pow.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1656 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/abs_max.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1219 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/accu.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1399 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/zeros.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1459 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/min.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1227 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/is_finite.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1169 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/solve.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1700 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/norm.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1337 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/get_sort_index.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1140 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/dot.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1269 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/transpose.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1609 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/access.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1139 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/size.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1140 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/abs.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1088 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/eval.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1467 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/sum.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1230 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/index_min.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1097 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/ncol.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1145 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/eye.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1792 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/randi.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1112 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/cos.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1121 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/as_scalar.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1162 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/diagmat.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1111 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/cout.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1421 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/array_div.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1117 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/sqrt.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1171 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/diagvec.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1116 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/endl.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1143 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/array_add.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1112 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/log.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1146 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/array_mult.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1389 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/ones.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     5491 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/optim_structs.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    38092 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/optim_trace.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1919 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/determine_bounds_type.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3024 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/error_reporting.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     2007 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/jacobian_adjust.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3958 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/transform_vals.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     3856 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/misc/numerical_hessian.hpp
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/constrained/
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     7773 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/constrained/sumt.hpp
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/zeros/
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    16983 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/zeros/broyden_df.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    13567 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/zeros/broyden.hpp
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/line_search/
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    11032 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/line_search/more_thuente.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1876 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/header_only_version/optim.hpp
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    12666 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/optim-master/README.md
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/dll/
+-rwxrwxr-x   0 davide    (1000) davide    (1000)    25130 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/dll/libblas.lib
+-rwxrwxr-x   0 davide    (1000) davide    (1000)  7635918 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/dll/liblapack.dll
+-rwxrwxr-x   0 davide    (1000) davide    (1000)   526747 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/dll/libblas.dll
+-rwxrwxr-x   0 davide    (1000) davide    (1000)   302302 2023-08-01 10:28:02.000000 rego-1.6.1/src/cypack/dll/liblapack.lib
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-08-01 10:28:02.000000 rego-1.6.1/src/rego.egg-info/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        1 2023-08-01 10:28:01.000000 rego-1.6.1/src/rego.egg-info/not-zip-safe
+-rw-rw-r--   0 davide    (1000) davide    (1000)      371 2023-08-01 10:28:02.000000 rego-1.6.1/src/rego.egg-info/SOURCES.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       13 2023-08-01 10:28:02.000000 rego-1.6.1/src/rego.egg-info/requires.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2545 2023-08-01 10:28:01.000000 rego-1.6.1/src/rego.egg-info/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)       12 2023-08-01 10:28:02.000000 rego-1.6.1/src/rego.egg-info/top_level.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        1 2023-08-01 10:28:01.000000 rego-1.6.1/src/rego.egg-info/dependency_links.txt
+-rwxrwxr-x   0 davide    (1000) davide    (1000)      115 2023-08-01 10:27:25.000000 rego-1.6.1/pyproject.toml
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1475 2023-08-01 10:28:02.000000 rego-1.6.1/setup.cfg
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1142 2023-08-01 10:27:25.000000 rego-1.6.1/README.md
+-rwxrwxr-x   0 davide    (1000) davide    (1000)     1552 2023-08-01 10:27:25.000000 rego-1.6.1/setup.py
```

### Comparing `rego-1.5.2/PKG-INFO` & `rego-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: rego
-Version: 1.5.2
+Version: 1.6.1
 Summary: Automatic Time Series Forecasting and Missing Value Imputation
-Home-page: https://channelattribution.io/docs/rego
+Home-page: https://channelattribution.io/rego
 Author: Davide Altomare, David Loris
 Author-email: info@channelattribution.io
 License: UNKNOWN
-Project-URL: Documentation, https://channelattribution.io/docs/rego
+Project-URL: Documentation, https://channelattribution.io/rego
 Project-URL: Code, https://github.com/DavideAltomare/rego
 Project-URL: Issue tracker, https://github.com/DavideAltomare/rego/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rego-1.5.2/LICENSE` & `rego-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/LICENSE` & `rego-1.6.1/src/cypack/optim-master/LICENSE`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/README.md` & `rego-1.6.1/src/cypack/optim-master/README.md`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/line_search/more_thuente.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/line_search/more_thuente.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/pso_dv.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/pso_dv.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/gd.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/gd.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/gd.ipp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/gd.ipp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/lbfgs.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/lbfgs.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/de_prmm.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/de_prmm.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/newton.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/newton.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/cg.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/cg.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/pso.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/pso.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/nm.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/nm.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/bfgs.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/bfgs.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/unconstrained/de.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/unconstrained/de.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/zeros/broyden_df.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/zeros/broyden_df.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/zeros/broyden.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/zeros/broyden.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/optim.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/optim.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/constrained/sumt.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/constrained/sumt.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/optim_trace.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/optim_trace.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/numerical_gradient.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/numerical_gradient.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/reset_negative_values.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/reset_negative_values.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/max.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/max.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/dot.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/dot.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/randi.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/randi.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/exp.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/exp.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/size.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/size.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/access.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/access.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/cos.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/cos.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/abs_max.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/abs_max.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/array_add.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/array_add.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/accu.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/accu.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/array_div.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/array_div.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/transpose.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/transpose.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/get_sort_index.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/get_sort_index.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/randu.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/randu.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/cout.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/cout.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/min.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/min.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/pow.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/pow.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/array_mult.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/array_mult.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/inv.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/inv.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/diagmat.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/diagmat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/randn.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/randn.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/eval.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/eval.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/sum.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/sum.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/ncol.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/ncol.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/sqrt.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/sqrt.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/abs.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/abs.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/solve.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/solve.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/zeros.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/zeros.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/set_size.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/set_size.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/log.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/log.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/index_min.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/index_min.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/endl.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/endl.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/as_scalar.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/as_scalar.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/eye.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/eye.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/hadamard.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/hadamard.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/is_finite.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/is_finite.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/norm.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/norm.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/ones.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/ones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/matrix_ops/diagvec.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/matrix_ops/diagvec.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/jacobian_adjust.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/jacobian_adjust.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/optim_options.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/optim_options.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/error_reporting.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/error_reporting.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/transform_vals.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/transform_vals.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/misc.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/misc.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/unit_vec.ipp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/unit_vec.ipp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/optim_structs.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/optim_structs.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/error_reporting.ipp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/error_reporting.ipp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/unit_vec.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/unit_vec.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/determine_bounds_type.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/determine_bounds_type.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/numerical_hessian.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/numerical_hessian.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/optim-master/header_only_version/misc/optim_matdefs.hpp` & `rego-1.6.1/src/cypack/optim-master/header_only_version/misc/optim_matdefs.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/rego.pyx` & `rego-1.6.1/src/cypack/rego.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -8,43 +8,43 @@
 from libcpp.string cimport string
 from libcpp.vector cimport vector
 from libcpp.list cimport list
 from libcpp.pair cimport pair
 import pandas as pd
 
 
-__version="1.5.2"
+__version="1.6.1"
 
 print("Visit https://channelattribution.io/docs/rego for more information about rego")
 print("Version: " + str(__version))
     
 #vector[vector[vector[vector[double]]]]
 #pair < vec3, pair < vec2, vec4 > >
 
 
     
 cdef extern from "functions.h":
 
-    pair[vector[vector[vector[double]]],pair[vector[vector[double]],vector[vector[vector[vector[double]]]]]] regpred_py(vector[vector[double]]& Y, double from_lag, double max_lag, double alpha, unsigned long int nsim, int flg_print, string direction, string loss_function, int pred_only, int flg_const, int flg_diff, vector[vector[vector[vector[double]]]]& vmodels);
+    pair[vector[vector[vector[double]]],pair[vector[vector[double]],vector[vector[vector[vector[double]]]]]] regpred_py(vector[vector[double]]& Y, double from_lag, double max_lag, double alpha, unsigned long int nsim, int flg_print, string direction, string loss_function, int pred_only, int flg_const, int flg_diff, double h_c, vector[vector[vector[vector[double]]]]& vmodels);
 
 
-def __regpred_py(vector[vector[double]] Y, double from_lag, double max_lag, double alpha, unsigned long int nsim, int flg_print, string direction, string loss_function, int pred_only, int flg_const, int flg_diff, vector[vector[vector[vector[double]]]] vmodels):
-    return(regpred_py(Y,from_lag,max_lag,alpha,nsim,flg_print,direction,loss_function,pred_only,flg_const,flg_diff,vmodels))
+def __regpred_py(vector[vector[double]] Y, double from_lag, double max_lag, double alpha, unsigned long int nsim, int flg_print, string direction, string loss_function, int pred_only, int flg_const, int flg_diff, double h_c, vector[vector[vector[vector[double]]]] vmodels):
+    return(regpred_py(Y,from_lag,max_lag,alpha,nsim,flg_print,direction,loss_function,pred_only,flg_const,flg_diff,h_c,vmodels))
 
 
 #start documentation
 
 """
 
 **Automatic time series forecasting and missing values imputation.**
 rego is a machine learning algorithm for predicting and imputing time series. It can automatically set all the parameters needed, thus in the minimal configuration it only requires the target variable and the dependent variables if present. It can address large problems with hundreds or thousands of dependent variables and problems in which the number of dependent variables is greater than the number of observations. Moreover it can be used not only for time series but also for any other real valued target variable. The algorithm implemented includes a Bayesian stochastic search methodology for model selection and a robust estimation based on bootstrapping. rego is fast because all the code is C++.
 
 """
         
-def regpred(Data, from_lag=1, max_lag="auto", alpha=0.05, nsim=1000, flg_print=1, direction="->", loss_function="MSE", flg_const=True, flg_diff=False, model=None):
+def regpred(Data, from_lag=1, max_lag="auto", alpha=0.05, nsim=1000, flg_print=1, direction="->", flg_const=True, flg_diff=False, model=None):
 
     '''
     
     Parameters
     ----------
     Data : DataFrame
         data.frame containing target variable at first column and regressors if present from second to last column.
@@ -56,16 +56,14 @@
         significance level for the confidence interval produced around predictions. If 0.05 then the algorithm will calculate a 95\% confidence interval around predictions.
     nsim : int
         number of bootstrap replications used for producing confidence interval around predictions.
     flg_print : bool, optional, default None
         if 1 some information during the evaluation will be printed.
     direction : string, default "->"
         if "->" then only a forward prediction will be executed, if "<-" then only a backward prediction will be executed, if "<->" then both a forward than a backward prediction will be executed if possible. For imputing missing values is convenient to leave default "<->".        
-    loss_function : string, default "MSE"
-        if "MAE" then mean absolute error is used as penalty function in regressions, if "MSE" then mean squared error is used as penalty function in regressions
     flg_const : bool, default True
         if True then a constant is included into the model
     flg_diff : bool, default False
         if True and no regressor is present then if the target variable exhibits a trend, it is one-step differentiated up to two times
     model: list
         estimated models from a previous train to be used in new data prediction without retraining
 
@@ -100,14 +98,18 @@
     >>> res=regpred(Data, max_lag=None)
 
     print final prediction 
     
     >>> print(res['predictions'])
 
     '''
+
+    loss_function="MSE" 
+    h=None 
+
     if (from_lag < 1):
        raise NameError("from_lag must be > 1")
 
     if max_lag != None:
         if max_lag!="auto":
             max_lag=float(max_lag)
             if (max_lag < 0):
@@ -129,14 +131,20 @@
        raise NameError("loss_function must be 'MAE' or 'MSE'")
        
     if (flg_const not in [0,1]):
        raise NameError("flg_const must be 0 or 1")
        
     if (flg_diff not in [0,1]):
        raise NameError("flg_diff must be 0 or 1")
+
+    if h != None:
+        if (type(h) != int):
+            raise NameError("flg_diff must be 0 or 1")
+    else:
+        h=-1
     
     if (max_lag == None):
         max_lag=0
 
     if (max_lag == "auto"):
         max_lag=-1
     
@@ -159,15 +167,15 @@
     if(str(type(Data))!="<class 'pandas.core.frame.DataFrame'>"):
         raise NameError("Data must be a Dataframe'")
     
     cols_Y=[str(x) for x in Data.columns.tolist()]
     Y=Data.to_numpy()
     del Data
                     
-    res0=__regpred_py(Y, from_lag, max_lag, alpha, nsim, flg_print, direction.encode('utf-8'), loss_function.encode('utf-8'), pred_only, flg_const, flg_diff, model)
+    res0=__regpred_py(Y, from_lag, max_lag, alpha, nsim, flg_print, direction.encode('utf-8'), loss_function.encode('utf-8'), pred_only, flg_const, flg_diff, h, model)
     
     prediction=pd.DataFrame(res0[0][0])
     prediction.columns=['real','fitted','lower_bound','predicted','upper_bound']
     del prediction["fitted"]
     
     if direction=="<->":
         fw_prediction=pd.DataFrame(res0[0][1])
```

### Comparing `rego-1.5.2/src/cypack/functions.cpp` & `rego-1.6.1/src/cypack/functions.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -27,20 +27,24 @@
 #include <list>
 #include <limits> 
 #include <functional>
 #include <ctime>
 
 
 #define OPTIM_ENABLE_ARMA_WRAPPERS
-#ifdef language_py
-  #ifdef _WIN32
-    #define ARMA_DONT_USE_LAPACK
-    #define ARMA_DONT_USE_BLAS
-  #endif
-#endif
+
+// #ifdef language_py
+//   #ifdef _WIN32
+//     #define ARMA_DONT_USE_LAPACK
+//     #define ARMA_DONT_USE_BLAS
+//   #endif
+// #endif
+#define ARMA_DONT_USE_LAPACK
+#define ARMA_DONT_USE_BLAS
+
 #define ARMA_USE_CXX11
 #define ARMA_64BIT_WORD
 #define ARMA_DONT_PRINT_ERRORS
 
 #include <armadillo>
 #include <optim.hpp>
 
@@ -139,43 +143,31 @@
     vv(k)=pow((*v)(k),(*w)(k));
    }
 
  return vv;
 
 }
 
-mat Cholesky(mat* M)
-{
-    double n=(*M).n_rows;
-    mat lower(n,n);
- 
-    // Decomposing a matrix into Lower Triangular
-    for (uli i = 0; i < n; i++) {
-        for (uli j = 0; j <= i; j++) {
-            uli sum = 0;
- 
-            if (j == i) // summation for diagonals
-            {
-                for (uli k = 0; k < j; k++){
-                    sum += pow(lower(j,k), 2);
-                    lower(j,j) = sqrt((*M)(j,j) - sum);
-                }
-            } else {
- 
-                // Evaluating L(i, j) using L(j, j)
-                for (uli k = 0; k < j; k++){
-                    sum += (lower(i,k) * lower(j,k));
-                    lower(i,j) = ((*M)(i,j) - sum) / lower(j,j);
-                }
-            }
+
+mat Cholesky(mat* input) {
+    double n=(*input).n_rows;
+    mat result(n,n);
+    for (size_t i = 0; i < n; ++i) {
+        for (size_t k = 0; k < i; ++k) {
+            double value = (*input)(i, k);
+            for (size_t j = 0; j < k; ++j)
+                value -= result(i, j) * result(k, j);
+            result(i, k) = value/result(k, k);
         }
+        double value = (*input)(i, i);
+        for (size_t j = 0; j < i; ++j)
+            value -= result(i, j) * result(i, j);
+        result(i, i) = std::sqrt(value);
     }
-
-    return(lower);
- 
+    return result;
 }
 
 
 vec forward_sub(mat* L, vec* b)
 {
     /*x = forward_sub(L, b) is the solution to L x = b
        L must be a lower-triangular matrix
@@ -215,19 +207,20 @@
     }
 
     return(x);
 
 }
 
 vec solve0(mat* A, vec* b){
- 
+
   mat L=Cholesky(A);
   mat Lt=trans(L);
 
   vec vy=forward_sub(&L,b);
+
   vec vx=back_sub(&Lt, &vy);
   
   return(vx);
 
 }
 
 vec solve_linear(mat* A, vec* b){
@@ -388,15 +381,14 @@
  x=lfactorial(2*h)+i*log(sigma)-lfactorial(i)+(2*h-2*i)*log(abs(mu))-lfactorial(2*h-2*i);
 
  return x;
 
 } //end function
 
 
-
 double log_FBF_Ga_Gb(vec* G_a, vec* G_b, uli edge, mat* edges, mat* YtY, uli add, double n, double h)
 {
   
   uli e1, e2, iwi;
   double i, p, b, S2, mu, sigma, logS2, ilogS2, logHhi, ilog4, log_num1, log_den1, log_w_1, log_num0i0, log_den0i0, log_w_0, log_FBF_unpasso;
   vec V1, V2, G1, V11, pa1, pa0, betah, vv(1), z1;
   uvec iw, ipa1;
@@ -423,23 +415,31 @@
 
   yty=(*YtY)(e2,e2);
     
   // //calcolo w1
    
   vv(0)=e2; Xty=conv_to<vec>::from(sub_mat(YtY,pa1,vv));
   XtX=sub_mat(YtY,pa1,pa1);
-  betah=solve_linear(&XtX,&Xty);
+  if(XtX.n_cols>1){
+   betah=solve_linear(&XtX,&Xty);
+  }else{
+   betah=conv_to<double>::from(Xty)/conv_to<double>::from(XtX);
+  }
 
   S2=conv_to<double>::from(yty-(trans(Xty)*betah));
   
   iw=find(pa1==e1); mu=conv_to<double>::from(betah.elem(iw));
   iwi=conv_to<uli>::from(iw); 
   z1=zeros<vec>(pa1.n_elem);
   z1(iwi)=1;
-  z1=solve_linear(&XtX,&z1);
+  if(XtX.n_cols>1){
+    z1=solve_linear(&XtX,&z1);
+  }else{
+    z1=conv_to<double>::from(z1)/conv_to<double>::from(XtX);
+  }
   
   sigma=conv_to<double>::from(z1.elem(iw));
   
   if(S2>0){
    log_w_1=(-n*(1-b)/2)*log(datum::pi*b*S2);
    logS2=log(S2);
    log_num1=-datum::inf;
@@ -468,16 +468,20 @@
   log_num0i0=lgamma((n-p)/2);
   log_den0i0=lgamma((n*b-p)/2);
 
   if(p==0){S2=conv_to<double>::from(yty);}
   else{
    vv(0)=e2; Xty=conv_to<vec>::from(sub_mat(YtY,pa0,vv));
    XtX=sub_mat(YtY,pa0,pa0);
-   betah=solve_linear(&XtX,&Xty); 
-
+   if(XtX.n_cols>1){
+    betah=solve_linear(&XtX,&Xty);
+   }else{
+    betah=conv_to<double>::from(Xty)/conv_to<double>::from(XtX); 
+   }
+ 
    S2=conv_to<double>::from(yty-(trans(Xty)*betah));
   }
 
   if(S2>0){
    log_w_0=(-(n*(1-b)/2))*log(datum::pi*b*S2)+log_num0i0-log_den0i0;
   }else{
    log_w_0=datum::inf;
@@ -494,15 +498,14 @@
 
   return log_FBF_unpasso;
 
 } // end function
 
 
 
-
 field<mat> FBF_heart(double nt, mat* YtY, vec* vG_base, double lcv, vec* vlcv, mat* edges, double n_tot_mod, double C, double maxne, double h, bool univariate)
 {
     
    uli t, add, edge, imq, limodR, s;
    double ltree, lM, sum_log_FBF, log_FBF_G, log_pi_G, log_num_MP_G, sum_log_RSMP, n_mod_r, log_FBF_t, log_FBF1;
    vec M_log_FBF, log_num_MP, log_sume, G, imod_R, M_log_RSMP, pRSMP, mov, vlM, qh, G_t, M_q, M_P;
    uvec iw;
@@ -716,15 +719,15 @@
  for(rr=1; rr<=rrmax; rr++){
   Mlogbin_sum=log_add(Mlogbin_sum,lchoose(lcv,rr));   
  }
  
  n_tot_mod_c=std::min(Mlogbin_sum,log(n_tot_mod_c));
  n_tot_mod_c=round(exp(n_tot_mod_c)); 
 
- YtY=(*Corr_c)*nobs_c;
+ YtY=(*Corr_c)*(nobs_c-1);
  heartRes=FBF_heart(nobs_c, &YtY, &vG_base, lcv, &vlcv, &edges, n_tot_mod_c, C_c, maxne, h_c, univariate);
  
  return(heartRes);
 
 } // end function
 
 
@@ -1037,15 +1040,15 @@
  Col<uli> vars_ar_idx; 
  vec logs_FBF_x;
  vec logs_FBF_ar;
  uli odiff;
  
 };
 
-str_out_uni_select model_univariate_selection(mat* Y, double from_lag, double max_lag, bool flg_diff){
+str_out_uni_select model_univariate_selection(mat* Y, double from_lag, double max_lag, bool flg_diff, double h_c){
 
   str_out_uni_select str_out;
   Col<uli> vretard;
   uli odiff=0;
   
   if((max_lag!=0) || (((*Y).n_cols-1)>0)){
     
@@ -1077,23 +1080,29 @@
     vec log_FBF_ar;
     
     if(from_lag<=max_lag){
     
       if(max_lag>0){
        vretard=linspace<Col<uli>>((uli)from_lag,(uli)max_lag,(uli)(max_lag-from_lag+1));
       }
-  
+    
       double nx=(*Y).n_cols-1;
       double nretard=vretard.n_rows;
       double nvars=nx+nretard;
       
-      double h_c=1; 
-      if(nvars>50){
-       h_c=2; 
-      } 
+      if(h_c==-1){
+       h_c=0; 
+       if(nvars>3){
+        h_c=1; 
+       } 
+       if(nvars>50){
+        h_c=2; 
+       } 
+      }
+
       double n_tot_mod_c=nvars*100;
       double C_c=0.01;
       double threshold; 
       
       str_input tab_input;
       field<mat> res;
     
@@ -1145,14 +1154,15 @@
         //x = randu<vec>(nr,1);
         for(uli k=0; k<nr; ++k){
           x(k)=distribution(gen);
         }
         
         YtY(1,0)=as_scalar(cor(y,x));
         YtY(0,1)=YtY(1,0);
+        YtY=YtY*(nr-1);
         
         v_log_FBF(j)=log_FBF_Ga_Gb(&G_a, &G_b, edge, &edges, &YtY, add, nr, h_c);
         
       }
       
       uli nth=(uli) (qt*v_log_FBF.size());
       v_log_FBF=sort(v_log_FBF);
@@ -1170,15 +1180,15 @@
         M_log_FBF_x.set_size(nx,3);
         
         for(uli j=0; j<nx; ++j){
           
           MY.col(1)=(*Y).col(j+1);
           MY1=MY.rows(find_finite(sum(MY,1)));
           nr=MY1.n_rows;
-          YtY=cor(MY1);
+          YtY=cor(MY1)*(nr-1);
           
           M_log_FBF_x(j,0)=0;
           M_log_FBF_x(j,1)=j+1;
           M_log_FBF_x(j,2)=log_FBF_Ga_Gb(&G_a, &G_b, edge, &edges, &YtY, add, nr, h_c);
           
         }
         
@@ -1195,15 +1205,15 @@
           mat Y0;
           
           while(((fbf-threshold)>0) & (odiff<2)){
             MY.col(0)=(*Y).col(0);
             MY.col(1)=linspace<vec>(1,(*Y).n_rows,(*Y).n_rows);
             MY1=MY.rows(find_finite(sum(MY,1)));
             nr=MY1.n_rows;
-            YtY=cor(MY1);
+            YtY=cor(MY1)*(nr-1);
             fbf=log_FBF_Ga_Gb(&G_a, &G_b, edge, &edges, &YtY, add, nr, h_c);
 
             if((fbf-threshold)>0){
               Y0=(*Y);
               (*Y).col(0)=shift((*Y).col(0),1);
               (*Y).submat(0,0,0,0)+=datum::nan;
               for(uli j=0; j<(*Y).n_rows; ++j){
@@ -1232,32 +1242,31 @@
           MY.col(1)=shift((*Y).col(0),vretard(j));
           if(vretard(j)>0){
             MY.submat(0,1,vretard(j)-1,1)+=datum::nan;
           }
           
           MY1=MY.rows(find_finite(sum(MY,1)));
           nr=MY1.n_rows;
-          YtY=cor(MY1);
+          YtY=cor(MY1)*(nr-1);
           
           M_log_FBF_ar(j,0)=1;
           M_log_FBF_ar(j,1)=vretard(j);
           M_log_FBF_ar(j,2)=log_FBF_Ga_Gb(&G_a, &G_b, edge, &edges, &YtY, add, nr, h_c);
         
         }
         
         M_log_FBF=join_cols(M_log_FBF,M_log_FBF_ar);
         
       }
       
       M_log_FBF.shed_row(0);
-      
+
       uvec ids=find(M_log_FBF.col(2)<=threshold);
       M_log_FBF.shed_rows(ids);
-      
-      
+            
       if(M_log_FBF.n_rows>0){
       
         nvar_max=(uli)2*std::pow(idfinite.n_rows,0.25); //nb: only non missing target is considered
         
         if(M_log_FBF.n_rows>nvar_max){
           ids = sort_index(M_log_FBF.col(2),"descend");
           ids=ids.rows(0,nvar_max-1);
@@ -1297,29 +1306,34 @@
    
   
   return(str_out);
 
 }
 
 
-field<vec> model_multivariate_selection(mat* Y, Col<uli>* ids_vars_x_uni, Col<uli>* ids_vars_ar_uni, string loss_function, bool flg_const, bool flg_arx){
+field<vec> model_multivariate_selection(mat* Y, Col<uli>* ids_vars_x_uni, Col<uli>* ids_vars_ar_uni, string loss_function, bool flg_const, bool flg_arx, double h_c){
         
     Col<uli> ids_vars_x,v_ar;
     vec vbeta_arx;
     vec vresid((*Y).n_rows,1);
 
     double nvars=(*Y).n_cols-1+(*ids_vars_ar_uni).n_rows; 
     
     if(nvars>0){
 
       double threshold=0.5;
-      double h_c=1; 
-      if(nvars>50){
-       h_c=2; 
-      } 
+      if(h_c==-1){
+       h_c=0; 
+       if(nvars>3){
+        h_c=1; 
+       } 
+       if(nvars>50){
+        h_c=2; 
+       } 
+      }
       double n_tot_mod_c=nvars*100;
       double C_c=0.01;
       double n_hpp_c=1;
        
       mat Y0;
       uvec u_ids_vars_x;
       if((*ids_vars_x_uni).n_rows>0){
@@ -1348,24 +1362,29 @@
       vec M_P;
     
       if((len_ar>0) || (Y0.n_cols>1)){
     	
 	      nr=tab_input.corY_nr;
         nc=tab_input.corY_nc;
   
-        h_c=1; 
-        if((nc-1)>50){
-         h_c=2; 
-        } 
+        if(h_c==-1){
+         h_c=0; 
+         if(nvars>3){
+          h_c=1; 
+         } 
+         if(nvars>50){
+          h_c=2; 
+         } 
+        }
+
     
         G_base_c=zeros<vec>(nc-1);
         
         res=FBF_RS(&tab_input.corY,nr,&G_base_c,h_c,C_c,n_tot_mod_c,n_hpp_c,univariate);
-      
-                
+       
         M_q=res(0,0);
   
 	      ids=find(M_q>=threshold);
 	      if(ids.n_rows>nvar_max){
           ids = sort_index(M_q,"descend");
           ids=ids.rows(0,nvar_max-1);
           ids=sort(ids);
@@ -1500,14 +1519,15 @@
 
 str_pred_out sarimax_pred(mat* Y, bool flg_sim, mat Mfitted, vec probs, uli nsim, string loss_function, bool pred_only, bool flg_const, field<vec> models)
 {
   
   Col<uli> ids_vars_x=conv_to< Col<uli> >::from(models(0,0));
   Col<uli> ids_vars_ar=conv_to< Col<uli> >::from(models(0,1));
   vec vbeta_arx=models(0,2);
+
   ///
   double const0=0;
   if(flg_const==1){
    if(vbeta_arx.n_rows>0){
     const0=vbeta_arx(vbeta_arx.n_rows-1);
     vbeta_arx.shed_row(vbeta_arx.n_rows-1);
    }
@@ -1744,27 +1764,15 @@
             veps(t)=(*Y)(t,0)-pred_x-pred_ar;
            }else{
             veps(t)=0;
            }
           }
         
         }
-        
-        // if(kpred==0){
-        //  cout << "--------" << endl;
-        //  cout << "tk:" << tk << endl;
-        //  cout << "pred_ma:" << pred_ma << endl;
-        //  cout << "pred_ar:" << pred_ar << endl;
-        //  cout << "eps-1:" << veps(tk-1) << endl;
-        //  cout << "eps:" << veps(tk) << endl;
-        //  cout << "target-1:" << (*Y)(tk-1,0) << endl;
-        //  cout << "target:" << (*Y)(tk,0) << endl;
-        //  cout << "pred:" << My_pred(tk,0) << endl;
-        // }
-      
+              
       }//end kpred 
       
     }//end t
   
   }//end s
   
   if(flg_sim==1){
@@ -1911,15 +1919,15 @@
  
  field<vec> models;
  mat predictions;
 
 };
 
 
-str_model_selection model_selection_prediction(mat* Y, double from_lag, double max_lag, vec probs, uli nsim, string loss_function, bool pred_only, bool flg_const, bool flg_diff, field<vec> models)
+str_model_selection model_selection_prediction(mat* Y, double from_lag, double max_lag, vec probs, uli nsim, string loss_function, bool pred_only, bool flg_const, bool flg_diff, field<vec> models, double h_c)
 {
 
   str_pred_out out_pred_i;
 
   str_out_uni_select out_uni_select_arx;
   field<vec> out_multi_select_arx;
 
@@ -1942,15 +1950,15 @@
   //SARIX
   
   uli ndiff=0;
   vec old_target=(*Y).col(0);
   
   if(pred_only==0){
     
-    out_uni_select_arx=model_univariate_selection(Y, from_lag, max_lag, flg_diff);
+    out_uni_select_arx=model_univariate_selection(Y, from_lag, max_lag, flg_diff, h_c);
     
     res_out.models(0,5)=out_uni_select_arx.odiff;
     ndiff=(uli)out_uni_select_arx.odiff;
     
   }else{
     
     ndiff=(uli)as_scalar(models(0,5));
@@ -1968,28 +1976,28 @@
   
   if(((flg_x_only==0) && (out_uni_select_arx.vars_ar_idx.n_rows>0) && (pred_only==0)) || ((flg_x_only==0) && (pred_only==1))){ //if it is a sarimax
     
     
     if(pred_only==0){
       
       
-      out_multi_select_arx=model_multivariate_selection(Y, &out_uni_select_arx.vars_x_idx, &out_uni_select_arx.vars_ar_idx, loss_function, flg_const, 1);
+      out_multi_select_arx=model_multivariate_selection(Y, &out_uni_select_arx.vars_x_idx, &out_uni_select_arx.vars_ar_idx, loss_function, flg_const, 1, h_c);
       
       
       res_out.models(0,0)=out_multi_select_arx(0,0);
       res_out.models(0,1)=out_multi_select_arx(0,1);
       res_out.models(0,2)=out_multi_select_arx(0,2);
       
       //MA
 
       vresid=out_multi_select_arx(0,3);
 
-      out_uni_select_ma=model_univariate_selection(&vresid, from_lag, max_lag, 0);
+      out_uni_select_ma=model_univariate_selection(&vresid, from_lag, max_lag, 0, h_c);
       
-      out_multi_select_ma=model_multivariate_selection(&vresid, &out_uni_select_ma.vars_x_idx, &out_uni_select_ma.vars_ar_idx, loss_function, flg_const, 0);
+      out_multi_select_ma=model_multivariate_selection(&vresid, &out_uni_select_ma.vars_x_idx, &out_uni_select_ma.vars_ar_idx, loss_function, flg_const, 0, h_c);
       
       res_out.models(0,3)=out_multi_select_ma(0,1);
       res_out.models(0,4)=out_multi_select_ma(0,2);
       
       models=res_out.models;
     
     }
@@ -2007,28 +2015,28 @@
   
   }
   
 
   if(flg_x_only==1){
      
     if(pred_only==0){
-    
-      out_multi_select_arx=model_multivariate_selection(Y, &out_uni_select_arx.vars_x_idx, &vretard_empty, loss_function, flg_const, 1);
+
+      out_multi_select_arx=model_multivariate_selection(Y, &out_uni_select_arx.vars_x_idx, &vretard_empty, loss_function, flg_const, 1, h_c);
 
       res_out.models(0,0)=out_multi_select_arx(0,0);
       res_out.models(0,1)=out_multi_select_arx(0,1);
       res_out.models(0,2)=out_multi_select_arx(0,2);
-      
+
       models=res_out.models;
-      
+                  
     }
-    
+          
     out_pred_i=sarimax_pred(Y, 0, Mfitted_empty, probs, nsim, loss_function, pred_only, flg_const, models);
     Mfitted=out_pred_i.fitted;
-    
+  
     out_pred_i=sarimax_pred(Y, 1, Mfitted, probs, nsim, loss_function, pred_only, flg_const, models);
     
     res_out.predictions=out_pred_i.predictions;
 
   }
   
   if(ndiff>0){
@@ -2088,21 +2096,25 @@
  field<vec> bw_models;
  vec bw_performances;
 
 };
 
 
 
-str_output regpred_cpp(mat* Y, double from_lag, double max_lag, double alpha, uli nsim, bool flg_print, string direction, string loss_function, bool pred_only, bool flg_const, bool flg_diff, vector < field<vec> > vmodels)
+str_output regpred_cpp(mat* Y, double from_lag, double max_lag, double alpha, uli nsim, bool flg_print, string direction, string loss_function, bool pred_only, bool flg_const, bool flg_diff, double h_c, vector < field<vec> > vmodels)
 {
   
   str_model_out tab_model;
   str_pred_out tab_pred;
   str_output str_out;
-   
+
+  if(max_lag==0){
+   from_lag=0;
+  }
+
   double pinf=(alpha/2);
   double psup=1-(alpha/2);
 
   vec probs={pinf, 0.5, psup};
 
   vec vresid_empty;
   vec vresid;
@@ -2136,15 +2148,15 @@
      printA("Forward prediction: model selection and prediction...");
     }
     
     if(pred_only==1){
      models0=vmodels[0];
     }
     
-    out_sel_pred=model_selection_prediction(Y, from_lag, max_lag, probs, nsim, loss_function,pred_only,flg_const,flg_diff,models0);
+    out_sel_pred=model_selection_prediction(Y, from_lag, max_lag, probs, nsim, loss_function,pred_only,flg_const,flg_diff,models0,h_c);
   
     predictions=out_sel_pred.predictions;
 
     str_out.fw_predictions=predictions;
     
     models=out_sel_pred.models;
     str_out.fw_models=models;
@@ -2172,15 +2184,15 @@
      printA("Backward prediction: model selection and prediction...");
     }
     
     if(pred_only==1){
      models0=vmodels[1];
     }
     
-    out_sel_pred=model_selection_prediction(&Yr, from_lag, max_lag, probs, nsim, loss_function,pred_only,flg_const,flg_diff,models0);
+    out_sel_pred=model_selection_prediction(&Yr, from_lag, max_lag, probs, nsim, loss_function,pred_only,flg_const,flg_diff,models0,h_c);
 
     predictions_rev=reverse(out_sel_pred.predictions);
     
     str_out.bw_predictions=predictions_rev;
     
     models=out_sel_pred.models;
     str_out.bw_models=models;
@@ -2314,29 +2326,29 @@
   
 }
 
 #ifdef language_py
 
 
 pair < svec3, pair < svec2, svec4 > > 
-regpred_py(svec2& Y, double from_lag, double max_lag, double alpha, uli nsim, bool flg_print, string direction, string loss_function, bool pred_only, bool flg_const, bool flg_diff, svec4& vmodels){
+regpred_py(svec2& Y, double from_lag, double max_lag, double alpha, uli nsim, bool flg_print, string direction, string loss_function, bool pred_only, bool flg_const, bool flg_diff, double h_c, svec4& vmodels){
   
   mat Y0=std_vec2_to_arma_mat(&Y);
   
   vector < field<vec> > vmodels0(2);
   if(pred_only==1){
    if((direction=="->") || (direction=="<->")){
     vmodels0[0]=std_vec3_to_arma_fie_vec(&vmodels[0]);
    }
    if((direction=="<-") || (direction=="<->")){
     vmodels0[1]=std_vec3_to_arma_fie_vec(&vmodels[1]);
    }
   }
     
-  str_output str_out=regpred_cpp(&Y0, from_lag, max_lag, alpha, nsim, flg_print, direction, loss_function, pred_only, flg_const, flg_diff, vmodels0);
+  str_output str_out=regpred_cpp(&Y0, from_lag, max_lag, alpha, nsim, flg_print, direction, loss_function, pred_only, flg_const, flg_diff, h_c, vmodels0);
 
   //store predictions
     
   svec3 vpredictions(3);
   
   svec2 predictions=arma_mat_to_std_vec2(&str_out.predictions);
   svec2 fw_predictions=arma_mat_to_std_vec2(&str_out.fw_predictions);
@@ -2453,15 +2465,15 @@
     R0[i0]=R1;
   }
   
   return(R0);
   
 }
 
-RcppExport SEXP regpred_R(SEXP Y_p, SEXP from_lag_p, SEXP max_lag_p, SEXP alpha_p, SEXP nsim_p, SEXP flg_print_p, SEXP direction_p, SEXP loss_function_p, SEXP pred_only_p, SEXP flg_const_p, SEXP flg_diff_p, SEXP vmodels_p)
+RcppExport SEXP regpred_R(SEXP Y_p, SEXP from_lag_p, SEXP max_lag_p, SEXP alpha_p, SEXP nsim_p, SEXP flg_print_p, SEXP direction_p, SEXP loss_function_p, SEXP pred_only_p, SEXP flg_const_p, SEXP flg_diff_p, SEXP h_c_p, SEXP vmodels_p)
 {
 
   NumericMatrix Y_0(Y_p); 
   mat Y(Y_0.begin(), Y_0.nrow(), Y_0.ncol(), false);
   
   NumericVector from_lag_0(from_lag_p); 
   double from_lag = Rcpp::as<double>(from_lag_0);
@@ -2488,28 +2500,31 @@
   bool pred_only = Rcpp::as<bool>(pred_only_0);
   
   NumericVector flg_const_0(flg_const_p);
   bool flg_const = Rcpp::as<bool>(flg_const_0);
   
   NumericVector flg_diff_0(flg_diff_p);
   bool flg_diff = Rcpp::as<bool>(flg_diff_0);
-  
+
+  NumericVector h_c_0(h_c_p); 
+  double h_c = Rcpp::as<double>(h_c_0);
+
   List vmodels(vmodels_p);
   
   vector < field<vec> > vmodels0(2);
   List fw_models;
   List bw_models;
   if(pred_only==1){
    vmodels0[0]=R_List2_vec_to_arma_fie_vec(vmodels[0]);
    vmodels0[1]=R_List2_vec_to_arma_fie_vec(vmodels[1]);
    fw_models=vmodels[0];
    bw_models=vmodels[1];
   }
 
-  str_output str_out=regpred_cpp(&Y, from_lag, max_lag, alpha, nsim, flg_print, direction, loss_function, pred_only, flg_const, flg_diff, vmodels0);
+  str_output str_out=regpred_cpp(&Y, from_lag, max_lag, alpha, nsim, flg_print, direction, loss_function, pred_only, flg_const, flg_diff, h_c, vmodels0);
   
   //store predictions
   
   NumericMatrix predictions=arma_mat_to_R_mat(&str_out.predictions);
   NumericMatrix fw_predictions=arma_mat_to_R_mat(&str_out.fw_predictions);
   NumericMatrix bw_predictions=arma_mat_to_R_mat(&str_out.bw_predictions);
```

### Comparing `rego-1.5.2/src/cypack/functions.h` & `rego-1.6.1/src/cypack/functions.h`

 * *Files 6% similar despite different names*

```diff
@@ -45,17 +45,17 @@
  mat bw_predictions;
  field<vec> bw_models;
  vec bw_performances;
 
 };
 
 
-str_output regpred_cpp(mat* Y, double from_lag, double max_lag, double alpha, uli nsim, bool flg_print, string direction, string loss_function, bool pred_only, bool flg_const, bool flg_diff, vector<field<vec>> models);
+str_output regpred_cpp(mat* Y, double from_lag, double max_lag, double alpha, uli nsim, bool flg_print, string direction, string loss_function, bool pred_only, bool flg_const, bool flg_diff, double h_c, vector<field<vec>> models);
 
 #ifdef language_py 
 pair < svec3, pair < svec2, svec4 > >
-regpred_py(svec2& Y, double from_lag, double max_lag, double alpha, uli nsim, bool flg_print, string direction, string loss_function, bool pred_only, bool flg_const, bool flg_diff, svec4& models);
+regpred_py(svec2& Y, double from_lag, double max_lag, double alpha, uli nsim, bool flg_print, string direction, string loss_function, bool pred_only, bool flg_const, bool flg_diff, double h_c, svec4& models);
 #endif
 
 #ifdef language_R
- RcppExport SEXP regpred_R(SEXP Y_p, SEXP from_lag_p, SEXP max_lag_p, SEXP alpha_p, SEXP nsim_p, SEXP flg_print_p, SEXP direction_p, SEXP loss_function_p, SEXP pred_only_p, SEXP flg_const_p, SEXP flg_diff_p, SEXP vmodels_p);
+ RcppExport SEXP regpred_R(SEXP Y_p, SEXP from_lag_p, SEXP max_lag_p, SEXP alpha_p, SEXP nsim_p, SEXP flg_print_p, SEXP direction_p, SEXP loss_function_p, SEXP pred_only_p, SEXP flg_const_p, SEXP flg_diff_p, SEXP h_c_p, SEXP vmodels_p);
 #endif
```

### Comparing `rego-1.5.2/src/cypack/generate_doc.py` & `rego-1.6.1/src/cypack/generate_doc.py`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo` & `rego-1.6.1/src/cypack/armadillo/include/armadillo`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_cube_slices_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_cube_slices_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/CubeToMatOp_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/CubeToMatOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_hypot_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_hypot_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/auxlib_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/auxlib_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cor_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cor_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_mean_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_mean_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_shift.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_shift.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_min_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_static_check.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_static_check.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/hdf5_name.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/hdf5_name.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/span.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/span.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_cov_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_cov_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/def_atlas.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/def_atlas.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_join_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_join_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_kron_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_kron_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_hist.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_hist.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_elem2_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_elem2_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_div.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_div.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_strans.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_strans.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_find_unique.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_find_unique.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_resize_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_resize_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_chi2rnd_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_chi2rnd_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/podarray_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/podarray_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_normalise_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_normalise_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_all_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_all_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/BaseCube_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/BaseCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_elem.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_elem.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_polyval_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_polyval_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_nonzeros_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_nonzeros_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_prod_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_prod_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_svd.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_svd.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/unwrap_cube.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/unwrap_cube.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_SortEigenvalue.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_SortEigenvalue.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/GlueCube_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/GlueCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_range_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_range_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_kmeans.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_kmeans.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/compiler_setup_post.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/compiler_setup_post.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cond_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cond_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_trimat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_trimat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_cube_each_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_cube_each_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_approx_equal.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_approx_equal.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_chi2rnd.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_chi2rnd.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_reverse_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_reverse_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_stddev.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_stddev.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cumsum_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cumsum_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_ostream_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_ostream_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_index_max_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_index_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_chi2rnd_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_chi2rnd_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/config.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/config.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtGlueCube_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtGlueCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fft_engine.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fft_engine.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/band_helper.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/band_helper.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SizeMat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SizeMat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/def_superlu.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/def_superlu.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_hist_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_hist_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_norm_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_norm_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_cor_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_cor_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_SymEigsSolver_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_SymEigsSolver_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_inplace_trans.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_inplace_trans.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_eig_pair.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_eig_pair.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_var.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_var.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/running_stat_vec_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/running_stat_vec_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_times_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_times_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_diagmat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_diagmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_quantile.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_quantile.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_trapz_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_trapz_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpBase_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpBase_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_resize_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_resize_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpRow_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpRow_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_reverse_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_reverse_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_inv_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_inv_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/compiler_extra.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/compiler_extra.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_rel_comparators.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_rel_comparators.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_sum.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_sum.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_mean_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_mean_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/def_lapack.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/def_lapack.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_diagvec_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_diagvec_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Op_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Op_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/distr_param.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/distr_param.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sort_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sort_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_cov.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_cov.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_schur.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_schur.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Op_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Op_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_hess.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_hess.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_stddev_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_stddev_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_version.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_version.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_as_scalar.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_as_scalar.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpBase_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpBase_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_elem2_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_elem2_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eOpCube_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eOpCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_hypot_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_hypot_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_schur.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_schur.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_stddev_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_stddev_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_powmat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_powmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtGlue_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_var_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_var_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_randi.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_randi.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_polyfit_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_polyfit_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_affmul_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_affmul_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpProxy.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpProxy.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_each_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_each_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mul_gemv.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mul_gemv.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_SparseGenMatProd_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_SparseGenMatProd_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_pinv_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_pinv_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mp_misc.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mp_misc.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_strans_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_strans_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_eigs_gen.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_eigs_gen.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_join_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_join_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_randperm.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_randperm.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_expmat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_expmat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_histc.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_histc.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_cmath.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_cmath.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_range.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_range.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_toeplitz_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_toeplitz_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_repmat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_repmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_norm_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_norm_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_trimat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_trimat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_join_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_join_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eGlue_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cx_scalar_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cx_scalar_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_max_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_polyval_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_polyval_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_plus.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_plus.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpSubview_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpSubview_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/csv_name.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/csv_name.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_unique.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_unique.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_hist_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_hist_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_min_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_elem_helper_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_elem_helper_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_reverse_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_reverse_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Gen_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Gen_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpMat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpMat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtSpOp_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtSpOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtSpGlue_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtSpGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtOpCube_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtOpCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/include_hdf5.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/include_hdf5.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_dotext_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_dotext_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_shift_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_shift_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arrayops_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arrayops_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_trimat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_trimat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_chol_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_chol_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/GenCube_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/GenCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_relational_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_relational_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_mean.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_mean.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sort_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sort_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpOp_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_symmat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_symmat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SizeCube_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SizeCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_all.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_all.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_intersect_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_intersect_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_accu.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_accu.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/access.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/access.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_trapz.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_trapz.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_fft.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_fft.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/xvec_htrans_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/xvec_htrans_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_solve_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_solve_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_relational_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_relational_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_htrans_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_htrans_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_sprandu.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_sprandu.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_cube_schur.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_cube_schur.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Cube_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Cube_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spdiagview_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spdiagview_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_expmat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_expmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_eig_gen.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_eig_gen.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/cond_rel_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/cond_rel_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_config.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_config.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SizeCube_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SizeCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_times_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_times_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_field_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_field_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_inv_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_inv_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_max_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/MapMat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/MapMat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_max_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_wishrnd.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_wishrnd.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_schur_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_schur_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/gmm_full_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/gmm_full_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_eps.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_eps.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtSpGlue_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtSpGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_interp2.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_interp2.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_rng_cxx11.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_rng_cxx11.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_toeplitz_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_toeplitz_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_sum_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_sum_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/typedef_elem_check.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/typedef_elem_check.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_affmul_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_affmul_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/config.hpp.cmake` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/config.hpp.cmake`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_nonzeros.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_nonzeros.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_min_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/def_arpack.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/def_arpack.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_TridiagEigen_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_TridiagEigen_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_reverse.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_reverse.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_chol.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_chol.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_vectorise_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_vectorise_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_fft2.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_fft2.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/gmm_diag_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/gmm_diag_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_times_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_times_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_wishrnd_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_wishrnd_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/gmm_misc_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/gmm_misc_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_diff.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_diff.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_trans.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_trans.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_quantile_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_quantile_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/include_atlas.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/include_atlas.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_DoubleShiftQR_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_DoubleShiftQR_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_logmat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_logmat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_reshape.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_reshape.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sp_plus_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sp_plus_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_atan2_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_atan2_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_var_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_var_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_index_min_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_index_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/translate_arpack.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/translate_arpack.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/translate_lapack.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/translate_lapack.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_roots_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_roots_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_histc_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_histc_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/OpCube_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/OpCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/OpCube_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/OpCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_DenseGenMatProd_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_DenseGenMatProd_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_normalise_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_normalise_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mul_herk.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mul_herk.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_spones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_spones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_vectorise_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_vectorise_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_dot_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_dot_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mul_gemm_mixed.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mul_gemm_mixed.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_join.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_join.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_field_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_field_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_htrans_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_htrans_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_size.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_size.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_max.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_max.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_speye.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_speye.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_htrans_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_htrans_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eglue_core_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eglue_core_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_reshape_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_reshape_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_shuffle.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_shuffle.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cond_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cond_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/diagmat_proxy.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/diagmat_proxy.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_polyfit_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_polyfit_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sqrtmat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sqrtmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_intersect_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_intersect_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/memory.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/memory.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_diagvec.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_diagvec.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_GenEigsSolver_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_GenEigsSolver_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_ostream_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_ostream_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_trunc_exp.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_trunc_exp.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Mat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Mat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_normalise_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_normalise_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/sympd_helper.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/sympd_helper.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/podarray_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/podarray_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/xtrans_mat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/xtrans_mat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_resize.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_resize.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_flip_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_flip_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/typedef_mat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/typedef_mat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_misc_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_misc_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/constants.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/constants.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_clamp_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_clamp_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_sort_index.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_sort_index.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_logmat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_logmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtOp_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_diff_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_diff_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpMat_iterators_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpMat_iterators_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_orth_null_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_orth_null_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_plus_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_plus_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_cross_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_cross_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_trace.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_trace.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_max_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sort_index_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sort_index_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cumprod_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cumprod_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_rng.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_rng.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eGlue_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_var_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_var_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_reshape_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_reshape_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_diff_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_diff_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_strans_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_strans_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/translate_blas.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/translate_blas.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpToDOp_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpToDOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_any_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_any_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_flip_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_flip_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_merge_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_merge_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpCol_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpCol_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/constants_old.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/constants_old.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpGlue_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_misc_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_misc_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_cube_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_cube_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sp_minus_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sp_minus_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/field_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/field_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_mvnrnd.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_mvnrnd.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_min_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Row_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Row_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cov_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cov_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_min_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_sum_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_sum_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_forward.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_forward.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_solve.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_solve.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_svds.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_svds.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Row_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Row_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cov_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cov_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/wall_clock_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/wall_clock_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_eig_sym.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_eig_sym.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_clamp.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_clamp.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/translate_atlas.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/translate_atlas.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_cube_relational.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_cube_relational.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/injector_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/injector_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_all_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_all_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtGlueCube_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtGlueCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/unwrap.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/unwrap.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_misc_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_misc_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sort_index_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sort_index_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/injector_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/injector_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_index_min.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_index_min.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_dot.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_dot.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_index_max.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_index_max.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_find.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_find.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_cumprod.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_cumprod.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/compiler_setup.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/compiler_setup.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eGlueCube_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eGlueCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_hist_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_hist_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_cross.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_cross.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Base_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Base_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_det.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_det.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_shuffle_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_shuffle_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_kron_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_kron_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_ostream.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_ostream.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_eye.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_eye.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_TridiagEigen_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_TridiagEigen_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_symmat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_symmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpRow_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpRow_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Gen_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Gen_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_toeplitz_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_toeplitz_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/CubeToMatOp_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/CubeToMatOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_kron_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_kron_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_str.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_str.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_quantile_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_quantile_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_strans_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_strans_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/translate_superlu.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/translate_superlu.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_each_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_each_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_merge_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_merge_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_elem1_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_elem1_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_powmat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_powmat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_find_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_find_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_DoubleShiftQR_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_DoubleShiftQR_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_symmat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_symmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_repmat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_repmat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_range_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_range_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_diagmat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_diagmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpToDOp_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpToDOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_cube_plus.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_cube_plus.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_cube_minus.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_cube_minus.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/debug.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/debug.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spdiagview_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spdiagview_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_fft_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_fft_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_max_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_powmat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_powmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_relational_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_relational_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/gmm_full_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/gmm_full_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_cumsum.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_cumsum.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_spsolve.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_spsolve.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eOp_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_cube_times.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_cube_times.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_polyfit.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_polyfit.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_syl_lyap.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_syl_lyap.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/diskio_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/diskio_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_wishrnd_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_wishrnd_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_log_det.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_log_det.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_expmat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_expmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_cx_attrib.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_cx_attrib.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/GenCube_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/GenCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpSubview_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpSubview_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_ones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_ones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_toeplitz.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_toeplitz.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtSpOp_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtSpOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_find_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_find_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_histc_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_histc_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_any_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_any_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_cube_slices_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_cube_slices_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtOpCube_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtOpCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_cross_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_cross_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_minus.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_minus.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/diskio_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/diskio_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_cor.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_cor.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_reverse_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_reverse_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpSubview_iterators_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpSubview_iterators_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mul_gemm.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mul_gemm.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/sp_auxlib_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/sp_auxlib_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_conv_to.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_conv_to.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_pinv.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_pinv.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_prod_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_prod_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_relational_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_relational_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_trig.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_trig.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_roots_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_roots_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_log_normpdf.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_log_normpdf.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpMat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpMat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sum_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sum_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_prod.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_prod.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/GenSpecialiser.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/GenSpecialiser.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eglue_core_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eglue_core_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/hdf5_misc.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/hdf5_misc.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cumsum_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cumsum_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/BaseCube_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/BaseCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/include_superlu.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/include_superlu.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_min_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_mean_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_mean_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_cov_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_cov_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_repelem.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_repelem.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/upgrade_val.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/upgrade_val.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_mvnrnd_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_mvnrnd_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_mixed_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_mixed_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sum_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sum_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_cube_div.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_cube_div.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SizeMat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SizeMat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/xtrans_mat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/xtrans_mat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_schur_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_schur_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_kron_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_kron_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpOp_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_minus_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_minus_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_randg.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_randg.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eGlueCube_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eGlueCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_diagmat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_diagmat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_diagmat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_diagmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_orth_null_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_orth_null_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_repmat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_repmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_atan2_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_atan2_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cor_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cor_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_fft_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_fft_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/strip.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/strip.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_unique_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_unique_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/field_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/field_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_index_max_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_index_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/restrictors.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/restrictors.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_regspace.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_regspace.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_chol_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_chol_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_normalise.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_normalise.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpCol_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpCol_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_kron.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_kron.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_min_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Mat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Mat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_DenseGenMatProd_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_DenseGenMatProd_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_conv_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_conv_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_find_unique_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_find_unique_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_times_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_times_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_misc.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_misc.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_diagmat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_diagmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_normcdf.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_normcdf.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/auxlib_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/auxlib_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_mean_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_mean_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/traits.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/traits.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Col_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Col_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/running_stat_vec_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/running_stat_vec_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_cube_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_cube_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_intersect.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_intersect.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_median_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_median_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_lu.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_lu.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Glue_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Glue_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/ProxyCube.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/ProxyCube.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_min_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arma_rng_cxx98.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arma_rng_cxx98.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_plus_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_plus_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/unwrap_spmat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/unwrap_spmat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eop_core_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eop_core_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_max_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_trapz_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_trapz_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/cond_rel_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/cond_rel_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Col_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Col_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/typedef_elem.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/typedef_elem.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_join_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_join_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_polyval.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_polyval.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_clamp_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_clamp_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_inv.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_inv.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_elem_helper_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_elem_helper_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpValProxy_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpValProxy_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sqrtmat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sqrtmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_hist_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_hist_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtGlue_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_numel.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_numel.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/running_stat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/running_stat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_relational_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_relational_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_max_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_randu.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_randu.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_SymEigsSolver_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_SymEigsSolver_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Glue_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Glue_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_symmat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_symmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_norm.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_norm.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_unique_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_unique_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mul_syrk.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mul_syrk.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_sprandn.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_sprandn.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_orth_null.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_orth_null.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/mtOp_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/mtOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_elem1_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_elem1_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_repelem_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_repelem_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_randn.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_randn.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/sp_auxlib_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/sp_auxlib_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_conv.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_conv.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_SparseGenMatProd_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_SparseGenMatProd_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_toeplitz_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_toeplitz_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_vectorise_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_vectorise_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_dot_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_dot_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_princomp_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_princomp_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/diagview_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/diagview_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Base_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Base_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Cube_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Cube_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_trimat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_trimat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_princomp.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_princomp.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_htrans_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_htrans_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_any.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_any.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_trimat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_trimat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_GenEigsSolver_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_GenEigsSolver_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/running_stat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/running_stat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/MapMat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/MapMat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/GlueCube_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/GlueCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_conv_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_conv_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_var_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_var_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_index_min_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_index_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sp_minus_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sp_minus_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_cor_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_cor_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_princomp_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_princomp_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_repmat_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_repmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_diagvec_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_diagvec_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/gmm_diag_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/gmm_diag_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_shift_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_shift_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_mixed_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_mixed_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_minus_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_minus_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/trimat_helper.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/trimat_helper.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/def_blas.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/def_blas.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/typedef_mat_fixed.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/typedef_mat_fixed.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eop_aux.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eop_aux.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_vectorise.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_vectorise.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_cond.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_cond.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_eigs_sym.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_eigs_sym.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/wall_clock_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/wall_clock_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_nonzeros_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_nonzeros_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eOpCube_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eOpCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_trunc_log.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_trunc_log.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_times.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_times.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_misc_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_misc_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_sp_plus_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_sp_plus_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_vectorise_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_vectorise_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/newarp_EigsSelect.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/newarp_EigsSelect.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_n_unique.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_n_unique.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_dotext_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_dotext_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_max_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/def_hdf5.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/def_hdf5.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eOp_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpGlue_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_sort.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_sort.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/subview_cube_each_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/subview_cube_each_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_pinv_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_pinv_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_symmat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_symmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/xvec_htrans_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/xvec_htrans_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spglue_relational_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spglue_relational_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/gmm_misc_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/gmm_misc_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_sqrtmat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_sqrtmat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cumprod_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cumprod_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/Proxy.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/Proxy.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_rank.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_rank.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_cx_scalar_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_cx_scalar_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/diagview_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/diagview_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_normalise_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_normalise_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_qr.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_qr.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/spop_repmat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/spop_repmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_min.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_min.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_zeros.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_zeros.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_median.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_median.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/arrayops_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/arrayops_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/SpValProxy_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/SpValProxy_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_repelem_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_repelem_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_normpdf.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_normpdf.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_flip.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_flip.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_strans_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_strans_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_shuffle_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_shuffle_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_logmat_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_logmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_inplace_strans.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_inplace_strans.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_qz.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_qz.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_interp1.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_interp1.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/operator_relational.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/operator_relational.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_find_unique_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_find_unique_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/promote_type.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/promote_type.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/op_median_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/op_median_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_mvnrnd_bones.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_mvnrnd_bones.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/fn_roots.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/fn_roots.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/eop_core_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/eop_core_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/include/armadillo_bits/glue_solve_meat.hpp` & `rego-1.6.1/src/cypack/armadillo/include/armadillo_bits/glue_solve_meat.hpp`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/NOTICE.txt` & `rego-1.6.1/src/cypack/armadillo/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/LICENSE.txt` & `rego-1.6.1/src/cypack/armadillo/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/armadillo/README.md` & `rego-1.6.1/src/cypack/armadillo/README.md`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/dll/libblas.dll` & `rego-1.6.1/src/cypack/dll/libblas.dll`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/dll/libblas.lib` & `rego-1.6.1/src/cypack/dll/libblas.lib`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/dll/liblapack.dll` & `rego-1.6.1/src/cypack/dll/liblapack.dll`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/cypack/dll/liblapack.lib` & `rego-1.6.1/src/cypack/dll/liblapack.lib`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/src/rego.egg-info/PKG-INFO` & `rego-1.6.1/src/rego.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: rego
-Version: 1.5.2
+Version: 1.6.1
 Summary: Automatic Time Series Forecasting and Missing Value Imputation
-Home-page: https://channelattribution.io/docs/rego
+Home-page: https://channelattribution.io/rego
 Author: Davide Altomare, David Loris
 Author-email: info@channelattribution.io
 License: UNKNOWN
-Project-URL: Documentation, https://channelattribution.io/docs/rego
+Project-URL: Documentation, https://channelattribution.io/rego
 Project-URL: Code, https://github.com/DavideAltomare/rego
 Project-URL: Issue tracker, https://github.com/DavideAltomare/rego/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rego-1.5.2/setup.py` & `rego-1.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 else:
 
   extensions = [Extension(name="rego", 
                         sources=["src/cypack/rego.pyx", "src/cypack/functions.cpp"],
 			 include_dirs=["src/cypack/armadillo/include","src/cypack/optim-master/header_only_version"], 
 			 language='c++', 
 			 extra_compile_args=['-std=c++11'],
-			 extra_link_args=['-pthread','-llapack', '-lblas'],
+			 #extra_link_args=['-pthread','-llapack', '-lblas'],
+			 extra_link_args=['-pthread'],
 			 cython_directives={"language_level":'3',"embedsignature": True})
   ]
 
  
 setup(
 	ext_modules = extensions,    
 	cmdclass={'build_ext': build_ext},
```

### Comparing `rego-1.5.2/README.md` & `rego-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `rego-1.5.2/setup.cfg` & `rego-1.6.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [metadata]
 name = rego
-version = 1.5.2
+version = 1.6.1
 description = Automatic Time Series Forecasting and Missing Value Imputation
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Davide Altomare, David Loris
 author_email = info@channelattribution.io
-url = https://channelattribution.io/docs/rego
+url = https://channelattribution.io/rego
 download_urls = https://pypi.org/project/rego
 project_urls = 
-	Documentation = https://channelattribution.io/docs/rego
+	Documentation = https://channelattribution.io/rego
 	Code = https://github.com/DavideAltomare/rego
 	Issue tracker = https://github.com/DavideAltomare/rego/issues
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Education
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering
```

