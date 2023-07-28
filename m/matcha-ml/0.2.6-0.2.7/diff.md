# Comparing `tmp/matcha_ml-0.2.6.tar.gz` & `tmp/matcha_ml-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matcha_ml-0.2.6.tar", max compression
+gzip compressed data, was "matcha_ml-0.2.7.tar", max compression
```

## Comparing `matcha_ml-0.2.6.tar` & `matcha_ml-0.2.7.tar`

### file list

```diff
@@ -1,118 +1,123 @@
--rw-r--r--   0        0        0    11357 2023-07-19 13:57:24.538459 matcha_ml-0.2.6/LICENSE
--rw-r--r--   0        0        0     4289 2023-07-19 13:57:24.538616 matcha_ml-0.2.6/README.md
--rw-r--r--   0        0        0     3811 2023-07-19 14:29:44.899515 matcha_ml-0.2.6/pyproject.toml
--rw-r--r--   0        0        0        6 2023-07-19 14:29:44.908241 matcha_ml-0.2.6/src/matcha_ml/VERSION
--rw-r--r--   0        0        0      220 2023-07-19 13:57:24.567863 matcha_ml-0.2.6/src/matcha_ml/__init__.py
--rw-r--r--   0        0        0       70 2023-07-19 13:57:24.568088 matcha_ml-0.2.6/src/matcha_ml/cli/__init__.py
--rw-r--r--   0        0        0     3893 2023-07-19 14:28:18.772178 matcha_ml-0.2.6/src/matcha_ml/cli/_validation.py
--rw-r--r--   0        0        0     8030 2023-07-19 14:28:18.772524 matcha_ml-0.2.6/src/matcha_ml/cli/cli.py
--rw-r--r--   0        0        0      769 2023-07-19 13:57:24.568737 matcha_ml-0.2.6/src/matcha_ml/cli/constants.py
--rw-r--r--   0        0        0     1817 2023-07-19 14:28:18.772911 matcha_ml-0.2.6/src/matcha_ml/cli/destroy.py
--rw-r--r--   0        0        0      278 2023-07-19 13:57:24.569287 matcha_ml-0.2.6/src/matcha_ml/cli/ui/emojis.py
--rw-r--r--   0        0        0     1173 2023-07-19 13:57:24.569546 matcha_ml-0.2.6/src/matcha_ml/cli/ui/print_messages.py
--rw-r--r--   0        0        0     2639 2023-07-19 14:28:18.773546 matcha_ml-0.2.6/src/matcha_ml/cli/ui/resource_message_builders.py
--rw-r--r--   0        0        0     1249 2023-07-19 14:28:18.773904 matcha_ml-0.2.6/src/matcha_ml/cli/ui/spinner.py
--rw-r--r--   0        0        0     1957 2023-07-19 14:28:18.774143 matcha_ml-0.2.6/src/matcha_ml/cli/ui/status_message_builders.py
--rw-r--r--   0        0        0     1063 2023-07-19 14:28:18.774485 matcha_ml-0.2.6/src/matcha_ml/cli/ui/user_approval_functions.py
--rw-r--r--   0        0        0      150 2023-07-19 14:28:18.774716 matcha_ml-0.2.6/src/matcha_ml/constants.py
--rw-r--r--   0        0        0      299 2023-07-19 14:28:18.775004 matcha_ml-0.2.6/src/matcha_ml/core/__init__.py
--rw-r--r--   0        0        0     2755 2023-07-19 14:28:18.775245 matcha_ml-0.2.6/src/matcha_ml/core/_validation.py
--rw-r--r--   0        0        0     9203 2023-07-19 14:28:18.775480 matcha_ml-0.2.6/src/matcha_ml/core/core.py
--rw-r--r--   0        0        0     2559 2023-07-19 14:28:18.775936 matcha_ml-0.2.6/src/matcha_ml/errors.py
--rw-r--r--   0        0        0      882 2023-07-19 13:57:24.572006 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/.gitignore
--rw-r--r--   0        0        0     1156 2023-07-19 13:57:24.572219 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/.terraform.lock.hcl
--rw-r--r--   0        0        0      440 2023-07-19 14:28:18.776357 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/main.tf
--rw-r--r--   0        0        0      762 2023-07-19 13:57:24.572721 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/output.tf
--rw-r--r--   0        0        0      110 2023-07-19 13:57:24.573124 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/resource_group/main.tf
--rw-r--r--   0        0        0      106 2023-07-19 13:57:24.573253 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/resource_group/output.tf
--rw-r--r--   0        0        0      235 2023-07-19 13:57:24.573443 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/resource_group/variables.tf
--rw-r--r--   0        0        0      776 2023-07-19 13:57:24.573629 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/state_storage/main.tf
--rw-r--r--   0        0        0     1819 2023-07-19 13:57:24.573797 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/state_storage/output.tf
--rw-r--r--   0        0        0      457 2023-07-19 13:57:24.573951 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/state_storage/variables.tf
--rw-r--r--   0        0        0      256 2023-07-19 13:57:24.574201 matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/variables.tf
--rw-r--r--   0        0        0      882 2023-07-19 13:57:24.574564 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/.gitignore
--rw-r--r--   0        0        0     9245 2023-07-19 13:57:24.574918 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/.terraform.lock.hcl
--rw-r--r--   0        0        0     4696 2023-07-19 13:57:24.575155 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/README.md
--rw-r--r--   0        0        0     2213 2023-07-19 13:57:24.575467 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/aks/README.md
--rw-r--r--   0        0        0      439 2023-07-19 13:57:24.575822 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/aks/main.tf
--rw-r--r--   0        0        0     1437 2023-07-19 13:57:24.576087 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/aks/output.tf
--rw-r--r--   0        0        0      386 2023-07-19 13:57:24.576296 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/aks/variables.tf
--rw-r--r--   0        0        0     1605 2023-07-19 13:57:24.576606 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/azure_container_registry/README.md
--rw-r--r--   0        0        0      484 2023-07-19 13:57:24.576809 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/azure_container_registry/main.tf
--rw-r--r--   0        0        0      327 2023-07-19 13:57:24.577295 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/azure_container_registry/output.tf
--rw-r--r--   0        0        0      462 2023-07-19 13:57:24.577469 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/azure_container_registry/variables.tf
--rw-r--r--   0        0        0      625 2023-07-19 13:57:24.577696 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/configure_kubectl.tf
--rw-r--r--   0        0        0      337 2023-07-19 13:57:24.577990 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/helm.tf
--rw-r--r--   0        0        0     1107 2023-07-19 13:57:24.578189 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/kubernetes.tf
--rw-r--r--   0        0        0     1885 2023-07-19 14:28:18.776812 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/main.tf
--rw-r--r--   0        0        0     2208 2023-07-19 13:57:24.578733 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/README.md
--rw-r--r--   0        0        0      308 2023-07-19 13:57:24.578903 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/getURI.tf
--rw-r--r--   0        0        0     1314 2023-07-19 13:57:24.579123 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/main.tf
--rw-r--r--   0        0        0      251 2023-07-19 13:57:24.579295 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/output.tf
--rw-r--r--   0        0        0      383 2023-07-19 13:57:24.579479 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/providers.tf
--rw-r--r--   0        0        0      803 2023-07-19 13:57:24.579662 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/variables.tf
--rw-r--r--   0        0        0       81 2023-07-19 13:57:24.579872 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/zenml_namespace.tf
--rw-r--r--   0        0        0     2458 2023-07-19 14:28:18.777114 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/output.tf
--rw-r--r--   0        0        0       33 2023-07-19 13:57:24.580447 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/printf.cmd
--rw-r--r--   0        0        0      782 2023-07-19 13:57:24.580721 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/providers.tf
--rw-r--r--   0        0        0      892 2023-07-19 13:57:24.581143 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/resource_group/README.md
--rw-r--r--   0        0        0       80 2023-07-19 13:57:24.581384 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/resource_group/main.tf
--rw-r--r--   0        0        0      111 2023-07-19 13:57:24.581545 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/resource_group/output.tf
--rw-r--r--   0        0        0       95 2023-07-19 13:57:24.581725 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/resource_group/variables.tf
--rw-r--r--   0        0        0     3010 2023-07-19 13:57:24.582085 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/README.md
--rw-r--r--   0        0        0     1894 2023-07-19 13:57:24.582500 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/istio.tf
--rw-r--r--   0        0        0     1158 2023-07-19 13:57:24.582689 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/main.tf
--rw-r--r--   0        0        0      663 2023-07-19 13:57:24.582873 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/outputs.tf
--rw-r--r--   0        0        0      925 2023-07-19 13:57:24.583130 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/permissions.tf
--rw-r--r--   0        0        0      380 2023-07-19 13:57:24.583582 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/providers.tf
--rw-r--r--   0        0        0      453 2023-07-19 13:57:24.583789 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/variables.tf
--rw-r--r--   0        0        0     2914 2023-07-19 13:57:24.584086 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/storage/README.md
--rw-r--r--   0        0        0      866 2023-07-19 13:57:24.584274 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/storage/main.tf
--rw-r--r--   0        0        0     1779 2023-07-19 13:57:24.584465 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/storage/output.tf
--rw-r--r--   0        0        0      124 2023-07-19 13:57:24.584675 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/storage/providers.tf
--rw-r--r--   0        0        0      454 2023-07-19 13:57:24.584870 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/storage/variables.tf
--rw-r--r--   0        0        0      754 2023-07-19 13:57:24.585157 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/variables.tf
--rw-r--r--   0        0        0     6080 2023-07-19 13:57:24.585488 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/README.md
--rw-r--r--   0        0        0      216 2023-07-19 13:57:24.585708 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/getURL.tf
--rw-r--r--   0        0        0      979 2023-07-19 13:57:24.586089 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/ingress.tf
--rw-r--r--   0        0        0     3026 2023-07-19 13:57:24.586498 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/main.tf
--rw-r--r--   0        0        0      704 2023-07-19 13:57:24.586731 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/outputs.tf
--rw-r--r--   0        0        0      292 2023-07-19 13:57:24.586936 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/providers.tf
--rw-r--r--   0        0        0     1943 2023-07-19 13:57:24.587532 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/sql.tf
--rw-r--r--   0        0        0     4701 2023-07-19 13:57:24.587990 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/variables.tf
--rw-r--r--   0        0        0      342 2023-07-19 13:57:24.588336 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/Chart.yaml
--rw-r--r--   0        0        0     1987 2023-07-19 13:57:24.588770 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/NOTES.txt
--rw-r--r--   0        0        0     2054 2023-07-19 13:57:24.589254 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/_helpers.tpl
--rw-r--r--   0        0        0     1565 2023-07-19 13:57:24.589472 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/cert-secret.yaml
--rw-r--r--   0        0        0      910 2023-07-19 13:57:24.589702 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/hpa.yaml
--rw-r--r--   0        0        0    10774 2023-07-19 13:57:24.589953 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-deployment.yaml
--rw-r--r--   0        0        0     2225 2023-07-19 13:57:24.590184 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-ingress.yaml
--rw-r--r--   0        0        0     3584 2023-07-19 13:57:24.590439 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-secret.yaml
--rw-r--r--   0        0        0      367 2023-07-19 13:57:24.590616 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-service.yaml
--rw-r--r--   0        0        0      316 2023-07-19 13:57:24.590824 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      379 2023-07-19 13:57:24.591193 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/tests/test-connection.yaml
--rw-r--r--   0        0        0    11587 2023-07-19 13:57:24.591487 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/values.yaml
--rw-r--r--   0        0        0     3453 2023-07-19 13:57:24.591783 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zenml_storage/README.md
--rw-r--r--   0        0        0     1102 2023-07-19 13:57:24.592009 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zenml_storage/main.tf
--rw-r--r--   0        0        0     1926 2023-07-19 13:57:24.592187 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zenml_storage/output.tf
--rw-r--r--   0        0        0      468 2023-07-19 13:57:24.592418 matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zenml_storage/variables.tf
--rw-r--r--   0        0        0      170 2023-07-19 14:28:18.777464 matcha_ml-0.2.6/src/matcha_ml/runners/__init__.py
--rw-r--r--   0        0        0     2478 2023-07-19 14:28:18.777841 matcha_ml-0.2.6/src/matcha_ml/runners/azure_runner.py
--rw-r--r--   0        0        0     6546 2023-07-19 14:28:18.778250 matcha_ml-0.2.6/src/matcha_ml/runners/base_runner.py
--rw-r--r--   0        0        0     2847 2023-07-19 14:28:18.778557 matcha_ml-0.2.6/src/matcha_ml/runners/remote_state_runner.py
--rw-r--r--   0        0        0      103 2023-07-19 13:57:24.593553 matcha_ml-0.2.6/src/matcha_ml/services/__init__.py
--rw-r--r--   0        0        0      646 2023-07-19 13:57:24.593744 matcha_ml-0.2.6/src/matcha_ml/services/_validation.py
--rw-r--r--   0        0        0     4711 2023-07-19 14:28:18.778966 matcha_ml-0.2.6/src/matcha_ml/services/analytics_service.py
--rw-r--r--   0        0        0    10848 2023-07-19 14:28:18.779487 matcha_ml-0.2.6/src/matcha_ml/services/azure_service.py
--rw-r--r--   0        0        0     4542 2023-07-19 14:28:18.780112 matcha_ml-0.2.6/src/matcha_ml/services/global_parameters_service.py
--rw-r--r--   0        0        0     5609 2023-07-19 14:28:18.780501 matcha_ml-0.2.6/src/matcha_ml/services/terraform_service.py
--rw-r--r--   0        0        0      213 2023-07-19 14:28:18.780856 matcha_ml-0.2.6/src/matcha_ml/state/__init__.py
--rw-r--r--   0        0        0    12364 2023-07-19 14:28:18.781389 matcha_ml-0.2.6/src/matcha_ml/state/matcha_state.py
--rw-r--r--   0        0        0    11275 2023-07-19 14:28:18.782017 matcha_ml-0.2.6/src/matcha_ml/state/remote_state_manager.py
--rw-r--r--   0        0        0       94 2023-07-19 13:57:24.595939 matcha_ml-0.2.6/src/matcha_ml/storage/__init__.py
--rw-r--r--   0        0        0     9883 2023-07-19 14:28:18.782566 matcha_ml-0.2.6/src/matcha_ml/storage/azure_storage.py
--rw-r--r--   0        0        0      184 2023-07-19 13:57:24.596527 matcha_ml-0.2.6/src/matcha_ml/templates/__init__.py
--rw-r--r--   0        0        0     1923 2023-07-19 14:28:18.783143 matcha_ml-0.2.6/src/matcha_ml/templates/azure_template.py
--rw-r--r--   0        0        0     7255 2023-07-19 13:57:24.597046 matcha_ml-0.2.6/src/matcha_ml/templates/base_template.py
--rw-r--r--   0        0        0      635 2023-07-19 13:57:24.597267 matcha_ml-0.2.6/src/matcha_ml/templates/remote_state_template.py
--rw-r--r--   0        0        0     6233 1970-01-01 00:00:00.000000 matcha_ml-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-19 13:57:24.538459 matcha_ml-0.2.7/LICENSE
+-rw-r--r--   0        0        0     4289 2023-07-19 13:57:24.538616 matcha_ml-0.2.7/README.md
+-rw-r--r--   0        0        0     3811 2023-07-28 14:19:49.158309 matcha_ml-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-07-28 14:19:49.184528 matcha_ml-0.2.7/src/matcha_ml/VERSION
+-rw-r--r--   0        0        0      220 2023-07-19 13:57:24.567863 matcha_ml-0.2.7/src/matcha_ml/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-19 13:57:24.568088 matcha_ml-0.2.7/src/matcha_ml/cli/__init__.py
+-rw-r--r--   0        0        0     3893 2023-07-19 14:28:18.772178 matcha_ml-0.2.7/src/matcha_ml/cli/_validation.py
+-rw-r--r--   0        0        0     8030 2023-07-19 14:28:18.772524 matcha_ml-0.2.7/src/matcha_ml/cli/cli.py
+-rw-r--r--   0        0        0     1226 2023-07-28 14:19:01.973876 matcha_ml-0.2.7/src/matcha_ml/cli/constants.py
+-rw-r--r--   0        0        0     1817 2023-07-19 14:28:18.772911 matcha_ml-0.2.7/src/matcha_ml/cli/destroy.py
+-rw-r--r--   0        0        0      278 2023-07-19 13:57:24.569287 matcha_ml-0.2.7/src/matcha_ml/cli/ui/emojis.py
+-rw-r--r--   0        0        0     1173 2023-07-19 13:57:24.569546 matcha_ml-0.2.7/src/matcha_ml/cli/ui/print_messages.py
+-rw-r--r--   0        0        0     2639 2023-07-19 14:28:18.773546 matcha_ml-0.2.7/src/matcha_ml/cli/ui/resource_message_builders.py
+-rw-r--r--   0        0        0     1358 2023-07-28 14:19:01.974497 matcha_ml-0.2.7/src/matcha_ml/cli/ui/spinner.py
+-rw-r--r--   0        0        0     2659 2023-07-28 14:19:01.975312 matcha_ml-0.2.7/src/matcha_ml/cli/ui/status_message_builders.py
+-rw-r--r--   0        0        0     1063 2023-07-19 14:28:18.774485 matcha_ml-0.2.7/src/matcha_ml/cli/ui/user_approval_functions.py
+-rw-r--r--   0        0        0      150 2023-07-21 14:25:12.611021 matcha_ml-0.2.7/src/matcha_ml/constants.py
+-rw-r--r--   0        0        0      299 2023-07-19 14:28:18.775004 matcha_ml-0.2.7/src/matcha_ml/core/__init__.py
+-rw-r--r--   0        0        0     2755 2023-07-19 14:28:18.775245 matcha_ml-0.2.7/src/matcha_ml/core/_validation.py
+-rw-r--r--   0        0        0     9883 2023-07-28 14:19:01.976024 matcha_ml-0.2.7/src/matcha_ml/core/core.py
+-rw-r--r--   0        0        0     2535 2023-07-28 14:19:01.976550 matcha_ml-0.2.7/src/matcha_ml/errors.py
+-rw-r--r--   0        0        0      882 2023-07-19 13:57:24.572006 matcha_ml-0.2.7/src/matcha_ml/infrastructure/remote_state_storage/.gitignore
+-rw-r--r--   0        0        0     1156 2023-07-19 13:57:24.572219 matcha_ml-0.2.7/src/matcha_ml/infrastructure/remote_state_storage/.terraform.lock.hcl
+-rw-r--r--   0        0        0      440 2023-07-19 14:28:18.776357 matcha_ml-0.2.7/src/matcha_ml/infrastructure/remote_state_storage/main.tf
+-rw-r--r--   0        0        0      896 2023-07-28 14:19:01.976828 matcha_ml-0.2.7/src/matcha_ml/infrastructure/remote_state_storage/output.tf
+-rw-r--r--   0        0        0      110 2023-07-19 13:57:24.573124 matcha_ml-0.2.7/src/matcha_ml/infrastructure/remote_state_storage/resource_group/main.tf
+-rw-r--r--   0        0        0      106 2023-07-19 13:57:24.573253 matcha_ml-0.2.7/src/matcha_ml/infrastructure/remote_state_storage/resource_group/output.tf
+-rw-r--r--   0        0        0      235 2023-07-19 13:57:24.573443 matcha_ml-0.2.7/src/matcha_ml/infrastructure/remote_state_storage/resource_group/variables.tf
+-rw-r--r--   0        0        0      776 2023-07-19 13:57:24.573629 matcha_ml-0.2.7/src/matcha_ml/infrastructure/remote_state_storage/state_storage/main.tf
+-rw-r--r--   0        0        0     1819 2023-07-19 13:57:24.573797 matcha_ml-0.2.7/src/matcha_ml/infrastructure/remote_state_storage/state_storage/output.tf
+-rw-r--r--   0        0        0      457 2023-07-19 13:57:24.573951 matcha_ml-0.2.7/src/matcha_ml/infrastructure/remote_state_storage/state_storage/variables.tf
+-rw-r--r--   0        0        0      256 2023-07-19 13:57:24.574201 matcha_ml-0.2.7/src/matcha_ml/infrastructure/remote_state_storage/variables.tf
+-rw-r--r--   0        0        0      882 2023-07-19 13:57:24.574564 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/.gitignore
+-rw-r--r--   0        0        0     9245 2023-07-19 13:57:24.574918 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/.terraform.lock.hcl
+-rw-r--r--   0        0        0     4696 2023-07-19 13:57:24.575155 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/README.md
+-rw-r--r--   0        0        0     2213 2023-07-19 13:57:24.575467 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/aks/README.md
+-rw-r--r--   0        0        0      439 2023-07-19 13:57:24.575822 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/aks/main.tf
+-rw-r--r--   0        0        0     1437 2023-07-19 13:57:24.576087 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/aks/output.tf
+-rw-r--r--   0        0        0      386 2023-07-19 13:57:24.576296 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/aks/variables.tf
+-rw-r--r--   0        0        0     1605 2023-07-19 13:57:24.576606 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/azure_container_registry/README.md
+-rw-r--r--   0        0        0      484 2023-07-19 13:57:24.576809 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/azure_container_registry/main.tf
+-rw-r--r--   0        0        0      327 2023-07-19 13:57:24.577295 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/azure_container_registry/output.tf
+-rw-r--r--   0        0        0      462 2023-07-19 13:57:24.577469 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/azure_container_registry/variables.tf
+-rw-r--r--   0        0        0      625 2023-07-19 13:57:24.577696 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/configure_kubectl.tf
+-rw-r--r--   0        0        0     2914 2023-07-28 14:19:01.977094 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/data_version_control_storage/README.md
+-rw-r--r--   0        0        0      870 2023-07-28 14:19:01.977222 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/data_version_control_storage/main.tf
+-rw-r--r--   0        0        0      514 2023-07-28 14:19:01.977425 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/data_version_control_storage/output.tf
+-rw-r--r--   0        0        0      124 2023-07-28 14:19:01.978067 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/data_version_control_storage/providers.tf
+-rw-r--r--   0        0        0      442 2023-07-28 14:19:01.978305 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/data_version_control_storage/variables.tf
+-rw-r--r--   0        0        0      337 2023-07-19 13:57:24.577990 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/helm.tf
+-rw-r--r--   0        0        0     1107 2023-07-19 13:57:24.578189 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/kubernetes.tf
+-rw-r--r--   0        0        0     2096 2023-07-28 14:19:01.978639 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/main.tf
+-rw-r--r--   0        0        0     2208 2023-07-19 13:57:24.578733 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/mlflow_module/README.md
+-rw-r--r--   0        0        0      308 2023-07-19 13:57:24.578903 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/mlflow_module/getURI.tf
+-rw-r--r--   0        0        0     1314 2023-07-19 13:57:24.579123 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/mlflow_module/main.tf
+-rw-r--r--   0        0        0      251 2023-07-19 13:57:24.579295 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/mlflow_module/output.tf
+-rw-r--r--   0        0        0      383 2023-07-19 13:57:24.579479 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/mlflow_module/providers.tf
+-rw-r--r--   0        0        0      803 2023-07-19 13:57:24.579662 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/mlflow_module/variables.tf
+-rw-r--r--   0        0        0       81 2023-07-19 13:57:24.579872 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/mlflow_module/zenml_namespace.tf
+-rw-r--r--   0        0        0     3090 2023-07-28 14:19:01.978931 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/output.tf
+-rw-r--r--   0        0        0       33 2023-07-19 13:57:24.580447 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/printf.cmd
+-rw-r--r--   0        0        0      782 2023-07-19 13:57:24.580721 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/providers.tf
+-rw-r--r--   0        0        0      892 2023-07-19 13:57:24.581143 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/resource_group/README.md
+-rw-r--r--   0        0        0       80 2023-07-19 13:57:24.581384 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/resource_group/main.tf
+-rw-r--r--   0        0        0      111 2023-07-19 13:57:24.581545 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/resource_group/output.tf
+-rw-r--r--   0        0        0       95 2023-07-19 13:57:24.581725 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/resource_group/variables.tf
+-rw-r--r--   0        0        0     3010 2023-07-19 13:57:24.582085 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/seldon/README.md
+-rw-r--r--   0        0        0     1894 2023-07-19 13:57:24.582500 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/seldon/istio.tf
+-rw-r--r--   0        0        0     1158 2023-07-19 13:57:24.582689 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/seldon/main.tf
+-rw-r--r--   0        0        0      663 2023-07-19 13:57:24.582873 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/seldon/outputs.tf
+-rw-r--r--   0        0        0      925 2023-07-19 13:57:24.583130 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/seldon/permissions.tf
+-rw-r--r--   0        0        0      380 2023-07-19 13:57:24.583582 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/seldon/providers.tf
+-rw-r--r--   0        0        0      453 2023-07-19 13:57:24.583789 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/seldon/variables.tf
+-rw-r--r--   0        0        0     2914 2023-07-19 13:57:24.584086 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/storage/README.md
+-rw-r--r--   0        0        0      866 2023-07-19 13:57:24.584274 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/storage/main.tf
+-rw-r--r--   0        0        0     1779 2023-07-19 13:57:24.584465 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/storage/output.tf
+-rw-r--r--   0        0        0      124 2023-07-19 13:57:24.584675 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/storage/providers.tf
+-rw-r--r--   0        0        0      454 2023-07-19 13:57:24.584870 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/storage/variables.tf
+-rw-r--r--   0        0        0      754 2023-07-19 13:57:24.585157 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/variables.tf
+-rw-r--r--   0        0        0     6080 2023-07-19 13:57:24.585488 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/README.md
+-rw-r--r--   0        0        0      216 2023-07-19 13:57:24.585708 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/getURL.tf
+-rw-r--r--   0        0        0      979 2023-07-19 13:57:24.586089 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/ingress.tf
+-rw-r--r--   0        0        0     3026 2023-07-19 13:57:24.586498 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/main.tf
+-rw-r--r--   0        0        0      704 2023-07-19 13:57:24.586731 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/outputs.tf
+-rw-r--r--   0        0        0      292 2023-07-19 13:57:24.586936 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/providers.tf
+-rw-r--r--   0        0        0     1943 2023-07-19 13:57:24.587532 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/sql.tf
+-rw-r--r--   0        0        0     4701 2023-07-19 13:57:24.587990 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/variables.tf
+-rw-r--r--   0        0        0      342 2023-07-19 13:57:24.588336 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/Chart.yaml
+-rw-r--r--   0        0        0     1987 2023-07-19 13:57:24.588770 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/NOTES.txt
+-rw-r--r--   0        0        0     2054 2023-07-19 13:57:24.589254 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1565 2023-07-19 13:57:24.589472 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/cert-secret.yaml
+-rw-r--r--   0        0        0      910 2023-07-19 13:57:24.589702 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/hpa.yaml
+-rw-r--r--   0        0        0    10774 2023-07-19 13:57:24.589953 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-deployment.yaml
+-rw-r--r--   0        0        0     2225 2023-07-19 13:57:24.590184 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-ingress.yaml
+-rw-r--r--   0        0        0     3584 2023-07-19 13:57:24.590439 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-secret.yaml
+-rw-r--r--   0        0        0      367 2023-07-19 13:57:24.590616 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-service.yaml
+-rw-r--r--   0        0        0      316 2023-07-19 13:57:24.590824 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      379 2023-07-19 13:57:24.591193 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/tests/test-connection.yaml
+-rw-r--r--   0        0        0    11587 2023-07-19 13:57:24.591487 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/values.yaml
+-rw-r--r--   0        0        0     3453 2023-07-19 13:57:24.591783 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zenml_storage/README.md
+-rw-r--r--   0        0        0     1102 2023-07-19 13:57:24.592009 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zenml_storage/main.tf
+-rw-r--r--   0        0        0     1926 2023-07-19 13:57:24.592187 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zenml_storage/output.tf
+-rw-r--r--   0        0        0      468 2023-07-19 13:57:24.592418 matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zenml_storage/variables.tf
+-rw-r--r--   0        0        0      170 2023-07-19 14:28:18.777464 matcha_ml-0.2.7/src/matcha_ml/runners/__init__.py
+-rw-r--r--   0        0        0     2345 2023-07-28 14:19:01.979919 matcha_ml-0.2.7/src/matcha_ml/runners/azure_runner.py
+-rw-r--r--   0        0        0     7202 2023-07-28 14:19:01.980527 matcha_ml-0.2.7/src/matcha_ml/runners/base_runner.py
+-rw-r--r--   0        0        0     2843 2023-07-28 14:19:01.981052 matcha_ml-0.2.7/src/matcha_ml/runners/remote_state_runner.py
+-rw-r--r--   0        0        0      103 2023-07-19 13:57:24.593553 matcha_ml-0.2.7/src/matcha_ml/services/__init__.py
+-rw-r--r--   0        0        0      646 2023-07-19 13:57:24.593744 matcha_ml-0.2.7/src/matcha_ml/services/_validation.py
+-rw-r--r--   0        0        0     5147 2023-07-28 14:19:01.981336 matcha_ml-0.2.7/src/matcha_ml/services/analytics_service.py
+-rw-r--r--   0        0        0    10848 2023-07-19 14:28:18.779487 matcha_ml-0.2.7/src/matcha_ml/services/azure_service.py
+-rw-r--r--   0        0        0     4542 2023-07-19 14:28:18.780112 matcha_ml-0.2.7/src/matcha_ml/services/global_parameters_service.py
+-rw-r--r--   0        0        0     5792 2023-07-28 14:19:01.981959 matcha_ml-0.2.7/src/matcha_ml/services/terraform_service.py
+-rw-r--r--   0        0        0      213 2023-07-19 14:28:18.780856 matcha_ml-0.2.7/src/matcha_ml/state/__init__.py
+-rw-r--r--   0        0        0    12394 2023-07-28 14:19:01.982957 matcha_ml-0.2.7/src/matcha_ml/state/matcha_state.py
+-rw-r--r--   0        0        0    11596 2023-07-28 14:19:01.983913 matcha_ml-0.2.7/src/matcha_ml/state/remote_state_manager.py
+-rw-r--r--   0        0        0       94 2023-07-19 13:57:24.595939 matcha_ml-0.2.7/src/matcha_ml/storage/__init__.py
+-rw-r--r--   0        0        0     9883 2023-07-19 14:28:18.782566 matcha_ml-0.2.7/src/matcha_ml/storage/azure_storage.py
+-rw-r--r--   0        0        0      184 2023-07-19 13:57:24.596527 matcha_ml-0.2.7/src/matcha_ml/templates/__init__.py
+-rw-r--r--   0        0        0     2041 2023-07-28 14:19:01.984823 matcha_ml-0.2.7/src/matcha_ml/templates/azure_template.py
+-rw-r--r--   0        0        0     7255 2023-07-19 13:57:24.597046 matcha_ml-0.2.7/src/matcha_ml/templates/base_template.py
+-rw-r--r--   0        0        0      635 2023-07-19 13:57:24.597267 matcha_ml-0.2.7/src/matcha_ml/templates/remote_state_template.py
+-rw-r--r--   0        0        0     6233 1970-01-01 00:00:00.000000 matcha_ml-0.2.7/PKG-INFO
```

### Comparing `matcha_ml-0.2.6/LICENSE` & `matcha_ml-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/README.md` & `matcha_ml-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/pyproject.toml` & `matcha_ml-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "matcha-ml"
-version = "0.2.6"
+version = "0.2.7"
 description = "Matcha: An open source tool for provisioning MLOps environments to the cloud."
 authors = ["FuzzyLabs <info@fuzzylabs.ai>"]
 license = "Apache-2.0"
 homepage = "http://fuzzylabs.github.io/matcha"
 documentation = "http://fuzzylabs.github.io/matcha"
 repository = "https://github.com/fuzzylabs/matcha"
 readme = "README.md"
