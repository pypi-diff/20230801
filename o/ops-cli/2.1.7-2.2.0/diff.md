# Comparing `tmp/ops-cli-2.1.7.tar.gz` & `tmp/ops-cli-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-cli-2.1.7.tar", last modified: Thu Oct 14 14:17:39 2021, max compression
+gzip compressed data, was "ops-cli-2.2.0.tar", last modified: Tue Aug  1 14:11:26 2023, max compression
```

## Comparing `ops-cli-2.1.7.tar` & `ops-cli-2.2.0.tar`

### file list

```diff
@@ -1,253 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.473292 ops-cli-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (121)    11335 2021-10-14 14:16:23.000000 ops-cli-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-10-14 14:16:23.000000 ops-cli-2.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    32484 2021-10-14 14:17:39.473292 ops-cli-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    31261 2021-10-14 14:16:23.000000 ops-cli-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.441292 ops-cli-2.1.7/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.449292 ops-cli-2.1.7/examples/aws-kubernetes/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/.opsconfig.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     8743 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.449292 ops-cli-2.1.7/examples/aws-kubernetes/clusters/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.449292 ops-cli-2.1.7/examples/aws-kubernetes/clusters/kubeconfigs/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/clusters/kubeconfigs/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/clusters/my-kubernetes-cluster.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.437292 ops-cli-2.1.7/examples/aws-kubernetes/compositions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.441292 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.453292 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/
--rw-r--r--   0 runner    (1001) docker     (121)      810 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/backends.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      549 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/common_variables.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      692 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/configure-local-kubectl.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)     1747 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/eks-cluster-autoscaler.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/eks-cluster.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      407 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/eks-worker-nodes-auth-configmap.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)     5994 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/eks-worker-nodes.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/outputs.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/providers.tf.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.453292 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)      599 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/scripts/fileexist.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/variables.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)     1824 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/vpc.tf.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.453292 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/common/
--rw-r--r--   0 runner    (1001) docker     (121)      810 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/common/backends.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      549 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/common/common_variables.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/common/providers.tf.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.453292 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm/
--rw-r--r--   0 runner    (1001) docker     (121)      810 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm/backends.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      816 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm/cluster-autoscaler.tf
--rw-r--r--   0 runner    (1001) docker     (121)      549 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm/common_variables.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      654 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm/dashboard.tf
--rw-r--r--   0 runner    (1001) docker     (121)      271 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm/kube-state-metrics.tf
--rw-r--r--   0 runner    (1001) docker     (121)      455 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm/kube2iam.tf
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm/provider_helm.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm/providers.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm/variables.tf.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.453292 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm-init/
--rw-r--r--   0 runner    (1001) docker     (121)      810 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm-init/backends.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      272 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm-init/helm-init.tf.jinja2
--rwxr-xr-x   0 runner    (1001) docker     (121)      871 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/aws-kubernetes/update.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.457292 ops-cli-2.1.7/examples/cassandra-stress/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/.opsconfig.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2243 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.457292 ops-cli-2.1.7/examples/cassandra-stress/ansible/
--rw-r--r--   0 runner    (1001) docker     (121)      414 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/ansible/install_stress_tool.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      758 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/ansible/setup.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      615 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/ansible/setup12.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.457292 ops-cli-2.1.7/examples/cassandra-stress/ansible/templates/
--rwxr-xr-x   0 runner    (1001) docker     (121)    14497 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/ansible/templates/cassandra-env.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)    41784 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/ansible/templates/cassandra_defaults.yaml
--rwxr-xr-x   0 runner    (1001) docker     (121)    32926 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/ansible/templates/cassandra_defaults_12.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3897 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/ansible/templates/stress.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/cluster1.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/cluster2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.457292 ops-cli-2.1.7/examples/cassandra-stress/terraform/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.457292 ops-cli-2.1.7/examples/cassandra-stress/terraform/main/
--rw-r--r--   0 runner    (1001) docker     (121)      616 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/terraform/main/main.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      681 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/terraform/main/variables.tf.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.457292 ops-cli-2.1.7/examples/cassandra-stress/terraform/modules/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.457292 ops-cli-2.1.7/examples/cassandra-stress/terraform/modules/cassandra/
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/terraform/modules/cassandra/main.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/terraform/modules/macros.tf.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.457292 ops-cli-2.1.7/examples/cassandra-stress/terraform/modules/shared_iam/
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/terraform/modules/shared_iam/default_policy.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.457292 ops-cli-2.1.7/examples/cassandra-stress/terraform/modules/vpc/
--rw-r--r--   0 runner    (1001) docker     (121)     7163 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/terraform/modules/vpc/main.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/cassandra-stress/terraform/user_data
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.445292 ops-cli-2.1.7/examples/features/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.457292 ops-cli-2.1.7/examples/features/ansible-vault/
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/ansible-vault/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.441292 ops-cli-2.1.7/examples/features/ansible-vault/cluster/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.457292 ops-cli-2.1.7/examples/features/ansible-vault/cluster/dev/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/ansible-vault/cluster/dev/dev.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.457292 ops-cli-2.1.7/examples/features/ansible-vault/cluster/prod/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/ansible-vault/cluster/prod/prod.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.457292 ops-cli-2.1.7/examples/features/ansible-vault/inventory/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/ansible-vault/inventory/hosts
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/ansible-vault/password_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/ansible-vault/password_prod.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.457292 ops-cli-2.1.7/examples/features/ansible-vault/playbook/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/ansible-vault/playbook/example.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.457292 ops-cli-2.1.7/examples/features/ansible-vault/vault/
--rw-r--r--   0 runner    (1001) docker     (121)      419 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/ansible-vault/vault/vault_dev.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      419 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/ansible-vault/vault/vault_prod.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/inventory/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/inventory/.opsconfig.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      709 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/inventory/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/inventory/local_inventory/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/inventory/local_inventory/hosts
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/inventory/my-aws-cluster.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/inventory/my-azure-cluster.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/packer/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/packer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/packer/clusters/
--rw-r--r--   0 runner    (1001) docker     (121)      250 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/packer/clusters/ubuntu.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/packer/packer/
--rw-r--r--   0 runner    (1001) docker     (121)      554 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/packer/packer/ubuntu.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/terraform-and-ansible/
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      708 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/terraform-and-ansible/ansible/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/ansible/ansible.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/terraform-and-ansible/ansible/playbooks/
--rw-r--r--   0 runner    (1001) docker     (121)      408 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/ansible/playbooks/site.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.445292 ops-cli-2.1.7/examples/features/terraform-and-ansible/ansible/roles/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.441292 ops-cli-2.1.7/examples/features/terraform-and-ansible/ansible/roles/common/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/terraform-and-ansible/ansible/roles/common/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/ansible/roles/common/tasks/main.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.445292 ops-cli-2.1.7/examples/features/terraform-and-ansible/ansible/roles/db/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/terraform-and-ansible/ansible/roles/db/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/ansible/roles/db/tasks/main.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.445292 ops-cli-2.1.7/examples/features/terraform-and-ansible/ansible/roles/web/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/terraform-and-ansible/ansible/roles/web/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/ansible/roles/web/tasks/main.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/terraform-and-ansible/ansible/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      401 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/ansible/tasks/copy-key.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/terraform-and-ansible/clusters/
--rw-r--r--   0 runner    (1001) docker     (121)      983 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/clusters/example.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/main/
--rw-r--r--   0 runner    (1001) docker     (121)      727 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/main/main.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/main/shared_variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/db/
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/db/instance.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      809 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/db/main.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)     2874 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/macros.tf.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/shared_iam/
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/shared_iam/default_policy.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/vpc/
--rw-r--r--   0 runner    (1001) docker     (121)     7257 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/vpc/main.tf.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.461292 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/web/
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/web/elb.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/web/instance.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/web/main.tf.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/user_data
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.465292 ops-cli-2.1.7/examples/features/terraform-hierarchical/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-hierarchical/.opsconfig.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      677 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-hierarchical/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.445292 ops-cli-2.1.7/examples/features/terraform-hierarchical/compositions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.445292 ops-cli-2.1.7/examples/features/terraform-hierarchical/compositions/terraform/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.465292 ops-cli-2.1.7/examples/features/terraform-hierarchical/compositions/terraform/cluster/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-hierarchical/compositions/terraform/cluster/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.465292 ops-cli-2.1.7/examples/features/terraform-hierarchical/compositions/terraform/network/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-hierarchical/compositions/terraform/network/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.445292 ops-cli-2.1.7/examples/features/terraform-hierarchical/config/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.465292 ops-cli-2.1.7/examples/features/terraform-hierarchical/config/env=dev/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.465292 ops-cli-2.1.7/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.465292 ops-cli-2.1.7/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster1/composition=cluster/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster1/composition=cluster/conf.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.465292 ops-cli-2.1.7/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster1/composition=network/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster1/composition=network/conf.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster1/conf.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.465292 ops-cli-2.1.7/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.465292 ops-cli-2.1.7/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster2/composition=cluster/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster2/composition=cluster/conf.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.465292 ops-cli-2.1.7/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster2/composition=network/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster2/composition=network/conf.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster2/conf.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      206 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-hierarchical/config/env=dev/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.445292 ops-cli-2.1.7/examples/features/terraform-hierarchical/modules/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.465292 ops-cli-2.1.7/examples/features/terraform-hierarchical/modules/cluster/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-hierarchical/modules/cluster/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.465292 ops-cli-2.1.7/examples/features/terraform-hierarchical/modules/network/
--rw-r--r--   0 runner    (1001) docker     (121)      359 2021-10-14 14:16:23.000000 ops-cli-2.1.7/examples/features/terraform-hierarchical/modules/network/main.tf
--rw-r--r--   0 runner    (1001) docker     (121)     4195 2021-10-14 14:17:35.000000 ops-cli-2.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-10-14 14:17:39.473292 ops-cli-2.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2553 2021-10-14 14:16:23.000000 ops-cli-2.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.449292 ops-cli-2.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.465292 ops-cli-2.1.7/src/ops/
--rw-r--r--   0 runner    (1001) docker     (121)     3492 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.465292 ops-cli-2.1.7/src/ops/ansible/
--rw-r--r--   0 runner    (1001) docker     (121)      603 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/ansible/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.469292 ops-cli-2.1.7/src/ops/ansible/callback_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      596 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/ansible/callback_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.469292 ops-cli-2.1.7/src/ops/ansible/filter_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      596 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/ansible/filter_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5595 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/ansible/filter_plugins/commonfilters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.469292 ops-cli-2.1.7/src/ops/ansible/vars_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      596 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/ansible/vars_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/ansible/vars_plugins/clusterconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/ansible/vars_plugins/opsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.469292 ops-cli-2.1.7/src/ops/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      873 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/cli/aws.py
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1718 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/cli/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6354 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/cli/helmfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     3101 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/cli/inventory.py
--rw-r--r--   0 runner    (1001) docker     (121)     2626 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/cli/packer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4377 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     5287 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/cli/playbook.py
--rw-r--r--   0 runner    (1001) docker     (121)     3373 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (121)    13182 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/cli/ssh.py
--rw-r--r--   0 runner    (1001) docker     (121)     5663 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/cli/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)    12446 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/cli/terraform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.445292 ops-cli-2.1.7/src/ops/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.469292 ops-cli-2.1.7/src/ops/data/ansible/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/data/ansible/ansible.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.469292 ops-cli-2.1.7/src/ops/data/ansible/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      888 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/data/ansible/tasks/deploy_prometheus_alert_rules.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2334 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/data/ansible/tasks/install_rpm.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/data/ansible/tasks/remove_prometheus_alert_rules.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.469292 ops-cli-2.1.7/src/ops/data/ssh/
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/data/ssh/ssh.config
--rw-r--r--   0 runner    (1001) docker     (121)      536 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/data/ssh/ssh.scb.proxy.config.tpl
--rw-r--r--   0 runner    (1001) docker     (121)      364 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/data/ssh/ssh.tunnel.config
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.469292 ops-cli-2.1.7/src/ops/data/terraform/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/data/terraform/terraformrc
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/git_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.469292 ops-cli-2.1.7/src/ops/hierarchical/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/hierarchical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7219 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/hierarchical/composition_config_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.473292 ops-cli-2.1.7/src/ops/inventory/
--rw-r--r--   0 runner    (1001) docker     (121)    17616 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/inventory/SKMS.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33507 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/inventory/azurerm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2000 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/inventory/caching.py
--rw-r--r--   0 runner    (1001) docker     (121)    11179 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/inventory/ec2inventory.py
--rw-r--r--   0 runner    (1001) docker     (121)    10885 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/inventory/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.473292 ops-cli-2.1.7/src/ops/inventory/plugin/
--rw-r--r--   0 runner    (1001) docker     (121)      725 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/inventory/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5910 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/inventory/plugin/azr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/inventory/plugin/cns.py
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/inventory/plugin/ec2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/inventory/plugin/legacy_pcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8517 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/inventory/plugin/skms.py
--rw-r--r--   0 runner    (1001) docker     (121)     4432 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/inventory/sshconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.473292 ops-cli-2.1.7/src/ops/jinja/
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/jinja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6988 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     5847 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/opsconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     4089 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/simpleconsul.py
--rw-r--r--   0 runner    (1001) docker     (121)     1703 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/simplessm.py
--rw-r--r--   0 runner    (1001) docker     (121)    10123 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/simplevault.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.473292 ops-cli-2.1.7/src/ops/terraform/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/terraform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21428 2021-10-14 14:16:23.000000 ops-cli-2.1.7/src/ops/terraform/terraform_cmd_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 14:17:39.473292 ops-cli-2.1.7/src/ops_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    32484 2021-10-14 14:17:39.000000 ops-cli-2.1.7/src/ops_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8420 2021-10-14 14:17:39.000000 ops-cli-2.1.7/src/ops_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-14 14:17:39.000000 ops-cli-2.1.7/src/ops_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-14 14:17:39.000000 ops-cli-2.1.7/src/ops_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3949 2021-10-14 14:17:39.000000 ops-cli-2.1.7/src/ops_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-10-14 14:17:39.000000 ops-cli-2.1.7/src/ops_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.766454 ops-cli-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-08-01 14:10:42.000000 ops-cli-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 14:10:42.000000 ops-cli-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    32366 2023-08-01 14:11:26.766454 ops-cli-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31261 2023-08-01 14:10:42.000000 ops-cli-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.738453 ops-cli-2.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.746454 ops-cli-2.2.0/examples/aws-kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/.opsconfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.746454 ops-cli-2.2.0/examples/aws-kubernetes/clusters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.746454 ops-cli-2.2.0/examples/aws-kubernetes/clusters/kubeconfigs/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/clusters/kubeconfigs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/clusters/my-kubernetes-cluster.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.738453 ops-cli-2.2.0/examples/aws-kubernetes/compositions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.738453 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.746454 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/backends.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/common_variables.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/configure-local-kubectl.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/eks-cluster-autoscaler.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/eks-cluster.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/eks-worker-nodes-auth-configmap.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/eks-worker-nodes.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/outputs.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/providers.tf.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.746454 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      599 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/scripts/fileexist.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/variables.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/vpc.tf.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.746454 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/common/backends.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/common/common_variables.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/common/providers.tf.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.750454 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm/backends.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm/cluster-autoscaler.tf
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm/common_variables.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm/dashboard.tf
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm/kube-state-metrics.tf
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm/kube2iam.tf
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm/provider_helm.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm/providers.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm/variables.tf.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.750454 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm-init/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm-init/backends.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm-init/helm-init.tf.jinja2
+-rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/aws-kubernetes/update.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.750454 ops-cli-2.2.0/examples/cassandra-stress/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/.opsconfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.750454 ops-cli-2.2.0/examples/cassandra-stress/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/ansible/install_stress_tool.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/ansible/setup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/ansible/setup12.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.750454 ops-cli-2.2.0/examples/cassandra-stress/ansible/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14497 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/ansible/templates/cassandra-env.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)    41784 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/ansible/templates/cassandra_defaults.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32926 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/ansible/templates/cassandra_defaults_12.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/ansible/templates/stress.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/cluster1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/cluster2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.750454 ops-cli-2.2.0/examples/cassandra-stress/terraform/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.750454 ops-cli-2.2.0/examples/cassandra-stress/terraform/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/terraform/main/main.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/terraform/main/variables.tf.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.750454 ops-cli-2.2.0/examples/cassandra-stress/terraform/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.750454 ops-cli-2.2.0/examples/cassandra-stress/terraform/modules/cassandra/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/terraform/modules/cassandra/main.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/terraform/modules/macros.tf.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.750454 ops-cli-2.2.0/examples/cassandra-stress/terraform/modules/shared_iam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/terraform/modules/shared_iam/default_policy.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.750454 ops-cli-2.2.0/examples/cassandra-stress/terraform/modules/vpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/terraform/modules/vpc/main.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/cassandra-stress/terraform/user_data
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.742453 ops-cli-2.2.0/examples/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.750454 ops-cli-2.2.0/examples/features/ansible-vault/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/ansible-vault/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.742453 ops-cli-2.2.0/examples/features/ansible-vault/cluster/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.750454 ops-cli-2.2.0/examples/features/ansible-vault/cluster/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/ansible-vault/cluster/dev/dev.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.750454 ops-cli-2.2.0/examples/features/ansible-vault/cluster/prod/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/ansible-vault/cluster/prod/prod.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.750454 ops-cli-2.2.0/examples/features/ansible-vault/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/ansible-vault/inventory/hosts
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/ansible-vault/password_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/ansible-vault/password_prod.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.750454 ops-cli-2.2.0/examples/features/ansible-vault/playbook/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/ansible-vault/playbook/example.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/ansible-vault/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/ansible-vault/vault/vault_dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/ansible-vault/vault/vault_prod.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/inventory/.opsconfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/inventory/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/inventory/local_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/inventory/local_inventory/hosts
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/inventory/my-aws-cluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/inventory/my-azure-cluster.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/packer/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/packer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/packer/clusters/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/packer/clusters/ubuntu.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/packer/packer/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/packer/packer/ubuntu.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-and-ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-and-ansible/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/ansible/ansible.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-and-ansible/ansible/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/ansible/playbooks/site.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.742453 ops-cli-2.2.0/examples/features/terraform-and-ansible/ansible/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.742453 ops-cli-2.2.0/examples/features/terraform-and-ansible/ansible/roles/common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-and-ansible/ansible/roles/common/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/ansible/roles/common/tasks/main.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.742453 ops-cli-2.2.0/examples/features/terraform-and-ansible/ansible/roles/db/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-and-ansible/ansible/roles/db/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/ansible/roles/db/tasks/main.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.742453 ops-cli-2.2.0/examples/features/terraform-and-ansible/ansible/roles/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-and-ansible/ansible/roles/web/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/ansible/roles/web/tasks/main.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-and-ansible/ansible/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/ansible/tasks/copy-key.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-and-ansible/clusters/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/clusters/example.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/main/main.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/main/shared_variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/db/instance.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/db/main.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/macros.tf.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/shared_iam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/shared_iam/default_policy.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/vpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/vpc/main.tf.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/web/elb.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/web/instance.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/web/main.tf.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/user_data
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-hierarchical/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-hierarchical/.opsconfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-hierarchical/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.742453 ops-cli-2.2.0/examples/features/terraform-hierarchical/compositions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.742453 ops-cli-2.2.0/examples/features/terraform-hierarchical/compositions/terraform/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.754454 ops-cli-2.2.0/examples/features/terraform-hierarchical/compositions/terraform/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-hierarchical/compositions/terraform/cluster/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.758454 ops-cli-2.2.0/examples/features/terraform-hierarchical/compositions/terraform/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-hierarchical/compositions/terraform/network/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.742453 ops-cli-2.2.0/examples/features/terraform-hierarchical/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.758454 ops-cli-2.2.0/examples/features/terraform-hierarchical/config/env=dev/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.758454 ops-cli-2.2.0/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.758454 ops-cli-2.2.0/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster1/composition=cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster1/composition=cluster/conf.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.758454 ops-cli-2.2.0/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster1/composition=network/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster1/composition=network/conf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster1/conf.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.758454 ops-cli-2.2.0/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.758454 ops-cli-2.2.0/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster2/composition=cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster2/composition=cluster/conf.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.758454 ops-cli-2.2.0/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster2/composition=network/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster2/composition=network/conf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-hierarchical/config/env=dev/cluster=cluster2/conf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-hierarchical/config/env=dev/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.742453 ops-cli-2.2.0/examples/features/terraform-hierarchical/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.758454 ops-cli-2.2.0/examples/features/terraform-hierarchical/modules/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-hierarchical/modules/cluster/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.758454 ops-cli-2.2.0/examples/features/terraform-hierarchical/modules/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-01 14:10:42.000000 ops-cli-2.2.0/examples/features/terraform-hierarchical/modules/network/main.tf
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-08-01 14:11:23.000000 ops-cli-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-01 14:11:26.766454 ops-cli-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-08-01 14:10:42.000000 ops-cli-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.742453 ops-cli-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.758454 ops-cli-2.2.0/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.758454 ops-cli-2.2.0/src/ops/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/ansible/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.758454 ops-cli-2.2.0/src/ops/ansible/callback_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/ansible/callback_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.758454 ops-cli-2.2.0/src/ops/ansible/filter_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/ansible/filter_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/ansible/filter_plugins/commonfilters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.758454 ops-cli-2.2.0/src/ops/ansible/vars_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/ansible/vars_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/ansible/vars_plugins/clusterconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/ansible/vars_plugins/opsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.762454 ops-cli-2.2.0/src/ops/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/cli/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/cli/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/cli/helmfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/cli/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/cli/packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/cli/playbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/cli/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/cli/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/cli/terraform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.742453 ops-cli-2.2.0/src/ops/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.762454 ops-cli-2.2.0/src/ops/data/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/data/ansible/ansible.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.762454 ops-cli-2.2.0/src/ops/data/ansible/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/data/ansible/tasks/deploy_prometheus_alert_rules.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/data/ansible/tasks/install_rpm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/data/ansible/tasks/remove_prometheus_alert_rules.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.762454 ops-cli-2.2.0/src/ops/data/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/data/ssh/ssh.config
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/data/ssh/ssh.scb.proxy.config.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/data/ssh/ssh.tunnel.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.762454 ops-cli-2.2.0/src/ops/data/terraform/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/data/terraform/terraformrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/git_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.762454 ops-cli-2.2.0/src/ops/hierarchical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/hierarchical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/hierarchical/composition_config_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.762454 ops-cli-2.2.0/src/ops/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)    17616 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/inventory/SKMS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33507 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/inventory/azurerm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/inventory/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/inventory/ec2inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/inventory/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.762454 ops-cli-2.2.0/src/ops/inventory/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/inventory/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/inventory/plugin/azr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/inventory/plugin/cns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/inventory/plugin/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/inventory/plugin/legacy_pcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/inventory/plugin/skms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/inventory/sshconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.762454 ops-cli-2.2.0/src/ops/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/jinja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/opsconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/simpleconsul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/simplessm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/simplevault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.762454 ops-cli-2.2.0/src/ops/terraform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/terraform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21428 2023-08-01 14:10:42.000000 ops-cli-2.2.0/src/ops/terraform/terraform_cmd_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:11:26.766454 ops-cli-2.2.0/src/ops_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    32366 2023-08-01 14:11:26.000000 ops-cli-2.2.0/src/ops_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-08-01 14:11:26.000000 ops-cli-2.2.0/src/ops_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:11:26.000000 ops-cli-2.2.0/src/ops_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-01 14:11:26.000000 ops-cli-2.2.0/src/ops_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-08-01 14:11:26.000000 ops-cli-2.2.0/src/ops_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-01 14:11:26.000000 ops-cli-2.2.0/src/ops_cli.egg-info/top_level.txt
```

### Comparing `ops-cli-2.1.7/LICENSE` & `ops-cli-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/PKG-INFO` & `ops-cli-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: ops-cli
-Version: 2.1.7
+Version: 2.2.0
 Summary: Ops - wrapper for Terraform, Ansible, and SSH for cloud automation
 Home-page: https://github.com/adobe/ops-cli
 Author: Adobe
 Author-email: noreply@adobe.com
 License: Apache2
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
@@ -175,15 +172,15 @@
 # create virtualenv
 mkvirtualenv ops
 workon ops
 
 # uninstall previous `ops` version (if you have it)
 pip uninstall ops --yes
 
