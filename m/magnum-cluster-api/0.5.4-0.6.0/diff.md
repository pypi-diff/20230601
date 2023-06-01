# Comparing `tmp/magnum_cluster_api-0.5.4.tar.gz` & `tmp/magnum_cluster_api-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnum_cluster_api-0.5.4.tar", max compression
+gzip compressed data, was "magnum_cluster_api-0.6.0.tar", max compression
```

## Comparing `magnum_cluster_api-0.5.4.tar` & `magnum_cluster_api-0.6.0.tar`

### file list

```diff
@@ -1,65 +1,78 @@
--rw-r--r--   0        0        0    10142 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/LICENSE
--rw-r--r--   0        0        0     2795 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/README.md
--rw-r--r--   0        0        0        0 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/.gitkeep
--rw-r--r--   0        0        0      349 2023-04-24 16:49:36.448924 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
--rw-r--r--   0        0        0      437 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
--rw-r--r--   0        0        0    29122 2023-04-24 16:49:36.448924 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/README.md
--rw-r--r--   0        0        0    14987 2023-04-24 16:49:36.448924 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
--rw-r--r--   0        0        0      827 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
--rw-r--r--   0        0        0     4034 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
--rw-r--r--   0        0        0     2982 2023-04-24 16:49:36.548924 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
--rw-r--r--   0        0        0      534 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
--rw-r--r--   0        0        0    13204 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
--rw-r--r--   0        0        0      508 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
--rw-r--r--   0        0        0      972 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
--rw-r--r--   0        0        0      758 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
--rw-r--r--   0        0        0      564 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     1807 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
--rw-r--r--   0        0        0      527 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
--rw-r--r--   0        0        0      989 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
--rw-r--r--   0        0        0     1180 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
--rw-r--r--   0        0        0      528 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      960 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
--rw-r--r--   0        0        0      663 2023-04-24 16:49:36.448924 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
--rw-r--r--   0        0        0    18003 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
--rw-r--r--   0        0        0      843 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/clients.py
--rw-r--r--   0        0        0        0 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/cmd/__init__.py
--rw-r--r--   0        0        0     4019 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/cmd/image_builder.py
--rw-r--r--   0        0        0     4182 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/cmd/image_loader.py
--rw-r--r--   0        0        0      956 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/cmd/proxy.py
--rw-r--r--   0        0        0     1778 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/conf.py
--rw-r--r--   0        0        0    10862 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/driver.py
--rw-r--r--   0        0        0     2155 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/helm.py
--rw-r--r--   0        0        0     3171 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/image_utils.py
--rw-r--r--   0        0        0     1116 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/images.py
--rw-r--r--   0        0        0        0 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/__init__.py
--rw-r--r--   0        0        0     4941 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/audit/policy.yaml
--rw-r--r--   0        0        0   235191 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/calico/v3.24.2.yaml
--rw-r--r--   0        0        0      623 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
--rw-r--r--   0        0        0     1430 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
--rw-r--r--   0        0        0     2263 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
--rw-r--r--   0        0        0     4506 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml
--rw-r--r--   0        0        0     4034 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml
--rw-r--r--   0        0        0      609 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml
--rw-r--r--   0        0        0     3307 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml
--rw-r--r--   0        0        0      194 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/csi-cinder-driver.yaml
--rw-r--r--   0        0        0     1526 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/monitor.py
--rw-r--r--   0        0        0     2880 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/objects.py
--rw-r--r--   0        0        0      828 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/privsep/__init__.py
--rw-r--r--   0        0        0     1333 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/privsep/haproxy.py
--rw-r--r--   0        0        0    11719 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/proxy/manager.py
--rw-r--r--   0        0        0     3616 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/proxy/structs.py
--rw-r--r--   0        0        0      580 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
--rw-r--r--   0        0        0     1511 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/proxy/utils.py
--rw-r--r--   0        0        0    73565 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/resources.py
--rw-r--r--   0        0        0     1492 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/service.py
--rw-r--r--   0        0        0      942 2023-04-24 16:49:35.164916 magnum_cluster_api-0.5.4/magnum_cluster_api/tests/conftest.py
--rw-r--r--   0        0        0     3445 2023-04-24 16:49:35.164916 magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_helm.py
--rw-r--r--   0        0        0     1731 2023-04-24 16:49:35.164916 magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_image_utils.py
--rw-r--r--   0        0        0     2759 2023-04-24 16:49:35.164916 magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_images.py
--rw-r--r--   0        0        0     1717 2023-04-24 16:49:35.164916 magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_resources.py
--rw-r--r--   0        0        0     1192 2023-04-24 16:49:35.164916 magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_utils.py
--rw-r--r--   0        0        0     7684 2023-04-24 16:49:35.164916 magnum_cluster_api-0.5.4/magnum_cluster_api/utils.py
--rw-r--r--   0        0        0     1186 2023-04-24 16:49:35.164916 magnum_cluster_api-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 magnum_cluster_api-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-06-01 16:40:59.661282 magnum_cluster_api-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2795 2023-06-01 16:40:59.661282 magnum_cluster_api-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/.gitkeep
+-rw-r--r--   0        0        0      349 2023-06-01 16:41:00.389285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
+-rw-r--r--   0        0        0      437 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
+-rw-r--r--   0        0        0    29122 2023-06-01 16:41:00.389285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/README.md
+-rw-r--r--   0        0        0    14987 2023-06-01 16:41:00.389285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
+-rw-r--r--   0        0        0      827 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
+-rw-r--r--   0        0        0     4034 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2982 2023-06-01 16:41:00.393285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
+-rw-r--r--   0        0        0      534 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
+-rw-r--r--   0        0        0    13204 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
+-rw-r--r--   0        0        0      508 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
+-rw-r--r--   0        0        0      972 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
+-rw-r--r--   0        0        0      758 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
+-rw-r--r--   0        0        0      564 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0     1807 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
+-rw-r--r--   0        0        0      527 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
+-rw-r--r--   0        0        0      989 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
+-rw-r--r--   0        0        0     1180 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
+-rw-r--r--   0        0        0      528 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      960 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
+-rw-r--r--   0        0        0      663 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
+-rw-r--r--   0        0        0    18003 2023-06-01 16:41:00.385285 magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
+-rw-r--r--   0        0        0     1977 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/clients.py
+-rw-r--r--   0        0        0        0 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/cmd/__init__.py
+-rw-r--r--   0        0        0     4019 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/cmd/image_builder.py
+-rw-r--r--   0        0        0     4714 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/cmd/image_loader.py
+-rw-r--r--   0        0        0      956 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/cmd/proxy.py
+-rw-r--r--   0        0        0     3278 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/conf.py
+-rw-r--r--   0        0        0    11915 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/driver.py
+-rw-r--r--   0        0        0     1167 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/exceptions.py
+-rw-r--r--   0        0        0     2888 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/helm.py
+-rw-r--r--   0        0        0     3464 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/image_utils.py
+-rw-r--r--   0        0        0     1116 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/images.py
+-rw-r--r--   0        0        0        0 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/__init__.py
+-rw-r--r--   0        0        0     4941 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/audit/policy.yaml
+-rw-r--r--   0        0        0   235191 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml
+-rw-r--r--   0        0        0      623 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
+-rw-r--r--   0        0        0     1430 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
+-rw-r--r--   0        0        0     2263 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
+-rw-r--r--   0        0        0     4506 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml
+-rw-r--r--   0        0        0     4034 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml
+-rw-r--r--   0        0        0      609 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml
+-rw-r--r--   0        0        0     3307 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml
+-rw-r--r--   0        0        0      194 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/csi-cinder-driver.yaml
+-rw-r--r--   0        0        0     3377 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml
+-rw-r--r--   0        0        0     3944 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml
+-rw-r--r--   0        0        0     1513 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml
+-rw-r--r--   0        0        0     2988 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml
+-rw-r--r--   0        0        0      143 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/manila-csi/csidriver.yaml
+-rw-r--r--   0        0        0     3127 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml
+-rw-r--r--   0        0        0      170 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-driverinfo.yaml
+-rw-r--r--   0        0        0     3530 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml
+-rw-r--r--   0        0        0     1423 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml
+-rw-r--r--   0        0        0     1526 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/monitor.py
+-rw-r--r--   0        0        0     5453 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/objects.py
+-rw-r--r--   0        0        0      828 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/privsep/__init__.py
+-rw-r--r--   0        0        0     1333 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/privsep/haproxy.py
+-rw-r--r--   0        0        0    11719 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/proxy/manager.py
+-rw-r--r--   0        0        0     3616 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/proxy/structs.py
+-rw-r--r--   0        0        0      580 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
+-rw-r--r--   0        0        0     1511 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/proxy/utils.py
+-rw-r--r--   0        0        0    78098 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/resources.py
+-rw-r--r--   0        0        0     1492 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/service.py
+-rw-r--r--   0        0        0     3119 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/functional/conftest.py
+-rw-r--r--   0        0        0      666 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/functional/test_clusters.py
+-rw-r--r--   0        0        0      942 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/conftest.py
+-rw-r--r--   0        0        0     3453 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_helm.py
+-rw-r--r--   0        0        0     1731 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_image_utils.py
+-rw-r--r--   0        0        0     2759 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_images.py
+-rw-r--r--   0        0        0     5366 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_objects.py
+-rw-r--r--   0        0        0     1717 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_resources.py
+-rw-r--r--   0        0        0     1192 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_utils.py
+-rw-r--r--   0        0        0    10350 2023-06-01 16:40:59.665282 magnum_cluster_api-0.6.0/magnum_cluster_api/utils.py
+-rw-r--r--   0        0        0     1220 2023-06-01 16:40:59.669282 magnum_cluster_api-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 magnum_cluster_api-0.6.0/PKG-INFO
```

### Comparing `magnum_cluster_api-0.5.4/LICENSE` & `magnum_cluster_api-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/README.md` & `magnum_cluster_api-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/README.md` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/values.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/cmd/image_builder.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/cmd/image_builder.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/cmd/image_loader.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/cmd/image_loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 IMAGES = [
     "docker.io/calico/cni:v3.24.2",
     "docker.io/calico/kube-controllers:v3.24.2",
     "docker.io/calico/node:v3.24.2",
     "docker.io/k8scloudprovider/cinder-csi-plugin:v1.25.3",
+    "docker.io/k8scloudprovider/manila-csi-plugin:v1.25.3",
     "docker.io/k8scloudprovider/openstack-cloud-controller-manager:v1.25.3",
+    "registry.k8s.io/sig-storage/nfsplugin:v4.2.0",
     "registry.k8s.io/coredns/coredns:v1.8.6",
     "registry.k8s.io/coredns/coredns:v1.9.3",
     CONF.auto_scaling.v1_22_image,
     CONF.auto_scaling.v1_23_image,
     CONF.auto_scaling.v1_24_image,
     CONF.auto_scaling.v1_25_image,
     CONF.auto_scaling.v1_26_image,
@@ -58,19 +60,26 @@
     "registry.k8s.io/kube-scheduler:v1.23.13",
     "registry.k8s.io/kube-scheduler:v1.24.7",
     "registry.k8s.io/kube-scheduler:v1.24.7",
     "registry.k8s.io/kube-scheduler:v1.25.3",
     "registry.k8s.io/kube-scheduler:v1.26.2",
     images.PAUSE,
     "registry.k8s.io/sig-storage/csi-attacher:v3.4.0",
+    "registry.k8s.io/sig-storage/csi-node-driver-registrar:v2.4.0",
     "registry.k8s.io/sig-storage/csi-node-driver-registrar:v2.5.1",
+    "registry.k8s.io/sig-storage/csi-node-driver-registrar:v2.6.2",
+    "registry.k8s.io/sig-storage/csi-provisioner:v3.0.0",
     "registry.k8s.io/sig-storage/csi-provisioner:v3.1.0",
+    "registry.k8s.io/sig-storage/csi-provisioner:v3.3.0",
     "registry.k8s.io/sig-storage/csi-resizer:v1.4.0",
+    "registry.k8s.io/sig-storage/csi-resizer:v1.8.0",
+    "registry.k8s.io/sig-storage/csi-snapshotter:v5.0.1",
     "registry.k8s.io/sig-storage/csi-snapshotter:v6.0.1",
     "registry.k8s.io/sig-storage/livenessprobe:v2.7.0",
+    "registry.k8s.io/sig-storage/livenessprobe:v2.8.0",
 ]
 
 
 @click.command()
 @click.option(
     "--repository",
     show_default=True,
```

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/cmd/proxy.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/cmd/proxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/conf.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/conf.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,16 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+from magnum.i18n import _
 from oslo_config import cfg
 