@@ -151,9 +151,9 @@
 module = [
     "python_terraform.*",
     "segment.*"
 ]
 ignore_missing_imports = true
 
 [tool.ruff.pylint]
-max-branches = 13
+max-branches = 14
 max-args = 6
```

### Comparing `matcha_ml-0.2.6/src/matcha_ml/cli/_validation.py` & `matcha_ml-0.2.7/src/matcha_ml/cli/_validation.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/cli/cli.py` & `matcha_ml-0.2.7/src/matcha_ml/cli/cli.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/cli/destroy.py` & `matcha_ml-0.2.7/src/matcha_ml/cli/destroy.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/cli/ui/print_messages.py` & `matcha_ml-0.2.7/src/matcha_ml/cli/ui/print_messages.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/cli/ui/resource_message_builders.py` & `matcha_ml-0.2.7/src/matcha_ml/cli/ui/resource_message_builders.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/cli/ui/spinner.py` & `matcha_ml-0.2.7/src/matcha_ml/cli/ui/spinner.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,17 +26,22 @@
         self.progress = Progress(
             SpinnerColumn(spinner_name=SPINNER),
             TimeElapsedColumn(),
             TextColumn("[progress.description]{task.description}"),
         )
         self.progress.add_task(description=status, total=None)
 
-    def __enter__(self) -> None:
-        """Call when a spinner object is created using a `with` statement."""
+    def __enter__(self) -> "Spinner":
+        """Call when a spinner object is created using a `with` statement.
+
+        Returns:
+            Spinner: the instance for a context manager.
+        """
         self.progress.start()