-# install ops-cli v2.1.7 stable release
+# install ops-cli v2.2.0 stable release
 pip install --upgrade ops-cli
 ```
 
 
 ### Terraform
 Optionally, install terraform to be able to access terraform plugin. See https://www.terraform.io/intro/getting-started/install.html
 Also for pretty formatting of terraform plan output you can install https://github.com/coinbase/terraform-landscape (use gem install for MacOS)
@@ -191,15 +188,15 @@
 
 ## Using docker image
 
 You can try out `ops-cli`, by using docker. The docker image has all required prerequisites (python, terraform, helm, git, ops-cli etc).
 
 To start out a container, running the latest `ops-cli` docker image run:
 ```sh
-docker run -it ghcr.io/adobe/ops-cli:2.1.7 bash
+docker run -it ghcr.io/adobe/ops-cli:2.2.0 bash
 ```
 
 After the container has started, you can start using `ops-cli`:
 ```sh
 ops help
 # usage: ops [-h] [--root-dir ROOT_DIR] [--verbose] [-e EXTRA_VARS]
 #           cluster_config_path
@@ -806,9 +803,7 @@
     brew link openssl --force
 ```
 
 # License
 [Apache License 2.0](/LICENSE)
 
 
-
-
```

### Comparing `ops-cli-2.1.7/README.md` & `ops-cli-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 # create virtualenv
 mkvirtualenv ops
 workon ops
 
 # uninstall previous `ops` version (if you have it)
 pip uninstall ops --yes
 
