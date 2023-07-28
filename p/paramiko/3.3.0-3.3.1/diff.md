# Comparing `tmp/paramiko-3.3.0.tar.gz` & `tmp/paramiko-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpvs0v_32g/dist/paramiko-3.3.0.tar", last modified: Fri Jul 28 19:23:28 2023, max compression
+gzip compressed data, was "/tmp/tmp4yvlkxou/dist/paramiko-3.3.1.tar", last modified: Fri Jul 28 20:15:35 2023, max compression
```

## Comparing `paramiko-3.3.0.tar` & `paramiko-3.3.1.tar`

### file list

```diff
@@ -1,269 +1,269 @@
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 19:23:28.000000 paramiko-3.3.0/
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-07-28 19:23:28.000000 paramiko-3.3.0/setup.cfg
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 19:23:28.000000 paramiko-3.3.0/paramiko/
--rw-r--r--   0 jforcier  (1000) users      (100)     5740 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/kex_group1.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7546 2023-05-25 18:00:56.000000 paramiko-3.3.0/paramiko/rsakey.py
--rw-r--r--   0 jforcier  (1000) users      (100)   129637 2023-05-25 18:00:56.000000 paramiko-3.3.0/paramiko/transport.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4648 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/proxy.py
--rw-r--r--   0 jforcier  (1000) users      (100)     8248 2023-05-25 18:00:56.000000 paramiko-3.3.0/paramiko/dsskey.py
--rw-r--r--   0 jforcier  (1000) users      (100)    13208 2023-05-25 18:00:56.000000 paramiko-3.3.0/paramiko/hostkeys.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1282 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/compress.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4436 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/kex_curve25519.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7756 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/common.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7457 2023-05-25 18:00:56.000000 paramiko-3.3.0/paramiko/ed25519key.py
--rw-r--r--   0 jforcier  (1000) users      (100)    10320 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/kex_gex.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7424 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/sftp_handle.py
--rw-r--r--   0 jforcier  (1000) users      (100)     9550 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7321 2023-05-25 18:00:56.000000 paramiko-3.3.0/paramiko/ssh_exception.py
--rw-r--r--   0 jforcier  (1000) users      (100)    11653 2023-05-25 18:00:56.000000 paramiko-3.3.0/paramiko/ecdsakey.py
--rw-r--r--   0 jforcier  (1000) users      (100)     9349 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/message.py
--rw-r--r--   0 jforcier  (1000) users      (100)    11204 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/_winapi.py
--rw-r--r--   0 jforcier  (1000) users      (100)    28887 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/ssh_gss.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4177 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/win_pageant.py
--rw-r--r--   0 jforcier  (1000) users      (100)    24562 2023-03-10 18:55:53.000000 paramiko-3.3.0/paramiko/kex_gss.py
--rw-r--r--   0 jforcier  (1000) users      (100)    27362 2023-07-28 18:55:00.000000 paramiko-3.3.0/paramiko/config.py
--rw-r--r--   0 jforcier  (1000) users      (100)    21666 2023-05-25 00:47:16.000000 paramiko-3.3.0/paramiko/packet.py
--rw-r--r--   0 jforcier  (1000) users      (100)     6471 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/sftp.py
--rw-r--r--   0 jforcier  (1000) users      (100)    35855 2023-06-09 17:41:24.000000 paramiko-3.3.0/paramiko/sftp_client.py
--rw-r--r--   0 jforcier  (1000) users      (100)    49191 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/channel.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5107 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/primes.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1918 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/win_openssh.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1833 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/kex_group14.py
--rw-r--r--   0 jforcier  (1000) users      (100)    30457 2023-05-25 18:00:56.000000 paramiko-3.3.0/paramiko/server.py
--rw-r--r--   0 jforcier  (1000) users      (100)    34492 2023-05-25 18:00:56.000000 paramiko-3.3.0/paramiko/client.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2288 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/kex_group16.py
--rw-r--r--   0 jforcier  (1000) users      (100)    19492 2023-03-10 18:55:53.000000 paramiko-3.3.0/paramiko/sftp_server.py
--rw-r--r--   0 jforcier  (1000) users      (100)    11437 2023-05-25 18:00:56.000000 paramiko-3.3.0/paramiko/auth_strategy.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3902 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/pipe.py
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-07-28 19:23:26.000000 paramiko-3.3.0/paramiko/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)    36007 2023-05-25 18:00:56.000000 paramiko-3.3.0/paramiko/pkey.py
--rw-r--r--   0 jforcier  (1000) users      (100)    15877 2023-05-25 18:00:56.000000 paramiko-3.3.0/paramiko/agent.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7225 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/buffered_pipe.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4423 2023-05-25 18:00:56.000000 paramiko-3.3.0/paramiko/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)    43006 2023-05-25 18:00:56.000000 paramiko-3.3.0/paramiko/auth_handler.py
--rw-r--r--   0 jforcier  (1000) users      (100)    21820 2023-06-09 17:41:24.000000 paramiko-3.3.0/paramiko/sftp_file.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5012 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/kex_ecdh_nist.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12544 2023-03-10 18:55:53.000000 paramiko-3.3.0/paramiko/sftp_si.py
--rw-r--r--   0 jforcier  (1000) users      (100)     8258 2023-03-10 18:55:53.000000 paramiko-3.3.0/paramiko/sftp_attr.py
--rw-r--r--   0 jforcier  (1000) users      (100)    19063 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/file.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4369 2023-03-03 18:55:05.000000 paramiko-3.3.0/paramiko/ber.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4992 2023-03-03 18:55:05.000000 paramiko-3.3.0/setup_helper.py
--rw-r--r--   0 jforcier  (1000) users      (100)      208 2023-05-25 18:00:56.000000 paramiko-3.3.0/MANIFEST.in
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/
--rw-r--r--   0 jforcier  (1000) users      (100)    12628 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/index.html
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/api/
--rw-r--r--   0 jforcier  (1000) users      (100)    42833 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/api/config.html
--rw-r--r--   0 jforcier  (1000) users      (100)    26848 2023-07-28 18:49:31.000000 paramiko-3.3.0/docs/api/hostkeys.html
--rw-r--r--   0 jforcier  (1000) users      (100)    15714 2023-07-28 18:49:31.000000 paramiko-3.3.0/docs/api/kex_gss.html
--rw-r--r--   0 jforcier  (1000) users      (100)   118448 2023-07-28 18:49:31.000000 paramiko-3.3.0/docs/api/keys.html
--rw-r--r--   0 jforcier  (1000) users      (100)    26728 2023-07-28 18:49:31.000000 paramiko-3.3.0/docs/api/file.html
--rw-r--r--   0 jforcier  (1000) users      (100)   180584 2023-07-28 18:49:31.000000 paramiko-3.3.0/docs/api/sftp.html
--rw-r--r--   0 jforcier  (1000) users      (100)    19937 2023-07-28 18:49:31.000000 paramiko-3.3.0/docs/api/packet.html
--rw-r--r--   0 jforcier  (1000) users      (100)    68501 2023-07-28 18:49:30.000000 paramiko-3.3.0/docs/api/agent.html
--rw-r--r--   0 jforcier  (1000) users      (100)    89315 2023-07-28 18:49:30.000000 paramiko-3.3.0/docs/api/channel.html
--rw-r--r--   0 jforcier  (1000) users      (100)   151247 2023-07-28 18:49:32.000000 paramiko-3.3.0/docs/api/transport.html
--rw-r--r--   0 jforcier  (1000) users      (100)     8827 2023-07-28 18:49:31.000000 paramiko-3.3.0/docs/api/pipe.html
--rw-r--r--   0 jforcier  (1000) users      (100)    17417 2023-07-28 18:49:30.000000 paramiko-3.3.0/docs/api/buffered_pipe.html
--rw-r--r--   0 jforcier  (1000) users      (100)    57007 2023-07-28 18:49:31.000000 paramiko-3.3.0/docs/api/ssh_gss.html
--rw-r--r--   0 jforcier  (1000) users      (100)    86230 2023-07-28 18:49:31.000000 paramiko-3.3.0/docs/api/server.html
--rw-r--r--   0 jforcier  (1000) users      (100)    44986 2023-07-28 18:49:30.000000 paramiko-3.3.0/docs/api/auth.html
--rw-r--r--   0 jforcier  (1000) users      (100)    61123 2023-07-28 18:49:30.000000 paramiko-3.3.0/docs/api/client.html
--rw-r--r--   0 jforcier  (1000) users      (100)    10464 2023-07-28 18:49:31.000000 paramiko-3.3.0/docs/api/proxy.html
--rw-r--r--   0 jforcier  (1000) users      (100)    27239 2023-07-28 18:49:31.000000 paramiko-3.3.0/docs/api/message.html
--rw-r--r--   0 jforcier  (1000) users      (100)    26644 2023-07-28 18:49:31.000000 paramiko-3.3.0/docs/api/ssh_exception.html
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/.doctrees/
--rw-r--r--   0 jforcier  (1000) users      (100)    11039 2023-05-25 18:10:49.000000 paramiko-3.3.0/docs/.doctrees/index.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)  1697523 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/.doctrees/environment.pickle
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/.doctrees/api/
--rw-r--r--   0 jforcier  (1000) users      (100)   480515 2023-07-28 18:49:29.000000 paramiko-3.3.0/docs/.doctrees/api/sftp.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)    61218 2023-05-25 02:01:15.000000 paramiko-3.3.0/docs/.doctrees/api/message.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)   154955 2023-05-25 18:10:49.000000 paramiko-3.3.0/docs/.doctrees/api/ssh_gss.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)   399594 2023-07-28 18:49:30.000000 paramiko-3.3.0/docs/.doctrees/api/transport.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)   108867 2023-05-25 18:10:46.000000 paramiko-3.3.0/docs/.doctrees/api/auth.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)   149321 2023-05-25 18:10:47.000000 paramiko-3.3.0/docs/.doctrees/api/client.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)    58553 2023-05-25 18:10:49.000000 paramiko-3.3.0/docs/.doctrees/api/ssh_exception.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)   309076 2023-05-25 18:10:47.000000 paramiko-3.3.0/docs/.doctrees/api/keys.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)    33228 2023-05-25 02:01:13.000000 paramiko-3.3.0/docs/.doctrees/api/buffered_pipe.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)    10146 2023-05-25 02:01:15.000000 paramiko-3.3.0/docs/.doctrees/api/pipe.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)    96476 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/.doctrees/api/config.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)    15222 2023-05-25 18:10:48.000000 paramiko-3.3.0/docs/.doctrees/api/proxy.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)    39759 2023-05-25 18:10:48.000000 paramiko-3.3.0/docs/.doctrees/api/packet.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)    58315 2023-05-25 18:10:47.000000 paramiko-3.3.0/docs/.doctrees/api/hostkeys.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)    33898 2023-05-25 18:10:47.000000 paramiko-3.3.0/docs/.doctrees/api/kex_gss.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)   171421 2023-05-25 18:10:45.000000 paramiko-3.3.0/docs/.doctrees/api/agent.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)    57030 2023-05-25 02:01:15.000000 paramiko-3.3.0/docs/.doctrees/api/file.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)   215303 2023-05-25 18:10:46.000000 paramiko-3.3.0/docs/.doctrees/api/channel.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)   218366 2023-05-25 18:10:48.000000 paramiko-3.3.0/docs/.doctrees/api/server.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)    55629 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/searchindex.js
--rw-r--r--   0 jforcier  (1000) users      (100)      230 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/.buildinfo
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/_static/
--rw-r--r--   0 jforcier  (1000) users      (100)    10854 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/_static/language_data.js
--rw-r--r--   0 jforcier  (1000) users      (100)      350 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/_static/documentation_options.js
--rw-r--r--   0 jforcier  (1000) users      (100)    16793 2023-03-21 23:06:01.000000 paramiko-3.3.0/docs/_static/searchtools.js
--rw-r--r--   0 jforcier  (1000) users      (100)       90 2023-03-21 23:06:01.000000 paramiko-3.3.0/docs/_static/plus.png
--rw-r--r--   0 jforcier  (1000) users      (100)   287630 2023-03-21 23:06:01.000000 paramiko-3.3.0/docs/_static/jquery-3.5.1.js
--rw-r--r--   0 jforcier  (1000) users      (100)    89476 2023-03-21 23:06:01.000000 paramiko-3.3.0/docs/_static/jquery.js
--rw-r--r--   0 jforcier  (1000) users      (100)     5327 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/_static/pygments.css
--rw-r--r--   0 jforcier  (1000) users      (100)       90 2023-03-21 23:06:01.000000 paramiko-3.3.0/docs/_static/minus.png
--rw-r--r--   0 jforcier  (1000) users      (100)    68420 2023-03-21 23:06:01.000000 paramiko-3.3.0/docs/_static/underscore-1.13.1.js
--rw-r--r--   0 jforcier  (1000) users      (100)     9630 2023-03-21 23:06:01.000000 paramiko-3.3.0/docs/_static/doctools.js
--rw-r--r--   0 jforcier  (1000) users      (100)      286 2023-03-21 23:06:01.000000 paramiko-3.3.0/docs/_static/file.png
--rw-r--r--   0 jforcier  (1000) users      (100)    19530 2023-03-21 23:06:01.000000 paramiko-3.3.0/docs/_static/underscore.js
--rw-r--r--   0 jforcier  (1000) users      (100)    14667 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/_static/basic.css
--rw-r--r--   0 jforcier  (1000) users      (100)    11230 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/_static/alabaster.css
--rw-r--r--   0 jforcier  (1000) users      (100)       42 2023-03-21 23:06:01.000000 paramiko-3.3.0/docs/_static/custom.css
--rw-r--r--   0 jforcier  (1000) users      (100)     5039 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/objects.inv
--rw-r--r--   0 jforcier  (1000) users      (100)   108580 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/genindex.html
--rw-r--r--   0 jforcier  (1000) users      (100)     5893 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/search.html
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/_sources/
--rw-r--r--   0 jforcier  (1000) users      (100)     1937 2023-05-22 16:22:05.000000 paramiko-3.3.0/docs/_sources/index.rst.txt
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/_sources/api/
--rw-r--r--   0 jforcier  (1000) users      (100)       84 2021-11-27 02:56:36.000000 paramiko-3.3.0/docs/_sources/api/transport.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     4944 2023-07-28 18:47:01.000000 paramiko-3.3.0/docs/_sources/api/config.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       82 2021-11-27 02:56:36.000000 paramiko-3.3.0/docs/_sources/api/proxy.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      103 2021-11-27 02:56:36.000000 paramiko-3.3.0/docs/_sources/api/pipe.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      131 2021-11-27 02:56:36.000000 paramiko-3.3.0/docs/_sources/api/hostkeys.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      303 2022-04-25 12:16:45.000000 paramiko-3.3.0/docs/_sources/api/keys.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      104 2021-11-27 02:56:36.000000 paramiko-3.3.0/docs/_sources/api/kex_gss.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       75 2021-11-27 02:56:36.000000 paramiko-3.3.0/docs/_sources/api/client.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      181 2023-05-22 16:22:05.000000 paramiko-3.3.0/docs/_sources/api/auth.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      327 2021-11-27 02:56:36.000000 paramiko-3.3.0/docs/_sources/api/sftp.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       50 2021-11-27 02:56:36.000000 paramiko-3.3.0/docs/_sources/api/channel.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      339 2023-03-03 18:55:05.000000 paramiko-3.3.0/docs/_sources/api/ssh_gss.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       61 2021-11-27 02:56:36.000000 paramiko-3.3.0/docs/_sources/api/file.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       50 2021-11-27 02:56:36.000000 paramiko-3.3.0/docs/_sources/api/message.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      103 2021-11-27 02:56:36.000000 paramiko-3.3.0/docs/_sources/api/agent.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      105 2021-11-27 02:56:36.000000 paramiko-3.3.0/docs/_sources/api/server.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       70 2023-01-13 01:10:51.000000 paramiko-3.3.0/docs/_sources/api/buffered_pipe.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       62 2021-11-27 02:56:36.000000 paramiko-3.3.0/docs/_sources/api/ssh_exception.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       55 2021-11-27 02:56:36.000000 paramiko-3.3.0/docs/_sources/api/packet.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)    12430 2023-07-28 19:23:28.000000 paramiko-3.3.0/docs/py-modindex.html
--rw-r--r--   0 jforcier  (1000) users      (100)    26436 2021-11-27 02:56:36.000000 paramiko-3.3.0/LICENSE
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 19:23:28.000000 paramiko-3.3.0/paramiko.egg-info/
--rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-07-28 19:23:28.000000 paramiko-3.3.0/paramiko.egg-info/dependency_links.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      340 2023-07-28 19:23:28.000000 paramiko-3.3.0/paramiko.egg-info/requires.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     6596 2023-07-28 19:23:28.000000 paramiko-3.3.0/paramiko.egg-info/SOURCES.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        9 2023-07-28 19:23:28.000000 paramiko-3.3.0/paramiko.egg-info/top_level.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     4185 2023-07-28 19:23:28.000000 paramiko-3.3.0/paramiko.egg-info/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-05-25 18:00:56.000000 paramiko-3.3.0/pytest.ini
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 19:23:28.000000 paramiko-3.3.0/tests/
--rw-r--r--   0 jforcier  (1000) users      (100)     2875 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/_loop.py
--rw-r--r--   0 jforcier  (1000) users      (100)      314 2021-11-27 02:56:36.000000 paramiko-3.3.0/tests/test_ecdsa_password_256.key
--rw-r--r--   0 jforcier  (1000) users      (100)      667 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/test_ecdsa_384_openssh.key
--rw-r--r--   0 jforcier  (1000) users      (100)     5950 2023-04-27 20:59:22.000000 paramiko-3.3.0/tests/test_proxy.py
--rw-r--r--   0 jforcier  (1000) users      (100)    30045 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/test_sftp.py
--rw-r--r--   0 jforcier  (1000) users      (100)      484 2022-04-25 12:16:45.000000 paramiko-3.3.0/tests/test_ed25519_password.key
--rw-r--r--   0 jforcier  (1000) users      (100)     8574 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/test_gssapi.py
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/blank_rsa.key
--rw-r--r--   0 jforcier  (1000) users      (100)    33006 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/test_pkey.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1876 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/test_rsa_openssh.key
--rw-r--r--   0 jforcier  (1000) users      (100)     1799 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/test_rsa_openssh_nopad.key
--rw-r--r--   0 jforcier  (1000) users      (100)    22311 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/auth.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1852 2023-04-27 20:59:22.000000 paramiko-3.3.0/tests/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1904 2023-04-27 20:59:22.000000 paramiko-3.3.0/tests/test_channelfile.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4432 2023-04-27 20:59:22.000000 paramiko-3.3.0/tests/test_message.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2638 2023-04-27 20:59:22.000000 paramiko-3.3.0/tests/test_buffered_pipe.py
--rw-r--r--   0 jforcier  (1000) users      (100)      288 2021-11-27 02:56:36.000000 paramiko-3.3.0/tests/test_ecdsa_384.key
--rw-r--r--   0 jforcier  (1000) users      (100)    45263 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/test_transport.py
--rw-r--r--   0 jforcier  (1000) users      (100)      444 2021-11-27 02:56:36.000000 paramiko-3.3.0/tests/test_ecdsa_password_521.key
--rw-r--r--   0 jforcier  (1000) users      (100)    36589 2023-07-28 18:55:00.000000 paramiko-3.3.0/tests/test_config.py
--rw-r--r--   0 jforcier  (1000) users      (100)    36976 2023-04-27 20:59:22.000000 paramiko-3.3.0/tests/test_kex.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5468 2023-05-26 14:16:03.000000 paramiko-3.3.0/tests/test_ssh_gss.py
--rw-r--r--   0 jforcier  (1000) users      (100)      387 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/badhash_key1.ed25519.key
--rw-r--r--   0 jforcier  (1000) users      (100)    14132 2023-06-09 17:41:24.000000 paramiko-3.3.0/tests/_util.py
--rw-r--r--   0 jforcier  (1000) users      (100)      464 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/test_ed25519-funky-padding_password.key
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 19:23:28.000000 paramiko-3.3.0/tests/_support/
--rw-r--r--   0 jforcier  (1000) users      (100)      883 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/_support/rsa-lonely.key
--rw-r--r--   0 jforcier  (1000) users      (100)      668 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/_support/dss.key
--rw-r--r--   0 jforcier  (1000) users      (100)     1209 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/_support/ed25519.key-cert.pub
--rw-r--r--   0 jforcier  (1000) users      (100)      432 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/_support/ed25519.key
--rw-r--r--   0 jforcier  (1000) users      (100)      883 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/_support/rsa.key
--rw-r--r--   0 jforcier  (1000) users      (100)     1035 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/_support/rsa-missing.key-cert.pub
--rw-r--r--   0 jforcier  (1000) users      (100)     1713 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/_support/dss.key-cert.pub
--rw-r--r--   0 jforcier  (1000) users      (100)     1035 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/_support/rsa.key-cert.pub
--rw-r--r--   0 jforcier  (1000) users      (100)     1291 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/_support/ecdsa-256.key-cert.pub
--rw-r--r--   0 jforcier  (1000) users      (100)      156 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/_support/ed448.key
--rw-r--r--   0 jforcier  (1000) users      (100)      227 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/_support/ecdsa-256.key
--rw-r--r--   0 jforcier  (1000) users      (100)    15272 2023-06-09 17:41:24.000000 paramiko-3.3.0/tests/test_sftp_big.py
--rw-r--r--   0 jforcier  (1000) users      (100)      209 2022-04-25 12:16:45.000000 paramiko-3.3.0/tests/test_rsa.key.pub
--rw-r--r--   0 jforcier  (1000) users      (100)     5302 2023-05-26 14:16:03.000000 paramiko-3.3.0/tests/test_kex_gss.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7208 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/test_file.py
--rw-r--r--   0 jforcier  (1000) users      (100)     6027 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/conftest.py
--rw-r--r--   0 jforcier  (1000) users      (100)      951 2021-11-27 02:56:36.000000 paramiko-3.3.0/tests/test_rsa_password.key
--rw-r--r--   0 jforcier  (1000) users      (100)     9714 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/pkey.py
--rw-r--r--   0 jforcier  (1000) users      (100)      736 2021-11-27 02:56:36.000000 paramiko-3.3.0/tests/test_dss_password.key
--rw-r--r--   0 jforcier  (1000) users      (100)     7453 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/_stub_sftp.py
--rw-r--r--   0 jforcier  (1000) users      (100)      399 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/test_ed25519-funky-padding.key
--rw-r--r--   0 jforcier  (1000) users      (100)      387 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/badhash_key2.ed25519.key
--rw-r--r--   0 jforcier  (1000) users      (100)     7247 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/test_hostkeys.py
--rw-r--r--   0 jforcier  (1000) users      (100)     6046 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/agent.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5095 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/test_packetizer.py
--rw-r--r--   0 jforcier  (1000) users      (100)    31084 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/test_client.py
--rw-r--r--   0 jforcier  (1000) users      (100)      365 2021-11-27 02:56:36.000000 paramiko-3.3.0/tests/test_ecdsa_521.key
--rw-r--r--   0 jforcier  (1000) users      (100)      379 2021-11-27 02:56:36.000000 paramiko-3.3.0/tests/test_ecdsa_password_384.key
--rw-r--r--   0 jforcier  (1000) users      (100)     4758 2023-05-25 18:00:56.000000 paramiko-3.3.0/tests/test_util.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2798 2023-04-27 20:59:22.000000 paramiko-3.3.0/tests/test_ssh_exception.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1458 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/test_dss_openssh.key
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 19:23:28.000000 paramiko-3.3.0/tests/configs/
--rw-r--r--   0 jforcier  (1000) users      (100)       92 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/no-canon
--rw-r--r--   0 jforcier  (1000) users      (100)       19 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/hostname-tokenized
--rw-r--r--   0 jforcier  (1000) users      (100)       96 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/canon-always
--rw-r--r--   0 jforcier  (1000) users      (100)      121 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-host-glob-list
--rw-r--r--   0 jforcier  (1000) users      (100)       27 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-all
--rw-r--r--   0 jforcier  (1000) users      (100)       33 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-host-glob
--rw-r--r--   0 jforcier  (1000) users      (100)      108 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/multi-canon-domains
--rw-r--r--   0 jforcier  (1000) users      (100)       99 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-host-from-match
--rw-r--r--   0 jforcier  (1000) users      (100)      262 2023-07-28 18:55:00.000000 paramiko-3.3.0/tests/configs/match-final
--rw-r--r--   0 jforcier  (1000) users      (100)      253 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-orighost
--rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/invalid
--rw-r--r--   0 jforcier  (1000) users      (100)      290 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-exec
--rw-r--r--   0 jforcier  (1000) users      (100)      156 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/zero-maxdots
--rw-r--r--   0 jforcier  (1000) users      (100)      113 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/canon-local-always
--rw-r--r--   0 jforcier  (1000) users      (100)       26 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-exec-no-arg
--rw-r--r--   0 jforcier  (1000) users      (100)       81 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-exec-negation
--rw-r--r--   0 jforcier  (1000) users      (100)       25 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-user-no-arg
--rw-r--r--   0 jforcier  (1000) users      (100)       33 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-orighost-no-arg
--rw-r--r--   0 jforcier  (1000) users      (100)      224 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-localuser
--rw-r--r--   0 jforcier  (1000) users      (100)       93 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-all-after-canonical
--rw-r--r--   0 jforcier  (1000) users      (100)       30 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-host-negated
--rw-r--r--   0 jforcier  (1000) users      (100)      206 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/deep-canon-maxdots
--rw-r--r--   0 jforcier  (1000) users      (100)      259 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-exec-canonical
--rw-r--r--   0 jforcier  (1000) users      (100)       30 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-localuser-no-arg
--rw-r--r--   0 jforcier  (1000) users      (100)      110 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/canon-local
--rw-r--r--   0 jforcier  (1000) users      (100)      320 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/robey
--rw-r--r--   0 jforcier  (1000) users      (100)       48 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-all-and-more-before
--rw-r--r--   0 jforcier  (1000) users      (100)      152 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-host-canonicalized
--rw-r--r--   0 jforcier  (1000) users      (100)       25 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-host-no-arg
--rw-r--r--   0 jforcier  (1000) users      (100)       32 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-host
--rw-r--r--   0 jforcier  (1000) users      (100)      122 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/fallback-no
--rw-r--r--   0 jforcier  (1000) users      (100)       48 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-all-and-more
--rw-r--r--   0 jforcier  (1000) users      (100)      184 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/deep-canon
--rw-r--r--   0 jforcier  (1000) users      (100)       53 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-user-explicit
--rw-r--r--   0 jforcier  (1000) users      (100)      151 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/canon
--rw-r--r--   0 jforcier  (1000) users      (100)       68 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/basic
--rw-r--r--   0 jforcier  (1000) users      (100)       93 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-orighost-canonical
--rw-r--r--   0 jforcier  (1000) users      (100)      123 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/fallback-yes
--rw-r--r--   0 jforcier  (1000) users      (100)      112 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/canon-ipv4
--rw-r--r--   0 jforcier  (1000) users      (100)      400 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-complex
--rw-r--r--   0 jforcier  (1000) users      (100)       99 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-canonical-yes
--rw-r--r--   0 jforcier  (1000) users      (100)       62 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-host-name
--rw-r--r--   0 jforcier  (1000) users      (100)      199 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-user
--rw-r--r--   0 jforcier  (1000) users      (100)       99 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/empty-canon
--rw-r--r--   0 jforcier  (1000) users      (100)       90 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-all-before-canonical
--rw-r--r--   0 jforcier  (1000) users      (100)      112 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/match-canonical-no
--rw-r--r--   0 jforcier  (1000) users      (100)       46 2023-03-03 18:55:05.000000 paramiko-3.3.0/tests/configs/hostname-exec-tokenized
--rw-r--r--   0 jforcier  (1000) users      (100)     3289 2023-03-03 18:55:05.000000 paramiko-3.3.0/setup.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2360 2023-05-25 18:00:56.000000 paramiko-3.3.0/README.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 19:23:28.000000 paramiko-3.3.0/demos/
--rw-r--r--   0 jforcier  (1000) users      (100)     4076 2023-03-03 18:55:05.000000 paramiko-3.3.0/demos/demo_sftp.py
--rw-r--r--   0 jforcier  (1000) users      (100)      883 2021-11-27 02:56:36.000000 paramiko-3.3.0/demos/test_rsa.key
--rw-r--r--   0 jforcier  (1000) users      (100)     5914 2023-03-03 18:55:05.000000 paramiko-3.3.0/demos/demo_server.py
--rwxr-xr-x   0 jforcier  (1000) users      (100)     4761 2023-03-03 18:55:05.000000 paramiko-3.3.0/demos/demo_keygen.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2780 2023-03-03 18:55:05.000000 paramiko-3.3.0/demos/interactive.py
--rwxr-xr-x   0 jforcier  (1000) users      (100)     6367 2023-03-03 18:55:05.000000 paramiko-3.3.0/demos/rforward.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3364 2023-03-03 18:55:05.000000 paramiko-3.3.0/demos/demo_simple.py
--rw-r--r--   0 jforcier  (1000) users      (100)      229 2021-11-27 02:56:36.000000 paramiko-3.3.0/demos/user_rsa_key.pub
--rw-r--r--   0 jforcier  (1000) users      (100)     7254 2023-03-03 18:55:05.000000 paramiko-3.3.0/demos/forward.py
--rwxr-xr-x   0 jforcier  (1000) users      (100)     5453 2023-03-03 18:55:05.000000 paramiko-3.3.0/demos/demo.py
--rw-r--r--   0 jforcier  (1000) users      (100)      887 2021-11-27 02:56:36.000000 paramiko-3.3.0/demos/user_rsa_key
--rw-r--r--   0 jforcier  (1000) users      (100)     4185 2023-07-28 19:23:28.000000 paramiko-3.3.0/PKG-INFO
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 20:15:35.000000 paramiko-3.3.1/
+-rw-r--r--   0 jforcier  (1000) users      (100)     3289 2023-03-03 18:55:05.000000 paramiko-3.3.1/setup.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4185 2023-07-28 20:15:35.000000 paramiko-3.3.1/PKG-INFO
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 20:15:35.000000 paramiko-3.3.1/tests/
+-rw-r--r--   0 jforcier  (1000) users      (100)    22311 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/auth.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8574 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/test_gssapi.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      288 2021-11-27 02:56:36.000000 paramiko-3.3.1/tests/test_ecdsa_384.key
+-rw-r--r--   0 jforcier  (1000) users      (100)     6046 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/agent.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4432 2023-04-27 20:59:22.000000 paramiko-3.3.1/tests/test_message.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      387 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/badhash_key2.ed25519.key
+-rw-r--r--   0 jforcier  (1000) users      (100)     5468 2023-05-26 14:16:03.000000 paramiko-3.3.1/tests/test_ssh_gss.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4758 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/test_util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1876 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/test_rsa_openssh.key
+-rw-r--r--   0 jforcier  (1000) users      (100)     5302 2023-05-26 14:16:03.000000 paramiko-3.3.1/tests/test_kex_gss.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      399 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/test_ed25519-funky-padding.key
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/blank_rsa.key
+-rw-r--r--   0 jforcier  (1000) users      (100)    15272 2023-06-09 17:41:24.000000 paramiko-3.3.1/tests/test_sftp_big.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      209 2022-04-25 12:16:45.000000 paramiko-3.3.1/tests/test_rsa.key.pub
+-rw-r--r--   0 jforcier  (1000) users      (100)     2638 2023-04-27 20:59:22.000000 paramiko-3.3.1/tests/test_buffered_pipe.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      379 2021-11-27 02:56:36.000000 paramiko-3.3.1/tests/test_ecdsa_password_384.key
+-rw-r--r--   0 jforcier  (1000) users      (100)      464 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/test_ed25519-funky-padding_password.key
+-rw-r--r--   0 jforcier  (1000) users      (100)     5950 2023-04-27 20:59:22.000000 paramiko-3.3.1/tests/test_proxy.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    36589 2023-07-28 18:55:00.000000 paramiko-3.3.1/tests/test_config.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      484 2022-04-25 12:16:45.000000 paramiko-3.3.1/tests/test_ed25519_password.key
+-rw-r--r--   0 jforcier  (1000) users      (100)     7247 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/test_hostkeys.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      667 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/test_ecdsa_384_openssh.key
+-rw-r--r--   0 jforcier  (1000) users      (100)     6027 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/conftest.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      314 2021-11-27 02:56:36.000000 paramiko-3.3.1/tests/test_ecdsa_password_256.key
+-rw-r--r--   0 jforcier  (1000) users      (100)      736 2021-11-27 02:56:36.000000 paramiko-3.3.1/tests/test_dss_password.key
+-rw-r--r--   0 jforcier  (1000) users      (100)    45263 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/test_transport.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      365 2021-11-27 02:56:36.000000 paramiko-3.3.1/tests/test_ecdsa_521.key
+-rw-r--r--   0 jforcier  (1000) users      (100)     7208 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/test_file.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    36976 2023-04-27 20:59:22.000000 paramiko-3.3.1/tests/test_kex.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      951 2021-11-27 02:56:36.000000 paramiko-3.3.1/tests/test_rsa_password.key
+-rw-r--r--   0 jforcier  (1000) users      (100)    31084 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/test_client.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1799 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/test_rsa_openssh_nopad.key
+-rw-r--r--   0 jforcier  (1000) users      (100)     9714 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/pkey.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1852 2023-04-27 20:59:22.000000 paramiko-3.3.1/tests/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2875 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/_loop.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 20:15:35.000000 paramiko-3.3.1/tests/configs/
+-rw-r--r--   0 jforcier  (1000) users      (100)       93 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-all-after-canonical
+-rw-r--r--   0 jforcier  (1000) users      (100)      112 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-canonical-no
+-rw-r--r--   0 jforcier  (1000) users      (100)      199 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-user
+-rw-r--r--   0 jforcier  (1000) users      (100)       99 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/empty-canon
+-rw-r--r--   0 jforcier  (1000) users      (100)       93 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-orighost-canonical
+-rw-r--r--   0 jforcier  (1000) users      (100)      259 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-exec-canonical
+-rw-r--r--   0 jforcier  (1000) users      (100)       68 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/basic
+-rw-r--r--   0 jforcier  (1000) users      (100)       33 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-host-glob
+-rw-r--r--   0 jforcier  (1000) users      (100)      108 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/multi-canon-domains
+-rw-r--r--   0 jforcier  (1000) users      (100)      112 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/canon-ipv4
+-rw-r--r--   0 jforcier  (1000) users      (100)      156 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/zero-maxdots
+-rw-r--r--   0 jforcier  (1000) users      (100)       99 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-host-from-match
+-rw-r--r--   0 jforcier  (1000) users      (100)       32 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-host
+-rw-r--r--   0 jforcier  (1000) users      (100)      152 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-host-canonicalized
+-rw-r--r--   0 jforcier  (1000) users      (100)      184 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/deep-canon
+-rw-r--r--   0 jforcier  (1000) users      (100)      151 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/canon
+-rw-r--r--   0 jforcier  (1000) users      (100)       90 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-all-before-canonical
+-rw-r--r--   0 jforcier  (1000) users      (100)       48 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-all-and-more
+-rw-r--r--   0 jforcier  (1000) users      (100)      122 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/fallback-no
+-rw-r--r--   0 jforcier  (1000) users      (100)       33 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-orighost-no-arg
+-rw-r--r--   0 jforcier  (1000) users      (100)       81 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-exec-negation
+-rw-r--r--   0 jforcier  (1000) users      (100)      320 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/robey
+-rw-r--r--   0 jforcier  (1000) users      (100)       96 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/canon-always
+-rw-r--r--   0 jforcier  (1000) users      (100)       25 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-host-no-arg
+-rw-r--r--   0 jforcier  (1000) users      (100)      224 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-localuser
+-rw-r--r--   0 jforcier  (1000) users      (100)       27 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-all
+-rw-r--r--   0 jforcier  (1000) users      (100)      110 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/canon-local
+-rw-r--r--   0 jforcier  (1000) users      (100)      121 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-host-glob-list
+-rw-r--r--   0 jforcier  (1000) users      (100)      206 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/deep-canon-maxdots
+-rw-r--r--   0 jforcier  (1000) users      (100)       30 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-host-negated
+-rw-r--r--   0 jforcier  (1000) users      (100)       25 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-user-no-arg
+-rw-r--r--   0 jforcier  (1000) users      (100)      123 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/fallback-yes
+-rw-r--r--   0 jforcier  (1000) users      (100)      290 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-exec
+-rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/invalid
+-rw-r--r--   0 jforcier  (1000) users      (100)      113 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/canon-local-always
+-rw-r--r--   0 jforcier  (1000) users      (100)       30 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-localuser-no-arg
+-rw-r--r--   0 jforcier  (1000) users      (100)       26 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-exec-no-arg
+-rw-r--r--   0 jforcier  (1000) users      (100)       53 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-user-explicit
+-rw-r--r--   0 jforcier  (1000) users      (100)       46 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/hostname-exec-tokenized
+-rw-r--r--   0 jforcier  (1000) users      (100)       92 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/no-canon
+-rw-r--r--   0 jforcier  (1000) users      (100)      253 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-orighost
+-rw-r--r--   0 jforcier  (1000) users      (100)      262 2023-07-28 18:55:00.000000 paramiko-3.3.1/tests/configs/match-final
+-rw-r--r--   0 jforcier  (1000) users      (100)       99 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-canonical-yes
+-rw-r--r--   0 jforcier  (1000) users      (100)      400 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-complex
+-rw-r--r--   0 jforcier  (1000) users      (100)       19 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/hostname-tokenized
+-rw-r--r--   0 jforcier  (1000) users      (100)       62 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-host-name
+-rw-r--r--   0 jforcier  (1000) users      (100)       48 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/configs/match-all-and-more-before
+-rw-r--r--   0 jforcier  (1000) users      (100)     2798 2023-04-27 20:59:22.000000 paramiko-3.3.1/tests/test_ssh_exception.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 20:15:35.000000 paramiko-3.3.1/tests/_support/
+-rw-r--r--   0 jforcier  (1000) users      (100)     1713 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/_support/dss.key-cert.pub
+-rw-r--r--   0 jforcier  (1000) users      (100)     1291 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/_support/ecdsa-256.key-cert.pub
+-rw-r--r--   0 jforcier  (1000) users      (100)     1035 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/_support/rsa.key-cert.pub
+-rw-r--r--   0 jforcier  (1000) users      (100)      156 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/_support/ed448.key
+-rw-r--r--   0 jforcier  (1000) users      (100)     1035 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/_support/rsa-missing.key-cert.pub
+-rw-r--r--   0 jforcier  (1000) users      (100)      432 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/_support/ed25519.key
+-rw-r--r--   0 jforcier  (1000) users      (100)      883 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/_support/rsa.key
+-rw-r--r--   0 jforcier  (1000) users      (100)     1209 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/_support/ed25519.key-cert.pub
+-rw-r--r--   0 jforcier  (1000) users      (100)      227 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/_support/ecdsa-256.key
+-rw-r--r--   0 jforcier  (1000) users      (100)      668 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/_support/dss.key
+-rw-r--r--   0 jforcier  (1000) users      (100)      883 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/_support/rsa-lonely.key
+-rw-r--r--   0 jforcier  (1000) users      (100)    14132 2023-06-09 17:41:24.000000 paramiko-3.3.1/tests/_util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      387 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/badhash_key1.ed25519.key
+-rw-r--r--   0 jforcier  (1000) users      (100)      444 2021-11-27 02:56:36.000000 paramiko-3.3.1/tests/test_ecdsa_password_521.key
+-rw-r--r--   0 jforcier  (1000) users      (100)    33006 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/test_pkey.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1458 2023-03-03 18:55:05.000000 paramiko-3.3.1/tests/test_dss_openssh.key
+-rw-r--r--   0 jforcier  (1000) users      (100)    30045 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/test_sftp.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5095 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/test_packetizer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1904 2023-04-27 20:59:22.000000 paramiko-3.3.1/tests/test_channelfile.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7453 2023-05-25 18:00:56.000000 paramiko-3.3.1/tests/_stub_sftp.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 20:15:35.000000 paramiko-3.3.1/demos/
+-rw-r--r--   0 jforcier  (1000) users      (100)     2780 2023-03-03 18:55:05.000000 paramiko-3.3.1/demos/interactive.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5914 2023-03-03 18:55:05.000000 paramiko-3.3.1/demos/demo_server.py
+-rwxr-xr-x   0 jforcier  (1000) users      (100)     4761 2023-03-03 18:55:05.000000 paramiko-3.3.1/demos/demo_keygen.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      883 2021-11-27 02:56:36.000000 paramiko-3.3.1/demos/test_rsa.key
+-rw-r--r--   0 jforcier  (1000) users      (100)     4076 2023-03-03 18:55:05.000000 paramiko-3.3.1/demos/demo_sftp.py
+-rwxr-xr-x   0 jforcier  (1000) users      (100)     6367 2023-03-03 18:55:05.000000 paramiko-3.3.1/demos/rforward.py
+-rwxr-xr-x   0 jforcier  (1000) users      (100)     5453 2023-03-03 18:55:05.000000 paramiko-3.3.1/demos/demo.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      887 2021-11-27 02:56:36.000000 paramiko-3.3.1/demos/user_rsa_key
+-rw-r--r--   0 jforcier  (1000) users      (100)      229 2021-11-27 02:56:36.000000 paramiko-3.3.1/demos/user_rsa_key.pub
+-rw-r--r--   0 jforcier  (1000) users      (100)     7254 2023-03-03 18:55:05.000000 paramiko-3.3.1/demos/forward.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3364 2023-03-03 18:55:05.000000 paramiko-3.3.1/demos/demo_simple.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 20:15:35.000000 paramiko-3.3.1/paramiko.egg-info/
+-rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-07-28 20:15:35.000000 paramiko-3.3.1/paramiko.egg-info/dependency_links.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)        9 2023-07-28 20:15:35.000000 paramiko-3.3.1/paramiko.egg-info/top_level.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     6596 2023-07-28 20:15:35.000000 paramiko-3.3.1/paramiko.egg-info/SOURCES.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     4185 2023-07-28 20:15:35.000000 paramiko-3.3.1/paramiko.egg-info/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)      340 2023-07-28 20:15:35.000000 paramiko-3.3.1/paramiko.egg-info/requires.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-07-28 20:15:35.000000 paramiko-3.3.1/setup.cfg
+-rw-r--r--   0 jforcier  (1000) users      (100)      208 2023-05-25 18:00:56.000000 paramiko-3.3.1/MANIFEST.in
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 20:15:35.000000 paramiko-3.3.1/docs/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 20:15:35.000000 paramiko-3.3.1/docs/_static/
+-rw-r--r--   0 jforcier  (1000) users      (100)    10854 2023-07-28 19:23:28.000000 paramiko-3.3.1/docs/_static/language_data.js
+-rw-r--r--   0 jforcier  (1000) users      (100)    11230 2023-07-28 19:23:28.000000 paramiko-3.3.1/docs/_static/alabaster.css
+-rw-r--r--   0 jforcier  (1000) users      (100)       42 2023-03-21 23:06:01.000000 paramiko-3.3.1/docs/_static/custom.css
+-rw-r--r--   0 jforcier  (1000) users      (100)    19530 2023-03-21 23:06:01.000000 paramiko-3.3.1/docs/_static/underscore.js
+-rw-r--r--   0 jforcier  (1000) users      (100)   287630 2023-03-21 23:06:01.000000 paramiko-3.3.1/docs/_static/jquery-3.5.1.js
+-rw-r--r--   0 jforcier  (1000) users      (100)      350 2023-07-28 19:23:28.000000 paramiko-3.3.1/docs/_static/documentation_options.js
+-rw-r--r--   0 jforcier  (1000) users      (100)     9630 2023-03-21 23:06:01.000000 paramiko-3.3.1/docs/_static/doctools.js
+-rw-r--r--   0 jforcier  (1000) users      (100)    89476 2023-03-21 23:06:01.000000 paramiko-3.3.1/docs/_static/jquery.js
+-rw-r--r--   0 jforcier  (1000) users      (100)       90 2023-03-21 23:06:01.000000 paramiko-3.3.1/docs/_static/plus.png
+-rw-r--r--   0 jforcier  (1000) users      (100)    68420 2023-03-21 23:06:01.000000 paramiko-3.3.1/docs/_static/underscore-1.13.1.js
+-rw-r--r--   0 jforcier  (1000) users      (100)       90 2023-03-21 23:06:01.000000 paramiko-3.3.1/docs/_static/minus.png
+-rw-r--r--   0 jforcier  (1000) users      (100)    14667 2023-07-28 19:23:28.000000 paramiko-3.3.1/docs/_static/basic.css
+-rw-r--r--   0 jforcier  (1000) users      (100)    16793 2023-03-21 23:06:01.000000 paramiko-3.3.1/docs/_static/searchtools.js
+-rw-r--r--   0 jforcier  (1000) users      (100)     5327 2023-07-28 19:23:28.000000 paramiko-3.3.1/docs/_static/pygments.css
+-rw-r--r--   0 jforcier  (1000) users      (100)      286 2023-03-21 23:06:01.000000 paramiko-3.3.1/docs/_static/file.png
+-rw-r--r--   0 jforcier  (1000) users      (100)    12430 2023-07-28 19:23:28.000000 paramiko-3.3.1/docs/py-modindex.html
+-rw-r--r--   0 jforcier  (1000) users      (100)     5039 2023-07-28 19:23:28.000000 paramiko-3.3.1/docs/objects.inv
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 20:15:35.000000 paramiko-3.3.1/docs/_sources/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 20:15:35.000000 paramiko-3.3.1/docs/_sources/api/
+-rw-r--r--   0 jforcier  (1000) users      (100)       62 2021-11-27 02:56:36.000000 paramiko-3.3.1/docs/_sources/api/ssh_exception.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     4944 2023-07-28 18:47:01.000000 paramiko-3.3.1/docs/_sources/api/config.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       70 2023-01-13 01:10:51.000000 paramiko-3.3.1/docs/_sources/api/buffered_pipe.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       50 2021-11-27 02:56:36.000000 paramiko-3.3.1/docs/_sources/api/channel.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       61 2021-11-27 02:56:36.000000 paramiko-3.3.1/docs/_sources/api/file.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       84 2021-11-27 02:56:36.000000 paramiko-3.3.1/docs/_sources/api/transport.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      103 2021-11-27 02:56:36.000000 paramiko-3.3.1/docs/_sources/api/agent.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      104 2021-11-27 02:56:36.000000 paramiko-3.3.1/docs/_sources/api/kex_gss.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       75 2021-11-27 02:56:36.000000 paramiko-3.3.1/docs/_sources/api/client.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      181 2023-05-22 16:22:05.000000 paramiko-3.3.1/docs/_sources/api/auth.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      131 2021-11-27 02:56:36.000000 paramiko-3.3.1/docs/_sources/api/hostkeys.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      105 2021-11-27 02:56:36.000000 paramiko-3.3.1/docs/_sources/api/server.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      327 2021-11-27 02:56:36.000000 paramiko-3.3.1/docs/_sources/api/sftp.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      339 2023-03-03 18:55:05.000000 paramiko-3.3.1/docs/_sources/api/ssh_gss.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       50 2021-11-27 02:56:36.000000 paramiko-3.3.1/docs/_sources/api/message.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       55 2021-11-27 02:56:36.000000 paramiko-3.3.1/docs/_sources/api/packet.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      103 2021-11-27 02:56:36.000000 paramiko-3.3.1/docs/_sources/api/pipe.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       82 2021-11-27 02:56:36.000000 paramiko-3.3.1/docs/_sources/api/proxy.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      303 2022-04-25 12:16:45.000000 paramiko-3.3.1/docs/_sources/api/keys.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     1937 2023-05-22 16:22:05.000000 paramiko-3.3.1/docs/_sources/index.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)   108580 2023-07-28 19:23:28.000000 paramiko-3.3.1/docs/genindex.html
+-rw-r--r--   0 jforcier  (1000) users      (100)    12628 2023-07-28 19:23:28.000000 paramiko-3.3.1/docs/index.html
+-rw-r--r--   0 jforcier  (1000) users      (100)     5893 2023-07-28 19:23:28.000000 paramiko-3.3.1/docs/search.html
+-rw-r--r--   0 jforcier  (1000) users      (100)      230 2023-07-28 19:23:28.000000 paramiko-3.3.1/docs/.buildinfo
+-rw-r--r--   0 jforcier  (1000) users      (100)    55629 2023-07-28 19:23:28.000000 paramiko-3.3.1/docs/searchindex.js
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 20:15:35.000000 paramiko-3.3.1/docs/api/
+-rw-r--r--   0 jforcier  (1000) users      (100)   151247 2023-07-28 18:49:32.000000 paramiko-3.3.1/docs/api/transport.html
+-rw-r--r--   0 jforcier  (1000) users      (100)    15714 2023-07-28 18:49:31.000000 paramiko-3.3.1/docs/api/kex_gss.html
+-rw-r--r--   0 jforcier  (1000) users      (100)    68501 2023-07-28 18:49:30.000000 paramiko-3.3.1/docs/api/agent.html
+-rw-r--r--   0 jforcier  (1000) users      (100)    42833 2023-07-28 19:23:28.000000 paramiko-3.3.1/docs/api/config.html
+-rw-r--r--   0 jforcier  (1000) users      (100)    89315 2023-07-28 18:49:30.000000 paramiko-3.3.1/docs/api/channel.html
+-rw-r--r--   0 jforcier  (1000) users      (100)    26848 2023-07-28 18:49:31.000000 paramiko-3.3.1/docs/api/hostkeys.html
+-rw-r--r--   0 jforcier  (1000) users      (100)    44986 2023-07-28 18:49:30.000000 paramiko-3.3.1/docs/api/auth.html
+-rw-r--r--   0 jforcier  (1000) users      (100)    19937 2023-07-28 18:49:31.000000 paramiko-3.3.1/docs/api/packet.html
+-rw-r--r--   0 jforcier  (1000) users      (100)   180584 2023-07-28 18:49:31.000000 paramiko-3.3.1/docs/api/sftp.html
+-rw-r--r--   0 jforcier  (1000) users      (100)    61123 2023-07-28 18:49:30.000000 paramiko-3.3.1/docs/api/client.html
+-rw-r--r--   0 jforcier  (1000) users      (100)     8827 2023-07-28 18:49:31.000000 paramiko-3.3.1/docs/api/pipe.html
+-rw-r--r--   0 jforcier  (1000) users      (100)    57007 2023-07-28 18:49:31.000000 paramiko-3.3.1/docs/api/ssh_gss.html
+-rw-r--r--   0 jforcier  (1000) users      (100)    86230 2023-07-28 18:49:31.000000 paramiko-3.3.1/docs/api/server.html
+-rw-r--r--   0 jforcier  (1000) users      (100)    17417 2023-07-28 18:49:30.000000 paramiko-3.3.1/docs/api/buffered_pipe.html
+-rw-r--r--   0 jforcier  (1000) users      (100)    26644 2023-07-28 18:49:31.000000 paramiko-3.3.1/docs/api/ssh_exception.html
+-rw-r--r--   0 jforcier  (1000) users      (100)    27239 2023-07-28 18:49:31.000000 paramiko-3.3.1/docs/api/message.html
+-rw-r--r--   0 jforcier  (1000) users      (100)    10464 2023-07-28 18:49:31.000000 paramiko-3.3.1/docs/api/proxy.html
+-rw-r--r--   0 jforcier  (1000) users      (100)    26728 2023-07-28 18:49:31.000000 paramiko-3.3.1/docs/api/file.html
+-rw-r--r--   0 jforcier  (1000) users      (100)   118448 2023-07-28 18:49:31.000000 paramiko-3.3.1/docs/api/keys.html
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 20:15:35.000000 paramiko-3.3.1/docs/.doctrees/
+-rw-r--r--   0 jforcier  (1000) users      (100)  1697523 2023-07-28 19:23:28.000000 paramiko-3.3.1/docs/.doctrees/environment.pickle
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 20:15:35.000000 paramiko-3.3.1/docs/.doctrees/api/
+-rw-r--r--   0 jforcier  (1000) users      (100)    33228 2023-05-25 02:01:13.000000 paramiko-3.3.1/docs/.doctrees/api/buffered_pipe.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)   480515 2023-07-28 18:49:29.000000 paramiko-3.3.1/docs/.doctrees/api/sftp.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)   108867 2023-05-25 18:10:46.000000 paramiko-3.3.1/docs/.doctrees/api/auth.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)   399594 2023-07-28 18:49:30.000000 paramiko-3.3.1/docs/.doctrees/api/transport.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)   218366 2023-05-25 18:10:48.000000 paramiko-3.3.1/docs/.doctrees/api/server.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)    39759 2023-05-25 18:10:48.000000 paramiko-3.3.1/docs/.doctrees/api/packet.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)   171421 2023-05-25 18:10:45.000000 paramiko-3.3.1/docs/.doctrees/api/agent.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)    33898 2023-05-25 18:10:47.000000 paramiko-3.3.1/docs/.doctrees/api/kex_gss.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)   309076 2023-05-25 18:10:47.000000 paramiko-3.3.1/docs/.doctrees/api/keys.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)    10146 2023-05-25 02:01:15.000000 paramiko-3.3.1/docs/.doctrees/api/pipe.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)    58553 2023-05-25 18:10:49.000000 paramiko-3.3.1/docs/.doctrees/api/ssh_exception.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)   215303 2023-05-25 18:10:46.000000 paramiko-3.3.1/docs/.doctrees/api/channel.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)    61218 2023-05-25 02:01:15.000000 paramiko-3.3.1/docs/.doctrees/api/message.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)   154955 2023-05-25 18:10:49.000000 paramiko-3.3.1/docs/.doctrees/api/ssh_gss.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)    96476 2023-07-28 19:23:28.000000 paramiko-3.3.1/docs/.doctrees/api/config.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)    15222 2023-05-25 18:10:48.000000 paramiko-3.3.1/docs/.doctrees/api/proxy.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)    58315 2023-05-25 18:10:47.000000 paramiko-3.3.1/docs/.doctrees/api/hostkeys.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)    57030 2023-05-25 02:01:15.000000 paramiko-3.3.1/docs/.doctrees/api/file.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)   149321 2023-05-25 18:10:47.000000 paramiko-3.3.1/docs/.doctrees/api/client.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)    11039 2023-05-25 18:10:49.000000 paramiko-3.3.1/docs/.doctrees/index.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)     4992 2023-03-03 18:55:05.000000 paramiko-3.3.1/setup_helper.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-05-25 18:00:56.000000 paramiko-3.3.1/pytest.ini
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-07-28 20:15:35.000000 paramiko-3.3.1/paramiko/
+-rw-r--r--   0 jforcier  (1000) users      (100)    19063 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/file.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4369 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/ber.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12544 2023-03-10 18:55:53.000000 paramiko-3.3.1/paramiko/sftp_si.py
+-rw-r--r--   0 jforcier  (1000) users      (100)   129637 2023-05-25 18:00:56.000000 paramiko-3.3.1/paramiko/transport.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    34492 2023-05-25 18:00:56.000000 paramiko-3.3.1/paramiko/client.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    30457 2023-05-25 18:00:56.000000 paramiko-3.3.1/paramiko/server.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    11653 2023-05-25 18:00:56.000000 paramiko-3.3.1/paramiko/ecdsakey.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5107 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/primes.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    43006 2023-05-25 18:00:56.000000 paramiko-3.3.1/paramiko/auth_handler.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    21666 2023-05-25 00:47:16.000000 paramiko-3.3.1/paramiko/packet.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1918 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/win_openssh.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3902 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/pipe.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    36007 2023-05-25 18:00:56.000000 paramiko-3.3.1/paramiko/pkey.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1833 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/kex_group14.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    13208 2023-05-25 18:00:56.000000 paramiko-3.3.1/paramiko/hostkeys.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    35855 2023-06-09 17:41:24.000000 paramiko-3.3.1/paramiko/sftp_client.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1282 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/compress.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4648 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/proxy.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    19492 2023-03-10 18:55:53.000000 paramiko-3.3.1/paramiko/sftp_server.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    49191 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/channel.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2288 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/kex_group16.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     6471 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/sftp.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7321 2023-05-25 18:00:56.000000 paramiko-3.3.1/paramiko/ssh_exception.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    15877 2023-05-25 18:00:56.000000 paramiko-3.3.1/paramiko/agent.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7756 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/common.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    11437 2023-05-25 18:00:56.000000 paramiko-3.3.1/paramiko/auth_strategy.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    24562 2023-03-10 18:55:53.000000 paramiko-3.3.1/paramiko/kex_gss.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7424 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/sftp_handle.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4423 2023-05-25 18:00:56.000000 paramiko-3.3.1/paramiko/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    28887 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/ssh_gss.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7457 2023-05-25 18:00:56.000000 paramiko-3.3.1/paramiko/ed25519key.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8248 2023-05-25 18:00:56.000000 paramiko-3.3.1/paramiko/dsskey.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    11204 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/_winapi.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5740 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/kex_group1.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     9349 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/message.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4177 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/win_pageant.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7546 2023-05-25 18:00:56.000000 paramiko-3.3.1/paramiko/rsakey.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     9550 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    10320 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/kex_gex.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    27362 2023-07-28 18:55:00.000000 paramiko-3.3.1/paramiko/config.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5012 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/kex_ecdh_nist.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-07-28 20:15:33.000000 paramiko-3.3.1/paramiko/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4436 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/kex_curve25519.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    21820 2023-06-09 17:41:24.000000 paramiko-3.3.1/paramiko/sftp_file.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8258 2023-03-10 18:55:53.000000 paramiko-3.3.1/paramiko/sftp_attr.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7225 2023-03-03 18:55:05.000000 paramiko-3.3.1/paramiko/buffered_pipe.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2360 2023-05-25 18:00:56.000000 paramiko-3.3.1/README.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    26436 2021-11-27 02:56:36.000000 paramiko-3.3.1/LICENSE
```

### Comparing `paramiko-3.3.0/paramiko/kex_group1.py` & `paramiko-3.3.1/paramiko/kex_group1.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/rsakey.py` & `paramiko-3.3.1/paramiko/rsakey.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/transport.py` & `paramiko-3.3.1/paramiko/transport.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/proxy.py` & `paramiko-3.3.1/paramiko/proxy.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/dsskey.py` & `paramiko-3.3.1/paramiko/dsskey.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/hostkeys.py` & `paramiko-3.3.1/paramiko/hostkeys.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/compress.py` & `paramiko-3.3.1/paramiko/compress.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/kex_curve25519.py` & `paramiko-3.3.1/paramiko/kex_curve25519.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/common.py` & `paramiko-3.3.1/paramiko/common.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/ed25519key.py` & `paramiko-3.3.1/paramiko/ed25519key.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/kex_gex.py` & `paramiko-3.3.1/paramiko/kex_gex.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/sftp_handle.py` & `paramiko-3.3.1/paramiko/sftp_handle.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/util.py` & `paramiko-3.3.1/paramiko/util.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/ssh_exception.py` & `paramiko-3.3.1/paramiko/ssh_exception.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/ecdsakey.py` & `paramiko-3.3.1/paramiko/ecdsakey.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/message.py` & `paramiko-3.3.1/paramiko/message.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/_winapi.py` & `paramiko-3.3.1/paramiko/_winapi.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/ssh_gss.py` & `paramiko-3.3.1/paramiko/ssh_gss.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/win_pageant.py` & `paramiko-3.3.1/paramiko/win_pageant.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/kex_gss.py` & `paramiko-3.3.1/paramiko/kex_gss.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/config.py` & `paramiko-3.3.1/paramiko/config.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/packet.py` & `paramiko-3.3.1/paramiko/packet.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/sftp.py` & `paramiko-3.3.1/paramiko/sftp.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/sftp_client.py` & `paramiko-3.3.1/paramiko/sftp_client.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/channel.py` & `paramiko-3.3.1/paramiko/channel.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/primes.py` & `paramiko-3.3.1/paramiko/primes.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/win_openssh.py` & `paramiko-3.3.1/paramiko/win_openssh.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/kex_group14.py` & `paramiko-3.3.1/paramiko/kex_group14.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/server.py` & `paramiko-3.3.1/paramiko/server.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/client.py` & `paramiko-3.3.1/paramiko/client.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/kex_group16.py` & `paramiko-3.3.1/paramiko/kex_group16.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/sftp_server.py` & `paramiko-3.3.1/paramiko/sftp_server.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/auth_strategy.py` & `paramiko-3.3.1/paramiko/auth_strategy.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/pipe.py` & `paramiko-3.3.1/paramiko/pipe.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/pkey.py` & `paramiko-3.3.1/paramiko/pkey.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/agent.py` & `paramiko-3.3.1/paramiko/agent.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/buffered_pipe.py` & `paramiko-3.3.1/paramiko/buffered_pipe.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/__init__.py` & `paramiko-3.3.1/paramiko/__init__.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/auth_handler.py` & `paramiko-3.3.1/paramiko/auth_handler.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/sftp_file.py` & `paramiko-3.3.1/paramiko/sftp_file.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/kex_ecdh_nist.py` & `paramiko-3.3.1/paramiko/kex_ecdh_nist.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/sftp_si.py` & `paramiko-3.3.1/paramiko/sftp_si.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/sftp_attr.py` & `paramiko-3.3.1/paramiko/sftp_attr.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/file.py` & `paramiko-3.3.1/paramiko/file.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko/ber.py` & `paramiko-3.3.1/paramiko/ber.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/setup_helper.py` & `paramiko-3.3.1/setup_helper.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/index.html` & `paramiko-3.3.1/docs/index.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/config.html` & `paramiko-3.3.1/docs/api/config.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/hostkeys.html` & `paramiko-3.3.1/docs/api/hostkeys.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/kex_gss.html` & `paramiko-3.3.1/docs/api/kex_gss.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/keys.html` & `paramiko-3.3.1/docs/api/keys.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/file.html` & `paramiko-3.3.1/docs/api/file.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/sftp.html` & `paramiko-3.3.1/docs/api/sftp.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/packet.html` & `paramiko-3.3.1/docs/api/packet.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/agent.html` & `paramiko-3.3.1/docs/api/agent.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/channel.html` & `paramiko-3.3.1/docs/api/channel.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/transport.html` & `paramiko-3.3.1/docs/api/transport.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/pipe.html` & `paramiko-3.3.1/docs/api/pipe.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/buffered_pipe.html` & `paramiko-3.3.1/docs/api/buffered_pipe.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/ssh_gss.html` & `paramiko-3.3.1/docs/api/ssh_gss.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/server.html` & `paramiko-3.3.1/docs/api/server.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/auth.html` & `paramiko-3.3.1/docs/api/auth.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/client.html` & `paramiko-3.3.1/docs/api/client.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/proxy.html` & `paramiko-3.3.1/docs/api/proxy.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/message.html` & `paramiko-3.3.1/docs/api/message.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/api/ssh_exception.html` & `paramiko-3.3.1/docs/api/ssh_exception.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/index.doctree` & `paramiko-3.3.1/docs/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/environment.pickle` & `paramiko-3.3.1/docs/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/sftp.doctree` & `paramiko-3.3.1/docs/.doctrees/api/sftp.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/message.doctree` & `paramiko-3.3.1/docs/.doctrees/api/message.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/ssh_gss.doctree` & `paramiko-3.3.1/docs/.doctrees/api/ssh_gss.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/transport.doctree` & `paramiko-3.3.1/docs/.doctrees/api/transport.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/auth.doctree` & `paramiko-3.3.1/docs/.doctrees/api/auth.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/client.doctree` & `paramiko-3.3.1/docs/.doctrees/api/client.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/ssh_exception.doctree` & `paramiko-3.3.1/docs/.doctrees/api/ssh_exception.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/keys.doctree` & `paramiko-3.3.1/docs/.doctrees/api/keys.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/buffered_pipe.doctree` & `paramiko-3.3.1/docs/.doctrees/api/buffered_pipe.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/pipe.doctree` & `paramiko-3.3.1/docs/.doctrees/api/pipe.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/config.doctree` & `paramiko-3.3.1/docs/.doctrees/api/config.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/proxy.doctree` & `paramiko-3.3.1/docs/.doctrees/api/proxy.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/packet.doctree` & `paramiko-3.3.1/docs/.doctrees/api/packet.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/hostkeys.doctree` & `paramiko-3.3.1/docs/.doctrees/api/hostkeys.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/kex_gss.doctree` & `paramiko-3.3.1/docs/.doctrees/api/kex_gss.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/agent.doctree` & `paramiko-3.3.1/docs/.doctrees/api/agent.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/file.doctree` & `paramiko-3.3.1/docs/.doctrees/api/file.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/channel.doctree` & `paramiko-3.3.1/docs/.doctrees/api/channel.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/.doctrees/api/server.doctree` & `paramiko-3.3.1/docs/.doctrees/api/server.doctree`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/searchindex.js` & `paramiko-3.3.1/docs/searchindex.js`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/_static/language_data.js` & `paramiko-3.3.1/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/_static/searchtools.js` & `paramiko-3.3.1/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/_static/jquery-3.5.1.js` & `paramiko-3.3.1/docs/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/_static/jquery.js` & `paramiko-3.3.1/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/_static/pygments.css` & `paramiko-3.3.1/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/_static/underscore-1.13.1.js` & `paramiko-3.3.1/docs/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/_static/doctools.js` & `paramiko-3.3.1/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/_static/underscore.js` & `paramiko-3.3.1/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/_static/basic.css` & `paramiko-3.3.1/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/_static/alabaster.css` & `paramiko-3.3.1/docs/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/objects.inv` & `paramiko-3.3.1/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/genindex.html` & `paramiko-3.3.1/docs/genindex.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/search.html` & `paramiko-3.3.1/docs/search.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/_sources/index.rst.txt` & `paramiko-3.3.1/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/_sources/api/config.rst.txt` & `paramiko-3.3.1/docs/_sources/api/config.rst.txt`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/docs/py-modindex.html` & `paramiko-3.3.1/docs/py-modindex.html`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/LICENSE` & `paramiko-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko.egg-info/SOURCES.txt` & `paramiko-3.3.1/paramiko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/paramiko.egg-info/PKG-INFO` & `paramiko-3.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paramiko
-Version: 3.3.0
+Version: 3.3.1
 Summary: SSH2 protocol library
 Home-page: https://paramiko.org
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: LGPL
 Project-URL: Docs, https://docs.paramiko.org
 Project-URL: Source, https://github.com/paramiko/paramiko