+        return self
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None:
```

### Comparing `matcha_ml-0.2.6/src/matcha_ml/cli/ui/user_approval_functions.py` & `matcha_ml-0.2.7/src/matcha_ml/cli/ui/user_approval_functions.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/core/_validation.py` & `matcha_ml-0.2.7/src/matcha_ml/core/_validation.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/core/core.py` & `matcha_ml-0.2.7/src/matcha_ml/core/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,41 @@
 """The core functionality for Matcha API."""
 import os
 from typing import Optional
+from warnings import warn
 
 from matcha_ml.cli._validation import get_command_validation
 from matcha_ml.cli.ui.print_messages import print_status
 from matcha_ml.cli.ui.status_message_builders import build_warning_status
 from matcha_ml.core._validation import is_valid_prefix, is_valid_region
 from matcha_ml.errors import MatchaError, MatchaInputError
 from matcha_ml.runners import AzureRunner
 from matcha_ml.services.analytics_service import AnalyticsEvent, track
 from matcha_ml.services.global_parameters_service import GlobalParameters
 from matcha_ml.state import MatchaStateService, RemoteStateManager
 from matcha_ml.state.matcha_state import MatchaState
 from matcha_ml.templates.azure_template import AzureTemplate
 
 
+MAJOR_MINOR_ZENML_VERSION = "0.36"
+
+
+def zenml_version_is_supported() -> None:
+    """Check the zenml version of the local environment against the version matcha is expecting."""
+    try:
+        import zenml
+        if zenml.__version__[:3] != MAJOR_MINOR_ZENML_VERSION:
+            warn(
+                f"Matcha expects ZenML version {MAJOR_MINOR_ZENML_VERSION}.x, but you have version {zenml.__version__}."
+            )
+    except:
+        warn(f"No local installation of ZenMl found. Defaulting to version {MAJOR_MINOR_ZENML_VERSION} for remote "
+             f"resources.")
+
+
 @track(event_name=AnalyticsEvent.GET)
 def get(
     resource_name: Optional[str],
     property_name: Optional[str],
 ) -> MatchaState:
     """Return information regarding a previously provisioned resource based on the resource and property names provided.
 
@@ -113,15 +130,17 @@
 
     if not remote_state_manager.is_state_provisioned():
         raise MatchaError(
             "Error - resources that have not been provisioned cannot be destroyed. Run 'matcha provision' to get started!"
         )
 
     template_runner = AzureRunner()
-    with remote_state_manager.use_lock(), remote_state_manager.use_remote_state():
+    with remote_state_manager.use_lock(
+        destroy=True
+    ), remote_state_manager.use_remote_state(destroy=True):
         template_runner.deprovision()
         remote_state_manager.deprovision_remote_state()
 
 
 def analytics_opt_out() -> None:
     """Disable the collection of anonymous usage data.
 