-# install ops-cli v2.1.7 stable release
+# install ops-cli v2.2.0 stable release
 pip install --upgrade ops-cli
 ```
 
 
 ### Terraform
 Optionally, install terraform to be able to access terraform plugin. See https://www.terraform.io/intro/getting-started/install.html
 Also for pretty formatting of terraform plan output you can install https://github.com/coinbase/terraform-landscape (use gem install for MacOS)
@@ -162,15 +162,15 @@
 
 ## Using docker image
 
 You can try out `ops-cli`, by using docker. The docker image has all required prerequisites (python, terraform, helm, git, ops-cli etc).
 
 To start out a container, running the latest `ops-cli` docker image run:
 ```sh
-docker run -it ghcr.io/adobe/ops-cli:2.1.7 bash
+docker run -it ghcr.io/adobe/ops-cli:2.2.0 bash
 ```
 
 After the container has started, you can start using `ops-cli`:
 ```sh
 ops help
 # usage: ops [-h] [--root-dir ROOT_DIR] [--verbose] [-e EXTRA_VARS]
 #           cluster_config_path
```

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/README.md` & `ops-cli-2.2.0/examples/aws-kubernetes/README.md`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/clusters/my-kubernetes-cluster.yaml` & `ops-cli-2.2.0/examples/aws-kubernetes/clusters/my-kubernetes-cluster.yaml`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/backends.tf.jinja2` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/backends.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/common_variables.tf.jinja2` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/common_variables.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/configure-local-kubectl.tf.jinja2` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/configure-local-kubectl.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/eks-cluster-autoscaler.tf.jinja2` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/eks-cluster-autoscaler.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/eks-cluster.tf.jinja2` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/eks-cluster.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/eks-worker-nodes.tf.jinja2` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/eks-worker-nodes.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/outputs.tf.jinja2` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/outputs.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/scripts/fileexist.sh` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/scripts/fileexist.sh`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/variables.tf.jinja2` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/variables.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/aws-eks/vpc.tf.jinja2` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/aws-eks/vpc.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/common/backends.tf.jinja2` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/common/backends.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/common/common_variables.tf.jinja2` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/common/common_variables.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm/backends.tf.jinja2` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm/backends.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm/cluster-autoscaler.tf` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm/cluster-autoscaler.tf`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm/common_variables.tf.jinja2` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm/common_variables.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm/dashboard.tf` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm/dashboard.tf`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/compositions/generic/helm-init/backends.tf.jinja2` & `ops-cli-2.2.0/examples/aws-kubernetes/compositions/generic/helm-init/backends.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/aws-kubernetes/update.sh` & `ops-cli-2.2.0/examples/aws-kubernetes/update.sh`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/cassandra-stress/README.md` & `ops-cli-2.2.0/examples/cassandra-stress/README.md`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/cassandra-stress/ansible/setup.yaml` & `ops-cli-2.2.0/examples/cassandra-stress/ansible/setup.yaml`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/cassandra-stress/ansible/setup12.yaml` & `ops-cli-2.2.0/examples/cassandra-stress/ansible/setup12.yaml`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/cassandra-stress/ansible/templates/cassandra-env.sh` & `ops-cli-2.2.0/examples/cassandra-stress/ansible/templates/cassandra-env.sh`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/cassandra-stress/ansible/templates/cassandra_defaults.yaml` & `ops-cli-2.2.0/examples/cassandra-stress/ansible/templates/cassandra_defaults.yaml`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/cassandra-stress/ansible/templates/cassandra_defaults_12.yaml` & `ops-cli-2.2.0/examples/cassandra-stress/ansible/templates/cassandra_defaults_12.yaml`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/cassandra-stress/ansible/templates/stress.yaml` & `ops-cli-2.2.0/examples/cassandra-stress/ansible/templates/stress.yaml`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/cassandra-stress/cluster1.yaml` & `ops-cli-2.2.0/examples/cassandra-stress/cluster1.yaml`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/cassandra-stress/cluster2.yaml` & `ops-cli-2.2.0/examples/cassandra-stress/cluster2.yaml`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/cassandra-stress/terraform/main/main.tf.jinja2` & `ops-cli-2.2.0/examples/cassandra-stress/terraform/main/main.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/cassandra-stress/terraform/main/variables.tf.jinja2` & `ops-cli-2.2.0/examples/cassandra-stress/terraform/main/variables.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/cassandra-stress/terraform/modules/cassandra/main.tf.jinja2` & `ops-cli-2.2.0/examples/cassandra-stress/terraform/modules/cassandra/main.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/cassandra-stress/terraform/modules/macros.tf.jinja2` & `ops-cli-2.2.0/examples/cassandra-stress/terraform/modules/macros.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/cassandra-stress/terraform/modules/shared_iam/default_policy.json` & `ops-cli-2.2.0/examples/cassandra-stress/terraform/modules/shared_iam/default_policy.json`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/cassandra-stress/terraform/modules/vpc/main.tf.jinja2` & `ops-cli-2.2.0/examples/cassandra-stress/terraform/modules/vpc/main.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/features/ansible-vault/README.md` & `ops-cli-2.2.0/examples/features/ansible-vault/README.md`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/features/inventory/README.md` & `ops-cli-2.2.0/examples/features/inventory/README.md`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/features/packer/packer/ubuntu.json` & `ops-cli-2.2.0/examples/features/packer/packer/ubuntu.json`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/features/terraform-and-ansible/README.md` & `ops-cli-2.2.0/examples/features/terraform-and-ansible/README.md`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/features/terraform-and-ansible/clusters/example.yaml` & `ops-cli-2.2.0/examples/features/terraform-and-ansible/clusters/example.yaml`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/main/main.tf.jinja2` & `ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/main/main.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/main/shared_variables.tf` & `ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/main/shared_variables.tf`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/db/instance.tf.jinja2` & `ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/db/instance.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/db/main.tf.jinja2` & `ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/db/main.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/macros.tf.jinja2` & `ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/macros.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/shared_iam/default_policy.json` & `ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/shared_iam/default_policy.json`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/vpc/main.tf.jinja2` & `ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/vpc/main.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/web/elb.tf.jinja2` & `ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/web/elb.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/web/instance.tf.jinja2` & `ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/web/instance.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/features/terraform-and-ansible/terraform/modules/web/main.tf.jinja2` & `ops-cli-2.2.0/examples/features/terraform-and-ansible/terraform/modules/web/main.tf.jinja2`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/examples/features/terraform-hierarchical/README.md` & `ops-cli-2.2.0/examples/features/terraform-hierarchical/README.md`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/requirements.txt` & `ops-cli-2.2.0/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 adal==1.2.7
-ansible==2.9.25
-awscli==1.20.33
-azure-applicationinsights==0.1.0
+ansible==8.2.0
+ansible-core==2.15.2; python_version >= '3.9'
+awscli==1.29.12
+azure==4.0.0
+azure-applicationinsights==0.1.1
 azure-batch==4.1.3