+auto_scaling_group = cfg.OptGroup(name="auto_scaling", title="Options for auto scaling")
+
+manila_client_group = cfg.OptGroup(
+    name="manila_client", title="Options for the Manila client"
+)
+
+
 auto_scaling_opts = [
     cfg.StrOpt(
         "image_repository",
         default="registry.k8s.io/autoscaling",
         help="Image repository for the cluster auto-scaler.",
     ),
     cfg.StrOpt(
@@ -43,9 +51,51 @@
     cfg.StrOpt(
         "v1_26_image",
         default="$image_repository/cluster-autoscaler:v1.26.1",
         help="Image for the cluster auto-scaler for Kubernetes v1.26.",
     ),
 ]
 
+
+manila_client_opts = [
+    cfg.StrOpt(
+        "region_name",
+        help=_(
+            "Region in Identity service catalog to use for "
+            "communication with the OpenStack service."
+        ),
+    ),
+    cfg.StrOpt(
+        "endpoint_type",
+        default="publicURL",
+        help=_(
+            "Type of endpoint in Identity service catalog to use "
+            "for communication with the OpenStack service."
+        ),
+    ),
+    cfg.StrOpt(
+        "api_version",
+        default="3",
+        help=_("Version of Manila API to use in manilaclient."),
+    ),
+]
+
+common_security_opts = [
+    cfg.StrOpt("ca_file", help=_("Optional CA cert file to use in SSL connections.")),
+    cfg.StrOpt("cert_file", help=_("Optional PEM-formatted certificate chain file.")),
+    cfg.StrOpt(
+        "key_file",
+        help=_("Optional PEM-formatted file that contains the " "private key."),
+    ),
+    cfg.BoolOpt(
+        "insecure",
+        default=False,
+        help=_("If set, then the server's certificate will not " "be verified."),
+    ),
+]
+
 CONF = cfg.CONF
-CONF.register_opts(auto_scaling_opts, "auto_scaling")
+CONF.register_group(auto_scaling_group)
+CONF.register_group(manila_client_group)
+CONF.register_opts(auto_scaling_opts, group=auto_scaling_group)
+CONF.register_opts(manila_client_opts, group=manila_client_group)
+CONF.register_opts(common_security_opts, group=manila_client_group)
```

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/driver.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/driver.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+
 import keystoneauth1
 from magnum import objects as magnum_objects
 from magnum.drivers.common import driver
+from tenacity import retry, stop_after_delay, wait_fixed
 
-from magnum_cluster_api import clients, monitor, objects, resources, utils
+from magnum_cluster_api import clients, exceptions, monitor, objects, resources, utils
 
 
 class BaseDriver(driver.Driver):
     def __init__(self):
         self.k8s_api = clients.get_pykube_api()
 
     def create_cluster(self, context, cluster, cluster_create_timeout):
@@ -52,15 +54,14 @@
         resources.apply_cluster_from_magnum_cluster(context, self.k8s_api, cluster)
 
     def update_cluster_status(self, context, cluster, use_admin_ctx=False):
         node_groups = [
             self.update_nodegroup_status(context, cluster, node_group)
             for node_group in cluster.nodegroups
         ]
-
         # TODO: watch for topology change instead
         osc = clients.get_openstack_api(context)
 
         capi_cluster = resources.Cluster(context, self.k8s_api, cluster).get_or_none()
 
         if cluster.status in (
             "CREATE_IN_PROGRESS",
@@ -178,17 +179,43 @@
         rollback=False,
     ):
         """
         Upgrade a cluster to a new version of Kubernetes.
         """
         # TODO: nodegroup?
 
+        # Get current generation
+        current_generation = resources.Cluster(
+            context, self.k8s_api, cluster
+        ).get_observed_generation()
         resources.apply_cluster_from_magnum_cluster(
             context, self.k8s_api, cluster, cluster_template=cluster_template
         )
+        # Wait till the generation has been increased
+        self.wait_capi_cluster_reconciliation_start(
+            context, cluster, current_generation
+        )
+
+    @retry(
+        stop=stop_after_delay(10),
+        wait=wait_fixed(1),
+    )
+    def wait_capi_cluster_reconciliation_start(
+        self, context, cluster: magnum_objects.Cluster, old_generation: int
+    ):
+        """Wait until the cluster's new generation is observed by capi-controller
+
+        This means the cluster reconciliation has been started and the conditions has been updated.
+        """
+        current_generation = resources.Cluster(
+            context, self.k8s_api, cluster
+        ).get_observed_generation()
+        if old_generation != current_generation:
+            return
+        raise exceptions.ClusterAPIReconcileTimeout()
 
     def delete_cluster(self, context, cluster):
         # NOTE(mnaser): This should be removed when this is fixed:
         #
         #               https://github.com/kubernetes-sigs/cluster-api-provider-openstack/issues/842
         #               https://github.com/kubernetes-sigs/cluster-api-provider-openstack/pull/990
         utils.delete_loadbalancers(context, cluster)
@@ -250,14 +277,15 @@
 
         nodegroup.save()
 
         return nodegroup
 
     def update_nodegroup(self, context, cluster, nodegroup):
         # TODO
+
         resources.apply_cluster_from_magnum_cluster(context, self.k8s_api, cluster)
 
     def delete_nodegroup(self, context, cluster, nodegroup):
         nodegroup.status = "DELETE_IN_PROGRESS"
         nodegroup.save()
 
         resources.apply_cluster_from_magnum_cluster(
```

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/helm.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/helm.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,66 +11,90 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import yaml
 from oslo_concurrency import processutils
 
+from magnum_cluster_api import exceptions
+
 
 class Command:
     def __call__(self, *args, **kwargs):
-        processutils.execute("helm", self.COMMAND, *args, **kwargs)
+        return processutils.execute("helm", *self.COMMAND, *args, **kwargs)
 
 
 class VersionCommand(Command):
-    COMMAND = "version"
+    COMMAND = ["version"]
 
 
 class ReleaseCommand(Command):
     def __init__(self, namespace, release_name):
         self.namespace = namespace
         self.release_name = release_name
 
     def __call__(self, *args, **kwargs):
-        super().__call__(
+        return super().__call__(
             "--namespace",
             self.namespace,
             self.release_name,
             *args,
             **kwargs,
         )
 
 
+class GetValuesReleaseCommand(ReleaseCommand):
+    COMMAND = ["get", "values"]
+
+    def __call__(self):
+        try:
+            return super().__call__(
+                "--namespace",
+                self.namespace,
+                self.release_name,
+                "--output",
+                "yaml",
+            )
+        except processutils.ProcessExecutionError as e:
+            if "release: not found" in e.stderr:
+                raise exceptions.HelmReleaseNotFound(self.release_name)
+            else:
+                raise
+
+
 class UpgradeReleaseCommand(ReleaseCommand):
-    COMMAND = "upgrade"
+    COMMAND = ["upgrade"]
 
     def __init__(self, namespace, release_name, chart_ref, values={}):
         super().__init__(namespace, release_name)
         self.chart_ref = chart_ref
         self.values = values
 
     def __call__(self):
-        super().__call__(
+        return super().__call__(
             self.chart_ref,
             "--install",
             "--wait",
             "--values",
             "-",
             process_input=yaml.dump(self.values),
         )
 
 
 class DeleteReleaseCommand(ReleaseCommand):
-    COMMAND = "delete"
+    COMMAND = ["delete"]
 
     def __init__(self, namespace, release_name, skip_missing=False):
         super().__init__(namespace, release_name)
         self.skip_missing = skip_missing
 
     def __call__(self):
         try:
-            super().__call__()
+            return super().__call__()
         except processutils.ProcessExecutionError as e:
-            if self.skip_missing and "release: not found" in e.stderr:
-                pass
+            if "release: not found" in e.stderr:
+                if self.skip_missing:
+                    pass
+                else:
+                    raise exceptions.HelmReleaseNotFound(self.release_name)
             else:
                 raise
```

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/image_utils.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/image_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 def update_manifest_images(cluster_uuid: str, file, repository=None, replacements=[]):
     with open(file) as fd:
         data = fd.read()
 
     docs = []
     for doc in yaml.safe_load_all(data):
         # Fix container image paths
-        if doc["kind"] in ("DaemonSet", "Deployment"):
+        if doc["kind"] in ("DaemonSet", "Deployment", "StatefulSet"):
             for container in itertools.chain(
                 doc["spec"]["template"]["spec"].get("initContainers", []),
                 doc["spec"]["template"]["spec"]["containers"],
             ):
                 for src, dst in replacements:
                     container["image"] = container["image"].replace(src, dst)
                 if repository:
@@ -59,14 +59,18 @@
     new_image_name = name
     if name.startswith("docker.io/calico"):
         new_image_name = name.replace("docker.io/calico/", f"{repository}/calico-")
     if name.startswith("docker.io/k8scloudprovider"):
         new_image_name = name.replace("docker.io/k8scloudprovider", repository)
     if name.startswith("registry.k8s.io/sig-storage"):
         new_image_name = name.replace("registry.k8s.io/sig-storage", repository)
+    if name.startswith("registry.k8s.io/provider-os"):
+        new_image_name = name.replace("registry.k8s.io/provider-os", repository)
+    if name.startswith("gcr.io/k8s-staging-sig-storage"):
+        new_image_name = name.replace("gcr.io/k8s-staging-sig-storage", repository)
     if new_image_name.startswith(f"{repository}/livenessprobe"):
         return new_image_name.replace("livenessprobe", "csi-livenessprobe")
     if new_image_name.startswith("registry.k8s.io/coredns"):
         return new_image_name.replace("registry.k8s.io/coredns", repository)
     if new_image_name.startswith("registry.k8s.io/autoscaling"):
         return new_image_name.replace("registry.k8s.io/autoscaling", repository)
     if (
```

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/images.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/audit/policy.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/audit/policy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/calico/v3.24.2.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml` & `magnum_cluster_api-0.6.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/monitor.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/monitor.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/privsep/__init__.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/privsep/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/privsep/haproxy.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/privsep/haproxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/proxy/manager.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/proxy/manager.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/proxy/structs.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/proxy/structs.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/proxy/templates/haproxy.cfg.j2` & `magnum_cluster_api-0.6.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/proxy/utils.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/proxy/utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/resources.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 from oslo_utils import encodeutils
 
 from magnum_cluster_api import clients, helm, image_utils, images, objects, utils
 
 CONF = cfg.CONF
 CLOUD_PROVIDER_TAG = "v1.25.3"
 CALICO_TAG = "v3.24.2"
-CSI_TAG = "v1.25.3"
+CINDER_CSI_TAG = "v1.25.3"
+MANILA_CSI_TAG = "v1.25.3"
 
 CLUSTER_CLASS_VERSION = pkg_resources.require("magnum_cluster_api")[0].version
 CLUSTER_CLASS_NAME = f"magnum-v{CLUSTER_CLASS_VERSION}"
 
 CLUSTER_UPGRADE_LABELS = {"kube_tag"}
 
 PLACEHOLDER = "PLACEHOLDER"
@@ -159,101 +160,191 @@
         manifests_path = pkg_resources.resource_filename(
             "magnum_cluster_api", "manifests"
         )
         calico_version = utils.get_cluster_label(self.cluster, "calico_tag", CALICO_TAG)
         ccm_version = utils.get_cluster_label(
             self.cluster, "cloud_provider_tag", CLOUD_PROVIDER_TAG
         )
-        csi_version = utils.get_cluster_label(
-            self.cluster, "cinder_csi_plugin_tag", CSI_TAG
-        )
 
         repository = utils.get_cluster_container_infra_prefix(self.cluster)
 
         osc = clients.get_openstack_api(self.context)
-        volume_types = osc.cinder().volume_types.list()
-        default_volume_type = osc.cinder().volume_types.default()
 
-        return pykube.ConfigMap(
-            self.api,
-            {
-                "apiVersion": pykube.ConfigMap.version,
-                "kind": pykube.ConfigMap.kind,
-                "metadata": {
-                    "name": self.cluster.uuid,
-                    "namespace": "magnum-system",
+        data = {
+            **{
+                os.path.basename(manifest): image_utils.update_manifest_images(
+                    self.cluster.uuid,
+                    manifest,
+                    repository=repository,
+                    replacements=[
+                        (
+                            "docker.io/k8scloudprovider/openstack-cloud-controller-manager:latest",
+                            f"docker.io/k8scloudprovider/openstack-cloud-controller-manager:{ccm_version}",
+                        ),
+                    ],
+                )
+                for manifest in glob.glob(os.path.join(manifests_path, "ccm/*.yaml"))
+            },
+            **{
+                "calico.yml": image_utils.update_manifest_images(
+                    self.cluster.uuid,
+                    os.path.join(manifests_path, f"calico/{calico_version}.yaml"),
+                    repository=repository,
+                )
+            },
+        }
+
+        if utils.is_cinder_csi_enabled(self.cluster):
+            volume_types = osc.cinder().volume_types.list()
+            default_volume_type = osc.cinder().volume_types.default()
+            csi_version = utils.get_cluster_label(
+                self.cluster, "cinder_csi_plugin_tag", CINDER_CSI_TAG
+            )
+            data = {
+                **data,
+                **{
+                    os.path.basename(manifest): image_utils.update_manifest_images(
+                        self.cluster.uuid,
+                        manifest,
+                        repository=repository,
+                        replacements=[
+                            (
+                                "docker.io/k8scloudprovider/cinder-csi-plugin:latest",
+                                f"docker.io/k8scloudprovider/cinder-csi-plugin:{csi_version}",
+                            ),
+                        ],
+                    )
+                    for manifest in glob.glob(
+                        os.path.join(manifests_path, "cinder-csi/*.yaml")
+                    )
+                },
+                **{
+                    f"storageclass-cinder-{vt.name}.yaml": yaml.dump(
+                        {
+                            "apiVersion": objects.StorageClass.version,
+                            "allowVolumeExpansion": True,
+                            "kind": objects.StorageClass.kind,
+                            "metadata": {
+                                "annotations": {
+                                    "storageclass.kubernetes.io/is-default-class": "true"
+                                }
+                                if default_volume_type.name == vt.name
+                                else {},
+                                "name": "cinder-%s" % vt.name.lower(),
+                            },
+                            "provisioner": "kubernetes.io/cinder",
+                            "parameters": {
+                                "type": vt.name,
+                            },
+                            "reclaimPolicy": "Delete",
+                            "volumeBindingMode": "Immediate",
+                        }
+                    )
+                    for vt in volume_types
+                    if vt.name != "__DEFAULT__"
                 },
-                "data": {
-                    **{
-                        os.path.basename(manifest): image_utils.update_manifest_images(
-                            self.cluster.uuid,
-                            manifest,
-                            repository=repository,
-                            replacements=[
-                                (
-                                    "docker.io/k8scloudprovider/openstack-cloud-controller-manager:latest",
-                                    f"docker.io/k8scloudprovider/openstack-cloud-controller-manager:{ccm_version}",
-                                ),
-                            ],
-                        )
-                        for manifest in glob.glob(
-                            os.path.join(manifests_path, "ccm/*.yaml")
-                        )
-                    },
-                    **{
-                        os.path.basename(manifest): image_utils.update_manifest_images(
-                            self.cluster.uuid,
-                            manifest,
-                            repository=repository,
-                            replacements=[
-                                (
-                                    "docker.io/k8scloudprovider/cinder-csi-plugin:latest",
-                                    f"docker.io/k8scloudprovider/cinder-csi-plugin:{csi_version}",
-                                ),
-                            ],
-                        )
-                        for manifest in glob.glob(
-                            os.path.join(manifests_path, "csi/*.yaml")
-                        )
-                    },
-                    **{
-                        "calico.yml": image_utils.update_manifest_images(
-                            self.cluster.uuid,
-                            os.path.join(
-                                manifests_path, f"calico/{calico_version}.yaml"
+            }
+
+        if utils.is_manila_csi_enabled(self.cluster):
+            share_types = osc.manila().share_types.list()
+            csi_version = utils.get_cluster_label(
+                self.cluster, "manila_csi_plugin_tag", MANILA_CSI_TAG
+            )
+            share_network_id = utils.get_cluster_label(
+                self.cluster, "manila_csi_share_network_id", None
+            )
+            data = {
+                **data,
+                **{
+                    "manila-csi-secret.yaml": yaml.dump(
+                        {
+                            "apiVersion": pykube.Secret.version,
+                            "kind": pykube.Secret.kind,
+                            "metadata": {
+                                "name": "csi-manila-secrets",
+                                "namespace": "kube-system",
+                            },
+                            "stringData": utils.generate_manila_csi_cloud_config(
+                                self.api,
+                                self.cluster,
                             ),
-                            repository=repository,
-                        )
-                    },
+                        },
+                    )
+                },
+                **{
+                    os.path.basename(manifest): image_utils.update_manifest_images(
+                        self.cluster.uuid,
+                        manifest,
+                        repository=repository,
+                    )
+                    for manifest in glob.glob(
+                        os.path.join(manifests_path, "nfs-csi/*.yaml")
+                    )
+                },
+                **{
+                    os.path.basename(manifest): image_utils.update_manifest_images(
+                        self.cluster.uuid,
+                        manifest,
+                        repository=repository,
+                        replacements=[
+                            (
+                                "registry.k8s.io/provider-os/manila-csi-plugin:latest",
+                                f"registry.k8s.io/provider-os/manila-csi-plugin:{csi_version}",
+                            ),
+                        ],
+                    )
+                    for manifest in glob.glob(
+                        os.path.join(manifests_path, "manila-csi/*.yaml")
+                    )
+                },
+            }
+            # NOTE: We only create StorageClasses if share_network_id specified.
+            if share_network_id:
+                data = {
+                    **data,
                     **{
-                        f"storageclass-{vt.name}.yaml": yaml.dump(
+                        f"storageclass-manila-{st.name}.yaml": yaml.dump(
                             {
                                 "apiVersion": objects.StorageClass.version,
                                 "allowVolumeExpansion": True,
                                 "kind": objects.StorageClass.kind,
                                 "metadata": {
-                                    "annotations": {
-                                        "storageclass.kubernetes.io/is-default-class": "true"
-                                    }
-                                    if default_volume_type.name == vt.name
-                                    else {},
-                                    "name": vt.name.lower(),
+                                    "name": "manila-%s" % st.name.lower(),
                                 },
-                                "provisioner": "kubernetes.io/cinder",
+                                "provisioner": "manila.csi.openstack.org",
                                 "parameters": {
-                                    "type": vt.name,
+                                    "type": st.name,
+                                    "shareNetworkID": share_network_id,
+                                    "csi.storage.k8s.io/provisioner-secret-name": "csi-manila-secrets",
+                                    "csi.storage.k8s.io/provisioner-secret-namespace": "kube-system",
+                                    "csi.storage.k8s.io/controller-expand-secret-name": "csi-manila-secrets",
+                                    "csi.storage.k8s.io/controller-expand-secret-namespace": "kube-system",
+                                    "csi.storage.k8s.io/node-stage-secret-name": "csi-manila-secrets",
+                                    "csi.storage.k8s.io/node-stage-secret-namespace": "kube-system",
+                                    "csi.storage.k8s.io/node-publish-secret-name": "csi-manila-secrets",
+                                    "csi.storage.k8s.io/node-publish-secret-namespace": "kube-system",
                                 },
                                 "reclaimPolicy": "Delete",
                                 "volumeBindingMode": "Immediate",
                             }
                         )
-                        for vt in volume_types
-                        if vt.name != "__DEFAULT__"
+                        for st in share_types
                     },
+                }
+
+        return pykube.ConfigMap(
+            self.api,
+            {
+                "apiVersion": pykube.ConfigMap.version,
+                "kind": pykube.ConfigMap.kind,
+                "metadata": {
+                    "name": self.cluster.uuid,
+                    "namespace": "magnum-system",
                 },
+                "data": data,
             },
         )
 
     def get_or_none(self) -> objects.Cluster:
         return pykube.ConfigMap.objects(
             self.api, namespace="magnum-system"
         ).get_or_none(name=self.cluster.uuid)
@@ -1330,28 +1421,40 @@
         )
         cni_version = utils.get_cluster_label(self.cluster, "calico_tag", CALICO_TAG)
         labels = {
             "cni": f"calico-{cni_version}",
             "ccm": f"openstack-cloud-controller-manager-{ccm_version}",
         }
 
-        if utils.get_cluster_label_as_bool(self.cluster, "cinder_csi_enabled", True):
+        if utils.is_cinder_csi_enabled(self.cluster):
             csi_version = utils.get_cluster_label(
-                self.cluster, "cinder_csi_plugin_tag", CSI_TAG
+                self.cluster, "cinder_csi_plugin_tag", CINDER_CSI_TAG
             )
             labels["csi"] = "cinder"
             labels["cinder-csi-version"] = csi_version
 
+        if utils.is_manila_csi_enabled(self.cluster):
+            manila_version = utils.get_cluster_label(
+                self.cluster, "manila_csi_plugin_tag", MANILA_CSI_TAG
+            )
+            labels["manila-csi-version"] = manila_version
+
         return {**super().labels, **labels}
 
     def get_or_none(self) -> objects.Cluster:
         return objects.Cluster.objects(self.api, namespace="magnum-system").get_or_none(
             name=utils.get_or_generate_cluster_api_name(self.api, self.cluster)
         )
 
+    def get_observed_generation(self) -> int:
+        capi_cluster = self.get_or_none()
+        if capi_cluster:
+            return capi_cluster.obj["status"]["observedGeneration"]
+        raise Exception("Cluster doesn't exists.")
+
     def get_object(self) -> objects.Cluster:
         return objects.Cluster(
             self.api,
             {
                 "apiVersion": objects.Cluster.version,
                 "kind": objects.Cluster.kind,
                 "metadata": {
```

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/service.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/service.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/tests/conftest.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_helm.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_helm.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import pytest
 import yaml
 from oslo_concurrency import processutils
 
-from magnum_cluster_api import helm
+from magnum_cluster_api import exceptions, helm
 
 
 def test_helm_upgrade(mocker):
     namespace = "test-namespace"
     release_name = "test-release"
     chart_ref = "test-chart"
     values = {"test": "value"}
@@ -73,15 +73,15 @@
     mock_execute = mocker.patch("oslo_concurrency.processutils.execute")
     mock_execute.side_effect = processutils.ProcessExecutionError(
         stderr=f"Error: uninstall: Release not loaded: {release_name}: release: not found"
     )
 
     delete = helm.DeleteReleaseCommand(namespace, release_name)
 
-    with pytest.raises(processutils.ProcessExecutionError):
+    with pytest.raises(exceptions.HelmReleaseNotFound):
         delete()
 
     mock_execute.assert_called_once_with(
         "helm",
         "delete",
         "--namespace",
         namespace,
```

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_image_utils.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_images.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_resources.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_resources.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_utils.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.4/magnum_cluster_api/utils.py` & `magnum_cluster_api-0.6.0/magnum_cluster_api/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,20 +17,24 @@
 import textwrap
 
 import pykube
 import shortuuid
 import yaml
 from magnum import objects as magnum_objects
 from magnum.common import context, exception, octavia
+from magnum.common.keystone import KeystoneClientV3
+from oslo_log import log as logging
 from oslo_serialization import base64
 from oslo_utils import strutils
 from tenacity import retry, retry_if_exception_type
 
 from magnum_cluster_api import clients, image_utils, images, objects
 
+LOG = logging.getLogger(__name__)
+
 
 def get_or_generate_cluster_api_cloud_config_secret_name(
     api: pykube.HTTPClient, cluster: magnum_objects.Cluster
 ) -> str:
     return f"{get_or_generate_cluster_api_name(api, cluster)}-cloud-config"
 
 
@@ -86,14 +90,42 @@
         application-credential-id={cloud_config["clouds"]["default"]["auth"]["application_credential_id"]}
         application-credential-secret={cloud_config["clouds"]["default"]["auth"]["application_credential_secret"]}
         tls-insecure={"false" if cloud_config["clouds"]["default"]["verify"] else "true"}
         """
     )
 
 
+def generate_manila_csi_cloud_config(
+    api: pykube.HTTPClient,
+    cluster: magnum_objects.Cluster,
+) -> str:
+    """
+    Generate coniguration of Openstack authentication  for manila csi
+    """
+    data = pykube.Secret.objects(api, namespace="magnum-system").get_by_name(
+        get_or_generate_cluster_api_cloud_config_secret_name(api, cluster)
+    )
+    clouds_yaml = base64.decode_as_text(data.obj["data"]["clouds.yaml"])
+    cloud_config = yaml.safe_load(clouds_yaml)
+
+    return {
+        "os-authURL": cloud_config["clouds"]["default"]["auth"]["auth_url"],
+        "os-region": cloud_config["clouds"]["default"]["region_name"],
+        "os-applicationCredentialID": cloud_config["clouds"]["default"]["auth"][
+            "application_credential_id"
+        ],
+        "os-applicationCredentialSecret": cloud_config["clouds"]["default"]["auth"][
+            "application_credential_secret"
+        ],
+        "os-TLSInsecure": "false"
+        if cloud_config["clouds"]["default"]["verify"]
+        else "true",
+    }
+
+
 def get_kube_tag(cluster: magnum_objects.Cluster) -> str:
     return get_cluster_label(cluster, "kube_tag", "v1.25.3")
 
 
 def get_auto_scaling_enabled(cluster: magnum_objects.Cluster) -> bool:
     return get_cluster_label_as_bool(cluster, "auto_scaling_enabled", False)
 
@@ -229,7 +261,60 @@
 
         if not candidates:
             return
 
         octavia.wait_for_lb_deleted(octavia_client, candidates)
     except Exception as e:
         raise exception.PreDeletionFailed(cluster_uuid=cluster.uuid, msg=str(e))
+
+
+def is_cinder_enabled():
+    """Check if Cinder service is deployed in the cloud."""
+
+    admin_context = context.make_admin_context()
+    keystone = KeystoneClientV3(admin_context)
+
+    try:
+        cinder_svc = keystone.client.services.list(type="volumev3")
+    except Exception:
+        LOG.exception("Failed to list services")
+        raise exception.ServicesListFailed()
+
+    # Always assume there is only one load balancing service configured.
+    if cinder_svc and cinder_svc[0].enabled:
+        return True
+
+    LOG.info("There is no volumev3 service enabled in the cloud.")
+    return False
+
+
+def is_manila_enabled():
+    """Check if Manila service is deployed in the cloud."""
+
+    admin_context = context.make_admin_context()
+    keystone = KeystoneClientV3(admin_context)
+
+    try:
+        manila_svc = keystone.client.services.list(type="sharev2")
+    except Exception:
+        LOG.exception("Failed to list services")
+        raise exception.ServicesListFailed()
+
+    if manila_svc and manila_svc[0].enabled:
+        return True
+
+    LOG.info("There is no sharev2 service enabled in the cloud.")
+    return False
+
+
+def is_cinder_csi_enabled(cluster: magnum_objects.Cluster) -> bool:
+    return (
+        get_cluster_label_as_bool(cluster, "cinder_csi_enabled", True)
+        and is_cinder_enabled()
+    )
+
+
+def is_manila_csi_enabled(cluster: magnum_objects.Cluster) -> bool:
+    return (
+        get_cluster_label_as_bool(cluster, "manila_csi_enabled", True)
+        and is_manila_enabled()
+    )
```

### Comparing `magnum_cluster_api-0.5.4/pyproject.toml` & `magnum_cluster_api-0.6.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnum-cluster-api"
-version = "0.5.4"
+version = "0.6.0"
 description = "Cluster API driver for Magnum"
 authors = ["Mohammed Naser <mnaser@vexxhost.com>"]
 readme = "README.md"
 packages = [{include = "magnum_cluster_api"}]
 include = ["magnum_cluster_api/charts/**/*"]
 
 [tool.poetry.dependencies]
@@ -16,14 +16,15 @@
 "oslo.context" = ">=4.1.0"
 "oslo.log" = ">=4.7.0"
 "oslo.privsep" = ">=2.7.0"
 "oslo.service" = ">=2.8.0"
 pykube-ng = "*"
 pyroute2 = ">=0.3.4"
 python = "^3.6"
+"python-manilaclient" = ">=3.3.2"
 requests = ">=2.27.1"
 semver = "^2.0.0"
 shortuuid = "*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "<7"
 pytest-mock = "^3.6.1"
```

### Comparing `magnum_cluster_api-0.5.4/PKG-INFO` & `magnum_cluster_api-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnum-cluster-api
-Version: 0.5.4
+Version: 0.6.0
 Summary: Cluster API driver for Magnum
 Author: Mohammed Naser
 Author-email: mnaser@vexxhost.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -19,14 +19,15 @@
 Requires-Dist: oslo.config (>=8.8.0)
 Requires-Dist: oslo.context (>=4.1.0)
 Requires-Dist: oslo.log (>=4.7.0)
 Requires-Dist: oslo.privsep (>=2.7.0)
 Requires-Dist: oslo.service (>=2.8.0)
 Requires-Dist: pykube-ng
 Requires-Dist: pyroute2 (>=0.3.4)
+Requires-Dist: python-manilaclient (>=3.3.2)
 Requires-Dist: requests (>=2.27.1)
 Requires-Dist: semver (>=2.0.0,<3.0.0)
 Requires-Dist: shortuuid
 Description-Content-Type: text/markdown
 
 ![Cluster API driver for Magnum](docs/static/logo.png?raw=true "Cluster API driver for Magnum")
```