@@ -180,14 +199,15 @@
         MatchaState: the information of the provisioned resources.
 
     Raises:
         MatchaError: If resources are already provisioned.
         MatchaError: If prefix is not valid.
         MatchaError: If region is not valid.
     """
+    zenml_version_is_supported()
     remote_state_manager = RemoteStateManager()
     template_runner = AzureRunner()
 
     if MatchaStateService.state_exists():
         matcha_state_service = MatchaStateService()
         if matcha_state_service.is_local_state_stale():
             template_runner.remove_matcha_dir()
```

### Comparing `matcha_ml-0.2.6/src/matcha_ml/errors.py` & `matcha_ml-0.2.7/src/matcha_ml/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,11 +77,9 @@
         """Initialize Matcha Terraform Error.
 
         Args:
             tf_error: terraform error
             *args: args
             **kwargs: kwargs
         """
-        message = (
-            f"Terraform failed because of the following error: '{tf_error}'."
-        )
+        message = f"Terraform failed because of the following error: '{tf_error}'."
         super().__init__(message, *args, **kwargs)
```

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/.gitignore` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/remote_state_storage/.gitignore`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/.terraform.lock.hcl` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/remote_state_storage/.terraform.lock.hcl`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/output.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/remote_state_storage/output.tf`

 * *Files 23% similar despite different names*

```diff
@@ -18,7 +18,12 @@
   value = var.prefix
 }
 
 output "cloud_azure_location"{
   description = "The Azure location in which the resources are provisioned" 
   value = var.location
 }
+
+output "cloud_azure_resource_group_name" {
+  description = "Name of the Azure resource group"
+  value = module.resource_group.name
+}
```

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/state_storage/main.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/remote_state_storage/state_storage/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/remote_state_storage/state_storage/output.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/remote_state_storage/state_storage/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/.gitignore` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/.terraform.lock.hcl` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/.terraform.lock.hcl`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/README.md` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/aks/README.md` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/aks/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/aks/output.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/aks/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/azure_container_registry/README.md` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/azure_container_registry/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/configure_kubectl.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/configure_kubectl.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/kubernetes.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/kubernetes.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/main.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/main.tf`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,22 @@
 
   prefix              = var.prefix
   resource_group_name = module.resource_group.name
   location            = var.location
   aks_principal_id    = module.aks.aks_principal_id
 }
 
+module "data_version_control_storage" {
+  source = "./data_version_control_storage"
+
+  resource_group_name = module.resource_group.name
+  prefix              = var.prefix
+  location            = var.location
+}
+
 module "aks" {
   source = "./aks"
 
   prefix              = var.prefix
   location            = var.location
   resource_group_name = module.resource_group.name
 }
```

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/README.md` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/mlflow_module/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/main.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/mlflow_module/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/mlflow_module/variables.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/mlflow_module/variables.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/output.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/output.tf`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 }
 
 output "pipeline_zenml_storage_path" {
   description = "The Azure Blob Storage Container path for storing ZenML artifacts"
   value       = module.zenml_storage.zenml_blobstorage_container_path
 }
 
+
 output "pipeline_zenml_connection_string" {
   description = "The primary connection string for the ZenML Azure Storage Account"
   value       = module.zenml_storage.zenml_primary_connection_string
   sensitive   = true
 }
 
 output "orchestrator_aks_k8s_context" {
@@ -71,7 +72,23 @@
   value = var.prefix
 }
 
 output "cloud_azure_location"{
   description = "The Azure location in which the resources are provisioned" 
   value = var.location
 }
+
+output "data_version_control_primary_connection_string"{
+  description = "The primary connection string for the ZenML Azure Storage Account"
+  value = module.data_version_control_storage.primary_connection_string
+  sensitive = true
+}
+
+output "data_version_control_storage_container_name"{
+  description = "The name of the container used for data version control"
+  value = module.data_version_control_storage.storage_container_name
+}
+
+output "data_version_control_storage_account_name"{
+  description = "The name of the storage account for data version control"
+  value = module.data_version_control_storage.storage_account_name
+}
```

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/providers.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/providers.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/resource_group/README.md` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/resource_group/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/README.md` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/seldon/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/istio.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/seldon/istio.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/main.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/seldon/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/outputs.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/seldon/outputs.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/seldon/permissions.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/seldon/permissions.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/storage/README.md` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/data_version_control_storage/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/storage/main.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/storage/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/storage/output.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/storage/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/variables.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/variables.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/README.md` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/ingress.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/ingress.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/main.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/outputs.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/outputs.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/sql.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/sql.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/variables.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/variables.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/NOTES.txt` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/_helpers.tpl` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/cert-secret.yaml` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/cert-secret.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/hpa.yaml` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/hpa.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-deployment.yaml` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-deployment.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-ingress.yaml` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-ingress.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-secret.yaml` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-secret.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/values.yaml` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/values.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zenml_storage/README.md` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zenml_storage/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zenml_storage/main.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zenml_storage/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/infrastructure/resources/zenml_storage/output.tf` & `matcha_ml-0.2.7/src/matcha_ml/infrastructure/resources/zenml_storage/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/runners/azure_runner.py` & `matcha_ml-0.2.7/src/matcha_ml/runners/azure_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,14 @@
 )
 from matcha_ml.cli.ui.status_message_builders import (
     build_status,
 )
 from matcha_ml.runners.base_runner import BaseRunner
 from matcha_ml.state.matcha_state import MatchaState, MatchaStateService
 
-RESOURCE_NAMES = [
-    "experiment_tracker",
-    "pipeline",
-    "orchestrator",
-    "cloud",
-    "container_registry",
-    "model_deployer",
-]
-
 
 class AzureRunner(BaseRunner):
     """A Runner class provides methods that interface with the Terraform service to facilitate the provisioning and deprovisioning of resources."""
 
     def __init__(self) -> None:
         """Initialize AzureRunner class."""
         super().__init__()
@@ -53,15 +44,15 @@
 
     def provision(self) -> None:
         """Provision resources required for the deployment."""
         self._check_terraform_installation()
         self._validate_terraform_config()
         self._validate_kubeconfig(base_path=".kube/config")
         self._initialize_terraform(msg="Matcha")
-        self._apply_terraform()
+        self._apply_terraform(msg="Matcha")
         tf_output = self.tfs.terraform_client.output()
         matcha_state_service = MatchaStateService(terraform_output=tf_output)
         self._show_terraform_outputs(matcha_state_service._state)
 
     def deprovision(self) -> None:
         """Destroy the provisioned resources."""
         self._check_matcha_directory_exists()
```

### Comparing `matcha_ml-0.2.6/src/matcha_ml/runners/base_runner.py` & `matcha_ml-0.2.7/src/matcha_ml/runners/base_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 """Run terraform templates to provision and deprovision resources."""
 import os
+from multiprocessing.pool import ThreadPool
 from typing import Optional, Tuple
 
 import typer
 
 from matcha_ml.cli.ui.emojis import Emojis
 from matcha_ml.cli.ui.print_messages import print_error, print_status
 from matcha_ml.cli.ui.spinner import Spinner
 from matcha_ml.cli.ui.status_message_builders import (
     build_status,
     build_substep_success_status,
+    terraform_status_update,
 )
 from matcha_ml.errors import MatchaTerraformError
-from matcha_ml.services.terraform_service import TerraformConfig, TerraformService
+from matcha_ml.services.terraform_service import (
+    TerraformConfig,
+    TerraformService,
+)
 
 SPINNER = "dots"
 
 
 class BaseRunner:
     """A BaseRunner class provides methods that interface with the Terraform service to facilitate the provisioning and deprovisioning of resources."""
 
@@ -91,19 +96,19 @@
             print_status(
                 build_status(
                     f"\n{Emojis.WAITING.value} Brewing matcha {Emojis.MATCHA.value}...\n"
                 )
             )
 
             with Spinner("Initializing"):
-                ret_code, _, err = self.tfs.init()
+                tf_result = self.tfs.init()
 
-                if ret_code != 0:
+                if tf_result.return_code != 0:
                     print_error("The command 'terraform init' failed.")
-                    raise MatchaTerraformError(tf_error=err)
+                    raise MatchaTerraformError(tf_error=tf_result.std_err)
 
             print_status(
                 build_substep_success_status(
                     f"{Emojis.CHECKMARK.value} {msg} {Emojis.MATCHA.value} initialized!\n"
                 )
             )
 
@@ -122,48 +127,64 @@
 
         if not self.tfs.check_matcha_directory_integrity():
             print_error(
                 "Error, the .matcha directory does not contain files relating to deployed resources. Please ensure you are trying to destroy resources that you have provisioned in the current working directory."
             )
             raise typer.Exit()
 
-    def _apply_terraform(self) -> None:
+    def _apply_terraform(self, msg: str = "") -> None:
         """Run terraform apply to create resources on cloud.
 
