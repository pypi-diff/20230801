# Comparing `tmp/struqture_py-1.4.0a3.tar.gz` & `tmp/struqture_py-1.4.0a4.tar.gz`

## Comparing `struqture_py-1.4.0a3.tar` & `struqture_py-1.4.0a4.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 struqture_py-1.4.0a3/local_dependencies/struqture/Cargo.toml
--rw-r--r--   0     1001      123    11363 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/LICENSE
--rw-r--r--   0     1001      123    28163 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/bosonic_hamiltonian.rs
--rw-r--r--   0     1001      123    19128 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/bosonic_hamiltonian_system.rs
--rw-r--r--   0     1001      123    46497 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/bosonic_indices.rs
--rw-r--r--   0     1001      123    24456 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/bosonic_noise_operator.rs
--rw-r--r--   0     1001      123    18496 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/bosonic_noise_system.rs
--rw-r--r--   0     1001      123    10535 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/bosonic_open_system.rs
--rw-r--r--   0     1001      123    23323 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/bosonic_operator.rs
--rw-r--r--   0     1001      123    17027 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/bosonic_system.rs
--rw-r--r--   0     1001      123     3411 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/mod.rs
--rw-r--r--   0     1001      123    28953 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/fermionic_hamiltonian.rs
--rw-r--r--   0     1001      123    20403 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/fermionic_hamiltonian_system.rs
--rw-r--r--   0     1001      123    59790 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/fermionic_indices.rs
--rw-r--r--   0     1001      123    28302 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/fermionic_noise_operator.rs
--rw-r--r--   0     1001      123    19642 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/fermionic_noise_system.rs
--rw-r--r--   0     1001      123    11708 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/fermionic_open_system.rs
--rw-r--r--   0     1001      123    24538 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/fermionic_operator.rs
--rw-r--r--   0     1001      123    18252 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/fermionic_system.rs
--rw-r--r--   0     1001      123     3509 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/mod.rs
--rw-r--r--   0     1001      123    37083 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/lib.rs
--rw-r--r--   0     1001      123     2201 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/mappings/jordan_wigner.rs
--rw-r--r--   0     1001      123      839 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/mappings/mod.rs
--rw-r--r--   0     1001      123    22877 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_decoherence_product.rs
--rw-r--r--   0     1001      123    31956 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_hamiltonian.rs
--rw-r--r--   0     1001      123    31154 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_hamiltonian_system.rs
--rw-r--r--   0     1001      123    38219 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_hermitian_product.rs
--rw-r--r--   0     1001      123    37280 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_noise_operator.rs
--rw-r--r--   0     1001      123    34265 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_noise_system.rs
--rw-r--r--   0     1001      123    17155 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_open_system.rs
--rw-r--r--   0     1001      123    30353 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_operator.rs
--rw-r--r--   0     1001      123    32647 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_plus_minus_operator.rs
--rw-r--r--   0     1001      123    19475 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_plus_minus_product.rs
--rw-r--r--   0     1001      123    29484 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_product.rs
--rw-r--r--   0     1001      123    29910 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_system.rs
--rw-r--r--   0     1001      123     9315 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mod.rs
--rw-r--r--   0     1001      123     1159 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/prelude.rs
--rw-r--r--   0     1001      123    25007 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/decoherence_operator.rs
--rw-r--r--   0     1001      123    38073 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/decoherence_product.rs
--rw-r--r--   0     1001      123    20752 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/mod.rs
--rw-r--r--   0     1001      123    27414 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/pauli_product.rs
--rw-r--r--   0     1001      123    30669 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/plus_minus_noise_operator.rs
--rw-r--r--   0     1001      123    27676 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/plus_minus_operator.rs
--rw-r--r--   0     1001      123    41997 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/plus_minus_product.rs
--rw-r--r--   0     1001      123    26523 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/spin_hamiltonian.rs
--rw-r--r--   0     1001      123    20836 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/spin_hamiltonian_system.rs
--rw-r--r--   0     1001      123    36667 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/spin_noise_operator.rs
--rw-r--r--   0     1001      123    20623 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/spin_noise_system.rs
--rw-r--r--   0     1001      123    13420 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/spin_open_system.rs
--rw-r--r--   0     1001      123    27404 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/spin_operator.rs
--rw-r--r--   0     1001      123    19056 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/spin_system.rs
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 struqture_py-1.4.0a3/local_dependencies/struqture-py-macros/Cargo.toml
--rw-r--r--   0     1001      123    11363 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture-py-macros/LICENSE
--rw-r--r--   0     1001      123     3868 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture-py-macros/src/lib.rs
--rw-r--r--   0     1001      123     6356 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture-py-macros/src/mappings.rs
--rw-r--r--   0     1001      123    35539 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture-py-macros/src/noiseless_system_wrapper.rs
--rw-r--r--   0     1001      123    46523 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture-py-macros/src/noisy_system_wrapper.rs
--rw-r--r--   0     1001      123    24031 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/local_dependencies/struqture-py-macros/src/product_wrapper.rs
--rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 struqture_py-1.4.0a3/Cargo.toml
--rw-r--r--   0     1001      123      701 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/build.rs
--rw-r--r--   0     1001      123      544 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/pyproject.toml
--rw-r--r--   0     1001      123     3257 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/bosons/boson_product.rs
--rw-r--r--   0     1001      123     5081 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/bosons/bosonic_hamiltonian_system.rs
--rw-r--r--   0     1001      123     4283 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/bosons/bosonic_noise_system.rs
--rw-r--r--   0     1001      123     2844 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/bosons/bosonic_open_system.rs
--rw-r--r--   0     1001      123     4459 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/bosons/bosonic_system.rs
--rw-r--r--   0     1001      123     3671 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/bosons/hermitian_boson_product.rs
--rw-r--r--   0     1001      123     2885 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/bosons/mod.rs
--rw-r--r--   0     1001      123     3609 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/fermions/fermion_product.rs
--rw-r--r--   0     1001      123     5507 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/fermions/fermionic_hamiltonian_system.rs
--rw-r--r--   0     1001      123     4502 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/fermions/fermionic_noise_system.rs
--rw-r--r--   0     1001      123     3045 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/fermions/fermionic_open_system.rs
--rw-r--r--   0     1001      123     4679 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/fermions/fermionic_system.rs
--rw-r--r--   0     1001      123     3925 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/fermions/hermitian_fermion_product.rs
--rw-r--r--   0     1001      123     2975 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/fermions/mod.rs
--rw-r--r--   0     1001      123     3200 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/lib.rs
--rw-r--r--   0     1001      123     9190 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/mixed_systems/mixed_decoherence_product.rs
--rw-r--r--   0     1001      123     6525 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/mixed_systems/mixed_hamiltonian_system.rs
--rw-r--r--   0     1001      123     9133 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/mixed_systems/mixed_hermitian_product.rs
--rw-r--r--   0     1001      123     4839 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/mixed_systems/mixed_noise_system.rs
--rw-r--r--   0     1001      123     3602 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/mixed_systems/mixed_open_system.rs
--rw-r--r--   0     1001      123     6971 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/mixed_systems/mixed_plus_minus_operator.rs
--rw-r--r--   0     1001      123     7594 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/mixed_systems/mixed_plus_minus_product.rs
--rw-r--r--   0     1001      123     8775 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/mixed_systems/mixed_product.rs
--rw-r--r--   0     1001      123     5437 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/mixed_systems/mixed_system.rs
--rw-r--r--   0     1001      123     2829 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/mixed_systems/mod.rs
--rw-r--r--   0     1001      123     4957 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/spins/decoherence_product.rs
--rw-r--r--   0     1001      123     2431 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/spins/mod.rs
--rw-r--r--   0     1001      123     4826 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/spins/pauli_product.rs
--rw-r--r--   0     1001      123     7413 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/spins/plus_minus_noise_operator.rs
--rw-r--r--   0     1001      123     9607 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/spins/plus_minus_operator.rs
--rw-r--r--   0     1001      123    12596 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/spins/plus_minus_product.rs
--rw-r--r--   0     1001      123     5527 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/spins/spin_hamiltonian_system.rs
--rw-r--r--   0     1001      123     4484 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/spins/spin_noise_system.rs
--rw-r--r--   0     1001      123     3332 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/spins/spin_open_system.rs
--rw-r--r--   0     1001      123     4917 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/src/spins/spin_system.rs
--rw-r--r--   0     1001      123  2048573 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/struqture_py/DEPENDENCIES
--rw-r--r--   0     1001      123      503 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/struqture_py/LICENSE_FOR_BINARY_DISTRIBUTION
--rw-r--r--   0     1001      123     2404 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/struqture_py/PYTHON_LICENSE
--rw-r--r--   0     1001      123      558 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/struqture_py/__init__.py
--rw-r--r--   0     1001      123    46086 2023-07-27 15:37:19.000000 struqture_py-1.4.0a3/Cargo.lock
--rw-r--r--   0        0        0     3747 1970-01-01 00:00:00.000000 struqture_py-1.4.0a3/PKG-INFO
+-rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 struqture_py-1.4.0a4/local_dependencies/struqture/Cargo.toml
+-rw-r--r--   0     1001      123    11363 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/LICENSE
+-rw-r--r--   0     1001      123    28163 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/bosonic_hamiltonian.rs
+-rw-r--r--   0     1001      123    19128 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/bosonic_hamiltonian_system.rs
+-rw-r--r--   0     1001      123    46497 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/bosonic_indices.rs
+-rw-r--r--   0     1001      123    24456 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/bosonic_noise_operator.rs
+-rw-r--r--   0     1001      123    18496 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/bosonic_noise_system.rs
+-rw-r--r--   0     1001      123    10535 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/bosonic_open_system.rs
+-rw-r--r--   0     1001      123    23323 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/bosonic_operator.rs
+-rw-r--r--   0     1001      123    17027 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/bosonic_system.rs
+-rw-r--r--   0     1001      123     3411 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/mod.rs
+-rw-r--r--   0     1001      123    28953 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/fermionic_hamiltonian.rs
+-rw-r--r--   0     1001      123    20403 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/fermionic_hamiltonian_system.rs
+-rw-r--r--   0     1001      123    59790 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/fermionic_indices.rs
+-rw-r--r--   0     1001      123    28302 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/fermionic_noise_operator.rs
+-rw-r--r--   0     1001      123    19642 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/fermionic_noise_system.rs
+-rw-r--r--   0     1001      123    11708 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/fermionic_open_system.rs
+-rw-r--r--   0     1001      123    24538 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/fermionic_operator.rs
+-rw-r--r--   0     1001      123    18252 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/fermionic_system.rs
+-rw-r--r--   0     1001      123     3509 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/mod.rs
+-rw-r--r--   0     1001      123    37083 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/lib.rs
+-rw-r--r--   0     1001      123     2201 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/mappings/jordan_wigner.rs
+-rw-r--r--   0     1001      123      839 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/mappings/mod.rs
+-rw-r--r--   0     1001      123    22877 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_decoherence_product.rs
+-rw-r--r--   0     1001      123    31956 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_hamiltonian.rs
+-rw-r--r--   0     1001      123    31154 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_hamiltonian_system.rs
+-rw-r--r--   0     1001      123    38219 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_hermitian_product.rs
+-rw-r--r--   0     1001      123    37280 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_noise_operator.rs
+-rw-r--r--   0     1001      123    34265 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_noise_system.rs
+-rw-r--r--   0     1001      123    17155 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_open_system.rs
+-rw-r--r--   0     1001      123    30353 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_operator.rs
+-rw-r--r--   0     1001      123    32647 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_plus_minus_operator.rs
+-rw-r--r--   0     1001      123    19475 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_plus_minus_product.rs
+-rw-r--r--   0     1001      123    29484 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_product.rs
+-rw-r--r--   0     1001      123    29910 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_system.rs
+-rw-r--r--   0     1001      123     9315 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mod.rs
+-rw-r--r--   0     1001      123     1159 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/prelude.rs
+-rw-r--r--   0     1001      123    25007 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/decoherence_operator.rs
+-rw-r--r--   0     1001      123    38073 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/decoherence_product.rs
+-rw-r--r--   0     1001      123    20752 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/mod.rs
+-rw-r--r--   0     1001      123    27414 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/pauli_product.rs
+-rw-r--r--   0     1001      123    30669 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/plus_minus_noise_operator.rs
+-rw-r--r--   0     1001      123    27676 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/plus_minus_operator.rs
+-rw-r--r--   0     1001      123    41997 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/plus_minus_product.rs
+-rw-r--r--   0     1001      123    26523 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/spin_hamiltonian.rs
+-rw-r--r--   0     1001      123    20836 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/spin_hamiltonian_system.rs
+-rw-r--r--   0     1001      123    36667 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/spin_noise_operator.rs
+-rw-r--r--   0     1001      123    20623 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/spin_noise_system.rs
+-rw-r--r--   0     1001      123    13420 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/spin_open_system.rs
+-rw-r--r--   0     1001      123    27404 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/spin_operator.rs
+-rw-r--r--   0     1001      123    19056 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/spin_system.rs
+-rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 struqture_py-1.4.0a4/local_dependencies/struqture-py-macros/Cargo.toml
+-rw-r--r--   0     1001      123    11363 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture-py-macros/LICENSE
+-rw-r--r--   0     1001      123     3868 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture-py-macros/src/lib.rs
+-rw-r--r--   0     1001      123     6356 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture-py-macros/src/mappings.rs
+-rw-r--r--   0     1001      123    35539 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture-py-macros/src/noiseless_system_wrapper.rs
+-rw-r--r--   0     1001      123    46523 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture-py-macros/src/noisy_system_wrapper.rs
+-rw-r--r--   0     1001      123    24031 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/local_dependencies/struqture-py-macros/src/product_wrapper.rs
+-rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 struqture_py-1.4.0a4/Cargo.toml
+-rw-r--r--   0     1001      123      701 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/build.rs
+-rw-r--r--   0     1001      123      544 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/pyproject.toml
+-rw-r--r--   0     1001      123     3257 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/bosons/boson_product.rs
+-rw-r--r--   0     1001      123     5081 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/bosons/bosonic_hamiltonian_system.rs
+-rw-r--r--   0     1001      123     4283 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/bosons/bosonic_noise_system.rs
+-rw-r--r--   0     1001      123     2844 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/bosons/bosonic_open_system.rs
+-rw-r--r--   0     1001      123     4459 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/bosons/bosonic_system.rs
+-rw-r--r--   0     1001      123     3671 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/bosons/hermitian_boson_product.rs
+-rw-r--r--   0     1001      123     2885 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/bosons/mod.rs
+-rw-r--r--   0     1001      123     3609 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/fermions/fermion_product.rs
+-rw-r--r--   0     1001      123     5507 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/fermions/fermionic_hamiltonian_system.rs
+-rw-r--r--   0     1001      123     4502 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/fermions/fermionic_noise_system.rs
+-rw-r--r--   0     1001      123     3045 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/fermions/fermionic_open_system.rs
+-rw-r--r--   0     1001      123     4679 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/fermions/fermionic_system.rs
+-rw-r--r--   0     1001      123     3925 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/fermions/hermitian_fermion_product.rs
+-rw-r--r--   0     1001      123     2975 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/fermions/mod.rs
+-rw-r--r--   0     1001      123     3200 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/lib.rs
+-rw-r--r--   0     1001      123     9190 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/mixed_systems/mixed_decoherence_product.rs
+-rw-r--r--   0     1001      123     6525 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/mixed_systems/mixed_hamiltonian_system.rs
+-rw-r--r--   0     1001      123     9133 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/mixed_systems/mixed_hermitian_product.rs
+-rw-r--r--   0     1001      123     4839 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/mixed_systems/mixed_noise_system.rs
+-rw-r--r--   0     1001      123     3602 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/mixed_systems/mixed_open_system.rs
+-rw-r--r--   0     1001      123     6971 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/mixed_systems/mixed_plus_minus_operator.rs
+-rw-r--r--   0     1001      123     7594 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/mixed_systems/mixed_plus_minus_product.rs
+-rw-r--r--   0     1001      123     8775 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/mixed_systems/mixed_product.rs
+-rw-r--r--   0     1001      123     5437 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/mixed_systems/mixed_system.rs
+-rw-r--r--   0     1001      123     2995 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/mixed_systems/mod.rs
+-rw-r--r--   0     1001      123     4957 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/spins/decoherence_product.rs
+-rw-r--r--   0     1001      123     2431 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/spins/mod.rs
+-rw-r--r--   0     1001      123     4826 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/spins/pauli_product.rs
+-rw-r--r--   0     1001      123     7413 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/spins/plus_minus_noise_operator.rs
+-rw-r--r--   0     1001      123     9607 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/spins/plus_minus_operator.rs
+-rw-r--r--   0     1001      123    12596 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/spins/plus_minus_product.rs
+-rw-r--r--   0     1001      123     5527 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/spins/spin_hamiltonian_system.rs
+-rw-r--r--   0     1001      123     4484 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/spins/spin_noise_system.rs
+-rw-r--r--   0     1001      123     3332 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/spins/spin_open_system.rs
+-rw-r--r--   0     1001      123     4917 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/src/spins/spin_system.rs
+-rw-r--r--   0     1001      123  2048573 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/struqture_py/DEPENDENCIES
+-rw-r--r--   0     1001      123      503 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/struqture_py/LICENSE_FOR_BINARY_DISTRIBUTION
+-rw-r--r--   0     1001      123     2404 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/struqture_py/PYTHON_LICENSE
+-rw-r--r--   0     1001      123      558 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/struqture_py/__init__.py
+-rw-r--r--   0     1001      123    46086 2023-08-01 10:05:30.000000 struqture_py-1.4.0a4/Cargo.lock
+-rw-r--r--   0        0        0     3747 1970-01-01 00:00:00.000000 struqture_py-1.4.0a4/PKG-INFO
```

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/Cargo.toml` & `struqture_py-1.4.0a4/local_dependencies/struqture/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "struqture"
-version = "1.4.0-alpha.3"
+version = "1.4.0-alpha.4"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 edition = "2021"
 rust-version = "1.57"
 categories = ["science", "simulation"]
 description = "HQS tool for representing operators, Hamiltonians and open systems."
 license = "Apache-2.0"
 include = ["Cargo.toml", "src*", "LICENSE", "../README.md"]
```

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/LICENSE` & `struqture_py-1.4.0a4/local_dependencies/struqture/LICENSE`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/bosonic_hamiltonian.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/bosonic_hamiltonian.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/bosonic_hamiltonian_system.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/bosonic_hamiltonian_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/bosonic_indices.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/bosonic_indices.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/bosonic_noise_operator.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/bosonic_noise_operator.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/bosonic_noise_system.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/bosonic_noise_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/bosonic_open_system.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/bosonic_open_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/bosonic_operator.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/bosonic_operator.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/bosonic_system.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/bosonic_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/bosons/mod.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/bosons/mod.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/fermionic_hamiltonian.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/fermionic_hamiltonian.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/fermionic_hamiltonian_system.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/fermionic_hamiltonian_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/fermionic_indices.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/fermionic_indices.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/fermionic_noise_operator.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/fermionic_noise_operator.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/fermionic_noise_system.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/fermionic_noise_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/fermionic_open_system.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/fermionic_open_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/fermionic_operator.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/fermionic_operator.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/fermionic_system.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/fermionic_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/fermions/mod.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/fermions/mod.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/lib.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/lib.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/mappings/jordan_wigner.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/mappings/jordan_wigner.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/mappings/mod.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/mappings/mod.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_decoherence_product.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_decoherence_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_hamiltonian.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_hamiltonian.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_hamiltonian_system.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_hamiltonian_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_hermitian_product.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_hermitian_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_noise_operator.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_noise_operator.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_noise_system.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_noise_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_open_system.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_open_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_operator.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_operator.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_plus_minus_operator.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_plus_minus_operator.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_plus_minus_product.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_plus_minus_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_product.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mixed_system.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mixed_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/mixed_systems/mod.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/mixed_systems/mod.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/prelude.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/decoherence_operator.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/decoherence_operator.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/decoherence_product.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/decoherence_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/mod.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/mod.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/pauli_product.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/pauli_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/plus_minus_noise_operator.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/plus_minus_noise_operator.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/plus_minus_operator.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/plus_minus_operator.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/plus_minus_product.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/plus_minus_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/spin_hamiltonian.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/spin_hamiltonian.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/spin_hamiltonian_system.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/spin_hamiltonian_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/spin_noise_operator.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/spin_noise_operator.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/spin_noise_system.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/spin_noise_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/spin_open_system.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/spin_open_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/spin_operator.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/spin_operator.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture/src/spins/spin_system.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture/src/spins/spin_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture-py-macros/LICENSE` & `struqture_py-1.4.0a4/local_dependencies/struqture-py-macros/LICENSE`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture-py-macros/src/lib.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture-py-macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture-py-macros/src/mappings.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture-py-macros/src/mappings.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture-py-macros/src/noiseless_system_wrapper.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture-py-macros/src/noiseless_system_wrapper.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture-py-macros/src/noisy_system_wrapper.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture-py-macros/src/noisy_system_wrapper.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/local_dependencies/struqture-py-macros/src/product_wrapper.rs` & `struqture_py-1.4.0a4/local_dependencies/struqture-py-macros/src/product_wrapper.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/Cargo.toml` & `struqture_py-1.4.0a4/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "struqture-py"
-version = "1.4.0-alpha.3"
+version = "1.4.0-alpha.4"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 edition = "2021"
 rust-version = "1.57"
 categories = ["science", "simulation"]
 description = "Python interface of struqture, the HQS tool for representing operators, Hamiltonians and open systems."
 license = "Apache-2.0"
 include=["src*", "struqture_py", "Cargo.toml", "build.rs", "pyproject.toml"]