@@ -76,11 +76,11 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
-Provides-Extra: gssapi
-Provides-Extra: invoke
 Provides-Extra: all
 Provides-Extra: ed25519
+Provides-Extra: gssapi
+Provides-Extra: invoke
```

### Comparing `paramiko-3.3.0/tests/_loop.py` & `paramiko-3.3.1/tests/_loop.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_ecdsa_384_openssh.key` & `paramiko-3.3.1/tests/test_ecdsa_384_openssh.key`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_proxy.py` & `paramiko-3.3.1/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_sftp.py` & `paramiko-3.3.1/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_gssapi.py` & `paramiko-3.3.1/tests/test_gssapi.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_pkey.py` & `paramiko-3.3.1/tests/test_pkey.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_rsa_openssh.key` & `paramiko-3.3.1/tests/test_rsa_openssh.key`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_rsa_openssh_nopad.key` & `paramiko-3.3.1/tests/test_rsa_openssh_nopad.key`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/auth.py` & `paramiko-3.3.1/tests/auth.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/__init__.py` & `paramiko-3.3.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_channelfile.py` & `paramiko-3.3.1/tests/test_channelfile.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_message.py` & `paramiko-3.3.1/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_buffered_pipe.py` & `paramiko-3.3.1/tests/test_buffered_pipe.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_transport.py` & `paramiko-3.3.1/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_config.py` & `paramiko-3.3.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_kex.py` & `paramiko-3.3.1/tests/test_kex.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_ssh_gss.py` & `paramiko-3.3.1/tests/test_ssh_gss.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/_util.py` & `paramiko-3.3.1/tests/_util.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/_support/rsa-lonely.key` & `paramiko-3.3.1/tests/_support/rsa.key`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/_support/dss.key` & `paramiko-3.3.1/tests/_support/dss.key`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/_support/ed25519.key-cert.pub` & `paramiko-3.3.1/tests/_support/ed25519.key-cert.pub`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/_support/rsa.key` & `paramiko-3.3.1/tests/_support/rsa-lonely.key`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/_support/rsa-missing.key-cert.pub` & `paramiko-3.3.1/tests/_support/rsa.key-cert.pub`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/_support/dss.key-cert.pub` & `paramiko-3.3.1/tests/_support/dss.key-cert.pub`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/_support/rsa.key-cert.pub` & `paramiko-3.3.1/tests/_support/rsa-missing.key-cert.pub`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/_support/ecdsa-256.key-cert.pub` & `paramiko-3.3.1/tests/_support/ecdsa-256.key-cert.pub`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_sftp_big.py` & `paramiko-3.3.1/tests/test_sftp_big.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_kex_gss.py` & `paramiko-3.3.1/tests/test_kex_gss.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_file.py` & `paramiko-3.3.1/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/conftest.py` & `paramiko-3.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_rsa_password.key` & `paramiko-3.3.1/tests/test_rsa_password.key`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/pkey.py` & `paramiko-3.3.1/tests/pkey.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_dss_password.key` & `paramiko-3.3.1/tests/test_dss_password.key`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/_stub_sftp.py` & `paramiko-3.3.1/tests/_stub_sftp.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_hostkeys.py` & `paramiko-3.3.1/tests/test_hostkeys.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/agent.py` & `paramiko-3.3.1/tests/agent.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_packetizer.py` & `paramiko-3.3.1/tests/test_packetizer.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_client.py` & `paramiko-3.3.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_util.py` & `paramiko-3.3.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_ssh_exception.py` & `paramiko-3.3.1/tests/test_ssh_exception.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/tests/test_dss_openssh.key` & `paramiko-3.3.1/tests/test_dss_openssh.key`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/setup.py` & `paramiko-3.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/README.rst` & `paramiko-3.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/demos/demo_sftp.py` & `paramiko-3.3.1/demos/demo_sftp.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/demos/test_rsa.key` & `paramiko-3.3.1/demos/test_rsa.key`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/demos/demo_server.py` & `paramiko-3.3.1/demos/demo_server.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/demos/demo_keygen.py` & `paramiko-3.3.1/demos/demo_keygen.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/demos/interactive.py` & `paramiko-3.3.1/demos/interactive.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/demos/rforward.py` & `paramiko-3.3.1/demos/rforward.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/demos/demo_simple.py` & `paramiko-3.3.1/demos/demo_simple.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/demos/forward.py` & `paramiko-3.3.1/demos/forward.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/demos/demo.py` & `paramiko-3.3.1/demos/demo.py`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/demos/user_rsa_key` & `paramiko-3.3.1/demos/user_rsa_key`

 * *Files identical despite different names*

### Comparing `paramiko-3.3.0/PKG-INFO` & `paramiko-3.3.1/paramiko.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paramiko
-Version: 3.3.0
+Version: 3.3.1
 Summary: SSH2 protocol library
 Home-page: https://paramiko.org
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: LGPL
 Project-URL: Docs, https://docs.paramiko.org
 Project-URL: Source, https://github.com/paramiko/paramiko
@@ -76,11 +76,11 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
-Provides-Extra: gssapi
-Provides-Extra: invoke
 Provides-Extra: all
 Provides-Extra: ed25519
+Provides-Extra: gssapi
+Provides-Extra: invoke
```