+        Args:
+            msg (str) : Name of the type of resource (e.g. "Remote State" or "Matcha").
+
         Raises:
             MatchaTerraformError: if 'terraform apply' failed.
         """
-        with Spinner("Applying"):
-            ret_code, _, err = self.tfs.apply()
+        with Spinner("Applying") as spinner:
+            pool = ThreadPool(processes=1)
+            _ = pool.apply_async(terraform_status_update, (spinner,))
 
-            if ret_code != 0:
-                raise MatchaTerraformError(tf_error=err)
-        print_status(
-            build_substep_success_status(
-                f"{Emojis.CHECKMARK.value} Matcha resources have been provisioned!\n"
+            tf_result = self.tfs.apply()
+
+            pool.terminate()
+
+            if tf_result.return_code != 0:
+                raise MatchaTerraformError(tf_error=tf_result.std_err)
+
+        if msg:
+            print_status(
+                build_substep_success_status(
+                    f"{Emojis.CHECKMARK.value} {msg} resources have been provisioned!\n"
+                )
+            )
+        else:
+            print_status(
+                build_substep_success_status(
+                    f"{Emojis.CHECKMARK.value} Resources have been provisioned!\n"
+                )
             )
-        )
 
     def _destroy_terraform(self, msg: str = "") -> None:
         """Destroy the provisioned resources.
 
         Raises:
             MatchaTerraformError: if 'terraform destroy' failed.
             msg (str) : Message to display. Default is empty string.
         """
         print()
         print_status(
             build_status(f"{Emojis.WAITING.value} Destroying {msg} resources...")
         )
         print()
         with Spinner("Destroying"):
-            ret_code, _, err = self.tfs.destroy()
+            tf_result = self.tfs.destroy()
 
-            if ret_code != 0:
-                raise MatchaTerraformError(tf_error=err)
+            if tf_result.return_code != 0:
+                raise MatchaTerraformError(tf_error=tf_result.std_err)
 
     def provision(self) -> Optional[Tuple[str, str, str]]:
         """Provision resources required for the deployment."""
         raise NotImplementedError
 
     def deprovision(self) -> None:
         """Destroy the provisioned resources."""
```

### Comparing `matcha_ml-0.2.6/src/matcha_ml/runners/remote_state_runner.py` & `matcha_ml-0.2.7/src/matcha_ml/runners/remote_state_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,15 @@
 
         account_name = ""
         container_name = ""
         resource_group_name = ""
 
         prefix = "remote_state_storage"
         account_name = tf_outputs[f"{prefix}_account_name"]["value"]
-        resource_group_name = tf_outputs[f"{prefix}_resource_group_name"][
-            "value"
-        ]
+        resource_group_name = tf_outputs[f"{prefix}_resource_group_name"]["value"]
         container_name = tf_outputs[f"{prefix}_container_name"]["value"]
 
         return account_name, container_name, resource_group_name
 
     def _clean_up(self) -> None:
         """Remove the whole .matcha directory when destroy full is run."""
         matcha_template_dir = os.path.join(os.getcwd(), ".matcha")
@@ -61,15 +59,15 @@
         Returns:
             Tuple[str, str]: account name, the container name and azure resource_group_name.
         """
         self._check_terraform_installation()
         self._validate_terraform_config()
         self._validate_kubeconfig(base_path=".kube/config")
         self._initialize_terraform(msg="Remote State")