-azure-common==1.1.27
+azure-common==1.1.28
+azure-core==1.28.0; python_version >= '3.7'
 azure-cosmosdb-nspkg==2.0.2
 azure-cosmosdb-table==1.0.6
-azure-datalake-store==0.0.52
+azure-datalake-store==0.0.53
 azure-eventgrid==1.3.0
 azure-graphrbac==0.40.0
 azure-keyvault==1.1.0
-azure-loganalytics==0.1.0
+azure-loganalytics==0.1.1
+azure-mgmt==4.0.0
 azure-mgmt-advisor==1.0.1
 azure-mgmt-applicationinsights==0.1.1
 azure-mgmt-authorization==0.50.0
 azure-mgmt-batch==5.0.1
 azure-mgmt-batchai==2.0.0
 azure-mgmt-billing==0.2.0
 azure-mgmt-cdn==3.1.0
@@ -44,15 +48,15 @@
 azure-mgmt-loganalytics==0.2.0
 azure-mgmt-logic==3.0.0
 azure-mgmt-machinelearningcompute==0.4.1
 azure-mgmt-managementgroups==0.1.0
 azure-mgmt-managementpartner==0.1.1
 azure-mgmt-maps==0.1.0
 azure-mgmt-marketplaceordering==0.1.0
-azure-mgmt-media==1.0.0
+azure-mgmt-media==1.0.1
 azure-mgmt-monitor==0.5.2
 azure-mgmt-msi==0.2.0
 azure-mgmt-network==2.7.0
 azure-mgmt-notificationhubs==2.1.0
 azure-mgmt-nspkg==3.0.2
 azure-mgmt-policyinsights==0.1.0
 azure-mgmt-powerbiembedded==2.0.0