@@ -17,24 +17,24 @@
 crate-type = ["cdylib", "rlib"]
 
 [dependencies.pyo3]
 version = "0.19"
 features = ["num-complex", "multiple-pymethods"]
 
 [dependencies]
-struqture = {version="1.4.0-alpha.3", path= "local_dependencies/struqture", default-features=false}
+struqture = {version="1.4.0-alpha.4", path= "local_dependencies/struqture", default-features=false}
 serde = { version = "1.0", features = ["derive"] }
 numpy = "0.19"
 qoqo_calculator = {version="1.1.2", default-features=false}
 qoqo_calculator_pyo3 = {version="1.1.2", default-features=false}
 bincode = "1.3"
 serde_json = "1.0"
 thiserror = "1.0"
 num-complex = "0.4"
-struqture-py-macros = {version="1.4.0-alpha.3", path= "local_dependencies/struqture-py-macros" }
+struqture-py-macros = {version="1.4.0-alpha.4", path= "local_dependencies/struqture-py-macros" }
 schemars = {version = "0.8"}
 
 
 [build-dependencies]
 quote = "1.0"
 syn = { version = "2.0", features = ["full", "visit"] }
 proc-macro2 = "1.0"
```

### Comparing `struqture_py-1.4.0a3/build.rs` & `struqture_py-1.4.0a4/build.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/pyproject.toml` & `struqture_py-1.4.0a4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "struqture-py"
-version = "1.4.0-alpha.3"
+version = "1.4.0-alpha.4"
 dependencies = [
   'numpy',
   'qoqo_calculator_pyo3>=1.1.2',
 ]
 license = {text="Apache-2.0 AND Apache-2.0 with LLVM-exception AND MIT AND Unicode-DFS-2016 AND BSD-2-Clause AND BSD-3-CLause"}
 maintainers = [{name = "HQS Quantum Simulations GmbH", email = "info@quantumsimulations.de"}]
 requires-python = ">=3.8"