-        self._apply_terraform()
+        self._apply_terraform(msg="Remote State")
         return self._get_terraform_output()
 
     def deprovision(self) -> None:
         """Destroy the provisioned resources."""
         self._check_matcha_directory_exists()
         self._check_terraform_installation()
         self._initialize_terraform(msg="Remote State")
```

### Comparing `matcha_ml-0.2.6/src/matcha_ml/services/_validation.py` & `matcha_ml-0.2.7/src/matcha_ml/services/_validation.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/services/analytics_service.py` & `matcha_ml-0.2.7/src/matcha_ml/services/analytics_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 """The analytics service interface.
 
 This approach to collecting usage data was inspired by ZenML; source: https://github.com/zenml-io/zenml/blob/main/src/zenml/utils/analytics_utils.py
 """
 import functools
+import logging
 from enum import Enum
 from time import perf_counter
 from typing import Any, Callable, Optional, Tuple
 from warnings import warn
 
 from segment import analytics
 
 from matcha_ml.errors import MatchaError
 from matcha_ml.services._validation import _check_uuid
 from matcha_ml.services.global_parameters_service import GlobalParameters
 from matcha_ml.state import MatchaState, MatchaStateService
 
-analytics.write_key = "qwBKAvY6MEUvv5XIs4rE07ohf5neT3sx"
+WRITE_KEY = "qwBKAvY6MEUvv5XIs4rE07ohf5neT3sx"
+
+# Suppress Segment warnings
+logging.getLogger("segment").setLevel(logging.FATAL)
 
 
 class AnalyticsEvent(str, Enum):
     """Analytics event enum class."""
 
     PROVISION = "provision"
     DESTROY = "destroy"
     GET = "get"
 
 
 def execute_analytics_event(
-    func: Callable, *args, **kwargs
+    func: Callable[..., Any], *args: Any, **kwargs: Any
 ) -> Tuple[Optional[MatchaState], Any]:
     """Exists to Temporarily fix misleading error messages coming from track decorator.
 
     Args:
         func (Callable): The function decorated by track.
+        *args (Any): arguments passed to the function.
+        **kwargs (Any): additional key word arguments passed to the function.
 
     Returns:
         The result of the call to func, the error code.
     """
     error_code, result = None, None
     try:
         result = func(*args, **kwargs)
