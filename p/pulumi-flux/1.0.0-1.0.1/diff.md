# Comparing `tmp/pulumi_flux-1.0.0.tar.gz` & `tmp/pulumi_flux-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_flux-1.0.0.tar", last modified: Sun Sep 25 09:48:59 2022, max compression
+gzip compressed data, was "pulumi_flux-1.0.1.tar", last modified: Fri Jul 28 11:13:48 2023, max compression
```

## Comparing `pulumi_flux-1.0.0.tar` & `pulumi_flux-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 09:48:59.123463 pulumi_flux-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-09-25 09:48:59.123463 pulumi_flux-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 09:48:59.123463 pulumi_flux-1.0.0/pulumi_flux/
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/pulumi_flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8106 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/pulumi_flux/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    11009 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/pulumi_flux/get_flux_install.py
--rw-r--r--   0 runner    (1001) docker     (121)    10645 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/pulumi_flux/get_flux_sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     3414 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/pulumi_flux/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/pulumi_flux/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/pulumi_flux/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 09:48:59.123463 pulumi_flux-1.0.0/pulumi_flux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-09-25 09:48:59.000000 pulumi_flux-1.0.0/pulumi_flux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-09-25 09:48:59.000000 pulumi_flux-1.0.0/pulumi_flux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-25 09:48:59.000000 pulumi_flux-1.0.0/pulumi_flux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-25 09:48:59.000000 pulumi_flux-1.0.0/pulumi_flux.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-25 09:48:59.000000 pulumi_flux-1.0.0/pulumi_flux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-25 09:48:59.000000 pulumi_flux-1.0.0/pulumi_flux.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-25 09:48:59.123463 pulumi_flux-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2129 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:13:48.963791 pulumi_flux-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-28 11:13:48.963791 pulumi_flux-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:13:48.959791 pulumi_flux-1.0.1/pulumi_flux/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21313 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:13:48.963791 pulumi_flux-1.0.1/pulumi_flux/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48304 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux/flux_bootstrap_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux/get_flux_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux/get_flux_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:13:48.959791 pulumi_flux-1.0.1/pulumi_flux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/pulumi_flux.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 11:13:48.963791 pulumi_flux-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-28 11:13:48.000000 pulumi_flux-1.0.1/setup.py
```

### Comparing `pulumi_flux-1.0.0/PKG-INFO` & `pulumi_flux-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: pulumi_flux
-Version: 1.0.0
-Summary: A Pulumi package for creating and managing flux cloud resources.
+Version: 1.0.1
+Summary: A Pulumi package for creating and managing Flux cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/oun/pulumi-flux
 Keywords: pulumi flux category/cloud
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# Flux Resource Provider
+# Flux Pulumi Provider
 