@@ -69,65 +73,68 @@
 azure-mgmt-servicefabric==0.2.0
 azure-mgmt-signalr==0.1.1
 azure-mgmt-sql==0.9.1
 azure-mgmt-storage==2.0.0
 azure-mgmt-subscription==0.2.0
 azure-mgmt-trafficmanager==0.50.0
 azure-mgmt-web==0.35.0
-azure-mgmt==4.0.0
 azure-nspkg==3.0.2
 azure-servicebus==0.21.1
 azure-servicefabric==6.3.0.0
 azure-servicemanagement-legacy==0.20.7
 azure-storage-blob==1.5.0
 azure-storage-common==1.4.2
 azure-storage-file==1.4.0
 azure-storage-queue==1.4.0
-azure==4.0.0
-backports.functools-lru-cache==1.6.4; python_version >= '2.6'
-boto3==1.18.33
+backports.functools-lru-cache==1.6.6; python_version >= '2.6'
 boto==2.49.0
-botocore==1.21.33; python_version >= '3.6'
-cachetools==4.2.4; python_version ~= '3.5'
-certifi==2021.10.8
-cffi==1.15.0
-charset-normalizer==2.0.7; python_version >= '3'
-colorama==0.4.3; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
-cryptography==35.0.0; python_version >= '3.6'
-deepmerge==0.3.0; python_version >= '3'
-docutils==0.15.2; python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2'
-gitdb==4.0.7; python_version >= '3.4'
-gitpython==3.1.24
-google-auth==2.3.0; python_version >= '3.6'
+boto3==1.28.12
+botocore==1.31.12; python_version >= '3.7'
+cachetools==5.3.1; python_version >= '3.7'
+certifi==2023.7.22; python_version >= '3.6'
+cffi==1.15.1
+charset-normalizer==3.2.0; python_full_version >= '3.7.0'
+colorama==0.4.4; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
+cryptography==41.0.2; python_version >= '3.7'
+deepmerge==1.1.0
+docutils==0.16; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
+gitdb==4.0.10; python_version >= '3.7'
+gitpython==3.1.32
+google-auth==2.22.0; python_version >= '3.6'
 hashmerge==0.2