```

### Comparing `struqture_py-1.4.0a3/src/bosons/boson_product.rs` & `struqture_py-1.4.0a4/src/bosons/boson_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/bosons/bosonic_hamiltonian_system.rs` & `struqture_py-1.4.0a4/src/bosons/bosonic_hamiltonian_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/bosons/bosonic_noise_system.rs` & `struqture_py-1.4.0a4/src/bosons/bosonic_noise_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/bosons/bosonic_open_system.rs` & `struqture_py-1.4.0a4/src/bosons/bosonic_open_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/bosons/bosonic_system.rs` & `struqture_py-1.4.0a4/src/bosons/bosonic_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/bosons/hermitian_boson_product.rs` & `struqture_py-1.4.0a4/src/bosons/hermitian_boson_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/bosons/mod.rs` & `struqture_py-1.4.0a4/src/bosons/mod.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/fermions/fermion_product.rs` & `struqture_py-1.4.0a4/src/fermions/fermion_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/fermions/fermionic_hamiltonian_system.rs` & `struqture_py-1.4.0a4/src/fermions/fermionic_hamiltonian_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/fermions/fermionic_noise_system.rs` & `struqture_py-1.4.0a4/src/fermions/fermionic_noise_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/fermions/fermionic_open_system.rs` & `struqture_py-1.4.0a4/src/fermions/fermionic_open_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/fermions/fermionic_system.rs` & `struqture_py-1.4.0a4/src/fermions/fermionic_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/fermions/hermitian_fermion_product.rs` & `struqture_py-1.4.0a4/src/fermions/hermitian_fermion_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/fermions/mod.rs` & `struqture_py-1.4.0a4/src/fermions/mod.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/lib.rs` & `struqture_py-1.4.0a4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/mixed_systems/mixed_decoherence_product.rs` & `struqture_py-1.4.0a4/src/mixed_systems/mixed_decoherence_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/mixed_systems/mixed_hamiltonian_system.rs` & `struqture_py-1.4.0a4/src/mixed_systems/mixed_hamiltonian_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/mixed_systems/mixed_hermitian_product.rs` & `struqture_py-1.4.0a4/src/mixed_systems/mixed_hermitian_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/mixed_systems/mixed_noise_system.rs` & `struqture_py-1.4.0a4/src/mixed_systems/mixed_noise_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/mixed_systems/mixed_open_system.rs` & `struqture_py-1.4.0a4/src/mixed_systems/mixed_open_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/mixed_systems/mixed_plus_minus_operator.rs` & `struqture_py-1.4.0a4/src/mixed_systems/mixed_plus_minus_operator.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/mixed_systems/mixed_plus_minus_product.rs` & `struqture_py-1.4.0a4/src/mixed_systems/mixed_plus_minus_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/mixed_systems/mixed_product.rs` & `struqture_py-1.4.0a4/src/mixed_systems/mixed_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/mixed_systems/mixed_system.rs` & `struqture_py-1.4.0a4/src/mixed_systems/mixed_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/mixed_systems/mod.rs` & `struqture_py-1.4.0a4/src/mixed_systems/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -56,21 +56,25 @@
 ///     MixedProduct
 ///     HermitianMixedProduct
 ///     MixedDecoherenceProduct
 ///     MixedSystem
 ///     MixedHamiltonianSystem
 ///     MixedLindbladNoiseSystem
 ///     MixedLindbladOpenSystem
