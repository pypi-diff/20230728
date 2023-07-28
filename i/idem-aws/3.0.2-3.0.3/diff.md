# Comparing `tmp/idem-aws-3.0.2.tar.gz` & `tmp/idem-aws-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-aws-3.0.2.tar", last modified: Sat Jul 22 15:46:02 2023, max compression
+gzip compressed data, was "idem-aws-3.0.3.tar", last modified: Fri Jul 28 19:34:56 2023, max compression
```

## Comparing `idem-aws-3.0.2.tar` & `idem-aws-3.0.3.tar`

### file list

```diff
@@ -1,690 +1,690 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.204168 idem-aws-3.0.2/
--rw-r--r--   0 root         (0) root         (0)    11342 2023-07-22 15:45:47.000000 idem-aws-3.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       54 2023-07-22 15:45:47.000000 idem-aws-3.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    11104 2023-07-22 15:46:02.204168 idem-aws-3.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9835 2023-07-22 15:45:47.000000 idem-aws-3.0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.160168 idem-aws-3.0.2/idem_aws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.156168 idem-aws-3.0.2/idem_aws/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.160168 idem-aws-3.0.2/idem_aws/acct/aws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.160168 idem-aws-3.0.2/idem_aws/acct/aws/contracts/
--rw-r--r--   0 root         (0) root         (0)     1127 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/acct/aws/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     5506 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/acct/aws/gsuite.py
--rw-r--r--   0 root         (0) root         (0)     1618 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/acct/aws/iam.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/acct/aws/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/acct/metadata/
--rw-r--r--   0 root         (0) root         (0)      534 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/acct/metadata/aws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.156168 idem-aws-3.0.2/idem_aws/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/autogen/aws/
--rw-r--r--   0 root         (0) root         (0)     7080 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/autogen/aws/function.py
--rw-r--r--   0 root         (0) root         (0)     9290 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/autogen/aws/init.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/autogen/aws/known_params.py
--rw-r--r--   0 root         (0) root         (0)     3023 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/autogen/aws/param.py
--rw-r--r--   0 root         (0) root         (0)     9682 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/autogen/aws/plugin.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/autogen/aws/possible_functions.py
--rw-r--r--   0 root         (0) root         (0)     3870 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/autogen/aws/resource.py
--rw-r--r--   0 root         (0) root         (0)     4045 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/autogen/aws/service.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/esm/
--rw-r--r--   0 root         (0) root         (0)     8838 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/esm/aws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/esm/contracts/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/esm/contracts/aws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.156168 idem-aws-3.0.2/idem_aws/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/exec/aws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/exec/aws/acm/
--rw-r--r--   0 root         (0) root         (0)     2000 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/acm/certificate_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/exec/aws/apigateway/
--rw-r--r--   0 root         (0) root         (0)     5430 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/apigateway/base_path_mapping.py
--rw-r--r--   0 root         (0) root         (0)     2600 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/apigateway/deployment.py
--rw-r--r--   0 root         (0) root         (0)     3322 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/apigateway/domain_name.py
--rw-r--r--   0 root         (0) root         (0)     1925 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/apigateway/integration.py
--rw-r--r--   0 root         (0) root         (0)     2971 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/apigateway/integration_response.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/apigateway/method.py
--rw-r--r--   0 root         (0) root         (0)     2145 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/apigateway/method_response.py
--rw-r--r--   0 root         (0) root         (0)     1136 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/apigateway/resource.py
--rw-r--r--   0 root         (0) root         (0)     2435 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/apigateway/rest_api.py
--rw-r--r--   0 root         (0) root         (0)     2608 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/apigateway/stage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/exec/aws/apigatewayv2/
--rw-r--r--   0 root         (0) root         (0)     3276 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/apigatewayv2/api.py
--rw-r--r--   0 root         (0) root         (0)     2069 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/apigatewayv2/authorizer.py
--rw-r--r--   0 root         (0) root         (0)     1890 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/apigatewayv2/domain_name.py
--rw-r--r--   0 root         (0) root         (0)     2184 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/apigatewayv2/integration.py
--rw-r--r--   0 root         (0) root         (0)     3761 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/apigatewayv2/route.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/exec/aws/application_autoscaling/
--rw-r--r--   0 root         (0) root         (0)     3192 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/application_autoscaling/scalable_target.py
--rw-r--r--   0 root         (0) root         (0)     3395 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/application_autoscaling/scaling_policy.py
--rw-r--r--   0 root         (0) root         (0)     2846 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/arn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/exec/aws/autoscaling/
--rw-r--r--   0 root         (0) root         (0)     3034 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/autoscaling/scaling_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/exec/aws/backup/
--rw-r--r--   0 root         (0) root         (0)     4661 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/backup/backup_vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/exec/aws/budgets/
--rw-r--r--   0 root         (0) root         (0)     4105 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/budgets/budget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/exec/aws/cloudformation/
--rw-r--r--   0 root         (0) root         (0)     2285 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/cloudformation/stack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/exec/aws/cloudfront/
--rw-r--r--   0 root         (0) root         (0)     4007 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/cloudfront/cache_policy.py
--rw-r--r--   0 root         (0) root         (0)     2697 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/cloudfront/distribution.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/cloudfront/origin_request_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/exec/aws/cloudwatch/
--rw-r--r--   0 root         (0) root         (0)     3012 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/cloudwatch/log_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/exec/aws/cloudwatchlogs/
--rw-r--r--   0 root         (0) root         (0)     1528 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/cloudwatchlogs/resource_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/exec/aws/config/
--rw-r--r--   0 root         (0) root         (0)     4538 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/config/configuration_aggregator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/exec/aws/costexplorer/
--rw-r--r--   0 root         (0) root         (0)     1660 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/costexplorer/cost_allocation_tag.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/exec/aws/docdb/
--rw-r--r--   0 root         (0) root         (0)     6138 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/docdb/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)     7293 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/docdb/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     4887 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/docdb/db_subnet_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.164168 idem-aws-3.0.2/idem_aws/exec/aws/dynamodb/
--rw-r--r--   0 root         (0) root         (0)     2434 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/dynamodb/table.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/dynamodb/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.168168 idem-aws-3.0.2/idem_aws/exec/aws/ec2/
--rw-r--r--   0 root         (0) root         (0)     8697 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/ami.py
--rw-r--r--   0 root         (0) root         (0)     4290 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/availability_zones.py
--rw-r--r--   0 root         (0) root         (0)     4206 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/elastic_ip.py
--rw-r--r--   0 root         (0) root         (0)     3405 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/flow_log.py
--rw-r--r--   0 root         (0) root         (0)    22062 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/instance.py
--rw-r--r--   0 root         (0) root         (0)     3299 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/instance_type.py
--rw-r--r--   0 root         (0) root         (0)     1511 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/internet_gateway.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/key_pair.py
--rw-r--r--   0 root         (0) root         (0)     7293 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/launch_template.py
--rw-r--r--   0 root         (0) root         (0)     8692 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/network_interface.py
--rw-r--r--   0 root         (0) root         (0)     4680 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/placement_group.py
--rw-r--r--   0 root         (0) root         (0)     5836 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/route.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/route_table.py
--rw-r--r--   0 root         (0) root         (0)     3265 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/route_table_association.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/security_group.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/security_group_rule.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4295 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/spot_instance_request.py
--rw-r--r--   0 root         (0) root         (0)     8595 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/subnet.py
--rw-r--r--   0 root         (0) root         (0)     4471 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/volume.py
--rw-r--r--   0 root         (0) root         (0)     4459 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/vpc.py
--rw-r--r--   0 root         (0) root         (0)     4081 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/vpc_endpoint.py
--rw-r--r--   0 root         (0) root         (0)     1952 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/vpc_peering_connection.py
--rw-r--r--   0 root         (0) root         (0)     2007 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/vpc_peering_connection_accepter.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ec2/vpc_peering_connection_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.168168 idem-aws-3.0.2/idem_aws/exec/aws/ecr/
--rw-r--r--   0 root         (0) root         (0)     5183 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ecr/image.py
--rw-r--r--   0 root         (0) root         (0)     3195 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ecr/lifecycle_policy.py
--rw-r--r--   0 root         (0) root         (0)     5504 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ecr/repository.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ecr/repository_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.168168 idem-aws-3.0.2/idem_aws/exec/aws/eks/
--rw-r--r--   0 root         (0) root         (0)     1665 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/eks/cluster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.168168 idem-aws-3.0.2/idem_aws/exec/aws/elasticache/
--rw-r--r--   0 root         (0) root         (0)     2934 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/elasticache/replication_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.168168 idem-aws-3.0.2/idem_aws/exec/aws/elb/
--rw-r--r--   0 root         (0) root         (0)     3023 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/elb/elb_hosted_zone_id.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/elb/load_balancer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.168168 idem-aws-3.0.2/idem_aws/exec/aws/elbv2/
--rw-r--r--   0 root         (0) root         (0)     3296 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/elbv2/listener.py
--rw-r--r--   0 root         (0) root         (0)     3346 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/elbv2/load_balancer.py
--rw-r--r--   0 root         (0) root         (0)     4861 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/elbv2/target_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.168168 idem-aws-3.0.2/idem_aws/exec/aws/es/
--rw-r--r--   0 root         (0) root         (0)     2387 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/es/elasticsearch_domain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.168168 idem-aws-3.0.2/idem_aws/exec/aws/events/
--rw-r--r--   0 root         (0) root         (0)     5682 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/events/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.168168 idem-aws-3.0.2/idem_aws/exec/aws/guardduty/
--rw-r--r--   0 root         (0) root         (0)     2423 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/guardduty/detector.py
--rw-r--r--   0 root         (0) root         (0)     5618 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/guardduty/member.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/guardduty/organization_admin_account.py
--rw-r--r--   0 root         (0) root         (0)     8636 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/guardduty/organization_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.168168 idem-aws-3.0.2/idem_aws/exec/aws/iam/
--rw-r--r--   0 root         (0) root         (0)     9324 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/iam/access_key.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/iam/group.py
--rw-r--r--   0 root         (0) root         (0)     1199 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/iam/group_membership.py
--rw-r--r--   0 root         (0) root         (0)     2099 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/iam/group_policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)     4749 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/iam/instance_profile.py
--rw-r--r--   0 root         (0) root         (0)     7709 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/iam/open_id_connect_provider.py
--rw-r--r--   0 root         (0) root         (0)     1842 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/iam/password_policy.py
--rw-r--r--   0 root         (0) root         (0)     6957 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/iam/policy.py
--rw-r--r--   0 root         (0) root         (0)     9723 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/iam/role.py
--rw-r--r--   0 root         (0) root         (0)     1218 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/iam/user.py
--rw-r--r--   0 root         (0) root         (0)     2945 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/iam/user_policy_attachment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.168168 idem-aws-3.0.2/idem_aws/exec/aws/kinesis/
--rw-r--r--   0 root         (0) root         (0)     2919 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/kinesis/stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.168168 idem-aws-3.0.2/idem_aws/exec/aws/kms/
--rw-r--r--   0 root         (0) root         (0)     3031 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/kms/key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.168168 idem-aws-3.0.2/idem_aws/exec/aws/lambda_aws/
--rw-r--r--   0 root         (0) root         (0)     4863 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/lambda_aws/function_event_invoke_config.py
--rw-r--r--   0 root         (0) root         (0)     5632 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/lambda_aws/function_provisioned_concurrency_config.py
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/lambda_aws/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/exec/aws/neptune/
--rw-r--r--   0 root         (0) root         (0)     7388 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/neptune/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     6621 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/neptune/db_instance.py
--rw-r--r--   0 root         (0) root         (0)     6854 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/neptune/db_parameter_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/exec/aws/organizations/
--rw-r--r--   0 root         (0) root         (0)     4486 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/organizations/account.py
--rw-r--r--   0 root         (0) root         (0)     2391 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/organizations/policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/exec/aws/rds/
--rw-r--r--   0 root         (0) root         (0)     5996 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/rds/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)     5001 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/rds/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     5971 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/rds/db_instance.py
--rw-r--r--   0 root         (0) root         (0)     6287 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/rds/db_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/rds/db_subnet_group.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/rds/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/exec/aws/route53/
--rw-r--r--   0 root         (0) root         (0)     5251 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/route53/hosted_zone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/exec/aws/s3/
--rw-r--r--   0 root         (0) root         (0)     2659 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/s3/bucket.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/s3/bucket_acl.py
--rw-r--r--   0 root         (0) root         (0)     1918 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/s3/bucket_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     1897 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/s3/bucket_logging.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/s3/bucket_replication.py
--rw-r--r--   0 root         (0) root         (0)     1956 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/s3/bucket_website.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/exec/aws/ses/
--rw-r--r--   0 root         (0) root         (0)     3203 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ses/domain_identity.py
--rw-r--r--   0 root         (0) root         (0)     4166 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/ses/identity_notification_topic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/exec/aws/sesv2/
--rw-r--r--   0 root         (0) root         (0)     4342 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/sesv2/event_destination.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/exec/aws/sns/
--rw-r--r--   0 root         (0) root         (0)     3682 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/sns/subscription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/exec/aws/sqs/
--rw-r--r--   0 root         (0) root         (0)     4684 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/sqs/queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/exec/aws/sts/
--rw-r--r--   0 root         (0) root         (0)     5261 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/sts/assume_role.py
--rw-r--r--   0 root         (0) root         (0)     1259 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/sts/caller_identity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/exec/aws/wafv2/
--rw-r--r--   0 root         (0) root         (0)     4859 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/wafv2/ip_set.py
--rw-r--r--   0 root         (0) root         (0)     7041 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/aws/wafv2/regex_pattern_set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/exec/boto3/
--rw-r--r--   0 root         (0) root         (0)      747 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/exec/boto3/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.156168 idem-aws-3.0.2/idem_aws/reconcile/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/reconcile/pending/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/reconcile/pending/aws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.156168 idem-aws-3.0.2/idem_aws/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/states/aws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/states/aws/acm/
--rw-r--r--   0 root         (0) root         (0)    28335 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/acm/certificate_manager.py
--rw-r--r--   0 root         (0) root         (0)    11132 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/acm/certificate_validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/states/aws/apigateway/
--rw-r--r--   0 root         (0) root         (0)    10257 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/apigateway/base_path_mapping.py
--rw-r--r--   0 root         (0) root         (0)    12091 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/apigateway/deployment.py
--rw-r--r--   0 root         (0) root         (0)    19520 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/apigateway/domain_name.py
--rw-r--r--   0 root         (0) root         (0)    15779 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/apigateway/integration.py
--rw-r--r--   0 root         (0) root         (0)    13752 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/apigateway/integration_response.py
--rw-r--r--   0 root         (0) root         (0)    12950 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/apigateway/method.py
--rw-r--r--   0 root         (0) root         (0)    12155 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/apigateway/method_response.py
--rw-r--r--   0 root         (0) root         (0)     9866 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/apigateway/resource.py
--rw-r--r--   0 root         (0) root         (0)    13732 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/apigateway/rest_api.py
--rw-r--r--   0 root         (0) root         (0)    13857 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/apigateway/stage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/states/aws/apigatewayv2/
--rw-r--r--   0 root         (0) root         (0)    15354 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/apigatewayv2/api.py
--rw-r--r--   0 root         (0) root         (0)    16244 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/apigatewayv2/authorizer.py
--rw-r--r--   0 root         (0) root         (0)    15119 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/apigatewayv2/domain_name.py
--rw-r--r--   0 root         (0) root         (0)    22693 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/apigatewayv2/integration.py
--rw-r--r--   0 root         (0) root         (0)    14022 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/apigatewayv2/route.py
--rw-r--r--   0 root         (0) root         (0)    16913 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/apigatewayv2/stage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.172168 idem-aws-3.0.2/idem_aws/states/aws/application_autoscaling/
--rw-r--r--   0 root         (0) root         (0)    31855 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/application_autoscaling/scalable_target.py
--rw-r--r--   0 root         (0) root         (0)    45934 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/application_autoscaling/scaling_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.176168 idem-aws-3.0.2/idem_aws/states/aws/autoscaling/
--rw-r--r--   0 root         (0) root         (0)    78777 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/autoscaling/auto_scaling_group.py
--rw-r--r--   0 root         (0) root         (0)    32523 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/autoscaling/launch_configuration.py
--rw-r--r--   0 root         (0) root         (0)    54968 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/autoscaling/scaling_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.176168 idem-aws-3.0.2/idem_aws/states/aws/backup/
--rw-r--r--   0 root         (0) root         (0)     8985 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/backup/backup_vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.176168 idem-aws-3.0.2/idem_aws/states/aws/budgets/
--rw-r--r--   0 root         (0) root         (0)    25523 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/budgets/budget.py
--rw-r--r--   0 root         (0) root         (0)    16456 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/budgets/budget_action.py
--rw-r--r--   0 root         (0) root         (0)     1768 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/caller_identity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.176168 idem-aws-3.0.2/idem_aws/states/aws/cloudformation/
--rw-r--r--   0 root         (0) root         (0)    32414 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/cloudformation/stack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.176168 idem-aws-3.0.2/idem_aws/states/aws/cloudfront/
--rw-r--r--   0 root         (0) root         (0)    24459 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/cloudfront/cache_policy.py
--rw-r--r--   0 root         (0) root         (0)   116104 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/cloudfront/distribution.py
--rw-r--r--   0 root         (0) root         (0)    15501 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/cloudfront/origin_request_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.176168 idem-aws-3.0.2/idem_aws/states/aws/cloudtrail/
--rw-r--r--   0 root         (0) root         (0)    37423 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/cloudtrail/trail.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.176168 idem-aws-3.0.2/idem_aws/states/aws/cloudwatch/
--rw-r--r--   0 root         (0) root         (0)    11420 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/cloudwatch/log_group.py
--rw-r--r--   0 root         (0) root         (0)    36075 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/cloudwatch/metric_alarm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.176168 idem-aws-3.0.2/idem_aws/states/aws/cloudwatchlogs/
--rw-r--r--   0 root         (0) root         (0)     8723 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/cloudwatchlogs/resource_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.176168 idem-aws-3.0.2/idem_aws/states/aws/config/
--rwxr-xr-x   0 root         (0) root         (0)    11422 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/config/config_recorder.py
--rwxr-xr-x   0 root         (0) root         (0)     9512 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/config/config_recorder_status.py
--rw-r--r--   0 root         (0) root         (0)    10463 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/config/configuration_aggregator.py
--rwxr-xr-x   0 root         (0) root         (0)    12062 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/config/delivery_channel.py
--rw-r--r--   0 root         (0) root         (0)    21665 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/config/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.176168 idem-aws-3.0.2/idem_aws/states/aws/costexplorer/
--rw-r--r--   0 root         (0) root         (0)    18653 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/costexplorer/anomaly_monitor.py
--rw-r--r--   0 root         (0) root         (0)    10751 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/costexplorer/anomaly_subscription.py
--rw-r--r--   0 root         (0) root         (0)    28397 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/costexplorer/cost_category.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.176168 idem-aws-3.0.2/idem_aws/states/aws/docdb/
--rw-r--r--   0 root         (0) root         (0)    28355 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/docdb/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)    12967 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/docdb/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    11755 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/docdb/db_subnet_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.176168 idem-aws-3.0.2/idem_aws/states/aws/dynamodb/
--rw-r--r--   0 root         (0) root         (0)    36228 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/dynamodb/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.180168 idem-aws-3.0.2/idem_aws/states/aws/ec2/
--rw-r--r--   0 root         (0) root         (0)    22039 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/ami.py
--rw-r--r--   0 root         (0) root         (0)    15794 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/dhcp_option.py
--rw-r--r--   0 root         (0) root         (0)    10017 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/dhcp_option_association.py
--rw-r--r--   0 root         (0) root         (0)    13002 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/elastic_ip.py
--rw-r--r--   0 root         (0) root         (0)    12633 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/flow_log.py
--rw-r--r--   0 root         (0) root         (0)    41622 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/instance.py
--rw-r--r--   0 root         (0) root         (0)    12429 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/internet_gateway.py
--rw-r--r--   0 root         (0) root         (0)     9711 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/key_pair.py
--rw-r--r--   0 root         (0) root         (0)    73447 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/launch_template.py
--rw-r--r--   0 root         (0) root         (0)    17418 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/nat_gateway.py
--rw-r--r--   0 root         (0) root         (0)    12093 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/network_interface.py
--rw-r--r--   0 root         (0) root         (0)    10946 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/placement_group.py
--rw-r--r--   0 root         (0) root         (0)    14835 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/route.py
--rw-r--r--   0 root         (0) root         (0)    15623 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/route_table.py
--rw-r--r--   0 root         (0) root         (0)     8933 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/route_table_association.py
--rw-r--r--   0 root         (0) root         (0)    12947 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/security_group.py
--rw-r--r--   0 root         (0) root         (0)    17979 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/security_group_rule.py
--rw-r--r--   0 root         (0) root         (0)    10513 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/snapshot.py
--rw-r--r--   0 root         (0) root         (0)    36976 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/spot_instance_request.py
--rw-r--r--   0 root         (0) root         (0)    20082 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/subnet.py
--rw-r--r--   0 root         (0) root         (0)    17765 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/transit_gateway.py
--rw-r--r--   0 root         (0) root         (0)    16953 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/transit_gateway_vpc_attachment.py
--rw-r--r--   0 root         (0) root         (0)    15331 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/volume.py
--rw-r--r--   0 root         (0) root         (0)    20607 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/vpc.py
--rw-r--r--   0 root         (0) root         (0)    19294 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/vpc_endpoint.py
--rw-r--r--   0 root         (0) root         (0)    14516 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/vpc_peering_connection.py
--rw-r--r--   0 root         (0) root         (0)     9225 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/vpc_peering_connection_accepter.py
--rw-r--r--   0 root         (0) root         (0)     9871 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ec2/vpc_peering_connection_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.180168 idem-aws-3.0.2/idem_aws/states/aws/ecr/
--rw-r--r--   0 root         (0) root         (0)    11587 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ecr/lifecycle_policy.py
--rw-r--r--   0 root         (0) root         (0)    13319 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ecr/repository.py
--rw-r--r--   0 root         (0) root         (0)    11708 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ecr/repository_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.180168 idem-aws-3.0.2/idem_aws/states/aws/efs/
--rw-r--r--   0 root         (0) root         (0)    25301 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/efs/file_system.py
--rw-r--r--   0 root         (0) root         (0)    22090 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/efs/mount_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.180168 idem-aws-3.0.2/idem_aws/states/aws/eks/
--rw-r--r--   0 root         (0) root         (0)    18084 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/eks/addon.py
--rw-r--r--   0 root         (0) root         (0)    29585 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/eks/cluster.py
--rw-r--r--   0 root         (0) root         (0)    17678 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/eks/fargate_profile.py
--rw-r--r--   0 root         (0) root         (0)    29787 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/eks/nodegroup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.180168 idem-aws-3.0.2/idem_aws/states/aws/elasticache/
--rw-r--r--   0 root         (0) root         (0)    16170 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/elasticache/cache_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    13492 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/elasticache/cache_subnet_group.py
--rw-r--r--   0 root         (0) root         (0)    51005 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/elasticache/replication_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.180168 idem-aws-3.0.2/idem_aws/states/aws/elb/
--rw-r--r--   0 root         (0) root         (0)    19828 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/elb/load_balancer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.180168 idem-aws-3.0.2/idem_aws/states/aws/elbv2/
--rw-r--r--   0 root         (0) root         (0)    32920 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/elbv2/listener.py
--rw-r--r--   0 root         (0) root         (0)    24159 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/elbv2/load_balancer.py
--rw-r--r--   0 root         (0) root         (0)    30475 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/elbv2/target_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.180168 idem-aws-3.0.2/idem_aws/states/aws/es/
--rw-r--r--   0 root         (0) root         (0)    36336 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/es/elasticsearch_domain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.180168 idem-aws-3.0.2/idem_aws/states/aws/events/
--rw-r--r--   0 root         (0) root         (0)    45318 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/events/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.180168 idem-aws-3.0.2/idem_aws/states/aws/guardduty/
--rw-r--r--   0 root         (0) root         (0)    15458 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/guardduty/detector.py
--rw-r--r--   0 root         (0) root         (0)    10351 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/guardduty/member.py
--rw-r--r--   0 root         (0) root         (0)     8768 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/guardduty/organization_admin_account.py
--rw-r--r--   0 root         (0) root         (0)     8981 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/guardduty/organization_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.184168 idem-aws-3.0.2/idem_aws/states/aws/iam/
--rw-r--r--   0 root         (0) root         (0)     9988 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/iam/access_key.py
--rw-r--r--   0 root         (0) root         (0)     8246 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/iam/group.py
--rw-r--r--   0 root         (0) root         (0)     8179 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/iam/group_membership.py
--rw-r--r--   0 root         (0) root         (0)     8776 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/iam/group_policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)    14496 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/iam/instance_profile.py
--rw-r--r--   0 root         (0) root         (0)    18389 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/iam/open_id_connect_provider.py
--rw-r--r--   0 root         (0) root         (0)    12320 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/iam/password_policy.py
--rw-r--r--   0 root         (0) root         (0)    14614 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/iam/policy.py
--rw-r--r--   0 root         (0) root         (0)    22433 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/iam/role.py
--rw-r--r--   0 root         (0) root         (0)    14539 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/iam/role_policy.py
--rw-r--r--   0 root         (0) root         (0)    10537 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/iam/role_policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)    15633 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/iam/service_linked_role.py
--rw-r--r--   0 root         (0) root         (0)    15522 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/iam/user.py
--rw-r--r--   0 root         (0) root         (0)    14079 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/iam/user_policy.py
--rw-r--r--   0 root         (0) root         (0)    11044 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/iam/user_policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)    13341 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/iam/user_ssh_key.py
--rw-r--r--   0 root         (0) root         (0)      169 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.184168 idem-aws-3.0.2/idem_aws/states/aws/kinesis/
--rw-r--r--   0 root         (0) root         (0)    24114 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/kinesis/stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.184168 idem-aws-3.0.2/idem_aws/states/aws/kms/
--rw-r--r--   0 root         (0) root         (0)    10460 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/kms/alias.py
--rw-r--r--   0 root         (0) root         (0)    22630 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/kms/key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.184168 idem-aws-3.0.2/idem_aws/states/aws/lambda_aws/
--rw-r--r--   0 root         (0) root         (0)    27963 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/lambda_aws/function.py
--rw-r--r--   0 root         (0) root         (0)    11651 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/lambda_aws/function_event_invoke_config.py
--rw-r--r--   0 root         (0) root         (0)    14029 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/lambda_aws/function_permission.py
--rw-r--r--   0 root         (0) root         (0)    10018 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/lambda_aws/function_provisioned_concurrency_config.py
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/lambda_aws/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.184168 idem-aws-3.0.2/idem_aws/states/aws/logs/
--rw-r--r--   0 root         (0) root         (0)    12064 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/logs/subscription_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.184168 idem-aws-3.0.2/idem_aws/states/aws/neptune/
--rw-r--r--   0 root         (0) root         (0)    32988 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/neptune/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)    13936 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/neptune/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    37556 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/neptune/db_instance.py
--rw-r--r--   0 root         (0) root         (0)    12467 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/neptune/db_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    14288 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/neptune/db_subnet_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.184168 idem-aws-3.0.2/idem_aws/states/aws/organizations/
--rw-r--r--   0 root         (0) root         (0)    17382 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/organizations/account.py
--rw-r--r--   0 root         (0) root         (0)     8251 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/organizations/organization.py
--rw-r--r--   0 root         (0) root         (0)    14282 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/organizations/organization_unit.py
--rw-r--r--   0 root         (0) root         (0)    13176 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/organizations/policy.py
--rw-r--r--   0 root         (0) root         (0)    11396 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/organizations/policy_attachment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.184168 idem-aws-3.0.2/idem_aws/states/aws/rds/
--rw-r--r--   0 root         (0) root         (0)    62077 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/rds/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)    14695 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/rds/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    39434 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/rds/db_instance.py
--rw-r--r--   0 root         (0) root         (0)    13874 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/rds/db_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    14036 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/rds/db_subnet_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.184168 idem-aws-3.0.2/idem_aws/states/aws/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/recursive_contracts/allow_sync_sls_name_and_name_tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.184168 idem-aws-3.0.2/idem_aws/states/aws/route53/
--rw-r--r--   0 root         (0) root         (0)    19436 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/route53/hosted_zone.py
--rw-r--r--   0 root         (0) root         (0)    14157 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/route53/hosted_zone_association.py
--rw-r--r--   0 root         (0) root         (0)    12020 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/route53/resource_record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.184168 idem-aws-3.0.2/idem_aws/states/aws/s3/
--rw-r--r--   0 root         (0) root         (0)    19835 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/s3/bucket.py
--rw-r--r--   0 root         (0) root         (0)    11122 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_acl.py
--rw-r--r--   0 root         (0) root         (0)    15157 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_encryption.py
--rw-r--r--   0 root         (0) root         (0)    26660 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)    14837 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_logging.py
--rw-r--r--   0 root         (0) root         (0)    17613 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_notification.py
--rw-r--r--   0 root         (0) root         (0)    11942 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_policy.py
--rw-r--r--   0 root         (0) root         (0)    27930 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_replication.py
--rw-r--r--   0 root         (0) root         (0)    10328 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_versioning.py
--rw-r--r--   0 root         (0) root         (0)    22433 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_website.py
--rw-r--r--   0 root         (0) root         (0)    12854 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/s3/public_access_block.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.188168 idem-aws-3.0.2/idem_aws/states/aws/ses/
--rw-r--r--   0 root         (0) root         (0)     6157 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ses/domain_identity.py
--rw-r--r--   0 root         (0) root         (0)    10384 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/ses/identity_notification_topic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.188168 idem-aws-3.0.2/idem_aws/states/aws/sesv2/
--rw-r--r--   0 root         (0) root         (0)    14618 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/sesv2/event_destination.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.188168 idem-aws-3.0.2/idem_aws/states/aws/sns/
--rw-r--r--   0 root         (0) root         (0)    11654 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/sns/subscription.py
--rw-r--r--   0 root         (0) root         (0)    13240 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/sns/topic.py
--rw-r--r--   0 root         (0) root         (0)     8687 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/sns/topic_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.188168 idem-aws-3.0.2/idem_aws/states/aws/sqs/
--rw-r--r--   0 root         (0) root         (0)    24690 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/sqs/queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.188168 idem-aws-3.0.2/idem_aws/states/aws/wafv2/
--rw-r--r--   0 root         (0) root         (0)     9933 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/wafv2/associate_web_acl.py
--rw-r--r--   0 root         (0) root         (0)    14712 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/wafv2/ip_set.py
--rw-r--r--   0 root         (0) root         (0)    12255 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/wafv2/regex_pattern_set.py
--rw-r--r--   0 root         (0) root         (0)   268538 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/states/aws/wafv2/web_acl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.160168 idem-aws-3.0.2/idem_aws/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.188168 idem-aws-3.0.2/idem_aws/tool/aws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.188168 idem-aws-3.0.2/idem_aws/tool/aws/acct/
--rw-r--r--   0 root         (0) root         (0)     1393 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/acct/assume_role.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.188168 idem-aws-3.0.2/idem_aws/tool/aws/acct/contracts/
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/acct/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      293 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/acct/esm.py
--rw-r--r--   0 root         (0) root         (0)      714 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/acct/init.py
--rw-r--r--   0 root         (0) root         (0)     1577 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/acct/key_name.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.188168 idem-aws-3.0.2/idem_aws/tool/aws/acm/
--rw-r--r--   0 root         (0) root         (0)     2485 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/acm/certificate_validation_utils.py
--rw-r--r--   0 root         (0) root         (0)     5339 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/acm/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2625 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/acm/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.188168 idem-aws-3.0.2/idem_aws/tool/aws/apigateway/
--rw-r--r--   0 root         (0) root         (0)     3883 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigateway/base_path_mapping.py
--rw-r--r--   0 root         (0) root         (0)     3341 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigateway/deployment.py
--rw-r--r--   0 root         (0) root         (0)     8767 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigateway/domain_name.py
--rw-r--r--   0 root         (0) root         (0)     4534 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigateway/integration.py
--rw-r--r--   0 root         (0) root         (0)     5000 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigateway/integration_response.py
--rw-r--r--   0 root         (0) root         (0)     4226 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigateway/method.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigateway/method_response.py
--rw-r--r--   0 root         (0) root         (0)     4087 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigateway/resource.py
--rw-r--r--   0 root         (0) root         (0)     7175 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigateway/rest_api.py
--rw-r--r--   0 root         (0) root         (0)     4417 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigateway/stage.py
--rw-r--r--   0 root         (0) root         (0)     2203 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigateway/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.188168 idem-aws-3.0.2/idem_aws/tool/aws/apigatewayv2/
--rw-r--r--   0 root         (0) root         (0)     5671 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigatewayv2/api.py
--rw-r--r--   0 root         (0) root         (0)     5125 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigatewayv2/authorizer.py
--rw-r--r--   0 root         (0) root         (0)     4842 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigatewayv2/domain_name.py
--rw-r--r--   0 root         (0) root         (0)     5187 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigatewayv2/integration.py
--rw-r--r--   0 root         (0) root         (0)     4793 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigatewayv2/route.py
--rw-r--r--   0 root         (0) root         (0)     4061 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigatewayv2/stage.py
--rw-r--r--   0 root         (0) root         (0)     2655 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/apigatewayv2/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.192168 idem-aws-3.0.2/idem_aws/tool/aws/application_autoscaling/
--rw-r--r--   0 root         (0) root         (0)     2724 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/application_autoscaling/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/application_autoscaling/scalable_target.py
--rw-r--r--   0 root         (0) root         (0)     1907 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/application_autoscaling/scaling_policy.py
--rw-r--r--   0 root         (0) root         (0)     4099 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/arn_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.192168 idem-aws-3.0.2/idem_aws/tool/aws/autoscaling/
--rw-r--r--   0 root         (0) root         (0)     5561 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/autoscaling/auto_scaling_group_utils.py
--rw-r--r--   0 root         (0) root         (0)     4257 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/autoscaling/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3367 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/autoscaling/scaling_policy.py
--rw-r--r--   0 root         (0) root         (0)     2946 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/autoscaling/tag.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/b64.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.192168 idem-aws-3.0.2/idem_aws/tool/aws/backup/
--rw-r--r--   0 root         (0) root         (0)     1042 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/backup/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2452 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/backup/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.192168 idem-aws-3.0.2/idem_aws/tool/aws/budgets/
--rw-r--r--   0 root         (0) root         (0)     5248 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/budgets/budget.py
--rw-r--r--   0 root         (0) root         (0)     3415 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/budgets/budget_action.py
--rw-r--r--   0 root         (0) root         (0)     3563 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/budgets/conversion_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.192168 idem-aws-3.0.2/idem_aws/tool/aws/cloudformation/
--rw-r--r--   0 root         (0) root         (0)    18904 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/cloudformation/stack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.192168 idem-aws-3.0.2/idem_aws/tool/aws/cloudfront/
--rw-r--r--   0 root         (0) root         (0)     6468 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/cloudfront/cloudfront_utils.py
--rw-r--r--   0 root         (0) root         (0)     4860 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/cloudfront/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     7618 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/cloudfront/distribution.py
--rw-r--r--   0 root         (0) root         (0)     2573 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/cloudfront/distribution_utils.py
--rw-r--r--   0 root         (0) root         (0)     2416 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/cloudfront/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.192168 idem-aws-3.0.2/idem_aws/tool/aws/cloudtrail/
--rw-r--r--   0 root         (0) root         (0)     3966 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/cloudtrail/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    13076 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/cloudtrail/trail.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.192168 idem-aws-3.0.2/idem_aws/tool/aws/cloudwatch/
--rw-r--r--   0 root         (0) root         (0)     3540 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/cloudwatch/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)      807 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/cloudwatch/log_group.py
--rw-r--r--   0 root         (0) root         (0)     4464 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/cloudwatch/metric_alarm.py
--rw-r--r--   0 root         (0) root         (0)     2033 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/cloudwatch/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.192168 idem-aws-3.0.2/idem_aws/tool/aws/cloudwatchlogs/
--rw-r--r--   0 root         (0) root         (0)      566 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/cloudwatchlogs/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/comment_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.192168 idem-aws-3.0.2/idem_aws/tool/aws/config/
--rw-r--r--   0 root         (0) root         (0)     1511 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/config/config_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     4483 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/config/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/config/delivery_channel.py
--rw-r--r--   0 root         (0) root         (0)     2578 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/config/rule.py
--rw-r--r--   0 root         (0) root         (0)     2434 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/config/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.192168 idem-aws-3.0.2/idem_aws/tool/aws/costexplorer/
--rw-r--r--   0 root         (0) root         (0)     1024 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/costexplorer/anomaly_monitor.py
--rw-r--r--   0 root         (0) root         (0)     3078 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/costexplorer/anomaly_subscription.py
--rw-r--r--   0 root         (0) root         (0)     2953 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/costexplorer/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     4859 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/costexplorer/cost_category.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.192168 idem-aws-3.0.2/idem_aws/tool/aws/docdb/
--rw-r--r--   0 root         (0) root         (0)    12556 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/docdb/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)     6638 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/docdb/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/docdb/db_subnet_group.py
--rw-r--r--   0 root         (0) root         (0)     3183 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/docdb/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.192168 idem-aws-3.0.2/idem_aws/tool/aws/dynamodb/
--rw-r--r--   0 root         (0) root         (0)    15527 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/dynamodb/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.196168 idem-aws-3.0.2/idem_aws/tool/aws/ec2/
--rw-r--r--   0 root         (0) root         (0)     3051 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/ami.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/availability_zones.py
--rw-r--r--   0 root         (0) root         (0)    37825 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/dhcp_option_association_utils.py
--rw-r--r--   0 root         (0) root         (0)     1774 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/elastic_ip.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/flow_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.196168 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/
--rw-r--r--   0 root         (0) root         (0)     1280 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/data.py
--rw-r--r--   0 root         (0) root         (0)     3450 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/key_pair.py
--rw-r--r--   0 root         (0) root         (0)    19912 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.196168 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/
--rw-r--r--   0 root         (0) root         (0)     4440 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/block_device_mappings.py
--rw-r--r--   0 root         (0) root         (0)     1813 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/bootstrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.196168 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/contracts/
--rw-r--r--   0 root         (0) root         (0)      677 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     1191 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/disable_api_termination.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/ebs_optimized.py
--rw-r--r--   0 root         (0) root         (0)     2287 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/iam_instance_profile_arn.py
--rw-r--r--   0 root         (0) root         (0)     8226 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/init.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/instance_initiated_shutdown_behavior.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/instance_type.py
--rw-r--r--   0 root         (0) root         (0)     1300 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/kernel_id.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/monitoring_enabled.py
--rw-r--r--   0 root         (0) root         (0)     4309 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/network_interfaces.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/placement.py
--rw-r--r--   0 root         (0) root         (0)     1119 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/private_ip_address.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/ram_disk_id.py
--rw-r--r--   0 root         (0) root         (0)      214 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/running.py
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/security_group_ids.py
--rw-r--r--   0 root         (0) root         (0)     1173 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/source_dest_check.py
--rw-r--r--   0 root         (0) root         (0)     1173 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/sriov_net_support.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/tags.py
--rw-r--r--   0 root         (0) root         (0)     1281 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/user_data.py
--rw-r--r--   0 root         (0) root         (0)     4843 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/internet_gateway.py
--rw-r--r--   0 root         (0) root         (0)     1585 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/key_pair.py
--rw-r--r--   0 root         (0) root         (0)     3658 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/launch_template.py
--rw-r--r--   0 root         (0) root         (0)     3948 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/network_interface.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/placement_group.py
--rw-r--r--   0 root         (0) root         (0)    12208 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/route_table.py
--rw-r--r--   0 root         (0) root         (0)     3924 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/security_group_rule.py
--rw-r--r--   0 root         (0) root         (0)     1801 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     2779 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/spot_instance_request.py
--rw-r--r--   0 root         (0) root         (0)    14415 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/subnet.py
--rw-r--r--   0 root         (0) root         (0)     2752 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/tag.py
--rw-r--r--   0 root         (0) root         (0)     3821 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/transit_gateway.py
--rw-r--r--   0 root         (0) root         (0)     3043 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/transit_gateway_vpc_attachment.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/volume.py
--rw-r--r--   0 root         (0) root         (0)     7822 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/vpc.py
--rw-r--r--   0 root         (0) root         (0)     8498 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/vpc_endpoint.py
--rw-r--r--   0 root         (0) root         (0)    10645 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ec2/vpc_peering_connection_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.196168 idem-aws-3.0.2/idem_aws/tool/aws/ecr/
--rw-r--r--   0 root         (0) root         (0)     4995 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ecr/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3190 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ecr/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.196168 idem-aws-3.0.2/idem_aws/tool/aws/efs/
--rw-r--r--   0 root         (0) root         (0)     2368 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/efs/file_system_utils.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/efs/mount_target_utils.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/efs/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.196168 idem-aws-3.0.2/idem_aws/tool/aws/eks/
--rw-r--r--   0 root         (0) root         (0)     4881 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/eks/addon.py
--rw-r--r--   0 root         (0) root         (0)     9514 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/eks/cluster.py
--rw-r--r--   0 root         (0) root         (0)     5220 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/eks/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     4559 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/eks/eks_utils.py
--rw-r--r--   0 root         (0) root         (0)     7710 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/eks/nodegroup.py
--rw-r--r--   0 root         (0) root         (0)     1868 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/eks/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.196168 idem-aws-3.0.2/idem_aws/tool/aws/elasticache/
--rw-r--r--   0 root         (0) root         (0)     9302 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/elasticache/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    20324 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/elasticache/elasticache_utils.py
--rw-r--r--   0 root         (0) root         (0)     1737 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/elasticache/parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.196168 idem-aws-3.0.2/idem_aws/tool/aws/elb/
--rw-r--r--   0 root         (0) root         (0)     1957 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/elb/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    19196 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/elb/load_balancer.py
--rw-r--r--   0 root         (0) root         (0)     2429 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/elb/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.200168 idem-aws-3.0.2/idem_aws/tool/aws/elbv2/
--rw-r--r--   0 root         (0) root         (0)     7683 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/elbv2/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    10904 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/elbv2/listener.py
--rw-r--r--   0 root         (0) root         (0)    10107 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/elbv2/load_balancer.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/elbv2/tag.py
--rw-r--r--   0 root         (0) root         (0)    10958 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/elbv2/target_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.200168 idem-aws-3.0.2/idem_aws/tool/aws/es/
--rw-r--r--   0 root         (0) root         (0)     9741 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/es/elasticsearch_domain.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/es/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.200168 idem-aws-3.0.2/idem_aws/tool/aws/events/
--rw-r--r--   0 root         (0) root         (0)     1707 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/events/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     7407 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/events/rule.py
--rw-r--r--   0 root         (0) root         (0)     2752 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/events/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.200168 idem-aws-3.0.2/idem_aws/tool/aws/guardduty/
--rw-r--r--   0 root         (0) root         (0)     1048 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/guardduty/config_utils.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/guardduty/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     7045 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/guardduty/detector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.200168 idem-aws-3.0.2/idem_aws/tool/aws/iam/
--rw-r--r--   0 root         (0) root         (0)    12684 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/iam/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     1649 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/iam/group.py
--rw-r--r--   0 root         (0) root         (0)     2324 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/iam/group_membership.py
--rw-r--r--   0 root         (0) root         (0)     2737 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/iam/password_policy.py
--rw-r--r--   0 root         (0) root         (0)     7466 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/iam/policy.py
--rw-r--r--   0 root         (0) root         (0)     1573 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/iam/role_policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)     1251 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/iam/service_linked_role.py
--rw-r--r--   0 root         (0) root         (0)     3720 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/iam/user.py
--rw-r--r--   0 root         (0) root         (0)     1486 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/iam/user_ssh_key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.200168 idem-aws-3.0.2/idem_aws/tool/aws/kinesis/
--rw-r--r--   0 root         (0) root         (0)     1976 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/kinesis/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    21390 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/kinesis/stream.py
--rw-r--r--   0 root         (0) root         (0)     2362 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/kinesis/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.200168 idem-aws-3.0.2/idem_aws/tool/aws/kms/
--rw-r--r--   0 root         (0) root         (0)      999 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/kms/alias.py
--rw-r--r--   0 root         (0) root         (0)     3195 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/kms/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3159 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/kms/key.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/kms/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.200168 idem-aws-3.0.2/idem_aws/tool/aws/lambda_aws/
--rw-r--r--   0 root         (0) root         (0)     3194 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/lambda_aws/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    16057 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/lambda_aws/function.py
--rw-r--r--   0 root         (0) root         (0)     4274 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/lambda_aws/function_event_invoke_config.py
--rw-r--r--   0 root         (0) root         (0)     2579 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/lambda_aws/function_permission.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/lambda_aws/function_provisioned_concurrency_config.py
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/lambda_aws/init.py
--rw-r--r--   0 root         (0) root         (0)     2689 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/lambda_aws/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.200168 idem-aws-3.0.2/idem_aws/tool/aws/logs/
--rw-r--r--   0 root         (0) root         (0)     1336 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/logs/subscription_filter_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.200168 idem-aws-3.0.2/idem_aws/tool/aws/neptune/
--rw-r--r--   0 root         (0) root         (0)     8991 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/neptune/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    12251 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/neptune/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)     6385 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/neptune/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    11654 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/neptune/db_instance.py
--rw-r--r--   0 root         (0) root         (0)     6128 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/neptune/db_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     1546 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/neptune/db_subnet_group.py
--rw-r--r--   0 root         (0) root         (0)     3258 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/neptune/tag.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/network_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.200168 idem-aws-3.0.2/idem_aws/tool/aws/organizations/
--rw-r--r--   0 root         (0) root         (0)     1793 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/organizations/account.py
--rw-r--r--   0 root         (0) root         (0)     4916 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/organizations/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/organizations/policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)     2704 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/organizations/tag.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.200168 idem-aws-3.0.2/idem_aws/tool/aws/rds/
--rw-r--r--   0 root         (0) root         (0)    12718 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/rds/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     5582 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/rds/parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.200168 idem-aws-3.0.2/idem_aws/tool/aws/route53/
--rw-r--r--   0 root         (0) root         (0)     5018 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/route53/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     1251 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/route53/hosted_zone_association.py
--rw-r--r--   0 root         (0) root         (0)     5900 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/route53/hosted_zone_utils.py
--rw-r--r--   0 root         (0) root         (0)     7422 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/route53/resource_record_utils.py
--rw-r--r--   0 root         (0) root         (0)     2663 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/route53/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.204168 idem-aws-3.0.2/idem_aws/tool/aws/s3/
--rw-r--r--   0 root         (0) root         (0)     1526 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/s3/bucket_acl.py
--rw-r--r--   0 root         (0) root         (0)     7925 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/s3/bucket_encryption.py
--rw-r--r--   0 root         (0) root         (0)     7403 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/s3/bucket_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     2440 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/s3/bucket_logging.py
--rw-r--r--   0 root         (0) root         (0)     2584 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/s3/bucket_replication.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/s3/bucket_versioning.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/s3/bucket_website.py
--rw-r--r--   0 root         (0) root         (0)     9894 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/s3/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3373 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/s3/s3_utils.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/search_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.204168 idem-aws-3.0.2/idem_aws/tool/aws/ses/
--rw-r--r--   0 root         (0) root         (0)     1214 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/ses/conversion_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.204168 idem-aws-3.0.2/idem_aws/tool/aws/sesv2/
--rw-r--r--   0 root         (0) root         (0)      563 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/sesv2/conversion_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.204168 idem-aws-3.0.2/idem_aws/tool/aws/sns/
--rw-r--r--   0 root         (0) root         (0)     3275 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/sns/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     7581 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/sns/sns_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.204168 idem-aws-3.0.2/idem_aws/tool/aws/sqs/
--rw-r--r--   0 root         (0) root         (0)     6482 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/sqs/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/sqs/queue_utils.py
--rw-r--r--   0 root         (0) root         (0)     3723 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/state_comparison_utils.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/state_utils.py
--rw-r--r--   0 root         (0) root         (0)      526 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/string_utils.py
--rw-r--r--   0 root         (0) root         (0)     5900 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/tag_utils.py
--rw-r--r--   0 root         (0) root         (0)     1548 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/test_state_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.204168 idem-aws-3.0.2/idem_aws/tool/aws/wafv2/
--rw-r--r--   0 root         (0) root         (0)     6843 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/wafv2/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3076 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/wafv2/ip_set_utils.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/wafv2/regex_pattern_set.py
--rw-r--r--   0 root         (0) root         (0)     3822 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/wafv2/tag.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/wafv2/web_acl.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/aws/waiter_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.204168 idem-aws-3.0.2/idem_aws/tool/boto3/
--rw-r--r--   0 root         (0) root         (0)     5478 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/boto3/client.py
--rw-r--r--   0 root         (0) root         (0)     5181 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/boto3/custom_waiter.py
--rw-r--r--   0 root         (0) root         (0)      429 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/boto3/exception.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/boto3/region.py
--rw-r--r--   0 root         (0) root         (0)     6270 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/boto3/resolve.py
--rw-r--r--   0 root         (0) root         (0)     5230 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/boto3/resource.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/boto3/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.204168 idem-aws-3.0.2/idem_aws/tool/heist/
--rw-r--r--   0 root         (0) root         (0)      906 2023-07-22 15:45:47.000000 idem-aws-3.0.2/idem_aws/tool/heist/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-22 15:46:01.000000 idem-aws-3.0.2/idem_aws/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:46:02.160168 idem-aws-3.0.2/idem_aws.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11104 2023-07-22 15:46:02.000000 idem-aws-3.0.2/idem_aws.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    22681 2023-07-22 15:46:02.000000 idem-aws-3.0.2/idem_aws.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 15:46:02.000000 idem-aws-3.0.2/idem_aws.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      580 2023-07-22 15:46:02.000000 idem-aws-3.0.2/idem_aws.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-22 15:46:02.000000 idem-aws-3.0.2/idem_aws.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      366 2023-07-22 15:45:47.000000 idem-aws-3.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-22 15:46:02.204168 idem-aws-3.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3188 2023-07-22 15:45:47.000000 idem-aws-3.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.571854 idem-aws-3.0.3/
+-rw-r--r--   0 root         (0) root         (0)    11342 2023-07-28 19:34:42.000000 idem-aws-3.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-28 19:34:42.000000 idem-aws-3.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11104 2023-07-28 19:34:56.571854 idem-aws-3.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9835 2023-07-28 19:34:42.000000 idem-aws-3.0.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.527854 idem-aws-3.0.3/idem_aws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.523854 idem-aws-3.0.3/idem_aws/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/acct/aws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/acct/aws/contracts/
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/acct/aws/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     5506 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/acct/aws/gsuite.py
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/acct/aws/iam.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/acct/aws/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/acct/metadata/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/acct/metadata/aws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.523854 idem-aws-3.0.3/idem_aws/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/autogen/aws/
+-rw-r--r--   0 root         (0) root         (0)     7080 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/autogen/aws/function.py
+-rw-r--r--   0 root         (0) root         (0)     9290 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/autogen/aws/init.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/autogen/aws/known_params.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/autogen/aws/param.py
+-rw-r--r--   0 root         (0) root         (0)    10201 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/autogen/aws/plugin.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/autogen/aws/possible_functions.py
+-rw-r--r--   0 root         (0) root         (0)     3870 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/autogen/aws/resource.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/autogen/aws/service.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/esm/
+-rw-r--r--   0 root         (0) root         (0)     8838 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/esm/aws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/esm/contracts/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/esm/contracts/aws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.523854 idem-aws-3.0.3/idem_aws/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/exec/aws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/exec/aws/acm/
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/acm/certificate_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/exec/aws/apigateway/
+-rw-r--r--   0 root         (0) root         (0)     5430 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/apigateway/base_path_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/apigateway/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/apigateway/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/apigateway/integration.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/apigateway/integration_response.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/apigateway/method.py
+-rw-r--r--   0 root         (0) root         (0)     2145 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/apigateway/method_response.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/apigateway/resource.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/apigateway/rest_api.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/apigateway/stage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/exec/aws/apigatewayv2/
+-rw-r--r--   0 root         (0) root         (0)     3276 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/apigatewayv2/api.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/apigatewayv2/authorizer.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/apigatewayv2/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/apigatewayv2/integration.py
+-rw-r--r--   0 root         (0) root         (0)     3761 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/apigatewayv2/route.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/exec/aws/application_autoscaling/
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/application_autoscaling/scalable_target.py
+-rw-r--r--   0 root         (0) root         (0)     3395 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/application_autoscaling/scaling_policy.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/arn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/exec/aws/autoscaling/
+-rw-r--r--   0 root         (0) root         (0)     3034 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/autoscaling/scaling_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/exec/aws/backup/
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/backup/backup_vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/exec/aws/budgets/
+-rw-r--r--   0 root         (0) root         (0)     4105 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/budgets/budget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/exec/aws/cloudformation/
+-rw-r--r--   0 root         (0) root         (0)     2285 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/cloudformation/stack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/exec/aws/cloudfront/
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/cloudfront/cache_policy.py
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/cloudfront/distribution.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/cloudfront/origin_request_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/exec/aws/cloudwatch/
+-rw-r--r--   0 root         (0) root         (0)     3012 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/cloudwatch/log_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/exec/aws/cloudwatchlogs/
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/cloudwatchlogs/resource_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/exec/aws/config/
+-rw-r--r--   0 root         (0) root         (0)     4538 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/config/configuration_aggregator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/exec/aws/costexplorer/
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/costexplorer/cost_allocation_tag.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/exec/aws/docdb/
+-rw-r--r--   0 root         (0) root         (0)     6138 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/docdb/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     7293 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/docdb/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     4887 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/docdb/db_subnet_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.531854 idem-aws-3.0.3/idem_aws/exec/aws/dynamodb/
+-rw-r--r--   0 root         (0) root         (0)     2434 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/dynamodb/table.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/dynamodb/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.535854 idem-aws-3.0.3/idem_aws/exec/aws/ec2/
+-rw-r--r--   0 root         (0) root         (0)     8697 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/ami.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/availability_zones.py
+-rw-r--r--   0 root         (0) root         (0)     4206 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/elastic_ip.py
+-rw-r--r--   0 root         (0) root         (0)     3405 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/flow_log.py
+-rw-r--r--   0 root         (0) root         (0)    22062 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/instance.py
+-rw-r--r--   0 root         (0) root         (0)     3299 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/instance_type.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/internet_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/key_pair.py
+-rw-r--r--   0 root         (0) root         (0)     7293 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/launch_template.py
+-rw-r--r--   0 root         (0) root         (0)     8692 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/network_interface.py
+-rw-r--r--   0 root         (0) root         (0)     4680 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/placement_group.py
+-rw-r--r--   0 root         (0) root         (0)     5836 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/route.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/route_table.py
+-rw-r--r--   0 root         (0) root         (0)     3265 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/route_table_association.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/security_group.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/security_group_rule.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/spot_instance_request.py
+-rw-r--r--   0 root         (0) root         (0)     8595 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/subnet.py
+-rw-r--r--   0 root         (0) root         (0)     4471 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/volume.py
+-rw-r--r--   0 root         (0) root         (0)     4527 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/vpc.py
+-rw-r--r--   0 root         (0) root         (0)     4081 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/vpc_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/vpc_peering_connection.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/vpc_peering_connection_accepter.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ec2/vpc_peering_connection_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.535854 idem-aws-3.0.3/idem_aws/exec/aws/ecr/
+-rw-r--r--   0 root         (0) root         (0)     5183 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ecr/image.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ecr/lifecycle_policy.py
+-rw-r--r--   0 root         (0) root         (0)     5504 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ecr/repository.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ecr/repository_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.535854 idem-aws-3.0.3/idem_aws/exec/aws/eks/
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/eks/cluster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.535854 idem-aws-3.0.3/idem_aws/exec/aws/elasticache/
+-rw-r--r--   0 root         (0) root         (0)     2934 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/elasticache/replication_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.535854 idem-aws-3.0.3/idem_aws/exec/aws/elb/
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/elb/elb_hosted_zone_id.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/elb/load_balancer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.535854 idem-aws-3.0.3/idem_aws/exec/aws/elbv2/
+-rw-r--r--   0 root         (0) root         (0)     3296 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/elbv2/listener.py
+-rw-r--r--   0 root         (0) root         (0)     3346 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/elbv2/load_balancer.py
+-rw-r--r--   0 root         (0) root         (0)     4861 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/elbv2/target_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.535854 idem-aws-3.0.3/idem_aws/exec/aws/es/
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/es/elasticsearch_domain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.535854 idem-aws-3.0.3/idem_aws/exec/aws/events/
+-rw-r--r--   0 root         (0) root         (0)     5682 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/events/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.535854 idem-aws-3.0.3/idem_aws/exec/aws/guardduty/
+-rw-r--r--   0 root         (0) root         (0)     2423 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/guardduty/detector.py
+-rw-r--r--   0 root         (0) root         (0)     5618 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/guardduty/member.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/guardduty/organization_admin_account.py
+-rw-r--r--   0 root         (0) root         (0)     8636 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/guardduty/organization_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.535854 idem-aws-3.0.3/idem_aws/exec/aws/iam/
+-rw-r--r--   0 root         (0) root         (0)     9324 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/iam/access_key.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/iam/group.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/iam/group_membership.py
+-rw-r--r--   0 root         (0) root         (0)     2099 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/iam/group_policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     4749 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/iam/instance_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7709 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/iam/open_id_connect_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/iam/password_policy.py
+-rw-r--r--   0 root         (0) root         (0)     6957 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/iam/policy.py
+-rw-r--r--   0 root         (0) root         (0)     9723 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/iam/role.py
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/iam/user.py
+-rw-r--r--   0 root         (0) root         (0)     2945 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/iam/user_policy_attachment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.535854 idem-aws-3.0.3/idem_aws/exec/aws/kinesis/
+-rw-r--r--   0 root         (0) root         (0)     2919 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/kinesis/stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.535854 idem-aws-3.0.3/idem_aws/exec/aws/kms/
+-rw-r--r--   0 root         (0) root         (0)     3031 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/kms/key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/exec/aws/lambda_aws/
+-rw-r--r--   0 root         (0) root         (0)     4863 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/lambda_aws/function_event_invoke_config.py
+-rw-r--r--   0 root         (0) root         (0)     5632 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/lambda_aws/function_provisioned_concurrency_config.py
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/lambda_aws/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/exec/aws/neptune/
+-rw-r--r--   0 root         (0) root         (0)     7388 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/neptune/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     6621 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/neptune/db_instance.py
+-rw-r--r--   0 root         (0) root         (0)     6854 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/neptune/db_parameter_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/exec/aws/organizations/
+-rw-r--r--   0 root         (0) root         (0)     4486 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/organizations/account.py
+-rw-r--r--   0 root         (0) root         (0)     2391 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/organizations/policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/exec/aws/rds/
+-rw-r--r--   0 root         (0) root         (0)     5996 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/rds/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5001 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/rds/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     5971 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/rds/db_instance.py
+-rw-r--r--   0 root         (0) root         (0)     6287 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/rds/db_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/rds/db_subnet_group.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/rds/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/exec/aws/route53/
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/route53/hosted_zone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/exec/aws/s3/
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/s3/bucket.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/s3/bucket_acl.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/s3/bucket_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/s3/bucket_logging.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/s3/bucket_replication.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/s3/bucket_website.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/exec/aws/ses/
+-rw-r--r--   0 root         (0) root         (0)     3203 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ses/domain_identity.py
+-rw-r--r--   0 root         (0) root         (0)     4166 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/ses/identity_notification_topic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/exec/aws/sesv2/
+-rw-r--r--   0 root         (0) root         (0)     4342 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/sesv2/event_destination.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/exec/aws/sns/
+-rw-r--r--   0 root         (0) root         (0)     3682 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/sns/subscription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/exec/aws/sqs/
+-rw-r--r--   0 root         (0) root         (0)     4684 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/sqs/queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/exec/aws/sts/
+-rw-r--r--   0 root         (0) root         (0)     5261 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/sts/assume_role.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/sts/caller_identity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/exec/aws/wafv2/
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/wafv2/ip_set.py
+-rw-r--r--   0 root         (0) root         (0)     7041 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/aws/wafv2/regex_pattern_set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/exec/boto3/
+-rw-r--r--   0 root         (0) root         (0)      747 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/exec/boto3/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.523854 idem-aws-3.0.3/idem_aws/reconcile/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/reconcile/pending/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/reconcile/pending/aws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.523854 idem-aws-3.0.3/idem_aws/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/states/aws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/states/aws/acm/
+-rw-r--r--   0 root         (0) root         (0)    28335 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/acm/certificate_manager.py
+-rw-r--r--   0 root         (0) root         (0)    11132 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/acm/certificate_validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.539854 idem-aws-3.0.3/idem_aws/states/aws/apigateway/
+-rw-r--r--   0 root         (0) root         (0)    10257 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/apigateway/base_path_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    12091 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/apigateway/deployment.py
+-rw-r--r--   0 root         (0) root         (0)    19520 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/apigateway/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)    15779 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/apigateway/integration.py
+-rw-r--r--   0 root         (0) root         (0)    13752 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/apigateway/integration_response.py
+-rw-r--r--   0 root         (0) root         (0)    12950 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/apigateway/method.py
+-rw-r--r--   0 root         (0) root         (0)    12155 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/apigateway/method_response.py
+-rw-r--r--   0 root         (0) root         (0)     9866 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/apigateway/resource.py
+-rw-r--r--   0 root         (0) root         (0)    13732 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/apigateway/rest_api.py
+-rw-r--r--   0 root         (0) root         (0)    13857 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/apigateway/stage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.543854 idem-aws-3.0.3/idem_aws/states/aws/apigatewayv2/
+-rw-r--r--   0 root         (0) root         (0)    15354 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/apigatewayv2/api.py
+-rw-r--r--   0 root         (0) root         (0)    16244 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/apigatewayv2/authorizer.py
+-rw-r--r--   0 root         (0) root         (0)    15119 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/apigatewayv2/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)    22693 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/apigatewayv2/integration.py
+-rw-r--r--   0 root         (0) root         (0)    14022 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/apigatewayv2/route.py
+-rw-r--r--   0 root         (0) root         (0)    16913 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/apigatewayv2/stage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.543854 idem-aws-3.0.3/idem_aws/states/aws/application_autoscaling/
+-rw-r--r--   0 root         (0) root         (0)    31855 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/application_autoscaling/scalable_target.py
+-rw-r--r--   0 root         (0) root         (0)    45934 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/application_autoscaling/scaling_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.543854 idem-aws-3.0.3/idem_aws/states/aws/autoscaling/
+-rw-r--r--   0 root         (0) root         (0)    78777 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/autoscaling/auto_scaling_group.py
+-rw-r--r--   0 root         (0) root         (0)    32523 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/autoscaling/launch_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    54968 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/autoscaling/scaling_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.543854 idem-aws-3.0.3/idem_aws/states/aws/backup/
+-rw-r--r--   0 root         (0) root         (0)     8985 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/backup/backup_vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.543854 idem-aws-3.0.3/idem_aws/states/aws/budgets/
+-rw-r--r--   0 root         (0) root         (0)    25523 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/budgets/budget.py
+-rw-r--r--   0 root         (0) root         (0)    16456 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/budgets/budget_action.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/caller_identity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.543854 idem-aws-3.0.3/idem_aws/states/aws/cloudformation/
+-rw-r--r--   0 root         (0) root         (0)    32414 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/cloudformation/stack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.543854 idem-aws-3.0.3/idem_aws/states/aws/cloudfront/
+-rw-r--r--   0 root         (0) root         (0)    24459 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/cloudfront/cache_policy.py
+-rw-r--r--   0 root         (0) root         (0)   116104 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/cloudfront/distribution.py
+-rw-r--r--   0 root         (0) root         (0)    15501 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/cloudfront/origin_request_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.543854 idem-aws-3.0.3/idem_aws/states/aws/cloudtrail/
+-rw-r--r--   0 root         (0) root         (0)    37423 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/cloudtrail/trail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.543854 idem-aws-3.0.3/idem_aws/states/aws/cloudwatch/
+-rw-r--r--   0 root         (0) root         (0)    11420 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/cloudwatch/log_group.py
+-rw-r--r--   0 root         (0) root         (0)    36075 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/cloudwatch/metric_alarm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.543854 idem-aws-3.0.3/idem_aws/states/aws/cloudwatchlogs/
+-rw-r--r--   0 root         (0) root         (0)     8723 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/cloudwatchlogs/resource_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.543854 idem-aws-3.0.3/idem_aws/states/aws/config/
+-rwxr-xr-x   0 root         (0) root         (0)    11422 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/config/config_recorder.py
+-rwxr-xr-x   0 root         (0) root         (0)     9512 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/config/config_recorder_status.py
+-rw-r--r--   0 root         (0) root         (0)    10463 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/config/configuration_aggregator.py
+-rwxr-xr-x   0 root         (0) root         (0)    12062 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/config/delivery_channel.py
+-rw-r--r--   0 root         (0) root         (0)    21665 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/config/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.543854 idem-aws-3.0.3/idem_aws/states/aws/costexplorer/
+-rw-r--r--   0 root         (0) root         (0)    18653 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/costexplorer/anomaly_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    10751 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/costexplorer/anomaly_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    28397 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/costexplorer/cost_category.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.543854 idem-aws-3.0.3/idem_aws/states/aws/docdb/
+-rw-r--r--   0 root         (0) root         (0)    28355 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/docdb/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    12967 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/docdb/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    11755 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/docdb/db_subnet_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.543854 idem-aws-3.0.3/idem_aws/states/aws/dynamodb/
+-rw-r--r--   0 root         (0) root         (0)    36228 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/dynamodb/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.547854 idem-aws-3.0.3/idem_aws/states/aws/ec2/
+-rw-r--r--   0 root         (0) root         (0)    22039 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/ami.py
+-rw-r--r--   0 root         (0) root         (0)    15794 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/dhcp_option.py
+-rw-r--r--   0 root         (0) root         (0)    10017 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/dhcp_option_association.py
+-rw-r--r--   0 root         (0) root         (0)    13002 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/elastic_ip.py
+-rw-r--r--   0 root         (0) root         (0)    12633 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/flow_log.py
+-rw-r--r--   0 root         (0) root         (0)    41622 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/instance.py
+-rw-r--r--   0 root         (0) root         (0)    12429 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/internet_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     9711 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/key_pair.py
+-rw-r--r--   0 root         (0) root         (0)    73447 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/launch_template.py
+-rw-r--r--   0 root         (0) root         (0)    17418 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/nat_gateway.py
+-rw-r--r--   0 root         (0) root         (0)    12093 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/network_interface.py
+-rw-r--r--   0 root         (0) root         (0)    10946 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/placement_group.py
+-rw-r--r--   0 root         (0) root         (0)    14835 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/route.py
+-rw-r--r--   0 root         (0) root         (0)    15623 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/route_table.py
+-rw-r--r--   0 root         (0) root         (0)     8933 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/route_table_association.py
+-rw-r--r--   0 root         (0) root         (0)    12947 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/security_group.py
+-rw-r--r--   0 root         (0) root         (0)    17979 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/security_group_rule.py
+-rw-r--r--   0 root         (0) root         (0)    10513 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    36976 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/spot_instance_request.py
+-rw-r--r--   0 root         (0) root         (0)    20082 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/subnet.py
+-rw-r--r--   0 root         (0) root         (0)    17765 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/transit_gateway.py
+-rw-r--r--   0 root         (0) root         (0)    16953 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/transit_gateway_vpc_attachment.py
+-rw-r--r--   0 root         (0) root         (0)    15331 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/volume.py
+-rw-r--r--   0 root         (0) root         (0)    19112 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/vpc.py
+-rw-r--r--   0 root         (0) root         (0)    19294 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/vpc_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)    14516 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/vpc_peering_connection.py
+-rw-r--r--   0 root         (0) root         (0)     9225 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/vpc_peering_connection_accepter.py
+-rw-r--r--   0 root         (0) root         (0)     9871 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ec2/vpc_peering_connection_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.547854 idem-aws-3.0.3/idem_aws/states/aws/ecr/
+-rw-r--r--   0 root         (0) root         (0)    11587 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ecr/lifecycle_policy.py
+-rw-r--r--   0 root         (0) root         (0)    13319 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ecr/repository.py
+-rw-r--r--   0 root         (0) root         (0)    11708 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ecr/repository_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.547854 idem-aws-3.0.3/idem_aws/states/aws/efs/
+-rw-r--r--   0 root         (0) root         (0)    25301 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/efs/file_system.py
+-rw-r--r--   0 root         (0) root         (0)    22090 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/efs/mount_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.547854 idem-aws-3.0.3/idem_aws/states/aws/eks/
+-rw-r--r--   0 root         (0) root         (0)    18084 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/eks/addon.py
+-rw-r--r--   0 root         (0) root         (0)    29585 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/eks/cluster.py
+-rw-r--r--   0 root         (0) root         (0)    17678 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/eks/fargate_profile.py
+-rw-r--r--   0 root         (0) root         (0)    29787 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/eks/nodegroup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.547854 idem-aws-3.0.3/idem_aws/states/aws/elasticache/
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/elasticache/cache_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    13492 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/elasticache/cache_subnet_group.py
+-rw-r--r--   0 root         (0) root         (0)    51005 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/elasticache/replication_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.547854 idem-aws-3.0.3/idem_aws/states/aws/elb/
+-rw-r--r--   0 root         (0) root         (0)    19828 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/elb/load_balancer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.547854 idem-aws-3.0.3/idem_aws/states/aws/elbv2/
+-rw-r--r--   0 root         (0) root         (0)    32920 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/elbv2/listener.py
+-rw-r--r--   0 root         (0) root         (0)    24159 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/elbv2/load_balancer.py
+-rw-r--r--   0 root         (0) root         (0)    30475 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/elbv2/target_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.547854 idem-aws-3.0.3/idem_aws/states/aws/es/
+-rw-r--r--   0 root         (0) root         (0)    36336 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/es/elasticsearch_domain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.547854 idem-aws-3.0.3/idem_aws/states/aws/events/
+-rw-r--r--   0 root         (0) root         (0)    45318 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/events/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.547854 idem-aws-3.0.3/idem_aws/states/aws/guardduty/
+-rw-r--r--   0 root         (0) root         (0)    15458 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/guardduty/detector.py
+-rw-r--r--   0 root         (0) root         (0)    10351 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/guardduty/member.py
+-rw-r--r--   0 root         (0) root         (0)     8768 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/guardduty/organization_admin_account.py
+-rw-r--r--   0 root         (0) root         (0)     8981 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/guardduty/organization_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.551854 idem-aws-3.0.3/idem_aws/states/aws/iam/
+-rw-r--r--   0 root         (0) root         (0)     9988 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/iam/access_key.py
+-rw-r--r--   0 root         (0) root         (0)     8246 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/iam/group.py
+-rw-r--r--   0 root         (0) root         (0)     8179 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/iam/group_membership.py
+-rw-r--r--   0 root         (0) root         (0)     8776 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/iam/group_policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)    14496 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/iam/instance_profile.py
+-rw-r--r--   0 root         (0) root         (0)    18389 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/iam/open_id_connect_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12320 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/iam/password_policy.py
+-rw-r--r--   0 root         (0) root         (0)    14614 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/iam/policy.py
+-rw-r--r--   0 root         (0) root         (0)    22433 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/iam/role.py
+-rw-r--r--   0 root         (0) root         (0)    14539 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/iam/role_policy.py
+-rw-r--r--   0 root         (0) root         (0)    10537 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/iam/role_policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)    15633 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/iam/service_linked_role.py
+-rw-r--r--   0 root         (0) root         (0)    15522 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/iam/user.py
+-rw-r--r--   0 root         (0) root         (0)    14079 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/iam/user_policy.py
+-rw-r--r--   0 root         (0) root         (0)    11044 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/iam/user_policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)    13341 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/iam/user_ssh_key.py
+-rw-r--r--   0 root         (0) root         (0)      169 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.551854 idem-aws-3.0.3/idem_aws/states/aws/kinesis/
+-rw-r--r--   0 root         (0) root         (0)    24114 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/kinesis/stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.551854 idem-aws-3.0.3/idem_aws/states/aws/kms/
+-rw-r--r--   0 root         (0) root         (0)    10460 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/kms/alias.py
+-rw-r--r--   0 root         (0) root         (0)    22630 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/kms/key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.551854 idem-aws-3.0.3/idem_aws/states/aws/lambda_aws/
+-rw-r--r--   0 root         (0) root         (0)    27963 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/lambda_aws/function.py
+-rw-r--r--   0 root         (0) root         (0)    11651 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/lambda_aws/function_event_invoke_config.py
+-rw-r--r--   0 root         (0) root         (0)    14029 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/lambda_aws/function_permission.py
+-rw-r--r--   0 root         (0) root         (0)    10018 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/lambda_aws/function_provisioned_concurrency_config.py
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/lambda_aws/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.551854 idem-aws-3.0.3/idem_aws/states/aws/logs/
+-rw-r--r--   0 root         (0) root         (0)    12064 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/logs/subscription_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.551854 idem-aws-3.0.3/idem_aws/states/aws/neptune/
+-rw-r--r--   0 root         (0) root         (0)    32988 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/neptune/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    13936 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/neptune/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    37556 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/neptune/db_instance.py
+-rw-r--r--   0 root         (0) root         (0)    12467 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/neptune/db_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    14288 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/neptune/db_subnet_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.551854 idem-aws-3.0.3/idem_aws/states/aws/organizations/
+-rw-r--r--   0 root         (0) root         (0)    17382 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/organizations/account.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/organizations/organization.py
+-rw-r--r--   0 root         (0) root         (0)    14282 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/organizations/organization_unit.py
+-rw-r--r--   0 root         (0) root         (0)    13176 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/organizations/policy.py
+-rw-r--r--   0 root         (0) root         (0)    11396 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/organizations/policy_attachment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.551854 idem-aws-3.0.3/idem_aws/states/aws/rds/
+-rw-r--r--   0 root         (0) root         (0)    62077 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/rds/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    14695 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/rds/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    39434 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/rds/db_instance.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/rds/db_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    14036 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/rds/db_subnet_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.551854 idem-aws-3.0.3/idem_aws/states/aws/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/recursive_contracts/allow_sync_sls_name_and_name_tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.551854 idem-aws-3.0.3/idem_aws/states/aws/route53/
+-rw-r--r--   0 root         (0) root         (0)    19436 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/route53/hosted_zone.py
+-rw-r--r--   0 root         (0) root         (0)    14157 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/route53/hosted_zone_association.py
+-rw-r--r--   0 root         (0) root         (0)    12020 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/route53/resource_record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.555854 idem-aws-3.0.3/idem_aws/states/aws/s3/
+-rw-r--r--   0 root         (0) root         (0)    19835 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/s3/bucket.py
+-rw-r--r--   0 root         (0) root         (0)    11122 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_acl.py
+-rw-r--r--   0 root         (0) root         (0)    15157 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_encryption.py
+-rw-r--r--   0 root         (0) root         (0)    26660 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)    14837 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_logging.py
+-rw-r--r--   0 root         (0) root         (0)    17613 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_notification.py
+-rw-r--r--   0 root         (0) root         (0)    11942 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_policy.py
+-rw-r--r--   0 root         (0) root         (0)    27930 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_replication.py
+-rw-r--r--   0 root         (0) root         (0)    10328 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_versioning.py
+-rw-r--r--   0 root         (0) root         (0)    22433 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_website.py
+-rw-r--r--   0 root         (0) root         (0)    12854 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/s3/public_access_block.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.555854 idem-aws-3.0.3/idem_aws/states/aws/ses/
+-rw-r--r--   0 root         (0) root         (0)     6157 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ses/domain_identity.py
+-rw-r--r--   0 root         (0) root         (0)    10384 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/ses/identity_notification_topic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.555854 idem-aws-3.0.3/idem_aws/states/aws/sesv2/
+-rw-r--r--   0 root         (0) root         (0)    14618 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/sesv2/event_destination.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.555854 idem-aws-3.0.3/idem_aws/states/aws/sns/
+-rw-r--r--   0 root         (0) root         (0)    11654 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/sns/subscription.py
+-rw-r--r--   0 root         (0) root         (0)    13240 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/sns/topic.py
+-rw-r--r--   0 root         (0) root         (0)     8687 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/sns/topic_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.555854 idem-aws-3.0.3/idem_aws/states/aws/sqs/
+-rw-r--r--   0 root         (0) root         (0)    24690 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/sqs/queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.555854 idem-aws-3.0.3/idem_aws/states/aws/wafv2/
+-rw-r--r--   0 root         (0) root         (0)     9933 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/wafv2/associate_web_acl.py
+-rw-r--r--   0 root         (0) root         (0)    14712 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/wafv2/ip_set.py
+-rw-r--r--   0 root         (0) root         (0)    12255 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/wafv2/regex_pattern_set.py
+-rw-r--r--   0 root         (0) root         (0)   268538 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/states/aws/wafv2/web_acl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.527854 idem-aws-3.0.3/idem_aws/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.555854 idem-aws-3.0.3/idem_aws/tool/aws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.555854 idem-aws-3.0.3/idem_aws/tool/aws/acct/
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/acct/assume_role.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.555854 idem-aws-3.0.3/idem_aws/tool/aws/acct/contracts/
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/acct/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      293 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/acct/esm.py
+-rw-r--r--   0 root         (0) root         (0)      714 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/acct/init.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/acct/key_name.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.555854 idem-aws-3.0.3/idem_aws/tool/aws/acm/
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/acm/certificate_validation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5339 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/acm/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2625 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/acm/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.555854 idem-aws-3.0.3/idem_aws/tool/aws/apigateway/
+-rw-r--r--   0 root         (0) root         (0)     3883 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigateway/base_path_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     3341 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigateway/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     8767 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigateway/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)     4534 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigateway/integration.py
+-rw-r--r--   0 root         (0) root         (0)     5000 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigateway/integration_response.py
+-rw-r--r--   0 root         (0) root         (0)     4226 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigateway/method.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigateway/method_response.py
+-rw-r--r--   0 root         (0) root         (0)     4087 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigateway/resource.py
+-rw-r--r--   0 root         (0) root         (0)     7175 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigateway/rest_api.py
+-rw-r--r--   0 root         (0) root         (0)     4417 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigateway/stage.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigateway/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.559854 idem-aws-3.0.3/idem_aws/tool/aws/apigatewayv2/
+-rw-r--r--   0 root         (0) root         (0)     5671 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigatewayv2/api.py
+-rw-r--r--   0 root         (0) root         (0)     5125 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigatewayv2/authorizer.py
+-rw-r--r--   0 root         (0) root         (0)     4842 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigatewayv2/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)     5187 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigatewayv2/integration.py
+-rw-r--r--   0 root         (0) root         (0)     4793 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigatewayv2/route.py
+-rw-r--r--   0 root         (0) root         (0)     4061 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigatewayv2/stage.py
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/apigatewayv2/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.559854 idem-aws-3.0.3/idem_aws/tool/aws/application_autoscaling/
+-rw-r--r--   0 root         (0) root         (0)     2724 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/application_autoscaling/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/application_autoscaling/scalable_target.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/application_autoscaling/scaling_policy.py
+-rw-r--r--   0 root         (0) root         (0)     4099 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/arn_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.559854 idem-aws-3.0.3/idem_aws/tool/aws/autoscaling/
+-rw-r--r--   0 root         (0) root         (0)     5561 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/autoscaling/auto_scaling_group_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4257 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/autoscaling/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3367 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/autoscaling/scaling_policy.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/autoscaling/tag.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/b64.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.559854 idem-aws-3.0.3/idem_aws/tool/aws/backup/
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/backup/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/backup/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.559854 idem-aws-3.0.3/idem_aws/tool/aws/budgets/
+-rw-r--r--   0 root         (0) root         (0)     5248 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/budgets/budget.py
+-rw-r--r--   0 root         (0) root         (0)     3415 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/budgets/budget_action.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/budgets/conversion_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.559854 idem-aws-3.0.3/idem_aws/tool/aws/cloudformation/
+-rw-r--r--   0 root         (0) root         (0)    18904 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/cloudformation/stack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.559854 idem-aws-3.0.3/idem_aws/tool/aws/cloudfront/
+-rw-r--r--   0 root         (0) root         (0)     6468 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/cloudfront/cloudfront_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4860 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/cloudfront/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7618 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/cloudfront/distribution.py
+-rw-r--r--   0 root         (0) root         (0)     2573 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/cloudfront/distribution_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/cloudfront/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.559854 idem-aws-3.0.3/idem_aws/tool/aws/cloudtrail/
+-rw-r--r--   0 root         (0) root         (0)     3966 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/cloudtrail/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    13076 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/cloudtrail/trail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.559854 idem-aws-3.0.3/idem_aws/tool/aws/cloudwatch/
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/cloudwatch/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)      807 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/cloudwatch/log_group.py
+-rw-r--r--   0 root         (0) root         (0)     4464 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/cloudwatch/metric_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/cloudwatch/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.559854 idem-aws-3.0.3/idem_aws/tool/aws/cloudwatchlogs/
+-rw-r--r--   0 root         (0) root         (0)      566 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/cloudwatchlogs/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/comment_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.559854 idem-aws-3.0.3/idem_aws/tool/aws/config/
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/config/config_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     4483 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/config/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/config/delivery_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/config/rule.py
+-rw-r--r--   0 root         (0) root         (0)     2434 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/config/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.559854 idem-aws-3.0.3/idem_aws/tool/aws/costexplorer/
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/costexplorer/anomaly_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/costexplorer/anomaly_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     2953 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/costexplorer/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/costexplorer/cost_category.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.559854 idem-aws-3.0.3/idem_aws/tool/aws/docdb/
+-rw-r--r--   0 root         (0) root         (0)    12556 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/docdb/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     6638 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/docdb/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/docdb/db_subnet_group.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/docdb/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.559854 idem-aws-3.0.3/idem_aws/tool/aws/dynamodb/
+-rw-r--r--   0 root         (0) root         (0)    15527 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/dynamodb/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.563854 idem-aws-3.0.3/idem_aws/tool/aws/ec2/
+-rw-r--r--   0 root         (0) root         (0)     3051 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/ami.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/availability_zones.py
+-rw-r--r--   0 root         (0) root         (0)    37825 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/dhcp_option_association_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/elastic_ip.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/flow_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.563854 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/data.py
+-rw-r--r--   0 root         (0) root         (0)     3450 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/key_pair.py
+-rw-r--r--   0 root         (0) root         (0)    19912 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.563854 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/block_device_mappings.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/bootstrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.563854 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/contracts/
+-rw-r--r--   0 root         (0) root         (0)      677 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/disable_api_termination.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/ebs_optimized.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/iam_instance_profile_arn.py
+-rw-r--r--   0 root         (0) root         (0)     8226 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/init.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/instance_initiated_shutdown_behavior.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/instance_type.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/kernel_id.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/monitoring_enabled.py
+-rw-r--r--   0 root         (0) root         (0)     4309 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/network_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/placement.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/private_ip_address.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/ram_disk_id.py
+-rw-r--r--   0 root         (0) root         (0)      214 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/running.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/security_group_ids.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/source_dest_check.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/sriov_net_support.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/user_data.py
+-rw-r--r--   0 root         (0) root         (0)     4843 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/internet_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/key_pair.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/launch_template.py
+-rw-r--r--   0 root         (0) root         (0)     3948 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/network_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/placement_group.py
+-rw-r--r--   0 root         (0) root         (0)    12208 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/route_table.py
+-rw-r--r--   0 root         (0) root         (0)     3924 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/security_group_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/spot_instance_request.py
+-rw-r--r--   0 root         (0) root         (0)    14415 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/subnet.py
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/tag.py
+-rw-r--r--   0 root         (0) root         (0)     3821 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/transit_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/transit_gateway_vpc_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/volume.py
+-rw-r--r--   0 root         (0) root         (0)     7822 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/vpc.py
+-rw-r--r--   0 root         (0) root         (0)     8498 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/vpc_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)    10645 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ec2/vpc_peering_connection_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.563854 idem-aws-3.0.3/idem_aws/tool/aws/ecr/
+-rw-r--r--   0 root         (0) root         (0)     4995 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ecr/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ecr/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.563854 idem-aws-3.0.3/idem_aws/tool/aws/efs/
+-rw-r--r--   0 root         (0) root         (0)     2368 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/efs/file_system_utils.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/efs/mount_target_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/efs/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.563854 idem-aws-3.0.3/idem_aws/tool/aws/eks/
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/eks/addon.py
+-rw-r--r--   0 root         (0) root         (0)     9514 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/eks/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5220 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/eks/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4559 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/eks/eks_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7710 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/eks/nodegroup.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/eks/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.563854 idem-aws-3.0.3/idem_aws/tool/aws/elasticache/
+-rw-r--r--   0 root         (0) root         (0)     9302 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/elasticache/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    20324 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/elasticache/elasticache_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/elasticache/parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.567855 idem-aws-3.0.3/idem_aws/tool/aws/elb/
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/elb/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    19196 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/elb/load_balancer.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/elb/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.567855 idem-aws-3.0.3/idem_aws/tool/aws/elbv2/
+-rw-r--r--   0 root         (0) root         (0)     7683 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/elbv2/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10904 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/elbv2/listener.py
+-rw-r--r--   0 root         (0) root         (0)    10107 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/elbv2/load_balancer.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/elbv2/tag.py
+-rw-r--r--   0 root         (0) root         (0)    10958 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/elbv2/target_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.567855 idem-aws-3.0.3/idem_aws/tool/aws/es/
+-rw-r--r--   0 root         (0) root         (0)     9741 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/es/elasticsearch_domain.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/es/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.567855 idem-aws-3.0.3/idem_aws/tool/aws/events/
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/events/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7407 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/events/rule.py
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/events/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.567855 idem-aws-3.0.3/idem_aws/tool/aws/guardduty/
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/guardduty/config_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/guardduty/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7045 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/guardduty/detector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.567855 idem-aws-3.0.3/idem_aws/tool/aws/iam/
+-rw-r--r--   0 root         (0) root         (0)    12684 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/iam/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/iam/group.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/iam/group_membership.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/iam/password_policy.py
+-rw-r--r--   0 root         (0) root         (0)     7466 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/iam/policy.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/iam/role_policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/iam/service_linked_role.py
+-rw-r--r--   0 root         (0) root         (0)     3720 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/iam/user.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/iam/user_ssh_key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.567855 idem-aws-3.0.3/idem_aws/tool/aws/kinesis/
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/kinesis/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    21390 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/kinesis/stream.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/kinesis/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.567855 idem-aws-3.0.3/idem_aws/tool/aws/kms/
+-rw-r--r--   0 root         (0) root         (0)      999 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/kms/alias.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/kms/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/kms/key.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/kms/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.567855 idem-aws-3.0.3/idem_aws/tool/aws/lambda_aws/
+-rw-r--r--   0 root         (0) root         (0)     3194 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/lambda_aws/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    16057 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/lambda_aws/function.py
+-rw-r--r--   0 root         (0) root         (0)     4274 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/lambda_aws/function_event_invoke_config.py
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/lambda_aws/function_permission.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/lambda_aws/function_provisioned_concurrency_config.py
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/lambda_aws/init.py
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/lambda_aws/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.567855 idem-aws-3.0.3/idem_aws/tool/aws/logs/
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/logs/subscription_filter_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.567855 idem-aws-3.0.3/idem_aws/tool/aws/neptune/
+-rw-r--r--   0 root         (0) root         (0)     8991 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/neptune/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12251 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/neptune/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     6385 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/neptune/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    11654 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/neptune/db_instance.py
+-rw-r--r--   0 root         (0) root         (0)     6128 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/neptune/db_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/neptune/db_subnet_group.py
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/neptune/tag.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/network_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.567855 idem-aws-3.0.3/idem_aws/tool/aws/organizations/
+-rw-r--r--   0 root         (0) root         (0)     1793 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/organizations/account.py
+-rw-r--r--   0 root         (0) root         (0)     4916 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/organizations/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/organizations/policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     2704 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/organizations/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.567855 idem-aws-3.0.3/idem_aws/tool/aws/rds/
+-rw-r--r--   0 root         (0) root         (0)    12718 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/rds/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5582 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/rds/parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.571854 idem-aws-3.0.3/idem_aws/tool/aws/route53/
+-rw-r--r--   0 root         (0) root         (0)     5018 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/route53/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/route53/hosted_zone_association.py
+-rw-r--r--   0 root         (0) root         (0)     5900 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/route53/hosted_zone_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7422 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/route53/resource_record_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2663 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/route53/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.571854 idem-aws-3.0.3/idem_aws/tool/aws/s3/
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/s3/bucket_acl.py
+-rw-r--r--   0 root         (0) root         (0)     7925 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/s3/bucket_encryption.py
+-rw-r--r--   0 root         (0) root         (0)     7403 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/s3/bucket_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/s3/bucket_logging.py
+-rw-r--r--   0 root         (0) root         (0)     2584 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/s3/bucket_replication.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/s3/bucket_versioning.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/s3/bucket_website.py
+-rw-r--r--   0 root         (0) root         (0)     9894 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/s3/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3373 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/s3/s3_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/search_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.571854 idem-aws-3.0.3/idem_aws/tool/aws/ses/
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/ses/conversion_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.571854 idem-aws-3.0.3/idem_aws/tool/aws/sesv2/
+-rw-r--r--   0 root         (0) root         (0)      563 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/sesv2/conversion_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.571854 idem-aws-3.0.3/idem_aws/tool/aws/sns/
+-rw-r--r--   0 root         (0) root         (0)     3275 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/sns/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7581 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/sns/sns_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.571854 idem-aws-3.0.3/idem_aws/tool/aws/sqs/
+-rw-r--r--   0 root         (0) root         (0)     6482 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/sqs/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/sqs/queue_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3723 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/state_comparison_utils.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/state_utils.py
+-rw-r--r--   0 root         (0) root         (0)      526 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/string_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5900 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/tag_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/test_state_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.571854 idem-aws-3.0.3/idem_aws/tool/aws/wafv2/
+-rw-r--r--   0 root         (0) root         (0)     6843 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/wafv2/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3076 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/wafv2/ip_set_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/wafv2/regex_pattern_set.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/wafv2/tag.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/wafv2/web_acl.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/aws/waiter_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.571854 idem-aws-3.0.3/idem_aws/tool/boto3/
+-rw-r--r--   0 root         (0) root         (0)     5478 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/boto3/client.py
+-rw-r--r--   0 root         (0) root         (0)     5181 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/boto3/custom_waiter.py
+-rw-r--r--   0 root         (0) root         (0)      429 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/boto3/exception.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/boto3/region.py
+-rw-r--r--   0 root         (0) root         (0)     6270 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/boto3/resolve.py
+-rw-r--r--   0 root         (0) root         (0)     5230 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/boto3/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/boto3/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.571854 idem-aws-3.0.3/idem_aws/tool/heist/
+-rw-r--r--   0 root         (0) root         (0)      906 2023-07-28 19:34:42.000000 idem-aws-3.0.3/idem_aws/tool/heist/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-28 19:34:55.000000 idem-aws-3.0.3/idem_aws/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:34:56.527854 idem-aws-3.0.3/idem_aws.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11104 2023-07-28 19:34:56.000000 idem-aws-3.0.3/idem_aws.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    22681 2023-07-28 19:34:56.000000 idem-aws-3.0.3/idem_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 19:34:56.000000 idem-aws-3.0.3/idem_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      580 2023-07-28 19:34:56.000000 idem-aws-3.0.3/idem_aws.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-28 19:34:56.000000 idem-aws-3.0.3/idem_aws.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      366 2023-07-28 19:34:42.000000 idem-aws-3.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 19:34:56.571854 idem-aws-3.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-07-28 19:34:42.000000 idem-aws-3.0.3/setup.py
```

### Comparing `idem-aws-3.0.2/LICENSE` & `idem-aws-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/PKG-INFO` & `idem-aws-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-aws
-Version: 3.0.2
+Version: 3.0.3
 Summary: AWS Cloud Provider for Idem
 Home-page: https://docs.idemproject.io/idem-aws/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-aws
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-aws/-/issues
```

### Comparing `idem-aws-3.0.2/README.rst` & `idem-aws-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/acct/aws/contracts/init.py` & `idem-aws-3.0.3/idem_aws/acct/aws/contracts/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/acct/aws/gsuite.py` & `idem-aws-3.0.3/idem_aws/acct/aws/gsuite.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/acct/aws/iam.py` & `idem-aws-3.0.3/idem_aws/acct/aws/iam.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/acct/aws/init.py` & `idem-aws-3.0.3/idem_aws/acct/aws/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/acct/metadata/aws.py` & `idem-aws-3.0.3/idem_aws/acct/metadata/aws.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/autogen/aws/function.py` & `idem-aws-3.0.3/idem_aws/autogen/aws/function.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/autogen/aws/init.py` & `idem-aws-3.0.3/idem_aws/autogen/aws/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/autogen/aws/known_params.py` & `idem-aws-3.0.3/idem_aws/autogen/aws/known_params.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/autogen/aws/param.py` & `idem-aws-3.0.3/idem_aws/autogen/aws/param.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/autogen/aws/plugin.py` & `idem-aws-3.0.3/idem_aws/autogen/aws/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,29 +23,46 @@
             "from dataclasses import field",
             "from dataclasses import make_dataclass",
             "from dict_tools import differ",
             "from typing import List",
             "from typing import Any",
             "from typing import Dict",
         ],