-The Flux Resource Provider lets you manage [FluxCD](https://fluxcd.io) resources.
+The Flux Provider lets you manage [FluxCD](https://fluxcd.io) resources.
+This provider wraps the existing [Terraform Provider Flux](https://github.com/fluxcd/terraform-provider-flux).
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
@@ -57,10 +59,10 @@
 
 ## Examples
 
 Find working Python code samples in the [`./examples`](https://github.com/oun/pulumi-flux/tree/main/examples) directory.
 
 ## Reference
 
-For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/foo/api-docs/).
+For detailed reference documentation, please visit the [the Pulumi registry](https://www.pulumi.com/registry/packages/flux/api-docs/).
```

### Comparing `pulumi_flux-1.0.0/README.md` & `pulumi_flux-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# Flux Resource Provider
+# Flux Pulumi Provider
 
-The Flux Resource Provider lets you manage [FluxCD](https://fluxcd.io) resources.
+The Flux Provider lets you manage [FluxCD](https://fluxcd.io) resources.
+This provider wraps the existing [Terraform Provider Flux](https://github.com/fluxcd/terraform-provider-flux).
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
@@ -46,8 +47,8 @@
 
 ## Examples
 
 Find working Python code samples in the [`./examples`](https://github.com/oun/pulumi-flux/tree/main/examples) directory.
 
 ## Reference
 
-For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/foo/api-docs/).
+For detailed reference documentation, please visit the [the Pulumi registry](https://www.pulumi.com/registry/packages/flux/api-docs/).
```

### Comparing `pulumi_flux-1.0.0/pulumi_flux/_utilities.py` & `pulumi_flux-1.0.1/pulumi_flux/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_flux-1.0.0/pulumi_flux/get_flux_install.py` & `pulumi_flux-1.0.1/pulumi_flux/get_flux_install.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,17 +95,14 @@
     @pulumi.getter
     def content(self) -> str:
         return pulumi.get(self, "content")
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="imagePullSecrets")
     def image_pull_secrets(self) -> Optional[str]:
         return pulumi.get(self, "image_pull_secrets")
```

### Comparing `pulumi_flux-1.0.0/pulumi_flux/get_flux_sync.py` & `pulumi_flux-1.0.1/pulumi_flux/get_flux_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,27 +17,24 @@
 ]
 
 @pulumi.output_type
 class GetFluxSyncResult:
     """
     A collection of values returned by getFluxSync.
     """
-    def __init__(__self__, branch=None, commit=None, content=None, git_implementation=None, id=None, interval=None, kustomize_content=None, kustomize_path=None, name=None, namespace=None, patch_file_paths=None, patch_names=None, path=None, secret=None, semver=None, tag=None, target_path=None, url=None):
+    def __init__(__self__, branch=None, commit=None, content=None, id=None, interval=None, kustomize_content=None, kustomize_path=None, name=None, namespace=None, patch_file_paths=None, patch_names=None, path=None, secret=None, semver=None, tag=None, target_path=None, url=None):
         if branch and not isinstance(branch, str):
             raise TypeError("Expected argument 'branch' to be a str")
         pulumi.set(__self__, "branch", branch)
         if commit and not isinstance(commit, str):
             raise TypeError("Expected argument 'commit' to be a str")
         pulumi.set(__self__, "commit", commit)
         if content and not isinstance(content, str):
             raise TypeError("Expected argument 'content' to be a str")
         pulumi.set(__self__, "content", content)
-        if git_implementation and not isinstance(git_implementation, str):
-            raise TypeError("Expected argument 'git_implementation' to be a str")
-        pulumi.set(__self__, "git_implementation", git_implementation)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if interval and not isinstance(interval, int):
             raise TypeError("Expected argument 'interval' to be a int")
         pulumi.set(__self__, "interval", interval)
         if kustomize_content and not isinstance(kustomize_content, str):
@@ -89,24 +86,16 @@
 
     @property
     @pulumi.getter
     def content(self) -> str:
         return pulumi.get(self, "content")
 
     @property
-    @pulumi.getter(name="gitImplementation")
-    def git_implementation(self) -> Optional[str]:
-        return pulumi.get(self, "git_implementation")
-
-    @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def interval(self) -> Optional[int]:
         return pulumi.get(self, "interval")
 
@@ -176,15 +165,14 @@
     def __await__(self):
         if False:
             yield self
         return GetFluxSyncResult(
             branch=self.branch,
             commit=self.commit,
             content=self.content,
-            git_implementation=self.git_implementation,
             id=self.id,
             interval=self.interval,
             kustomize_content=self.kustomize_content,
             kustomize_path=self.kustomize_path,
             name=self.name,
             namespace=self.namespace,
             patch_file_paths=self.patch_file_paths,
@@ -195,15 +183,14 @@
             tag=self.tag,
             target_path=self.target_path,
             url=self.url)
 
 
 def get_flux_sync(branch: Optional[str] = None,
                   commit: Optional[str] = None,
-                  git_implementation: Optional[str] = None,
                   interval: Optional[int] = None,
                   name: Optional[str] = None,
                   namespace: Optional[str] = None,
                   patch_names: Optional[Sequence[str]] = None,
                   secret: Optional[str] = None,
                   semver: Optional[str] = None,
                   tag: Optional[str] = None,
@@ -212,15 +199,14 @@
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFluxSyncResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     __args__['branch'] = branch
     __args__['commit'] = commit
-    __args__['gitImplementation'] = git_implementation
     __args__['interval'] = interval
     __args__['name'] = name
     __args__['namespace'] = namespace
     __args__['patchNames'] = patch_names
     __args__['secret'] = secret
     __args__['semver'] = semver
     __args__['tag'] = tag
@@ -229,15 +215,14 @@
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('flux:index/getFluxSync:getFluxSync', __args__, opts=opts, typ=GetFluxSyncResult).value
 
     return AwaitableGetFluxSyncResult(
         branch=__ret__.branch,
         commit=__ret__.commit,
         content=__ret__.content,
-        git_implementation=__ret__.git_implementation,
         id=__ret__.id,
         interval=__ret__.interval,
         kustomize_content=__ret__.kustomize_content,
         kustomize_path=__ret__.kustomize_path,
         name=__ret__.name,
         namespace=__ret__.namespace,
         patch_file_paths=__ret__.patch_file_paths,
@@ -249,15 +234,14 @@
         target_path=__ret__.target_path,
         url=__ret__.url)
 
 
 @_utilities.lift_output_func(get_flux_sync)
 def get_flux_sync_output(branch: Optional[pulumi.Input[Optional[str]]] = None,
                          commit: Optional[pulumi.Input[Optional[str]]] = None,
-                         git_implementation: Optional[pulumi.Input[Optional[str]]] = None,
                          interval: Optional[pulumi.Input[Optional[int]]] = None,
                          name: Optional[pulumi.Input[Optional[str]]] = None,
                          namespace: Optional[pulumi.Input[Optional[str]]] = None,
                          patch_names: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                          secret: Optional[pulumi.Input[Optional[str]]] = None,
                          semver: Optional[pulumi.Input[Optional[str]]] = None,
                          tag: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_flux-1.0.0/pulumi_flux.egg-info/PKG-INFO` & `pulumi_flux-1.0.1/pulumi_flux.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: pulumi-flux
-Version: 1.0.0
-Summary: A Pulumi package for creating and managing flux cloud resources.
+Version: 1.0.1
+Summary: A Pulumi package for creating and managing Flux cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/oun/pulumi-flux
 Keywords: pulumi flux category/cloud
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# Flux Resource Provider
+# Flux Pulumi Provider
 
-The Flux Resource Provider lets you manage [FluxCD](https://fluxcd.io) resources.
+The Flux Provider lets you manage [FluxCD](https://fluxcd.io) resources.
+This provider wraps the existing [Terraform Provider Flux](https://github.com/fluxcd/terraform-provider-flux).
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
@@ -57,10 +59,10 @@
 
 ## Examples
 
 Find working Python code samples in the [`./examples`](https://github.com/oun/pulumi-flux/tree/main/examples) directory.
 
 ## Reference
 
-For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/foo/api-docs/).
+For detailed reference documentation, please visit the [the Pulumi registry](https://www.pulumi.com/registry/packages/flux/api-docs/).
```

### Comparing `pulumi_flux-1.0.0/setup.py` & `pulumi_flux-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.0.0"
-PLUGIN_VERSION = "1.0.0"
+VERSION = "1.0.1"
+PLUGIN_VERSION = "1.0.1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'flux', PLUGIN_VERSION, '--server', 'github://api.github.com/oun'])
         except OSError as error:
@@ -34,16 +34,17 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "flux Pulumi Package - Development Version"
 
 
 setup(name='pulumi_flux',
+      python_requires='>=3.7',
       version=VERSION,
-      description="A Pulumi package for creating and managing flux cloud resources.",
+      description="A Pulumi package for creating and managing Flux cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
       keywords='pulumi flux category/cloud',
       url='https://www.pulumi.com',
```