+///     MixedPlusMinusProduct
+///     MixedPlusMinusOperator
 ///
 #[pymodule]
 pub fn mixed_systems(_py: Python, m: &PyModule) -> PyResult<()> {
     // pyo3_log::init();
     m.add_class::<MixedProductWrapper>()?;
     m.add_class::<HermitianMixedProductWrapper>()?;
     m.add_class::<MixedDecoherenceProductWrapper>()?;
     m.add_class::<MixedSystemWrapper>()?;
     m.add_class::<MixedHamiltonianSystemWrapper>()?;
     m.add_class::<MixedLindbladNoiseSystemWrapper>()?;
     m.add_class::<MixedLindbladOpenSystemWrapper>()?;
+    m.add_class::<MixedPlusMinusProductWrapper>()?;
+    m.add_class::<MixedPlusMinusOperatorWrapper>()?;
 
     Ok(())
 }
```

### Comparing `struqture_py-1.4.0a3/src/spins/decoherence_product.rs` & `struqture_py-1.4.0a4/src/spins/decoherence_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/spins/mod.rs` & `struqture_py-1.4.0a4/src/spins/mod.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/spins/pauli_product.rs` & `struqture_py-1.4.0a4/src/spins/pauli_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/spins/plus_minus_noise_operator.rs` & `struqture_py-1.4.0a4/src/spins/plus_minus_noise_operator.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/spins/plus_minus_operator.rs` & `struqture_py-1.4.0a4/src/spins/plus_minus_operator.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/spins/plus_minus_product.rs` & `struqture_py-1.4.0a4/src/spins/plus_minus_product.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/spins/spin_hamiltonian_system.rs` & `struqture_py-1.4.0a4/src/spins/spin_hamiltonian_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/spins/spin_noise_system.rs` & `struqture_py-1.4.0a4/src/spins/spin_noise_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/spins/spin_open_system.rs` & `struqture_py-1.4.0a4/src/spins/spin_open_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/src/spins/spin_system.rs` & `struqture_py-1.4.0a4/src/spins/spin_system.rs`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/struqture_py/DEPENDENCIES` & `struqture_py-1.4.0a4/struqture_py/DEPENDENCIES`

 * *Files 0% similar despite different names*