@@ -53,14 +59,17 @@
     """
 
     def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
         """Decorator function.
 
         Args:
             func (Callable[..., Any]): The function that is being decorated
+
+        Returns:
+            Callable[..., Any]: The function that is being decorated
         """
 
         @functools.wraps(func)
         def inner(*args: Any, **kwargs: Any) -> Any:
             """The internal function that does the logic of capturing analytics and executing the function that's being wrapped.
 
             Raises:
@@ -106,19 +115,21 @@
                             raise err
 
                 if event_name.value in [event_name.DESTROY]:
                     ts = perf_counter()
                     result, error_code = execute_analytics_event(func, *args, **kwargs)
                     te = perf_counter()
 
-                analytics.track(
+                client = analytics.Client(WRITE_KEY, max_retries=1, debug=False)
+
+                client.track(
                     global_params.user_id,
                     event_name.value,
                     {
-                        "time_taken": te - ts,
+                        "time_taken": float(te) - float(ts),  # type: ignore
                         "error_type": f"{error_code.__class__}.{error_code.__class__.__name__}",
                         "command_succeeded": error_code is None,
                         "matcha_state_uuid": matcha_state_uuid,
                     },
                 )
                 if error_code is not None:
                     raise error_code
```

### Comparing `matcha_ml-0.2.6/src/matcha_ml/services/azure_service.py` & `matcha_ml-0.2.7/src/matcha_ml/services/azure_service.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/services/global_parameters_service.py` & `matcha_ml-0.2.7/src/matcha_ml/services/global_parameters_service.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/services/terraform_service.py` & `matcha_ml-0.2.7/src/matcha_ml/services/terraform_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 """The Terraform service interface."""
 import dataclasses
 import glob
 import os
 from pathlib import Path
-from typing import Optional, Tuple
+from typing import Optional
 
 import python_terraform
 
 
 @dataclasses.dataclass
+class TerraformResult:
+    """A class to hold the result of the terraform commands."""
+
+    return_code: int
+    std_out: str
+    std_err: str
+
+
+@dataclasses.dataclass
 class TerraformConfig:
     """Configuration required for terraform."""
 
     # Path to terraform template are stored
     working_dir: str = os.path.join(
         os.getcwd(), ".matcha", "infrastructure", "resources"
     )
@@ -62,17 +71,15 @@
         try:
             self.terraform_client.cmd(cmd="-help")
         except Exception:
             return False
 
         return True
 
-    def verify_kubectl_config_file(
-        self, config_path: str = ".kube/config"
-    ) -> None:
+    def verify_kubectl_config_file(self, config_path: str = ".kube/config") -> None:
         """Checks if kubeconfig is present at location ~/.kube/config.
 
         Args:
             config_path (str): Relative path to location of kubeconfig
 
         If not, it creates a empty config file.
         """
@@ -118,52 +125,52 @@
         """Get the path to the `.terraform` folder generated on completion of `terraform init`.
 
         Returns:
             Path: a Path object that represents the path to the `.terraform` folder.
         """
         return Path(os.path.join(self.config.working_dir, ".terraform"))
 
-    def init(self) -> Tuple[int, str, str]:
+    def init(self) -> TerraformResult:
         """Run `terraform init` with the initialized Terraform client from the python_terraform module.
 
         Returns:
             Tuple[int, str, str]: return code of Terraform, standard output and standard error.
         """
         ret_code, out, err = self.terraform_client.init(
             capture_output=self.config.capture_output,
             raise_on_error=False,
         )
 
-        return ret_code, out, err
+        return TerraformResult(ret_code, out, err)
 
-    def apply(self) -> Tuple[int, str, str]:
+    def apply(self) -> TerraformResult:
         """Run `terraform apply` with the initialized Terraform client from the python_terraform module.
 
         Returns:
             Tuple[int, str, str]: return code of Terraform, standard output and standard error.
         """
         # once terraform init is success, call terraform apply
         ret_code, out, err = self.terraform_client.apply(
             input=False,
             capture_output=self.config.capture_output,
             raise_on_error=False,
             skip_plan=True,
             auto_approve=True,
         )
 
-        return ret_code, out, err
+        return TerraformResult(ret_code, out, err)
 
-    def destroy(self) -> Tuple[int, str, str]:
+    def destroy(self) -> TerraformResult:
         """Destroy the provisioned resources with the initialized Terraform client from the python_terraform module..
 
         Returns:
             Tuple[int, str, str]: return code of terraform, standard output and standard error.
         """
         # Reference: https://github.com/beelit94/python-terraform/issues/108
         ret_code, out, err = self.terraform_client.destroy(
             capture_output=self.config.capture_output,
             raise_on_error=False,
             force=python_terraform.IsNotFlagged,
             auto_approve=True,
         )
 
-        return ret_code, out, err
+        return TerraformResult(ret_code, out, err)
```

### Comparing `matcha_ml-0.2.6/src/matcha_ml/state/matcha_state.py` & `matcha_ml-0.2.7/src/matcha_ml/state/matcha_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 RESOURCE_NAMES = [
     "experiment_tracker",
     "pipeline",
     "orchestrator",
     "cloud",
     "container_registry",
     "model_deployer",
+    "data_version_control",
 ]
 
 
 @dataclass
 class MatchaResource:
     """A class to represent a resource in the state."""
 
@@ -136,15 +137,15 @@
 
         Args:
             matcha_state (Optional[MatchaState]): MatchaState object to initialize the service with. Defaults to None.
             terraform_output (Optional[dict]): Output from Terraform to be parsed into a MatchaState object on initialization. Defaults to None.
 
         Raises:
             MatchaError: if the state file does not exist.
-            MatchaError: if MatchaStateService is initialize with both 'matcha_state' and 'terraform_output' arguments.
+            MatchaError: if MatchaStateService is initialized with both 'matcha_state' and 'terraform_output' arguments.
         """
         if matcha_state is not None and terraform_output is not None:
             raise MatchaError(
                 "MatchaStateService constructor cannot be called with both 'matcha_state' and 'terraform_output' arguments."
             )
 
         if matcha_state is not None:
@@ -199,15 +200,15 @@
             for key in RESOURCE_NAMES:
                 if key in output_name:
                     resource_type = key
                     break
 
             if resource_type is None:
                 raise MatchaInputError(
-                    "A valid resource type for the output '{output_name}' does not exist."
+                    f"A valid resource type for the output '{output_name}' does not exist."
                 )
 
             flavor_and_resource_name = output_name[len(resource_type) + 1 :]
 
             flavor, resource_name = flavor_and_resource_name.split("_", maxsplit=1)
             resource_name = resource_name.replace("_", "-")
             resource_type = resource_type.replace("_", "-")
```

### Comparing `matcha_ml-0.2.6/src/matcha_ml/state/remote_state_manager.py` & `matcha_ml-0.2.7/src/matcha_ml/state/remote_state_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,25 +288,29 @@
         """
         self.azure_storage.upload_folder(
             container_name=self.configuration.remote_state_bucket.container_name,
             src_folder_path=local_folder_path,
         )
 
     @contextlib.contextmanager
-    def use_remote_state(self) -> Iterator[None]:
+    def use_remote_state(self, destroy: bool = False) -> Iterator[None]:
         """Context manager to use remote state.
 
         Downloads the state before executing the code.
         Upload the state when context is finished.
+
+        Args:
+            destroy (bool): Flag for whether the command being run is 'destroy' or not.
         """
         self.download(os.getcwd())
 
         yield None
 
-        self.upload(os.path.join(".matcha", "infrastructure"))
+        if not destroy:
+            self.upload(os.path.join(".matcha", "infrastructure"))
 
     def lock(self) -> None:
         """Lock remote state.
 
         Raises:
             MatchaError: if the state is already locked
         """
@@ -331,14 +335,19 @@
         else:
             self.azure_storage.delete_blob(
                 container_name=self.configuration.remote_state_bucket.container_name,
                 blob_name=LOCK_FILE_NAME,
             )
 
     @contextlib.contextmanager
-    def use_lock(self) -> Iterator[None]:
-        """Context manager to lock state."""
+    def use_lock(self, destroy: bool = False) -> Iterator[None]:
+        """Context manager to lock state.
+
+        Args:
+            destroy (bool): Flag for whether the command being run is 'destroy' or not.
+        """
         self.lock()
         try:
             yield
         finally:
-            self.unlock()
+            if not destroy:
+                self.unlock()
```

### Comparing `matcha_ml-0.2.6/src/matcha_ml/storage/azure_storage.py` & `matcha_ml-0.2.7/src/matcha_ml/storage/azure_storage.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/templates/azure_template.py` & `matcha_ml-0.2.7/src/matcha_ml/templates/azure_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     "storage",
     "seldon",
     "zenml_storage",
     "zen_server",
     "azure_container_registry",
     "zen_server/zenml_helm",
     "zen_server/zenml_helm/templates",
+    "data_version_control_storage",
 ]
 
 
 class AzureTemplate(BaseTemplate):
     """A template tailored for provisioning the resources on azure.
 
     Inherits:
@@ -49,10 +50,11 @@
             verbose (Optional[bool]): additional output is shown when True. Defaults to False.
         """
         super().build_template(config, template_src, destination, verbose)
 
         # Add matcha.state file one directory above the template
         config_dict = vars(config)
         _ = config_dict.pop("password", None)