-        "functions": NamespaceDict(
-            get=hub.pop_create.aws.plugin.generate_get(shared_resource_data),
-            list=hub.pop_create.aws.plugin.generate_list(shared_resource_data),
-            create=hub.pop_create.aws.plugin.generate_present(shared_resource_data),
-            update=hub.pop_create.aws.plugin.generate_update(shared_resource_data),
-            delete=hub.pop_create.aws.plugin.generate_absent(shared_resource_data),
-            present=hub.pop_create.aws.plugin.generate_present(shared_resource_data),
-            absent=hub.pop_create.aws.plugin.generate_absent(shared_resource_data),
-            describe=hub.pop_create.aws.plugin.generate_list(shared_resource_data),
-            convert_raw_resource_to_present_async=hub.pop_create.aws.plugin.generate_convert_raw_to_present(
-                shared_resource_data.get("resource_name"), shared_resource_data["get"]
-            ),
-        ),
+        "functions": NamespaceDict(),
     }
 
+    get = hub.pop_create.aws.plugin.generate_get(shared_resource_data)
+    if get:
+        plugin["functions"]["get"] = get
+
+    list_ = hub.pop_create.aws.plugin.generate_list(shared_resource_data)
+    if list_:
+        plugin["functions"]["list"] = list_
+        plugin["functions"]["describe"] = list_
+
+    create = hub.pop_create.aws.plugin.generate_present(shared_resource_data)
+    if create:
+        plugin["functions"]["create"] = create
+        plugin["functions"]["present"] = create
+
+    delete = hub.pop_create.aws.plugin.generate_absent(shared_resource_data)
+    if delete:
+        plugin["functions"]["delete"] = delete
+        plugin["functions"]["absent"] = delete
+
+    update = hub.pop_create.aws.plugin.generate_update(shared_resource_data)
+    if update:
+        plugin["functions"]["update"] = update
+
+    plugin["functions"][
+        "convert_raw_resource_to_present_async"
+    ] = hub.pop_create.aws.plugin.generate_convert_raw_to_present(
+        shared_resource_data.get("resource_name"), shared_resource_data["get"]
+    )
+
     # Add all tests functions
     plugin = hub.pop_create.aws.plugin.add_tests_functions(plugin)
 
     return plugin
 
 
 def create_tags_plugin(
@@ -75,38 +92,44 @@
     }
 
     return plugin
 
 
 def generate_get(hub, shared_resource_data):
     get_function_definition = shared_resource_data.get("get", {})