```diff
@@ -95150,15 +95150,15 @@
 00173ad0: 4152 4520 4f52 2054 4845 2055 5345 204f  ARE OR THE USE O
 00173ae0: 5220 4f54 4845 5220 4445 414c 494e 4753  R OTHER DEALINGS
 00173af0: 2049 4e20 5448 450a 534f 4654 5741 5245   IN THE.SOFTWARE
 00173b00: 2e0a 0a0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ....============
 00173b10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00173b20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00173b30: 3d3d 3d3d 3d3d 3d3d 0a73 7472 7571 7475  ========.struqtu
-00173b40: 7265 2031 2e34 2e30 2d61 6c70 6861 2e33  re 1.4.0-alpha.3
+00173b40: 7265 2031 2e34 2e30 2d61 6c70 6861 2e34  re 1.4.0-alpha.4
 00173b50: 0a62 7920 4851 5320 5175 616e 7475 6d20  .by HQS Quantum 
 00173b60: 5369 6d75 6c61 7469 6f6e 7320 3c69 6e66  Simulations <inf
 00173b70: 6f40 7175 616e 7475 6d73 696d 756c 6174  o@quantumsimulat
 00173b80: 696f 6e73 2e64 653e 0a48 5153 2074 6f6f  ions.de>.HQS too
 00173b90: 6c20 666f 7220 7265 7072 6573 656e 7469  l for representi
 00173ba0: 6e67 206f 7065 7261 746f 7273 2c20 4861  ng operators, Ha
 00173bb0: 6d69 6c74 6f6e 6961 6e73 2061 6e64 206f  miltonians and o
@@ -95879,15 +95879,15 @@
 00176860: 0a20 2020 6c69 6d69 7461 7469 6f6e 7320  .   limitations 
 00176870: 756e 6465 7220 7468 6520 4c69 6365 6e73  under the Licens
 00176880: 652e 0a0a 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d  e....===========
 00176890: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 001768a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 001768b0: 3d3d 3d3d 3d3d 3d3d 3d0a 7374 7275 7174  =========.struqt
 001768c0: 7572 652d 7079 2031 2e34 2e30 2d61 6c70  ure-py 1.4.0-alp
-001768d0: 6861 2e33 0a62 7920 4851 5320 5175 616e  ha.3.by HQS Quan
+001768d0: 6861 2e34 0a62 7920 4851 5320 5175 616e  ha.4.by HQS Quan
 001768e0: 7475 6d20 5369 6d75 6c61 7469 6f6e 7320  tum Simulations 
 001768f0: 3c69 6e66 6f40 7175 616e 7475 6d73 696d  <info@quantumsim
 00176900: 756c 6174 696f 6e73 2e64 653e 0a50 7974  ulations.de>.Pyt
 00176910: 686f 6e20 696e 7465 7266 6163 6520 6f66  hon interface of
 00176920: 2073 7472 7571 7475 7265 2c20 7468 6520   struqture, the 
 00176930: 4851 5320 746f 6f6c 2066 6f72 2072 6570  HQS tool for rep
 00176940: 7265 7365 6e74 696e 6720 6f70 6572 6174  resenting operat
@@ -96610,15 +96610,15 @@
 00179610: 6174 696f 6e73 2075 6e64 6572 2074 6865  ations under the
 00179620: 204c 6963 656e 7365 2e0a 0a0a 3d3d 3d3d   License....====
 00179630: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00179640: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00179650: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00179660: 0a73 7472 7571 7475 7265 2d70 792d 6d61  .struqture-py-ma
 00179670: 6372 6f73 2031 2e34 2e30 2d61 6c70 6861  cros 1.4.0-alpha
-00179680: 2e33 0a62 7920 4851 5320 5175 616e 7475  .3.by HQS Quantu
+00179680: 2e34 0a62 7920 4851 5320 5175 616e 7475  .4.by HQS Quantu
 00179690: 6d20 5369 6d75 6c61 7469 6f6e 7320 3c69  m Simulations <i
 001796a0: 6e66 6f40 7175 616e 7475 6d73 696d 756c  nfo@quantumsimul
 001796b0: 6174 696f 6e73 2e64 653e 0a4d 6163 726f  ations.de>.Macro
 001796c0: 7320 666f 7220 7374 7275 7174 7572 652d  s for struqture-
 001796d0: 7079 2063 7261 7465 2e0a 4c69 6365 6e73  py crate..Licens
 001796e0: 653a 2041 7061 6368 652d 322e 300a 2d2d  e: Apache-2.0.--
 001796f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
```