+        config_dict["resource-group-name"] = f"{config_dict['prefix']}-resources"
         initial_state_file_dict = {"cloud": config_dict}
         matcha_state = MatchaState.from_dict(initial_state_file_dict)
         MatchaStateService(matcha_state=matcha_state)
```

### Comparing `matcha_ml-0.2.6/src/matcha_ml/templates/base_template.py` & `matcha_ml-0.2.7/src/matcha_ml/templates/base_template.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/src/matcha_ml/templates/remote_state_template.py` & `matcha_ml-0.2.7/src/matcha_ml/templates/remote_state_template.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.6/PKG-INFO` & `matcha_ml-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matcha-ml
-Version: 0.2.6
+Version: 0.2.7
 Summary: Matcha: An open source tool for provisioning MLOps environments to the cloud.
 Home-page: http://fuzzylabs.github.io/matcha
 License: Apache-2.0
 Keywords: production,mlops,devops,machine learning
 Author: FuzzyLabs
 Author-email: info@fuzzylabs.ai
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: matcha-ml Version: 0.2.6 Summary: Matcha: An open
+Metadata-Version: 2.1 Name: matcha-ml Version: 0.2.7 Summary: Matcha: An open
 source tool for provisioning MLOps environments to the cloud. Home-page: http:/
 /fuzzylabs.github.io/matcha License: Apache-2.0 Keywords:
 production,mlops,devops,machine learning Author: FuzzyLabs Author-email:
 info@fuzzylabs.ai Requires-Python: >=3.8,<4.0 Classifier: Development Status ::
 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