+    if not get_function_definition:
+        return {}
     params = get_function_definition.get("params", {})
     return {
         "doc": f"\n{get_function_definition.get('doc', '')}",
         "params": params,
         "hardcoded": dict(
             **get_function_definition.get("hardcoded", {}),
         ),
     }
 
 
 def generate_list(hub, shared_resource_data):
     describe_function_definition = shared_resource_data.get("list", {})
+    if not describe_function_definition:
+        return {}
     params = describe_function_definition.get("params", {})
     return {
         "doc": f"{describe_function_definition.get('doc', '')}",
         "params": params,
         "hardcoded": dict(
             **describe_function_definition.get("hardcoded", {}),
         ),
     }
 
 
 def generate_update(hub, shared_resource_data):
     update_function_definition = shared_resource_data.get("update", {})
+    if not update_function_definition:
+        return {}
     params = update_function_definition.get("params", {})
     if "Name" in params:
         # it gets added by default in header params by pop-create
         params.pop("Name")
     if "tags" not in params.keys():
         params["tags"] = hub.pop_create.aws.known_params.TAGS_PARAMETER.copy()
     return {
@@ -116,14 +139,16 @@
             **update_function_definition.get("hardcoded", {}),
         ),
     }
 
 
 def generate_present(hub, shared_resource_data):
     create_function_definition = shared_resource_data.get("create", {})
