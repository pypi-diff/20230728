# Comparing `tmp/port_pulumi-1.1.1.tar.gz` & `tmp/port_pulumi-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_pulumi-1.1.1.tar", last modified: Sat Jul 22 11:47:06 2023, max compression
+gzip compressed data, was "port_pulumi-1.2.1.tar", last modified: Fri Jul 28 05:39:12 2023, max compression
```

## Comparing `port_pulumi-1.1.1.tar` & `port_pulumi-1.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:47:06.652286 port_pulumi-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-22 11:47:06.652286 port_pulumi-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:47:06.652286 port_pulumi-1.1.1/port_pulumi/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    98686 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    36131 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    34831 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/blueprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:47:06.652286 port_pulumi-1.1.1/port_pulumi/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    22683 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    79853 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:47:06.652286 port_pulumi-1.1.1/port_pulumi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 11:47:06.652286 port_pulumi-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:39:12.880571 port_pulumi-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-28 05:39:12.876572 port_pulumi-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:39:12.876572 port_pulumi-1.2.1/port_pulumi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98686 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38402 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34831 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi/blueprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:39:12.876572 port_pulumi-1.2.1/port_pulumi/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22683 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79853 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:39:12.876572 port_pulumi-1.2.1/port_pulumi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/port_pulumi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 05:39:12.880571 port_pulumi-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-28 05:39:12.000000 port_pulumi-1.2.1/setup.py
```

### Comparing `port_pulumi-1.1.1/PKG-INFO` & `port_pulumi-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port_pulumi
-Version: 1.1.1
+Version: 1.2.1
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi-port
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `port_pulumi-1.1.1/README.md` & `port_pulumi-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.1/port_pulumi/__init__.py` & `port_pulumi-1.2.1/port_pulumi/__init__.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.1/port_pulumi/_inputs.py` & `port_pulumi-1.2.1/port_pulumi/_inputs.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.1/port_pulumi/_utilities.py` & `port_pulumi-1.2.1/port_pulumi/_utilities.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.1/port_pulumi/action.py` & `port_pulumi-1.2.1/port_pulumi/action.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
                  approval_webhook_notification: Optional[pulumi.Input['ActionApprovalWebhookNotificationArgs']] = None,
                  azure_method: Optional[pulumi.Input['ActionAzureMethodArgs']] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  github_method: Optional[pulumi.Input['ActionGithubMethodArgs']] = None,
                  gitlab_method: Optional[pulumi.Input['ActionGitlabMethodArgs']] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  kafka_method: Optional[pulumi.Input['ActionKafkaMethodArgs']] = None,
+                 order_properties: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  required_approval: Optional[pulumi.Input[bool]] = None,
                  user_properties: Optional[pulumi.Input['ActionUserPropertiesArgs']] = None,
                  webhook_method: Optional[pulumi.Input['ActionWebhookMethodArgs']] = None):
         """
         The set of arguments for constructing a Action resource.
         :param pulumi.Input[str] blueprint: The blueprint identifier the action relates to
         :param pulumi.Input[str] identifier: Identifier
@@ -41,14 +42,15 @@
         :param pulumi.Input['ActionApprovalWebhookNotificationArgs'] approval_webhook_notification: The webhook notification of the approval
         :param pulumi.Input['ActionAzureMethodArgs'] azure_method: The invocation method of the action
         :param pulumi.Input[str] description: Description
         :param pulumi.Input['ActionGithubMethodArgs'] github_method: The invocation method of the action
         :param pulumi.Input['ActionGitlabMethodArgs'] gitlab_method: The invocation method of the action
         :param pulumi.Input[str] icon: Icon
         :param pulumi.Input['ActionKafkaMethodArgs'] kafka_method: The invocation method of the action
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] order_properties: Order properties
         :param pulumi.Input[bool] required_approval: Require approval before invoking the action
         :param pulumi.Input['ActionUserPropertiesArgs'] user_properties: User properties
         :param pulumi.Input['ActionWebhookMethodArgs'] webhook_method: The invocation method of the action
         """
         pulumi.set(__self__, "blueprint", blueprint)
         pulumi.set(__self__, "identifier", identifier)
         pulumi.set(__self__, "title", title)
@@ -65,14 +67,16 @@
             pulumi.set(__self__, "github_method", github_method)
         if gitlab_method is not None:
             pulumi.set(__self__, "gitlab_method", gitlab_method)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if kafka_method is not None:
             pulumi.set(__self__, "kafka_method", kafka_method)
+        if order_properties is not None:
+            pulumi.set(__self__, "order_properties", order_properties)
         if required_approval is not None:
             pulumi.set(__self__, "required_approval", required_approval)
         if user_properties is not None:
             pulumi.set(__self__, "user_properties", user_properties)
         if webhook_method is not None:
             pulumi.set(__self__, "webhook_method", webhook_method)
 
@@ -217,14 +221,26 @@
         return pulumi.get(self, "kafka_method")
 
     @kafka_method.setter
     def kafka_method(self, value: Optional[pulumi.Input['ActionKafkaMethodArgs']]):
         pulumi.set(self, "kafka_method", value)
 
     @property
+    @pulumi.getter(name="orderProperties")
+    def order_properties(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Order properties
+        """
+        return pulumi.get(self, "order_properties")
+
+    @order_properties.setter
+    def order_properties(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "order_properties", value)
+
+    @property
     @pulumi.getter(name="requiredApproval")
     def required_approval(self) -> Optional[pulumi.Input[bool]]:
         """
         Require approval before invoking the action
         """
         return pulumi.get(self, "required_approval")
 
@@ -266,14 +282,15 @@
                  blueprint: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  github_method: Optional[pulumi.Input['ActionGithubMethodArgs']] = None,
                  gitlab_method: Optional[pulumi.Input['ActionGitlabMethodArgs']] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  kafka_method: Optional[pulumi.Input['ActionKafkaMethodArgs']] = None,
+                 order_properties: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  required_approval: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  trigger: Optional[pulumi.Input[str]] = None,
                  user_properties: Optional[pulumi.Input['ActionUserPropertiesArgs']] = None,
                  webhook_method: Optional[pulumi.Input['ActionWebhookMethodArgs']] = None):
         """
         Input properties used for looking up and filtering Action resources.
@@ -283,14 +300,15 @@
         :param pulumi.Input[str] blueprint: The blueprint identifier the action relates to
         :param pulumi.Input[str] description: Description
         :param pulumi.Input['ActionGithubMethodArgs'] github_method: The invocation method of the action
         :param pulumi.Input['ActionGitlabMethodArgs'] gitlab_method: The invocation method of the action
         :param pulumi.Input[str] icon: Icon
         :param pulumi.Input[str] identifier: Identifier
         :param pulumi.Input['ActionKafkaMethodArgs'] kafka_method: The invocation method of the action
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] order_properties: Order properties
         :param pulumi.Input[bool] required_approval: Require approval before invoking the action
         :param pulumi.Input[str] title: Title
         :param pulumi.Input[str] trigger: The trigger type of the action
         :param pulumi.Input['ActionUserPropertiesArgs'] user_properties: User properties
         :param pulumi.Input['ActionWebhookMethodArgs'] webhook_method: The invocation method of the action
         """
         if approval_email_notification is not None:
@@ -309,14 +327,16 @@
             pulumi.set(__self__, "gitlab_method", gitlab_method)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if identifier is not None:
             pulumi.set(__self__, "identifier", identifier)
         if kafka_method is not None:
             pulumi.set(__self__, "kafka_method", kafka_method)
+        if order_properties is not None:
+            pulumi.set(__self__, "order_properties", order_properties)
         if required_approval is not None:
             pulumi.set(__self__, "required_approval", required_approval)
         if title is not None:
             pulumi.set(__self__, "title", title)
         if trigger is not None:
             pulumi.set(__self__, "trigger", trigger)
         if user_properties is not None:
@@ -441,14 +461,26 @@
         return pulumi.get(self, "kafka_method")
 
     @kafka_method.setter
     def kafka_method(self, value: Optional[pulumi.Input['ActionKafkaMethodArgs']]):
         pulumi.set(self, "kafka_method", value)
 
     @property
+    @pulumi.getter(name="orderProperties")
+    def order_properties(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Order properties
+        """
+        return pulumi.get(self, "order_properties")
+
+    @order_properties.setter
+    def order_properties(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "order_properties", value)
+
+    @property
     @pulumi.getter(name="requiredApproval")
     def required_approval(self) -> Optional[pulumi.Input[bool]]:
         """
         Require approval before invoking the action
         """
         return pulumi.get(self, "required_approval")
 
@@ -516,14 +548,15 @@
                  blueprint: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  github_method: Optional[pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']]] = None,
                  gitlab_method: Optional[pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  kafka_method: Optional[pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']]] = None,
+                 order_properties: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  required_approval: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  trigger: Optional[pulumi.Input[str]] = None,
                  user_properties: Optional[pulumi.Input[pulumi.InputType['ActionUserPropertiesArgs']]] = None,
                  webhook_method: Optional[pulumi.Input[pulumi.InputType['ActionWebhookMethodArgs']]] = None,
                  __props__=None):
         """
@@ -536,14 +569,15 @@
         :param pulumi.Input[str] blueprint: The blueprint identifier the action relates to
         :param pulumi.Input[str] description: Description
         :param pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']] github_method: The invocation method of the action
         :param pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']] gitlab_method: The invocation method of the action
         :param pulumi.Input[str] icon: Icon
         :param pulumi.Input[str] identifier: Identifier
         :param pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']] kafka_method: The invocation method of the action
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] order_properties: Order properties
         :param pulumi.Input[bool] required_approval: Require approval before invoking the action
         :param pulumi.Input[str] title: Title
         :param pulumi.Input[str] trigger: The trigger type of the action
         :param pulumi.Input[pulumi.InputType['ActionUserPropertiesArgs']] user_properties: User properties
         :param pulumi.Input[pulumi.InputType['ActionWebhookMethodArgs']] webhook_method: The invocation method of the action
         """
         ...
@@ -575,14 +609,15 @@
                  blueprint: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  github_method: Optional[pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']]] = None,
                  gitlab_method: Optional[pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  kafka_method: Optional[pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']]] = None,
+                 order_properties: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  required_approval: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  trigger: Optional[pulumi.Input[str]] = None,
                  user_properties: Optional[pulumi.Input[pulumi.InputType['ActionUserPropertiesArgs']]] = None,
                  webhook_method: Optional[pulumi.Input[pulumi.InputType['ActionWebhookMethodArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
@@ -603,14 +638,15 @@
             __props__.__dict__["github_method"] = github_method
             __props__.__dict__["gitlab_method"] = gitlab_method
             __props__.__dict__["icon"] = icon
             if identifier is None and not opts.urn:
                 raise TypeError("Missing required property 'identifier'")
             __props__.__dict__["identifier"] = identifier
             __props__.__dict__["kafka_method"] = kafka_method
+            __props__.__dict__["order_properties"] = order_properties
             __props__.__dict__["required_approval"] = required_approval
             if title is None and not opts.urn:
                 raise TypeError("Missing required property 'title'")
             __props__.__dict__["title"] = title
             if trigger is None and not opts.urn:
                 raise TypeError("Missing required property 'trigger'")
             __props__.__dict__["trigger"] = trigger
@@ -632,14 +668,15 @@
             blueprint: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             github_method: Optional[pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']]] = None,
             gitlab_method: Optional[pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']]] = None,
             icon: Optional[pulumi.Input[str]] = None,
             identifier: Optional[pulumi.Input[str]] = None,
             kafka_method: Optional[pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']]] = None,
+            order_properties: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             required_approval: Optional[pulumi.Input[bool]] = None,
             title: Optional[pulumi.Input[str]] = None,
             trigger: Optional[pulumi.Input[str]] = None,
             user_properties: Optional[pulumi.Input[pulumi.InputType['ActionUserPropertiesArgs']]] = None,
             webhook_method: Optional[pulumi.Input[pulumi.InputType['ActionWebhookMethodArgs']]] = None) -> 'Action':
         """
         Get an existing Action resource's state with the given name, id, and optional extra
@@ -654,14 +691,15 @@
         :param pulumi.Input[str] blueprint: The blueprint identifier the action relates to
         :param pulumi.Input[str] description: Description
         :param pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']] github_method: The invocation method of the action
         :param pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']] gitlab_method: The invocation method of the action
         :param pulumi.Input[str] icon: Icon
         :param pulumi.Input[str] identifier: Identifier
         :param pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']] kafka_method: The invocation method of the action
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] order_properties: Order properties
         :param pulumi.Input[bool] required_approval: Require approval before invoking the action
         :param pulumi.Input[str] title: Title
         :param pulumi.Input[str] trigger: The trigger type of the action
         :param pulumi.Input[pulumi.InputType['ActionUserPropertiesArgs']] user_properties: User properties
         :param pulumi.Input[pulumi.InputType['ActionWebhookMethodArgs']] webhook_method: The invocation method of the action
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -674,14 +712,15 @@
         __props__.__dict__["blueprint"] = blueprint
         __props__.__dict__["description"] = description
         __props__.__dict__["github_method"] = github_method
         __props__.__dict__["gitlab_method"] = gitlab_method
         __props__.__dict__["icon"] = icon
         __props__.__dict__["identifier"] = identifier
         __props__.__dict__["kafka_method"] = kafka_method
+        __props__.__dict__["order_properties"] = order_properties
         __props__.__dict__["required_approval"] = required_approval
         __props__.__dict__["title"] = title
         __props__.__dict__["trigger"] = trigger
         __props__.__dict__["user_properties"] = user_properties
         __props__.__dict__["webhook_method"] = webhook_method
         return Action(resource_name, opts=opts, __props__=__props__)
 
@@ -762,14 +801,22 @@
     def kafka_method(self) -> pulumi.Output[Optional['outputs.ActionKafkaMethod']]:
         """
         The invocation method of the action
         """
         return pulumi.get(self, "kafka_method")
 
     @property
+    @pulumi.getter(name="orderProperties")
+    def order_properties(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        Order properties
+        """
+        return pulumi.get(self, "order_properties")
+
+    @property
     @pulumi.getter(name="requiredApproval")
     def required_approval(self) -> pulumi.Output[Optional[bool]]:
         """
         Require approval before invoking the action
         """
         return pulumi.get(self, "required_approval")
```

### Comparing `port_pulumi-1.1.1/port_pulumi/blueprint.py` & `port_pulumi-1.2.1/port_pulumi/blueprint.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.1/port_pulumi/config/vars.py` & `port_pulumi-1.2.1/port_pulumi/config/vars.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.1/port_pulumi/entity.py` & `port_pulumi-1.2.1/port_pulumi/entity.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.1/port_pulumi/outputs.py` & `port_pulumi-1.2.1/port_pulumi/outputs.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.1/port_pulumi/provider.py` & `port_pulumi-1.2.1/port_pulumi/provider.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.1/port_pulumi.egg-info/PKG-INFO` & `port_pulumi-1.2.1/port_pulumi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-pulumi
-Version: 1.1.1
+Version: 1.2.1
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi-port
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `port_pulumi-1.1.1/port_pulumi.egg-info/SOURCES.txt` & `port_pulumi-1.2.1/port_pulumi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.1/setup.py` & `port_pulumi-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.1.1"
-PLUGIN_VERSION = "1.1.1"
+VERSION = "1.2.1"
+PLUGIN_VERSION = "1.2.1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'port', PLUGIN_VERSION, '--server', 'github://api.github.com/port-labs/pulumi-port'])
         except OSError as error:
```