-himl==0.7.3
-hvac==0.11.0
-idna==3.3; python_version >= '3'
-inflection==0.3.1
-isodate==0.6.0
-jinja2==2.11.3
-jmespath==0.10.0; python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2'
-kubernetes==18.20.0
+himl==0.15.0
+hvac==1.1.1
+idna==3.4; python_version >= '3.5'
+inflection==0.5.1
+isodate==0.6.1
+jinja2==3.1.2
+jmespath==1.0.1; python_version >= '3.7'
+kubernetes==26.1.0
 lru-cache==0.2.3
-markupsafe==2.0.1; python_version >= '3.6'
-msrest==0.6.21
+markupsafe==2.1.3; python_version >= '3.7'
+msal==1.23.0
+msrest==0.7.1; python_version >= '3.6'
 msrestazure==0.6.4
-oauthlib==3.1.1; python_version >= '3.6'
+oauthlib==3.2.2; python_version >= '3.6'
+packaging==23.1; python_version >= '3.7'
 passgen==1.1.1
-pathlib2==2.3.6
-pyasn1-modules==0.2.8
-pyasn1==0.4.8
-pycparser==2.20; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-pyjwt==2.2.0; python_version >= '3.6'
+pathlib2==2.3.7.post1
+pyasn1==0.5.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
+pyasn1-modules==0.3.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
+pycparser==2.21
+pyhcl==0.4.4
+pyjwt==2.8.0; python_version >= '3.7'
 python-consul==1.1.0
 python-dateutil==2.8.2; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'
-pyyaml==5.4.1
-requests-oauthlib==1.3.0
-requests==2.26.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
+pyyaml==6.0.1; python_version >= '3.6'
+requests==2.31.0; python_version >= '3.7'
+requests-oauthlib==1.3.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
+resolvelib==1.0.1
 rsa==4.7.2; python_version >= '3.5' and python_version < '4'
-s3transfer==0.5.0; python_version >= '3.6'
-simpledi==0.3
+s3transfer==0.6.1; python_version >= '3.7'
+setuptools==68.0.0; python_version >= '3.7'
+simpledi==0.4.1
 six==1.16.0
-smmap==4.0.0; python_version >= '3.5'
-typing-extensions==3.10.0.2; python_version < '3.10'
-urllib3==1.26.7; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'
-websocket-client==1.2.1; python_version >= '3.6'
+smmap==5.0.0; python_version >= '3.6'
+typing-extensions==4.7.1; python_version >= '3.7'
+urllib3==1.26.16; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
+websocket-client==1.6.1; python_version >= '3.7'
```

### Comparing `ops-cli-2.1.7/setup.py` & `ops-cli-2.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 with open('README.md') as f:
     _readme = f.read()
 
 _mydir = os.path.abspath(os.path.dirname(sys.argv[0]))
 _requires = [r for r in open(os.path.sep.join((_mydir, 'requirements.txt')), "r").read().split('\n') if len(r) > 1]
 setup(
     name='ops-cli',
-    version='2.1.7',
+    version='2.2.0',
     description='Ops - wrapper for Terraform, Ansible, and SSH for cloud automation',
     long_description=_readme + '\n\n',
     long_description_content_type='text/markdown',
     url='https://github.com/adobe/ops-cli',
     python_requires='>=3.5',
     author='Adobe',
     author_email='noreply@adobe.com',
@@ -35,19 +35,17 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Text Processing :: Markup :: HTML'
     ],
     package_dir={'': 'src'},
```

### Comparing `ops-cli-2.1.7/src/ops/__init__.py` & `ops-cli-2.2.0/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/ansible/__init__.py` & `ops-cli-2.2.0/src/ops/ansible/__init__.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/ansible/callback_plugins/__init__.py` & `ops-cli-2.2.0/src/ops/ansible/callback_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/ansible/filter_plugins/__init__.py` & `ops-cli-2.2.0/src/ops/ansible/filter_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/ansible/filter_plugins/commonfilters.py` & `ops-cli-2.2.0/src/ops/ansible/filter_plugins/commonfilters.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/ansible/vars_plugins/__init__.py` & `ops-cli-2.2.0/src/ops/ansible/vars_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/ansible/vars_plugins/clusterconfig.py` & `ops-cli-2.2.0/src/ops/ansible/vars_plugins/clusterconfig.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/ansible/vars_plugins/opsconfig.py` & `ops-cli-2.2.0/src/ops/ansible/vars_plugins/opsconfig.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/cli/__init__.py` & `ops-cli-2.2.0/src/ops/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/cli/config.py` & `ops-cli-2.2.0/src/ops/cli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
             get_cluster_name(
                 self.cluster_config_path))
 
         context_cliargs = dict(context.CLIARGS)
         context_cliargs['extra_vars'] = tuple(extra_vars)
 
         context.CLIARGS = ImmutableDict(context_cliargs)