+    if not create_function_definition:
+        return {}
     params = create_function_definition.get("params", {})
     if "Name" in params:
         # it gets added by default in header params by pop-create
         params.pop("Name")
 
     if "Tags" not in params.keys():
         params["tags"] = hub.pop_create.aws.known_params.TAGS_PARAMETER.copy()
@@ -134,25 +159,29 @@
             **create_function_definition.get("hardcoded", {}),
         ),
     }
 
 
 def generate_absent(hub, shared_resource_data):
     delete_function_definition = shared_resource_data.get("delete", {})
+    if not delete_function_definition:
+        return {}
     return {
         "doc": f"{delete_function_definition.get('doc', '')}",
         "params": delete_function_definition.get("params", {}),
         "hardcoded": dict(
             **delete_function_definition.get("hardcoded", {}),
         ),
     }
 
 
 def generate_get_tags_for_resource(hub, tag_functions):
     list_tags_function_definition = tag_functions.get("list_tags", {})
+    if not list_tags_function_definition:
+        return {}
     return {
         "doc": f"Get tags for a given resource.\n",
         "params": dict(
             resource_id=hub.pop_create.aws.known_params.RESOURCE_ID_PARAMETER.copy(),
         ),
         "hardcoded": dict(
             **list_tags_function_definition.get("hardcoded", {}),
@@ -186,26 +215,26 @@
                 old_tags=hub.pop_create.aws.known_params.OLD_TAGS_PARAMETER.copy(),
                 new_tags=hub.pop_create.aws.known_params.NEW_TAGS_PARAMETER.copy(),
             ),
             "hardcoded": dict(
                 untag_resource_boto3_function=untag_resource_function_definition.get(
                     "hardcoded", {}
                 ).get("boto3_function"),
-                untag_resource_input_params=untag_resource_function_definition.get(
-                    "params", {}
-                ).keys(),
+                untag_resource_input_params=list(
+                    untag_resource_function_definition.get("params", {}).keys()
+                ),
                 untag_resource_documentation=untag_resource_function_definition.get(
                     "hardcoded", {}
                 ).get("boto3_documentation"),
                 tag_resource_boto3_function=tag_resource_function_definition.get(
                     "hardcoded", {}
                 ).get("boto3_function"),
-                tag_resource_input_params=tag_resource_function_definition.get(
-                    "params", {}
-                ).keys(),
+                tag_resource_input_params=list(
+                    tag_resource_function_definition.get("params", {}).keys()
+                ),
                 tag_resource_documentation=tag_resource_function_definition.get(
                     "hardcoded", {}
                 ).get("boto3_documentation"),
                 single_update=False,
             ),
         }