### Comparing `struqture_py-1.4.0a3/struqture_py/PYTHON_LICENSE` & `struqture_py-1.4.0a4/struqture_py/PYTHON_LICENSE`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/struqture_py/__init__.py` & `struqture_py-1.4.0a4/struqture_py/__init__.py`

 * *Files identical despite different names*

### Comparing `struqture_py-1.4.0a3/Cargo.lock` & `struqture_py-1.4.0a4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1330,15 +1330,15 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "struqture"
-version = "1.4.0-alpha.3"
+version = "1.4.0-alpha.4"
 dependencies = [
  "bincode",
  "itertools",
  "jsonschema",
  "nalgebra",
  "ndarray",
  "num-complex",
@@ -1351,15 +1351,15 @@
  "test-case",
  "thiserror",
  "tinyvec",
 ]
 
 [[package]]
 name = "struqture-py"
-version = "1.4.0-alpha.3"
+version = "1.4.0-alpha.4"
 dependencies = [
  "bincode",
  "nalgebra",
  "ndarray",
  "num-complex",
  "numpy",
  "proc-macro2",
@@ -1376,15 +1376,15 @@
  "syn 2.0.27",
  "test-case",
  "thiserror",
 ]
 
 [[package]]
 name = "struqture-py-macros"
-version = "1.4.0-alpha.3"
+version = "1.4.0-alpha.4"
 dependencies = [
  "num-complex",
  "proc-macro2",
  "quote",
  "syn 2.0.27",
 ]
```

### Comparing `struqture_py-1.4.0a3/PKG-INFO` & `struqture_py-1.4.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struqture-py
-Version: 1.4.0a3
+Version: 1.4.0a4
 Requires-Dist: numpy
 Requires-Dist: qoqo_calculator_pyo3 >=1.1.2
 License-File: LICENSE
 Summary: Python interface of struqture, the HQS tool for representing operators, Hamiltonians and open systems.
 Author: HQS Quantum Simulations <info@quantumsimulations.de>
 Author-email: HQS Quantum Simulations <info@quantumsimulations.de>
 Maintainer-email: HQS Quantum Simulations GmbH <info@quantumsimulations.de>
```