+        setattr(load_extra_vars, 'extra_vars', {})
         variable_manager._extra_vars = load_extra_vars(
             loader=data_loader)
 
         variables = variable_manager.get_vars()
 
         rendered = self.template.render(self.cluster_config_path, variables)
 
@@ -154,16 +155,19 @@
                 self.cluster_config_path))
         extra_vars.extend(configurations)
 
         context_cliargs = dict(context.CLIARGS)
         context_cliargs['extra_vars'] = tuple(extra_vars)
 
         context.CLIARGS = ImmutableDict(context_cliargs)
+        setattr(load_extra_vars, 'extra_vars', {})
         variable_manager._extra_vars = load_extra_vars(
             loader=data_loader)
 
         read_variables = variable_manager.get_vars()
 
         templar = Templar(data_loader, variables=read_variables)
-        templar._filter_loader = self.template.filter_plugin_loader
+
+        for filter in self.template.filter_plugin_loader.all():
+            templar.environment.filters.update(filter.filters())
 
         return templar.template(read_variables, fail_on_undefined=True)
```

### Comparing `ops-cli-2.1.7/src/ops/cli/config_generator.py` & `ops-cli-2.2.0/src/ops/cli/config_generator.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/cli/helmfile.py` & `ops-cli-2.2.0/src/ops/cli/helmfile.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/cli/inventory.py` & `ops-cli-2.2.0/src/ops/cli/inventory.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/cli/packer.py` & `ops-cli-2.2.0/src/ops/cli/packer.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/cli/parser.py` & `ops-cli-2.2.0/src/ops/cli/parser.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/cli/playbook.py` & `ops-cli-2.2.0/src/ops/cli/playbook.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/cli/run.py` & `ops-cli-2.2.0/src/ops/cli/run.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/cli/ssh.py` & `ops-cli-2.2.0/src/ops/cli/ssh.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/cli/sync.py` & `ops-cli-2.2.0/src/ops/cli/sync.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/cli/terraform.py` & `ops-cli-2.2.0/src/ops/cli/terraform.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/data/ansible/tasks/deploy_prometheus_alert_rules.yml` & `ops-cli-2.2.0/src/ops/data/ansible/tasks/deploy_prometheus_alert_rules.yml`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/data/ansible/tasks/install_rpm.yml` & `ops-cli-2.2.0/src/ops/data/ansible/tasks/install_rpm.yml`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/data/ansible/tasks/remove_prometheus_alert_rules.yml` & `ops-cli-2.2.0/src/ops/data/ansible/tasks/remove_prometheus_alert_rules.yml`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/data/ssh/ssh.config` & `ops-cli-2.2.0/src/ops/data/ssh/ssh.config`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/data/ssh/ssh.scb.proxy.config.tpl` & `ops-cli-2.2.0/src/ops/data/ssh/ssh.scb.proxy.config.tpl`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/git_utils.py` & `ops-cli-2.2.0/src/ops/git_utils.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/hierarchical/composition_config_generator.py` & `ops-cli-2.2.0/src/ops/hierarchical/composition_config_generator.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/inventory/SKMS.py` & `ops-cli-2.2.0/src/ops/inventory/SKMS.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/inventory/__init__.py` & `ops-cli-2.2.0/src/ops/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/inventory/azurerm.py` & `ops-cli-2.2.0/src/ops/inventory/azurerm.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/inventory/caching.py` & `ops-cli-2.2.0/src/ops/inventory/caching.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/inventory/ec2inventory.py` & `ops-cli-2.2.0/src/ops/inventory/ec2inventory.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/inventory/generator.py` & `ops-cli-2.2.0/src/ops/inventory/generator.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/inventory/plugin/__init__.py` & `ops-cli-2.2.0/src/ops/inventory/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/inventory/plugin/azr.py` & `ops-cli-2.2.0/src/ops/inventory/plugin/azr.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/inventory/plugin/cns.py` & `ops-cli-2.2.0/src/ops/inventory/plugin/cns.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/inventory/plugin/ec2.py` & `ops-cli-2.2.0/src/ops/inventory/plugin/ec2.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/inventory/plugin/legacy_pcs.py` & `ops-cli-2.2.0/src/ops/inventory/plugin/legacy_pcs.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/inventory/plugin/skms.py` & `ops-cli-2.2.0/src/ops/inventory/plugin/skms.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/inventory/sshconfig.py` & `ops-cli-2.2.0/src/ops/inventory/sshconfig.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/jinja/__init__.py` & `ops-cli-2.2.0/src/ops/jinja/__init__.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/main.py` & `ops-cli-2.2.0/src/ops/main.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/opsconfig.py` & `ops-cli-2.2.0/src/ops/opsconfig.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/simpleconsul.py` & `ops-cli-2.2.0/src/ops/simpleconsul.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/simplessm.py` & `ops-cli-2.2.0/src/ops/simplessm.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/simplevault.py` & `ops-cli-2.2.0/src/ops/simplevault.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops/terraform/terraform_cmd_generator.py` & `ops-cli-2.2.0/src/ops/terraform/terraform_cmd_generator.py`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops_cli.egg-info/PKG-INFO` & `ops-cli-2.2.0/src/ops_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: ops-cli
-Version: 2.1.7
+Version: 2.2.0
 Summary: Ops - wrapper for Terraform, Ansible, and SSH for cloud automation
 Home-page: https://github.com/adobe/ops-cli
 Author: Adobe
 Author-email: noreply@adobe.com
 License: Apache2
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
@@ -175,15 +172,15 @@
 # create virtualenv
 mkvirtualenv ops
 workon ops
 
 # uninstall previous `ops` version (if you have it)
 pip uninstall ops --yes
 
-# install ops-cli v2.1.7 stable release
+# install ops-cli v2.2.0 stable release
 pip install --upgrade ops-cli
 ```
 
 
 ### Terraform
 Optionally, install terraform to be able to access terraform plugin. See https://www.terraform.io/intro/getting-started/install.html
 Also for pretty formatting of terraform plan output you can install https://github.com/coinbase/terraform-landscape (use gem install for MacOS)
@@ -191,15 +188,15 @@
 
 ## Using docker image
 
 You can try out `ops-cli`, by using docker. The docker image has all required prerequisites (python, terraform, helm, git, ops-cli etc).
 
 To start out a container, running the latest `ops-cli` docker image run:
 ```sh