```

### Comparing `idem-aws-3.0.2/idem_aws/autogen/aws/possible_functions.py` & `idem-aws-3.0.3/idem_aws/autogen/aws/possible_functions.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/autogen/aws/resource.py` & `idem-aws-3.0.3/idem_aws/autogen/aws/resource.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/autogen/aws/service.py` & `idem-aws-3.0.3/idem_aws/autogen/aws/service.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/conf.py` & `idem-aws-3.0.3/idem_aws/conf.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/esm/aws.py` & `idem-aws-3.0.3/idem_aws/esm/aws.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/esm/contracts/aws.py` & `idem-aws-3.0.3/idem_aws/esm/contracts/aws.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/acm/certificate_manager.py` & `idem-aws-3.0.3/idem_aws/exec/aws/acm/certificate_manager.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/apigateway/base_path_mapping.py` & `idem-aws-3.0.3/idem_aws/exec/aws/apigateway/base_path_mapping.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/apigateway/deployment.py` & `idem-aws-3.0.3/idem_aws/exec/aws/apigateway/deployment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/apigateway/domain_name.py` & `idem-aws-3.0.3/idem_aws/exec/aws/apigateway/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/apigateway/integration.py` & `idem-aws-3.0.3/idem_aws/exec/aws/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/apigateway/integration_response.py` & `idem-aws-3.0.3/idem_aws/exec/aws/apigateway/integration_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/apigateway/method.py` & `idem-aws-3.0.3/idem_aws/exec/aws/apigateway/method.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/apigateway/method_response.py` & `idem-aws-3.0.3/idem_aws/exec/aws/apigateway/method_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/apigateway/resource.py` & `idem-aws-3.0.3/idem_aws/exec/aws/apigateway/resource.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/apigateway/rest_api.py` & `idem-aws-3.0.3/idem_aws/exec/aws/apigateway/rest_api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/apigateway/stage.py` & `idem-aws-3.0.3/idem_aws/exec/aws/apigateway/stage.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/apigatewayv2/api.py` & `idem-aws-3.0.3/idem_aws/exec/aws/apigatewayv2/api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/apigatewayv2/authorizer.py` & `idem-aws-3.0.3/idem_aws/exec/aws/apigatewayv2/authorizer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/apigatewayv2/domain_name.py` & `idem-aws-3.0.3/idem_aws/exec/aws/apigatewayv2/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/apigatewayv2/integration.py` & `idem-aws-3.0.3/idem_aws/exec/aws/apigatewayv2/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/apigatewayv2/route.py` & `idem-aws-3.0.3/idem_aws/exec/aws/apigatewayv2/route.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/application_autoscaling/scalable_target.py` & `idem-aws-3.0.3/idem_aws/exec/aws/application_autoscaling/scalable_target.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/application_autoscaling/scaling_policy.py` & `idem-aws-3.0.3/idem_aws/exec/aws/application_autoscaling/scaling_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/arn.py` & `idem-aws-3.0.3/idem_aws/exec/aws/arn.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/autoscaling/scaling_policy.py` & `idem-aws-3.0.3/idem_aws/exec/aws/autoscaling/scaling_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/backup/backup_vault.py` & `idem-aws-3.0.3/idem_aws/exec/aws/backup/backup_vault.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/budgets/budget.py` & `idem-aws-3.0.3/idem_aws/exec/aws/budgets/budget.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/cloudformation/stack.py` & `idem-aws-3.0.3/idem_aws/exec/aws/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/cloudfront/cache_policy.py` & `idem-aws-3.0.3/idem_aws/exec/aws/cloudfront/cache_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/cloudfront/distribution.py` & `idem-aws-3.0.3/idem_aws/exec/aws/cloudfront/distribution.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/cloudfront/origin_request_policy.py` & `idem-aws-3.0.3/idem_aws/exec/aws/cloudfront/origin_request_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/cloudwatch/log_group.py` & `idem-aws-3.0.3/idem_aws/exec/aws/cloudwatch/log_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/cloudwatchlogs/resource_policy.py` & `idem-aws-3.0.3/idem_aws/exec/aws/cloudwatchlogs/resource_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/config/configuration_aggregator.py` & `idem-aws-3.0.3/idem_aws/exec/aws/config/configuration_aggregator.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/costexplorer/cost_allocation_tag.py` & `idem-aws-3.0.3/idem_aws/exec/aws/costexplorer/cost_allocation_tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/data.py` & `idem-aws-3.0.3/idem_aws/exec/aws/data.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/docdb/db_cluster.py` & `idem-aws-3.0.3/idem_aws/exec/aws/docdb/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/docdb/db_cluster_parameter_group.py` & `idem-aws-3.0.3/idem_aws/exec/aws/docdb/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/docdb/db_subnet_group.py` & `idem-aws-3.0.3/idem_aws/exec/aws/docdb/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/dynamodb/table.py` & `idem-aws-3.0.3/idem_aws/exec/aws/dynamodb/table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/dynamodb/tag.py` & `idem-aws-3.0.3/idem_aws/exec/aws/dynamodb/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/ami.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/ami.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/availability_zones.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/availability_zones.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/elastic_ip.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/elastic_ip.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/flow_log.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/flow_log.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/instance.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/instance_type.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/instance_type.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/internet_gateway.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/internet_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/key_pair.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/key_pair.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/launch_template.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/launch_template.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/network_interface.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/network_interface.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/placement_group.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/placement_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/route.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/route.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/route_table.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/route_table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/route_table_association.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/route_table_association.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/security_group.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/security_group_rule.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/security_group_rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/snapshot.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/snapshot.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/spot_instance_request.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/spot_instance_request.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/subnet.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/volume.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/vpc.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/vpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Exec module for managing EC2 Virtual Private Gateways."""
 from typing import Dict
 from typing import List
 
 __func_alias__ = {"list_": "list"}
 
 
 async def get(
@@ -18,18 +19,18 @@
     Args:
         name (str):
             The name of the Idem state
 
         resource_id (str, Optional):
             ID of the VPC
 
-        default(bool, Optional):
+        default (bool, Optional):
             Indicate whether the VPC is the default VPC
 
-        filters(list, Optional):
+        filters (list[str], Optional):
             One or more filters: for example, tag :<key>, tag-key. A complete list of filters can be found at
             https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_vpcs
 
     Returns:
         Dict[str, Any]:
             Returns VPC in present format
```

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/vpc_endpoint.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/vpc_endpoint.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/vpc_peering_connection.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/vpc_peering_connection_accepter.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/vpc_peering_connection_accepter.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ec2/vpc_peering_connection_options.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ec2/vpc_peering_connection_options.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ecr/image.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ecr/image.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ecr/lifecycle_policy.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ecr/lifecycle_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ecr/repository.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ecr/repository.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ecr/repository_policy.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ecr/repository_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/eks/cluster.py` & `idem-aws-3.0.3/idem_aws/exec/aws/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/elasticache/replication_group.py` & `idem-aws-3.0.3/idem_aws/exec/aws/elasticache/replication_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/elb/elb_hosted_zone_id.py` & `idem-aws-3.0.3/idem_aws/exec/aws/elb/elb_hosted_zone_id.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/elb/load_balancer.py` & `idem-aws-3.0.3/idem_aws/exec/aws/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/elbv2/listener.py` & `idem-aws-3.0.3/idem_aws/exec/aws/elbv2/listener.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/elbv2/load_balancer.py` & `idem-aws-3.0.3/idem_aws/exec/aws/elbv2/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/elbv2/target_group.py` & `idem-aws-3.0.3/idem_aws/exec/aws/elbv2/target_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/es/elasticsearch_domain.py` & `idem-aws-3.0.3/idem_aws/exec/aws/es/elasticsearch_domain.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/events/rule.py` & `idem-aws-3.0.3/idem_aws/exec/aws/events/rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/guardduty/detector.py` & `idem-aws-3.0.3/idem_aws/exec/aws/guardduty/detector.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/guardduty/member.py` & `idem-aws-3.0.3/idem_aws/exec/aws/guardduty/member.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/guardduty/organization_admin_account.py` & `idem-aws-3.0.3/idem_aws/exec/aws/guardduty/organization_admin_account.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/guardduty/organization_configuration.py` & `idem-aws-3.0.3/idem_aws/exec/aws/guardduty/organization_configuration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/iam/access_key.py` & `idem-aws-3.0.3/idem_aws/exec/aws/iam/access_key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/iam/group.py` & `idem-aws-3.0.3/idem_aws/exec/aws/iam/group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/iam/group_membership.py` & `idem-aws-3.0.3/idem_aws/exec/aws/iam/group_membership.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/iam/group_policy_attachment.py` & `idem-aws-3.0.3/idem_aws/exec/aws/iam/group_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/iam/instance_profile.py` & `idem-aws-3.0.3/idem_aws/exec/aws/iam/instance_profile.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/iam/open_id_connect_provider.py` & `idem-aws-3.0.3/idem_aws/exec/aws/iam/open_id_connect_provider.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/iam/password_policy.py` & `idem-aws-3.0.3/idem_aws/exec/aws/iam/password_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/iam/policy.py` & `idem-aws-3.0.3/idem_aws/exec/aws/iam/policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/iam/role.py` & `idem-aws-3.0.3/idem_aws/exec/aws/iam/role.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/iam/user.py` & `idem-aws-3.0.3/idem_aws/exec/aws/iam/user.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/iam/user_policy_attachment.py` & `idem-aws-3.0.3/idem_aws/exec/aws/iam/user_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/kinesis/stream.py` & `idem-aws-3.0.3/idem_aws/exec/aws/kinesis/stream.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/kms/key.py` & `idem-aws-3.0.3/idem_aws/exec/aws/kms/key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/lambda_aws/function_event_invoke_config.py` & `idem-aws-3.0.3/idem_aws/exec/aws/lambda_aws/function_event_invoke_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/lambda_aws/function_provisioned_concurrency_config.py` & `idem-aws-3.0.3/idem_aws/exec/aws/lambda_aws/function_provisioned_concurrency_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/neptune/db_cluster_parameter_group.py` & `idem-aws-3.0.3/idem_aws/exec/aws/neptune/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/neptune/db_instance.py` & `idem-aws-3.0.3/idem_aws/exec/aws/neptune/db_instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/neptune/db_parameter_group.py` & `idem-aws-3.0.3/idem_aws/exec/aws/neptune/db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/organizations/account.py` & `idem-aws-3.0.3/idem_aws/exec/aws/organizations/account.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/organizations/policy.py` & `idem-aws-3.0.3/idem_aws/exec/aws/organizations/policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/rds/db_cluster.py` & `idem-aws-3.0.3/idem_aws/exec/aws/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/rds/db_cluster_parameter_group.py` & `idem-aws-3.0.3/idem_aws/exec/aws/rds/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/rds/db_instance.py` & `idem-aws-3.0.3/idem_aws/exec/aws/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/rds/db_parameter_group.py` & `idem-aws-3.0.3/idem_aws/exec/aws/rds/db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/rds/db_subnet_group.py` & `idem-aws-3.0.3/idem_aws/exec/aws/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/rds/tag.py` & `idem-aws-3.0.3/idem_aws/exec/aws/rds/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/route53/hosted_zone.py` & `idem-aws-3.0.3/idem_aws/exec/aws/route53/hosted_zone.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/s3/bucket.py` & `idem-aws-3.0.3/idem_aws/exec/aws/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/s3/bucket_acl.py` & `idem-aws-3.0.3/idem_aws/exec/aws/s3/bucket_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/s3/bucket_lifecycle.py` & `idem-aws-3.0.3/idem_aws/exec/aws/s3/bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/s3/bucket_logging.py` & `idem-aws-3.0.3/idem_aws/exec/aws/s3/bucket_logging.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/s3/bucket_replication.py` & `idem-aws-3.0.3/idem_aws/exec/aws/s3/bucket_replication.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/s3/bucket_website.py` & `idem-aws-3.0.3/idem_aws/exec/aws/s3/bucket_website.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ses/domain_identity.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ses/domain_identity.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/ses/identity_notification_topic.py` & `idem-aws-3.0.3/idem_aws/exec/aws/ses/identity_notification_topic.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/sesv2/event_destination.py` & `idem-aws-3.0.3/idem_aws/exec/aws/sesv2/event_destination.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/sns/subscription.py` & `idem-aws-3.0.3/idem_aws/exec/aws/sns/subscription.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/sqs/queue.py` & `idem-aws-3.0.3/idem_aws/exec/aws/sqs/queue.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/sts/assume_role.py` & `idem-aws-3.0.3/idem_aws/exec/aws/sts/assume_role.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/sts/caller_identity.py` & `idem-aws-3.0.3/idem_aws/exec/aws/sts/caller_identity.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/wafv2/ip_set.py` & `idem-aws-3.0.3/idem_aws/exec/aws/wafv2/ip_set.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/aws/wafv2/regex_pattern_set.py` & `idem-aws-3.0.3/idem_aws/exec/aws/wafv2/regex_pattern_set.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/exec/boto3/init.py` & `idem-aws-3.0.3/idem_aws/exec/boto3/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/reconcile/pending/aws.py` & `idem-aws-3.0.3/idem_aws/reconcile/pending/aws.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/acm/certificate_manager.py` & `idem-aws-3.0.3/idem_aws/states/aws/acm/certificate_manager.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/acm/certificate_validation.py` & `idem-aws-3.0.3/idem_aws/states/aws/acm/certificate_validation.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/apigateway/base_path_mapping.py` & `idem-aws-3.0.3/idem_aws/states/aws/apigateway/base_path_mapping.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/apigateway/deployment.py` & `idem-aws-3.0.3/idem_aws/states/aws/apigateway/deployment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/apigateway/domain_name.py` & `idem-aws-3.0.3/idem_aws/states/aws/apigateway/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/apigateway/integration.py` & `idem-aws-3.0.3/idem_aws/states/aws/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/apigateway/integration_response.py` & `idem-aws-3.0.3/idem_aws/states/aws/apigateway/integration_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/apigateway/method.py` & `idem-aws-3.0.3/idem_aws/states/aws/apigateway/method.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/apigateway/method_response.py` & `idem-aws-3.0.3/idem_aws/states/aws/apigateway/method_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/apigateway/resource.py` & `idem-aws-3.0.3/idem_aws/states/aws/apigateway/resource.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/apigateway/rest_api.py` & `idem-aws-3.0.3/idem_aws/states/aws/apigateway/rest_api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/apigateway/stage.py` & `idem-aws-3.0.3/idem_aws/states/aws/apigateway/stage.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/apigatewayv2/api.py` & `idem-aws-3.0.3/idem_aws/states/aws/apigatewayv2/api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/apigatewayv2/authorizer.py` & `idem-aws-3.0.3/idem_aws/states/aws/apigatewayv2/authorizer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/apigatewayv2/domain_name.py` & `idem-aws-3.0.3/idem_aws/states/aws/apigatewayv2/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/apigatewayv2/integration.py` & `idem-aws-3.0.3/idem_aws/states/aws/apigatewayv2/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/apigatewayv2/route.py` & `idem-aws-3.0.3/idem_aws/states/aws/apigatewayv2/route.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/apigatewayv2/stage.py` & `idem-aws-3.0.3/idem_aws/states/aws/apigatewayv2/stage.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/application_autoscaling/scalable_target.py` & `idem-aws-3.0.3/idem_aws/states/aws/application_autoscaling/scalable_target.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/application_autoscaling/scaling_policy.py` & `idem-aws-3.0.3/idem_aws/states/aws/application_autoscaling/scaling_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/autoscaling/auto_scaling_group.py` & `idem-aws-3.0.3/idem_aws/states/aws/autoscaling/auto_scaling_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/autoscaling/launch_configuration.py` & `idem-aws-3.0.3/idem_aws/states/aws/autoscaling/launch_configuration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/autoscaling/scaling_policy.py` & `idem-aws-3.0.3/idem_aws/states/aws/autoscaling/scaling_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/backup/backup_vault.py` & `idem-aws-3.0.3/idem_aws/states/aws/backup/backup_vault.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/budgets/budget.py` & `idem-aws-3.0.3/idem_aws/states/aws/budgets/budget.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/budgets/budget_action.py` & `idem-aws-3.0.3/idem_aws/states/aws/budgets/budget_action.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/caller_identity.py` & `idem-aws-3.0.3/idem_aws/states/aws/caller_identity.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/cloudformation/stack.py` & `idem-aws-3.0.3/idem_aws/states/aws/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/cloudfront/cache_policy.py` & `idem-aws-3.0.3/idem_aws/states/aws/cloudfront/cache_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/cloudfront/distribution.py` & `idem-aws-3.0.3/idem_aws/states/aws/cloudfront/distribution.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/cloudfront/origin_request_policy.py` & `idem-aws-3.0.3/idem_aws/states/aws/cloudfront/origin_request_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/cloudtrail/trail.py` & `idem-aws-3.0.3/idem_aws/states/aws/cloudtrail/trail.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/cloudwatch/log_group.py` & `idem-aws-3.0.3/idem_aws/states/aws/cloudwatch/log_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/cloudwatch/metric_alarm.py` & `idem-aws-3.0.3/idem_aws/states/aws/cloudwatch/metric_alarm.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/cloudwatchlogs/resource_policy.py` & `idem-aws-3.0.3/idem_aws/states/aws/cloudwatchlogs/resource_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/config/config_recorder.py` & `idem-aws-3.0.3/idem_aws/states/aws/config/config_recorder.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/config/config_recorder_status.py` & `idem-aws-3.0.3/idem_aws/states/aws/config/config_recorder_status.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/config/configuration_aggregator.py` & `idem-aws-3.0.3/idem_aws/states/aws/config/configuration_aggregator.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/config/delivery_channel.py` & `idem-aws-3.0.3/idem_aws/states/aws/config/delivery_channel.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/config/rule.py` & `idem-aws-3.0.3/idem_aws/states/aws/config/rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/costexplorer/anomaly_monitor.py` & `idem-aws-3.0.3/idem_aws/states/aws/costexplorer/anomaly_monitor.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/costexplorer/anomaly_subscription.py` & `idem-aws-3.0.3/idem_aws/states/aws/costexplorer/anomaly_subscription.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/costexplorer/cost_category.py` & `idem-aws-3.0.3/idem_aws/states/aws/costexplorer/cost_category.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/data.py` & `idem-aws-3.0.3/idem_aws/states/aws/data.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/docdb/db_cluster.py` & `idem-aws-3.0.3/idem_aws/states/aws/docdb/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/docdb/db_cluster_parameter_group.py` & `idem-aws-3.0.3/idem_aws/states/aws/docdb/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/docdb/db_subnet_group.py` & `idem-aws-3.0.3/idem_aws/states/aws/docdb/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/dynamodb/table.py` & `idem-aws-3.0.3/idem_aws/states/aws/dynamodb/table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/ami.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/ami.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/dhcp_option.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/dhcp_option.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/dhcp_option_association.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/dhcp_option_association.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/elastic_ip.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/elastic_ip.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/flow_log.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/flow_log.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/instance.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/internet_gateway.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/internet_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/key_pair.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/key_pair.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/launch_template.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/launch_template.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/nat_gateway.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/nat_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/network_interface.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/network_interface.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/placement_group.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/placement_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/route.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/route.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/route_table.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/route_table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/route_table_association.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/route_table_association.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/security_group.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/security_group_rule.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/security_group_rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/snapshot.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/snapshot.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/spot_instance_request.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/spot_instance_request.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/subnet.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/transit_gateway.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/transit_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/transit_gateway_vpc_attachment.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/volume.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/vpc.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/vpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,8 @@
-"""
-Autogenerated state module using `pop-create-idem <https://gitlab.com/saltstack/pop/pop-create-idem>`__
-
-hub.exec.boto3.client.ec2.create_vpc
-hub.exec.boto3.client.ec2.delete_vpc
-hub.exec.boto3.client.ec2.describe_vpcs
-resource = await hub.tool.boto3.resource.create(ctx, "ec2", "Vpc", name)
-hub.tool.boto3.resource.exec(resource, associate_dhcp_options, *args, **kwargs)
-hub.tool.boto3.resource.exec(resource, attach_classic_link_instance, *args, **kwargs)
-hub.tool.boto3.resource.exec(resource, attach_internet_gateway, *args, **kwargs)
-hub.tool.boto3.resource.exec(resource, create_network_acl, *args, **kwargs)
-hub.tool.boto3.resource.exec(resource, create_route_table, *args, **kwargs)
-hub.tool.boto3.resource.exec(resource, create_security_group, *args, **kwargs)
-hub.tool.boto3.resource.exec(resource, create_subnet, *args, **kwargs)
-hub.tool.boto3.resource.exec(resource, create_tags, *args, **kwargs)
-hub.tool.boto3.resource.exec(resource, delete, *args, **kwargs)
-hub.tool.boto3.resource.exec(resource, describe_attribute, *args, **kwargs)
-hub.tool.boto3.resource.exec(resource, detach_classic_link_instance, *args, **kwargs)
-hub.tool.boto3.resource.exec(resource, detach_internet_gateway, *args, **kwargs)
-hub.tool.boto3.resource.exec(resource, disable_classic_link, *args, **kwargs)
-hub.tool.boto3.resource.exec(resource, enable_classic_link, *args, **kwargs)
-hub.tool.boto3.resource.exec(resource, modify_attribute, *args, **kwargs)
-hub.tool.boto3.resource.exec(resource, request_vpc_peering_connection, *args, **kwargs)
-"""
+"""State module for managing EC2 Virtual Private Gateways."""
 import copy
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
@@ -72,63 +49,61 @@
     or List[
         make_dataclass("Tag", [("Key", str), ("Value", str, field(default=None))])
     ] = None,
     enable_dns_hostnames: bool = None,
     enable_dns_support: bool = None,
 ) -> Dict[str, Any]:
     """
-    **Autogenerated function**
-
     Creates a VPC with the specified IPv4 CIDR block. The smallest VPC you can create uses a /28 netmask (16 IPv4
     addresses), and the largest uses a /16 netmask (65,536 IPv4 addresses). For more information about how large to
     make your VPC, see Your VPC and subnets in the Amazon Virtual Private Cloud User Guide. You can optionally
     request an IPv6 CIDR block for the VPC. You can request an Amazon-provided IPv6 CIDR block from Amazon's pool of
     IPv6 addresses, or an IPv6 CIDR block from an IPv6 address pool that you provisioned through bring your own IP
     addresses (BYOIP). By default, each instance you launch in the VPC has the default DHCP options, which include
     only a default DNS server that we provide (AmazonProvidedDNS). For more information, see DHCP options sets in
     the Amazon Virtual Private Cloud User Guide. You can specify the instance tenancy value for the VPC when you
     create it. You can't change this value for the VPC after you create it. For more information, see Dedicated
     Instances in the Amazon Elastic Compute Cloud User Guide.
 
     Args:
-        name(str): An Idem name of the resource.
-        resource_id(str): AWS VPC ID
+        name (str): An Idem name of the resource.
+        resource_id (str, Optional): AWS VPC ID
         cidr_block_association_set(List, Optional): Information about the IPv4 CIDR blocks associated with the VPC.
             Defaults to None.
             * CidrBlock (str) -- An IPv4 CIDR block to associate with the VPC.
             * Ipv4IpamPoolId (str) -- Associate a CIDR allocated from an IPv4 IPAM pool to a VPC.
             * Ipv4NetmaskLength (int) -- The netmask length of the IPv4 CIDR you would like to associate from an Amazon VPC IP Address Manager (IPAM) pool.