-docker run -it ghcr.io/adobe/ops-cli:2.1.7 bash
+docker run -it ghcr.io/adobe/ops-cli:2.2.0 bash
 ```
 
 After the container has started, you can start using `ops-cli`:
 ```sh
 ops help
 # usage: ops [-h] [--root-dir ROOT_DIR] [--verbose] [-e EXTRA_VARS]
 #           cluster_config_path
@@ -806,9 +803,7 @@
     brew link openssl --force
 ```
 
 # License
 [Apache License 2.0](/LICENSE)
 
 
-
-
```

### Comparing `ops-cli-2.1.7/src/ops_cli.egg-info/SOURCES.txt` & `ops-cli-2.2.0/src/ops_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ops-cli-2.1.7/src/ops_cli.egg-info/requires.txt` & `ops-cli-2.2.0/src/ops_cli.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 adal==1.2.7
-ansible==2.9.25
-awscli==1.20.33
-azure-applicationinsights==0.1.0
+ansible==8.2.0
+awscli==1.29.12
+azure==4.0.0
+azure-applicationinsights==0.1.1
 azure-batch==4.1.3
-azure-common==1.1.27
+azure-common==1.1.28
 azure-cosmosdb-nspkg==2.0.2
 azure-cosmosdb-table==1.0.6
-azure-datalake-store==0.0.52
+azure-datalake-store==0.0.53
 azure-eventgrid==1.3.0
 azure-graphrbac==0.40.0
 azure-keyvault==1.1.0
-azure-loganalytics==0.1.0
+azure-loganalytics==0.1.1
+azure-mgmt==4.0.0
 azure-mgmt-advisor==1.0.1
 azure-mgmt-applicationinsights==0.1.1
 azure-mgmt-authorization==0.50.0
 azure-mgmt-batch==5.0.1
 azure-mgmt-batchai==2.0.0
 azure-mgmt-billing==0.2.0
 azure-mgmt-cdn==3.1.0
@@ -44,15 +46,15 @@
 azure-mgmt-loganalytics==0.2.0
 azure-mgmt-logic==3.0.0
 azure-mgmt-machinelearningcompute==0.4.1
 azure-mgmt-managementgroups==0.1.0
 azure-mgmt-managementpartner==0.1.1
 azure-mgmt-maps==0.1.0
 azure-mgmt-marketplaceordering==0.1.0
-azure-mgmt-media==1.0.0
+azure-mgmt-media==1.0.1
 azure-mgmt-monitor==0.5.2
 azure-mgmt-msi==0.2.0
 azure-mgmt-network==2.7.0
 azure-mgmt-notificationhubs==2.1.0
 azure-mgmt-nspkg==3.0.2
 azure-mgmt-policyinsights==0.1.0
 azure-mgmt-powerbiembedded==2.0.0
@@ -69,93 +71,92 @@
 azure-mgmt-servicefabric==0.2.0
 azure-mgmt-signalr==0.1.1
 azure-mgmt-sql==0.9.1
 azure-mgmt-storage==2.0.0
 azure-mgmt-subscription==0.2.0
 azure-mgmt-trafficmanager==0.50.0
 azure-mgmt-web==0.35.0
-azure-mgmt==4.0.0
 azure-nspkg==3.0.2
 azure-servicebus==0.21.1
 azure-servicefabric==6.3.0.0
 azure-servicemanagement-legacy==0.20.7
 azure-storage-blob==1.5.0
 azure-storage-common==1.4.2
 azure-storage-file==1.4.0
 azure-storage-queue==1.4.0
-azure==4.0.0
-boto3==1.18.33
 boto==2.49.0
-certifi==2021.10.8
-cffi==1.15.0
-gitpython==3.1.24
+boto3==1.28.12
+cffi==1.15.1
+deepmerge==1.1.0
+gitpython==3.1.32
 hashmerge==0.2
-himl==0.7.3
-hvac==0.11.0
-inflection==0.3.1
-isodate==0.6.0
-jinja2==2.11.3
-kubernetes==18.20.0
+himl==0.15.0
+hvac==1.1.1
+inflection==0.5.1
+isodate==0.6.1
+jinja2==3.1.2
+kubernetes==26.1.0
 lru-cache==0.2.3
-msrest==0.6.21
+msal==1.23.0
 msrestazure==0.6.4
 passgen==1.1.1
-pathlib2==2.3.6
-pyasn1-modules==0.2.8
-pyasn1==0.4.8
+pathlib2==2.3.7.post1
+pycparser==2.21
+pyhcl==0.4.4
 python-consul==1.1.0
-pyyaml==5.4.1
-requests-oauthlib==1.3.0
-simpledi==0.3
+resolvelib==1.0.1
+simpledi==0.4.1
 six==1.16.0
 
-[:python_version < "3.10"]
-typing-extensions==3.10.0.2
+[:python_full_version >= "3.7.0"]
+charset-normalizer==3.2.0
 
 [:python_version >= "2.6"]
-backports.functools-lru-cache==1.6.4
-
-[:python_version >= "2.6" and python_version not in "3.0, 3.1, 3.2"]
-docutils==0.15.2
-jmespath==0.10.0
+backports.functools-lru-cache==1.6.6
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2"]
 python-dateutil==2.8.2
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"]
-pycparser==2.20
+requests-oauthlib==1.3.1
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"]
-colorama==0.4.3
-
-[:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4" and python_version < "4"]
-urllib3==1.26.7
+colorama==0.4.4
+docutils==0.16
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5"]
-requests==2.26.0
-
-[:python_version >= "3"]
-charset-normalizer==2.0.7
-deepmerge==0.3.0
-idna==3.3
-
-[:python_version >= "3.4"]
-gitdb==4.0.7
+pyasn1==0.5.0
+pyasn1-modules==0.3.0
+urllib3==1.26.16
 
 [:python_version >= "3.5"]
-smmap==4.0.0
+idna==3.4
 
 [:python_version >= "3.5" and python_version < "4"]
 rsa==4.7.2
 
 [:python_version >= "3.6"]
-botocore==1.21.33
-cryptography==35.0.0
-google-auth==2.3.0
-markupsafe==2.0.1
-oauthlib==3.1.1
-pyjwt==2.2.0
-s3transfer==0.5.0
-websocket-client==1.2.1
+certifi==2023.7.22
+google-auth==2.22.0
+msrest==0.7.1
+oauthlib==3.2.2
+pyyaml==6.0.1
+smmap==5.0.0
+
+[:python_version >= "3.7"]
+azure-core==1.28.0
+botocore==1.31.12
+cachetools==5.3.1
+cryptography==41.0.2
+gitdb==4.0.10
+jmespath==1.0.1
+markupsafe==2.1.3
+packaging==23.1
+pyjwt==2.8.0
+requests==2.31.0
+s3transfer==0.6.1
+setuptools==68.0.0
+typing-extensions==4.7.1
+websocket-client==1.6.1
 
-[:python_version ~= "3.5"]
-cachetools==4.2.4
+[:python_version >= "3.9"]
+ansible-core==2.15.2
```