-        ipv6_cidr_block_association_set(List, Optional): Information about the IPv6 CIDR blocks associated with the VPC.
+        ipv6_cidr_block_association_set (List, Optional): Information about the IPv6 CIDR blocks associated with the VPC.
             Defaults to None.
             * Ipv6CidrBlock (str) -- An IPv6 CIDR block from the IPv6 address pool. You must also specify Ipv6Pool in the request.
             * Ipv6IpamPoolId (str) -- Associates a CIDR allocated from an IPv6 IPAM pool to a VPC.
             * Ipv6NetmaskLength (int) -- The netmask length of the IPv6 CIDR you would like to associate from an
                 Amazon VPC IP Address Manager (IPAM) pool.
             * Ipv6CidrBlockNetworkBorderGroup (str) -- The name of the location from which we advertise the IPV6 CIDR
                 block. Use this parameter to limit the CIDR block to this location. You must set AmazonProvidedIpv6CidrBlock
                 to true to use this parameter. You can have one IPv6 CIDR block association per network border group.
             * AmazonProvidedIpv6CidrBlock (boolean) -- Requests an Amazon-provided IPv6 CIDR block with a /56 prefix
                 length for the VPC. You cannot specify the range of IPv6 addresses, or the size of the CIDR block.
-        instance_tenancy(str, Optional): The tenancy options for instances launched into the VPC. For default, instances are launched
+        instance_tenancy (str, Optional): The tenancy options for instances launched into the VPC. For default, instances are launched
             with shared tenancy by default. You can launch instances with any tenancy into a shared tenancy
             VPC. For dedicated, instances are launched as dedicated tenancy instances by default. You can
             only launch instances with a tenancy of dedicated or host into a dedicated tenancy VPC.
             Important: The host value cannot be used with this parameter. Use the default or dedicated
             values only. Default: default. Defaults to None.
-        tags(Dict or List, Optional): Dict in the format of {tag-key: tag-value} or List of tags in the format of
+        tags (Dict or List, Optional): Dict in the format of {tag-key: tag-value} or List of tags in the format of
             [{"Key": tag-key, "Value": tag-value}] to associate with the VPC.
             Each tag consists of a key name and an associated value. Defaults to None.
             * Key (str, Optional): The key of the tag. Constraints: Tag keys are case-sensitive and accept a maximum of 127 Unicode
                 characters. May not begin with aws:.
             * Value(str, Optional): The value of the tag. Constraints: Tag values are case-sensitive and accept a maximum of 256
                 Unicode characters.
-        enable_dns_hostnames(bool, Optional): Indicates whether the instances launched in the VPC get DNS hostnames. If enabled, instances
+        enable_dns_hostnames (bool, Optional): Indicates whether the instances launched in the VPC get DNS hostnames. If enabled, instances
             in the VPC get DNS hostnames; otherwise, they do not. You cannot modify the DNS resolution and DNS hostnames attributes in the same request.
             Use separate requests for each attribute. You can only enable DNS hostnames if you've enabled DNS support.
-        enable_dns_support(bool, Optional): Indicates whether the DNS resolution is supported for the VPC. If enabled, queries to the Amazon provided
+        enable_dns_support (bool, Optional): Indicates whether the DNS resolution is supported for the VPC. If enabled, queries to the Amazon provided
             DNS server at the 169.254.169.253 IP address, or the reserved IP address at the base of the VPC network range "plus two" succeed. If disabled,
             the Amazon provided DNS service in the VPC that resolves public DNS hostnames to IP addresses is not enabled. You cannot modify the DNS resolution
             and DNS hostnames attributes in the same request. Use separate requests for each attribute.
 
     Request Syntax:
         [vpc-resource-id]:
           aws.ec2.vpc.present:
```

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/vpc_endpoint.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/vpc_endpoint.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/vpc_peering_connection.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/vpc_peering_connection_accepter.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/vpc_peering_connection_accepter.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ec2/vpc_peering_connection_options.py` & `idem-aws-3.0.3/idem_aws/states/aws/ec2/vpc_peering_connection_options.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ecr/lifecycle_policy.py` & `idem-aws-3.0.3/idem_aws/states/aws/ecr/lifecycle_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ecr/repository.py` & `idem-aws-3.0.3/idem_aws/states/aws/ecr/repository.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ecr/repository_policy.py` & `idem-aws-3.0.3/idem_aws/states/aws/ecr/repository_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/efs/file_system.py` & `idem-aws-3.0.3/idem_aws/states/aws/efs/file_system.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/efs/mount_target.py` & `idem-aws-3.0.3/idem_aws/states/aws/efs/mount_target.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/eks/addon.py` & `idem-aws-3.0.3/idem_aws/states/aws/eks/addon.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/eks/cluster.py` & `idem-aws-3.0.3/idem_aws/states/aws/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/eks/fargate_profile.py` & `idem-aws-3.0.3/idem_aws/states/aws/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/eks/nodegroup.py` & `idem-aws-3.0.3/idem_aws/states/aws/eks/nodegroup.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/elasticache/cache_parameter_group.py` & `idem-aws-3.0.3/idem_aws/states/aws/elasticache/cache_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/elasticache/cache_subnet_group.py` & `idem-aws-3.0.3/idem_aws/states/aws/elasticache/cache_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/elasticache/replication_group.py` & `idem-aws-3.0.3/idem_aws/states/aws/elasticache/replication_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/elb/load_balancer.py` & `idem-aws-3.0.3/idem_aws/states/aws/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/elbv2/listener.py` & `idem-aws-3.0.3/idem_aws/states/aws/elbv2/listener.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/elbv2/load_balancer.py` & `idem-aws-3.0.3/idem_aws/states/aws/elbv2/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/elbv2/target_group.py` & `idem-aws-3.0.3/idem_aws/states/aws/elbv2/target_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/es/elasticsearch_domain.py` & `idem-aws-3.0.3/idem_aws/states/aws/es/elasticsearch_domain.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/events/rule.py` & `idem-aws-3.0.3/idem_aws/states/aws/events/rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/guardduty/detector.py` & `idem-aws-3.0.3/idem_aws/states/aws/guardduty/detector.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/guardduty/member.py` & `idem-aws-3.0.3/idem_aws/states/aws/guardduty/member.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/guardduty/organization_admin_account.py` & `idem-aws-3.0.3/idem_aws/states/aws/guardduty/organization_admin_account.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/guardduty/organization_configuration.py` & `idem-aws-3.0.3/idem_aws/states/aws/guardduty/organization_configuration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/iam/access_key.py` & `idem-aws-3.0.3/idem_aws/states/aws/iam/access_key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/iam/group.py` & `idem-aws-3.0.3/idem_aws/states/aws/iam/group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/iam/group_membership.py` & `idem-aws-3.0.3/idem_aws/states/aws/iam/group_membership.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/iam/group_policy_attachment.py` & `idem-aws-3.0.3/idem_aws/states/aws/iam/group_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/iam/instance_profile.py` & `idem-aws-3.0.3/idem_aws/states/aws/iam/instance_profile.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/iam/open_id_connect_provider.py` & `idem-aws-3.0.3/idem_aws/states/aws/iam/open_id_connect_provider.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/iam/password_policy.py` & `idem-aws-3.0.3/idem_aws/states/aws/iam/password_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/iam/policy.py` & `idem-aws-3.0.3/idem_aws/states/aws/iam/policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/iam/role.py` & `idem-aws-3.0.3/idem_aws/states/aws/iam/role.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/iam/role_policy.py` & `idem-aws-3.0.3/idem_aws/states/aws/iam/role_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/iam/role_policy_attachment.py` & `idem-aws-3.0.3/idem_aws/states/aws/iam/role_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/iam/service_linked_role.py` & `idem-aws-3.0.3/idem_aws/states/aws/iam/service_linked_role.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/iam/user.py` & `idem-aws-3.0.3/idem_aws/states/aws/iam/user.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/iam/user_policy.py` & `idem-aws-3.0.3/idem_aws/states/aws/iam/user_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/iam/user_policy_attachment.py` & `idem-aws-3.0.3/idem_aws/states/aws/iam/user_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/iam/user_ssh_key.py` & `idem-aws-3.0.3/idem_aws/states/aws/iam/user_ssh_key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/kinesis/stream.py` & `idem-aws-3.0.3/idem_aws/states/aws/kinesis/stream.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/kms/alias.py` & `idem-aws-3.0.3/idem_aws/states/aws/kms/alias.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/kms/key.py` & `idem-aws-3.0.3/idem_aws/states/aws/kms/key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/lambda_aws/function.py` & `idem-aws-3.0.3/idem_aws/states/aws/lambda_aws/function.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/lambda_aws/function_event_invoke_config.py` & `idem-aws-3.0.3/idem_aws/states/aws/lambda_aws/function_event_invoke_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/lambda_aws/function_permission.py` & `idem-aws-3.0.3/idem_aws/states/aws/lambda_aws/function_permission.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/lambda_aws/function_provisioned_concurrency_config.py` & `idem-aws-3.0.3/idem_aws/states/aws/lambda_aws/function_provisioned_concurrency_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/logs/subscription_filter.py` & `idem-aws-3.0.3/idem_aws/states/aws/logs/subscription_filter.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/neptune/db_cluster.py` & `idem-aws-3.0.3/idem_aws/states/aws/neptune/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/neptune/db_cluster_parameter_group.py` & `idem-aws-3.0.3/idem_aws/states/aws/neptune/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/neptune/db_instance.py` & `idem-aws-3.0.3/idem_aws/states/aws/neptune/db_instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/neptune/db_parameter_group.py` & `idem-aws-3.0.3/idem_aws/states/aws/neptune/db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/neptune/db_subnet_group.py` & `idem-aws-3.0.3/idem_aws/states/aws/neptune/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/organizations/account.py` & `idem-aws-3.0.3/idem_aws/states/aws/organizations/account.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/organizations/organization.py` & `idem-aws-3.0.3/idem_aws/states/aws/organizations/organization.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/organizations/organization_unit.py` & `idem-aws-3.0.3/idem_aws/states/aws/organizations/organization_unit.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/organizations/policy.py` & `idem-aws-3.0.3/idem_aws/states/aws/organizations/policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/organizations/policy_attachment.py` & `idem-aws-3.0.3/idem_aws/states/aws/organizations/policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/rds/db_cluster.py` & `idem-aws-3.0.3/idem_aws/states/aws/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/rds/db_cluster_parameter_group.py` & `idem-aws-3.0.3/idem_aws/states/aws/rds/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/rds/db_instance.py` & `idem-aws-3.0.3/idem_aws/states/aws/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/rds/db_parameter_group.py` & `idem-aws-3.0.3/idem_aws/states/aws/rds/db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/rds/db_subnet_group.py` & `idem-aws-3.0.3/idem_aws/states/aws/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/route53/hosted_zone.py` & `idem-aws-3.0.3/idem_aws/states/aws/route53/hosted_zone.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/route53/hosted_zone_association.py` & `idem-aws-3.0.3/idem_aws/states/aws/route53/hosted_zone_association.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/route53/resource_record.py` & `idem-aws-3.0.3/idem_aws/states/aws/route53/resource_record.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/s3/bucket.py` & `idem-aws-3.0.3/idem_aws/states/aws/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_acl.py` & `idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_encryption.py` & `idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_encryption.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_lifecycle.py` & `idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_logging.py` & `idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_logging.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_notification.py` & `idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_notification.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_policy.py` & `idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_replication.py` & `idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_replication.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_versioning.py` & `idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_versioning.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/s3/bucket_website.py` & `idem-aws-3.0.3/idem_aws/states/aws/s3/bucket_website.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/s3/public_access_block.py` & `idem-aws-3.0.3/idem_aws/states/aws/s3/public_access_block.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ses/domain_identity.py` & `idem-aws-3.0.3/idem_aws/states/aws/ses/domain_identity.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/ses/identity_notification_topic.py` & `idem-aws-3.0.3/idem_aws/states/aws/ses/identity_notification_topic.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/sesv2/event_destination.py` & `idem-aws-3.0.3/idem_aws/states/aws/sesv2/event_destination.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/sns/subscription.py` & `idem-aws-3.0.3/idem_aws/states/aws/sns/subscription.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/sns/topic.py` & `idem-aws-3.0.3/idem_aws/states/aws/sns/topic.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/sns/topic_policy.py` & `idem-aws-3.0.3/idem_aws/states/aws/sns/topic_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/sqs/queue.py` & `idem-aws-3.0.3/idem_aws/states/aws/sqs/queue.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/wafv2/associate_web_acl.py` & `idem-aws-3.0.3/idem_aws/states/aws/wafv2/associate_web_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/wafv2/ip_set.py` & `idem-aws-3.0.3/idem_aws/states/aws/wafv2/ip_set.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/wafv2/regex_pattern_set.py` & `idem-aws-3.0.3/idem_aws/states/aws/wafv2/regex_pattern_set.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/states/aws/wafv2/web_acl.py` & `idem-aws-3.0.3/idem_aws/states/aws/wafv2/web_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/acct/assume_role.py` & `idem-aws-3.0.3/idem_aws/tool/aws/acct/assume_role.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/acct/init.py` & `idem-aws-3.0.3/idem_aws/tool/aws/acct/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/acct/key_name.py` & `idem-aws-3.0.3/idem_aws/tool/aws/acct/key_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/acm/certificate_validation_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/acm/certificate_validation_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/acm/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/acm/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/acm/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/acm/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigateway/base_path_mapping.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigateway/base_path_mapping.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigateway/deployment.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigateway/deployment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigateway/domain_name.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigateway/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigateway/integration.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigateway/integration_response.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigateway/integration_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigateway/method.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigateway/method.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigateway/method_response.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigateway/method_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigateway/resource.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigateway/resource.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigateway/rest_api.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigateway/rest_api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigateway/stage.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigateway/stage.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigateway/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigateway/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigatewayv2/api.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigatewayv2/api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigatewayv2/authorizer.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigatewayv2/authorizer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigatewayv2/domain_name.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigatewayv2/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigatewayv2/integration.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigatewayv2/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigatewayv2/route.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigatewayv2/route.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigatewayv2/stage.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigatewayv2/stage.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/apigatewayv2/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/apigatewayv2/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/application_autoscaling/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/application_autoscaling/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/application_autoscaling/scalable_target.py` & `idem-aws-3.0.3/idem_aws/tool/aws/application_autoscaling/scalable_target.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/application_autoscaling/scaling_policy.py` & `idem-aws-3.0.3/idem_aws/tool/aws/application_autoscaling/scaling_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/arn_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/arn_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/autoscaling/auto_scaling_group_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/autoscaling/auto_scaling_group_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/autoscaling/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/autoscaling/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/autoscaling/scaling_policy.py` & `idem-aws-3.0.3/idem_aws/tool/aws/autoscaling/scaling_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/autoscaling/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/autoscaling/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/backup/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/backup/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/backup/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/backup/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/budgets/budget.py` & `idem-aws-3.0.3/idem_aws/tool/aws/budgets/budget.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/budgets/budget_action.py` & `idem-aws-3.0.3/idem_aws/tool/aws/budgets/budget_action.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/budgets/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/budgets/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/cloudformation/stack.py` & `idem-aws-3.0.3/idem_aws/tool/aws/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/cloudfront/cloudfront_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/cloudfront/cloudfront_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/cloudfront/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/cloudfront/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/cloudfront/distribution.py` & `idem-aws-3.0.3/idem_aws/tool/aws/cloudfront/distribution.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/cloudfront/distribution_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/cloudfront/distribution_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/cloudfront/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/cloudfront/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/cloudtrail/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/cloudtrail/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/cloudtrail/trail.py` & `idem-aws-3.0.3/idem_aws/tool/aws/cloudtrail/trail.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/cloudwatch/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/cloudwatch/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/cloudwatch/log_group.py` & `idem-aws-3.0.3/idem_aws/tool/aws/cloudwatch/log_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/cloudwatch/metric_alarm.py` & `idem-aws-3.0.3/idem_aws/tool/aws/cloudwatch/metric_alarm.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/cloudwatch/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/cloudwatch/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/cloudwatchlogs/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/cloudwatchlogs/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/comment_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/comment_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/config/config_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/config/config_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/config/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/config/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/config/delivery_channel.py` & `idem-aws-3.0.3/idem_aws/tool/aws/config/delivery_channel.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/config/rule.py` & `idem-aws-3.0.3/idem_aws/tool/aws/config/rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/config/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/config/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/costexplorer/anomaly_monitor.py` & `idem-aws-3.0.3/idem_aws/tool/aws/costexplorer/anomaly_monitor.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/costexplorer/anomaly_subscription.py` & `idem-aws-3.0.3/idem_aws/tool/aws/costexplorer/anomaly_subscription.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/costexplorer/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/costexplorer/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/costexplorer/cost_category.py` & `idem-aws-3.0.3/idem_aws/tool/aws/costexplorer/cost_category.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/docdb/db_cluster.py` & `idem-aws-3.0.3/idem_aws/tool/aws/docdb/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/docdb/db_cluster_parameter_group.py` & `idem-aws-3.0.3/idem_aws/tool/aws/docdb/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/docdb/db_subnet_group.py` & `idem-aws-3.0.3/idem_aws/tool/aws/docdb/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/docdb/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/docdb/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/dynamodb/table.py` & `idem-aws-3.0.3/idem_aws/tool/aws/dynamodb/table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/ami.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/ami.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/availability_zones.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/availability_zones.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/dhcp_option_association_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/dhcp_option_association_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/elastic_ip.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/elastic_ip.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/flow_log.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/flow_log.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/data.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/data.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/key_pair.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/key_pair.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/state.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/state.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/block_device_mappings.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/block_device_mappings.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/bootstrap.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/bootstrap.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/contracts/init.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/contracts/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/disable_api_termination.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/disable_api_termination.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/ebs_optimized.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/ebs_optimized.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/iam_instance_profile_arn.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/iam_instance_profile_arn.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/init.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/instance_initiated_shutdown_behavior.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/instance_initiated_shutdown_behavior.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/instance_type.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/instance_type.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/kernel_id.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/kernel_id.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/monitoring_enabled.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/monitoring_enabled.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/network_interfaces.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/network_interfaces.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/placement.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/placement.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/private_ip_address.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/private_ip_address.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/ram_disk_id.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/ram_disk_id.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/security_group_ids.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/security_group_ids.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/source_dest_check.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/source_dest_check.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/sriov_net_support.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/sriov_net_support.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/tags.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/tags.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/instance/update/user_data.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/instance/update/user_data.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/internet_gateway.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/internet_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/key_pair.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/key_pair.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/launch_template.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/launch_template.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/network_interface.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/network_interface.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/placement_group.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/placement_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/route_table.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/route_table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/security_group_rule.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/security_group_rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/snapshot.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/snapshot.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/spot_instance_request.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/spot_instance_request.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/subnet.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/transit_gateway.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/transit_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/transit_gateway_vpc_attachment.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/volume.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/vpc.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/vpc.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/vpc_endpoint.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/vpc_endpoint.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ec2/vpc_peering_connection_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ec2/vpc_peering_connection_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ecr/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ecr/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ecr/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ecr/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/efs/file_system_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/efs/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/efs/mount_target_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/efs/mount_target_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/efs/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/efs/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/eks/addon.py` & `idem-aws-3.0.3/idem_aws/tool/aws/eks/addon.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/eks/cluster.py` & `idem-aws-3.0.3/idem_aws/tool/aws/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/eks/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/eks/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/eks/eks_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/eks/eks_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/eks/nodegroup.py` & `idem-aws-3.0.3/idem_aws/tool/aws/eks/nodegroup.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/eks/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/eks/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/elasticache/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/elasticache/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/elasticache/elasticache_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/elasticache/elasticache_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/elasticache/parameters.py` & `idem-aws-3.0.3/idem_aws/tool/aws/elasticache/parameters.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/elb/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/elb/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/elb/load_balancer.py` & `idem-aws-3.0.3/idem_aws/tool/aws/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/elb/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/elb/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/elbv2/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/elbv2/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/elbv2/listener.py` & `idem-aws-3.0.3/idem_aws/tool/aws/elbv2/listener.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/elbv2/load_balancer.py` & `idem-aws-3.0.3/idem_aws/tool/aws/elbv2/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/elbv2/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/elbv2/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/elbv2/target_group.py` & `idem-aws-3.0.3/idem_aws/tool/aws/elbv2/target_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/es/elasticsearch_domain.py` & `idem-aws-3.0.3/idem_aws/tool/aws/es/elasticsearch_domain.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/es/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/es/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/events/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/events/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/events/rule.py` & `idem-aws-3.0.3/idem_aws/tool/aws/events/rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/events/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/events/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/guardduty/config_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/guardduty/config_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/guardduty/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/guardduty/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/guardduty/detector.py` & `idem-aws-3.0.3/idem_aws/tool/aws/guardduty/detector.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/iam/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/iam/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/iam/group.py` & `idem-aws-3.0.3/idem_aws/tool/aws/iam/group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/iam/group_membership.py` & `idem-aws-3.0.3/idem_aws/tool/aws/iam/group_membership.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/iam/password_policy.py` & `idem-aws-3.0.3/idem_aws/tool/aws/iam/password_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/iam/policy.py` & `idem-aws-3.0.3/idem_aws/tool/aws/iam/policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/iam/role_policy_attachment.py` & `idem-aws-3.0.3/idem_aws/tool/aws/iam/role_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/iam/service_linked_role.py` & `idem-aws-3.0.3/idem_aws/tool/aws/iam/service_linked_role.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/iam/user.py` & `idem-aws-3.0.3/idem_aws/tool/aws/iam/user.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/iam/user_ssh_key.py` & `idem-aws-3.0.3/idem_aws/tool/aws/iam/user_ssh_key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/kinesis/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/kinesis/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/kinesis/stream.py` & `idem-aws-3.0.3/idem_aws/tool/aws/kinesis/stream.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/kinesis/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/kinesis/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/kms/alias.py` & `idem-aws-3.0.3/idem_aws/tool/aws/kms/alias.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/kms/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/kms/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/kms/key.py` & `idem-aws-3.0.3/idem_aws/tool/aws/kms/key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/kms/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/kms/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/lambda_aws/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/lambda_aws/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/lambda_aws/function.py` & `idem-aws-3.0.3/idem_aws/tool/aws/lambda_aws/function.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/lambda_aws/function_event_invoke_config.py` & `idem-aws-3.0.3/idem_aws/tool/aws/lambda_aws/function_event_invoke_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/lambda_aws/function_permission.py` & `idem-aws-3.0.3/idem_aws/tool/aws/lambda_aws/function_permission.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/lambda_aws/function_provisioned_concurrency_config.py` & `idem-aws-3.0.3/idem_aws/tool/aws/lambda_aws/function_provisioned_concurrency_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/lambda_aws/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/lambda_aws/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/logs/subscription_filter_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/logs/subscription_filter_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/neptune/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/neptune/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/neptune/db_cluster.py` & `idem-aws-3.0.3/idem_aws/tool/aws/neptune/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/neptune/db_cluster_parameter_group.py` & `idem-aws-3.0.3/idem_aws/tool/aws/neptune/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/neptune/db_instance.py` & `idem-aws-3.0.3/idem_aws/tool/aws/neptune/db_instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/neptune/db_parameter_group.py` & `idem-aws-3.0.3/idem_aws/tool/aws/neptune/db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/neptune/db_subnet_group.py` & `idem-aws-3.0.3/idem_aws/tool/aws/neptune/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/neptune/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/neptune/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/network_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/network_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/organizations/account.py` & `idem-aws-3.0.3/idem_aws/tool/aws/organizations/account.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/organizations/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/organizations/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/organizations/policy_attachment.py` & `idem-aws-3.0.3/idem_aws/tool/aws/organizations/policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/organizations/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/organizations/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/parameters.py` & `idem-aws-3.0.3/idem_aws/tool/aws/parameters.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/rds/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/rds/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/rds/parameters.py` & `idem-aws-3.0.3/idem_aws/tool/aws/rds/parameters.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/route53/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/route53/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/route53/hosted_zone_association.py` & `idem-aws-3.0.3/idem_aws/tool/aws/route53/hosted_zone_association.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/route53/hosted_zone_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/route53/hosted_zone_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/route53/resource_record_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/route53/resource_record_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/route53/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/route53/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/s3/bucket_acl.py` & `idem-aws-3.0.3/idem_aws/tool/aws/s3/bucket_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/s3/bucket_encryption.py` & `idem-aws-3.0.3/idem_aws/tool/aws/s3/bucket_encryption.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/s3/bucket_lifecycle.py` & `idem-aws-3.0.3/idem_aws/tool/aws/s3/bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/s3/bucket_logging.py` & `idem-aws-3.0.3/idem_aws/tool/aws/s3/bucket_logging.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/s3/bucket_replication.py` & `idem-aws-3.0.3/idem_aws/tool/aws/s3/bucket_replication.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/s3/bucket_versioning.py` & `idem-aws-3.0.3/idem_aws/tool/aws/s3/bucket_versioning.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/s3/bucket_website.py` & `idem-aws-3.0.3/idem_aws/tool/aws/s3/bucket_website.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/s3/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/s3/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/s3/s3_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/search_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/search_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/ses/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/ses/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/sesv2/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/sesv2/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/sns/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/sns/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/sns/sns_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/sns/sns_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/sqs/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/sqs/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/sqs/queue_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/sqs/queue_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/state_comparison_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/state_comparison_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/state_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/string_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/string_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/tag_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/tag_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/test_state_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/wafv2/conversion_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/wafv2/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/wafv2/ip_set_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/wafv2/ip_set_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/wafv2/regex_pattern_set.py` & `idem-aws-3.0.3/idem_aws/tool/aws/wafv2/regex_pattern_set.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/wafv2/tag.py` & `idem-aws-3.0.3/idem_aws/tool/aws/wafv2/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/wafv2/web_acl.py` & `idem-aws-3.0.3/idem_aws/tool/aws/wafv2/web_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/aws/waiter_utils.py` & `idem-aws-3.0.3/idem_aws/tool/aws/waiter_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/boto3/client.py` & `idem-aws-3.0.3/idem_aws/tool/boto3/client.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/boto3/custom_waiter.py` & `idem-aws-3.0.3/idem_aws/tool/boto3/custom_waiter.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/boto3/region.py` & `idem-aws-3.0.3/idem_aws/tool/boto3/region.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/boto3/resolve.py` & `idem-aws-3.0.3/idem_aws/tool/boto3/resolve.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/boto3/resource.py` & `idem-aws-3.0.3/idem_aws/tool/boto3/resource.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/boto3/session.py` & `idem-aws-3.0.3/idem_aws/tool/boto3/session.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws/tool/heist/bootstrap.py` & `idem-aws-3.0.3/idem_aws/tool/heist/bootstrap.py`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws.egg-info/PKG-INFO` & `idem-aws-3.0.3/idem_aws.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-aws
-Version: 3.0.2
+Version: 3.0.3
 Summary: AWS Cloud Provider for Idem
 Home-page: https://docs.idemproject.io/idem-aws/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-aws
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-aws/-/issues
```

### Comparing `idem-aws-3.0.2/idem_aws.egg-info/SOURCES.txt` & `idem-aws-3.0.3/idem_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-aws-3.0.2/idem_aws.egg-info/requires.txt` & `idem-aws-3.0.3/idem_aws.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 pgpy<0.7.0,>=0.6.0
 deepdiff<6.0.0,>=5.8.0
 heist<7.0.0,>=6.1.0
 pop-serial<2.0.0,>=1.1.0
 cryptography<42.0.0,>=39.0.1
 
 [autogen]
-pop-create-idem==2.0.4
+pop-create-idem==4.3.2
 inflect
 textwrap3
 tqdm
 
 [bootstrap]
 heist-salt<6.0.0,>=5.3.1
 
 [full]
-heist-salt<6.0.0,>=5.3.1
-pop-create-idem==2.0.4
-localstack-ext
-inflect
-localstack
 tqdm
-textwrap3
+heist-salt<6.0.0,>=5.3.1
 msgpack
-aws-google-auth>=0.0.35
+pop-create-idem==4.3.2
+inflect
 localstack-client
+aws-google-auth>=0.0.35
+textwrap3
+localstack
+localstack-ext
 
 [google_auth]
 aws-google-auth>=0.0.35
 msgpack
 
 [localstack]
 localstack
```

### Comparing `idem-aws-3.0.2/setup.py` & `idem-aws-3.0.3/setup.py`

 * *Files identical despite different names*

