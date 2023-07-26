# Comparing `tmp/harmony_toolbox-1.0.8.tar.gz` & `tmp/harmony_toolbox-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmony_toolbox-1.0.8.tar", last modified: Fri Jun 30 15:15:06 2023, max compression
+gzip compressed data, was "harmony_toolbox-1.1.0.tar", last modified: Wed Jul 26 01:12:31 2023, max compression
```

## Comparing `harmony_toolbox-1.0.8.tar` & `harmony_toolbox-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-06-30 15:15:06.559696 harmony_toolbox-1.0.8/
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1066 2023-04-04 17:13:12.000000 harmony_toolbox-1.0.8/LICENSE
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      146 2023-04-04 17:13:12.000000 harmony_toolbox-1.0.8/MANIFEST.in
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-06-30 15:15:06.560698 harmony_toolbox-1.0.8/PKG-INFO
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1058 2023-04-04 17:13:12.000000 harmony_toolbox-1.0.8/README.md
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      121 2023-04-04 17:13:12.000000 harmony_toolbox-1.0.8/pyproject.toml
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      151 2023-06-28 21:56:07.000000 harmony_toolbox-1.0.8/requirements.txt
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      736 2023-06-30 15:15:06.568699 harmony_toolbox-1.0.8/setup.cfg
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)       37 2023-04-04 17:13:12.000000 harmony_toolbox-1.0.8/setup.py
-drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-06-30 15:15:06.095536 harmony_toolbox-1.0.8/src/
-drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-06-30 15:15:06.373089 harmony_toolbox-1.0.8/src/harmony_toolbox.egg-info/
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-06-30 15:15:05.000000 harmony_toolbox-1.0.8/src/harmony_toolbox.egg-info/PKG-INFO
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      344 2023-06-30 15:15:06.000000 harmony_toolbox-1.0.8/src/harmony_toolbox.egg-info/SOURCES.txt
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        1 2023-06-30 15:15:05.000000 harmony_toolbox-1.0.8/src/harmony_toolbox.egg-info/dependency_links.txt
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        8 2023-06-30 15:15:05.000000 harmony_toolbox-1.0.8/src/harmony_toolbox.egg-info/top_level.txt
-drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-06-30 15:15:06.521301 harmony_toolbox-1.0.8/src/toolbox/
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-03-24 16:13:56.000000 harmony_toolbox-1.0.8/src/toolbox/__init__.py
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     2478 2023-06-30 15:08:41.000000 harmony_toolbox-1.0.8/src/toolbox/config.py
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    51262 2023-06-28 22:08:54.000000 harmony_toolbox-1.0.8/src/toolbox/library.py
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    33700 2023-06-28 22:24:38.000000 harmony_toolbox-1.0.8/src/toolbox/toolbox.py
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-07-26 01:12:31.138245 harmony_toolbox-1.1.0/
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1066 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.0/LICENSE
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      146 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.0/MANIFEST.in
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-07-26 01:12:31.139245 harmony_toolbox-1.1.0/PKG-INFO
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1058 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.0/README.md
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      121 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.0/pyproject.toml
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      141 2023-06-30 15:28:08.000000 harmony_toolbox-1.1.0/requirements.txt
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      736 2023-07-26 01:12:31.146247 harmony_toolbox-1.1.0/setup.cfg
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)       37 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.0/setup.py
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-07-26 01:12:30.732547 harmony_toolbox-1.1.0/src/
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-07-26 01:12:30.987246 harmony_toolbox-1.1.0/src/harmony_toolbox.egg-info/
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-07-26 01:12:30.000000 harmony_toolbox-1.1.0/src/harmony_toolbox.egg-info/PKG-INFO
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      344 2023-07-26 01:12:30.000000 harmony_toolbox-1.1.0/src/harmony_toolbox.egg-info/SOURCES.txt
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        1 2023-07-26 01:12:30.000000 harmony_toolbox-1.1.0/src/harmony_toolbox.egg-info/dependency_links.txt
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        8 2023-07-26 01:12:30.000000 harmony_toolbox-1.1.0/src/harmony_toolbox.egg-info/top_level.txt
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-07-26 01:12:31.107245 harmony_toolbox-1.1.0/src/toolbox/
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-03-24 16:13:56.000000 harmony_toolbox-1.1.0/src/toolbox/__init__.py
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     2297 2023-07-19 18:56:52.000000 harmony_toolbox-1.1.0/src/toolbox/config.py
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    48485 2023-07-20 20:30:13.000000 harmony_toolbox-1.1.0/src/toolbox/library.py
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    30860 2023-07-26 00:27:49.000000 harmony_toolbox-1.1.0/src/toolbox/toolbox.py
```

### Comparing `harmony_toolbox-1.0.8/LICENSE` & `harmony_toolbox-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `harmony_toolbox-1.0.8/PKG-INFO` & `harmony_toolbox-1.1.0/src/harmony_toolbox.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: harmony_toolbox
-Version: 1.0.8
+Name: harmony-toolbox
+Version: 1.1.0
 Summary: Harmony ONE Validator Node Toolbox and Easy Setup
 Home-page: https://github.com/easy-node-pro/harmony-toolbox
 Author: EasyNode.PRO
 Author-email: support@easynode.pro
 Project-URL: Bug Tracker, https://github.com/easy-node-pro/harmony-toolbox/issues
 Project-URL: repository, https://github.com/easy-node-pro/harmony-toolbox
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harmony_toolbox-1.0.8/README.md` & `harmony_toolbox-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `harmony_toolbox-1.0.8/setup.cfg` & `harmony_toolbox-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = harmony_toolbox
-version = 1.0.8
+version = 1.1.0
 author = EasyNode.PRO
 author_email = support@easynode.pro
 description = Harmony ONE Validator Node Toolbox and Easy Setup
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/easy-node-pro/harmony-toolbox
 project_urls =
```

### Comparing `harmony_toolbox-1.0.8/src/harmony_toolbox.egg-info/PKG-INFO` & `harmony_toolbox-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: harmony-toolbox
-Version: 1.0.8
+Name: harmony_toolbox
+Version: 1.1.0
 Summary: Harmony ONE Validator Node Toolbox and Easy Setup
 Home-page: https://github.com/easy-node-pro/harmony-toolbox
 Author: EasyNode.PRO
 Author-email: support@easynode.pro
 Project-URL: Bug Tracker, https://github.com/easy-node-pro/harmony-toolbox/issues
 Project-URL: repository, https://github.com/easy-node-pro/harmony-toolbox
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harmony_toolbox-1.0.8/src/toolbox/config.py` & `harmony_toolbox-1.1.0/src/toolbox/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import os
 import socket
-import urllib.request
 import requests
-from os import environ
-from concurrent.futures import ThreadPoolExecutor, TimeoutError
+from os import environ, path
+from dotenv import load_dotenv
+
+load_dotenv(f"{path.expanduser('~')}/.easynode.env")
+
 
 def get_url(timeout=5) -> str:
     try:
         response = requests.get("https://ident.me", timeout=timeout)
         response.raise_for_status()  # Raises a HTTPError if the response was unsuccessful
         result = response.text
     except requests.exceptions.RequestException as x:
         print(type(x), x)
-        result = '0.0.0.0'
+        result = "0.0.0.0"
     return result
 
 
 class EnvironmentVariables:
-    easy_version = "1.0.8"
+    easy_version = "1.1.0"
     server_host_name = socket.gethostname()
-    user_home_dir = os.path.expanduser("~")
+    user_home_dir = path.expanduser("~")
     dotenv_file = f"{user_home_dir}/.easynode.env"
-    active_user = os.path.split(user_home_dir)[-1]
-    harmony_dir = environ.get("HARMONY_DIR") or os.path.join(user_home_dir, "harmony")
-    harmony_app = os.path.join(harmony_dir, "harmony")
-    bls_key_file = os.path.join(harmony_dir, "blskey.pass")
-    hmy_app = os.path.join(harmony_dir, "hmy")
-    harmony_conf = os.path.join(harmony_dir, "harmony.conf")
-    bls_key_dir = os.path.join(hmy_app, ".hmy", "blskeys")
-    hmy_wallet_store = os.path.join(user_home_dir, ".hmy_cli", "account-keys", active_user)
-    toolbox_location = os.path.join(user_home_dir, "harmony-toolbox")
-    validator_data = os.path.join(toolbox_location, "metadata", "validator.json")
-    password_path = os.path.join(harmony_dir, "passphrase.txt")
+    active_user = path.split(user_home_dir)[-1]
+    harmony_dir = environ.get("HARMONY_DIR") or f"{user_home_dir}/harmony"
+    bls_key_file = path.join(harmony_dir, "blskey.pass")
+    hmy_app = path.join(harmony_dir, "hmy")
+    harmony_conf = path.join(harmony_dir, "harmony.conf")
+    bls_key_dir = path.join(harmony_dir, ".hmy", "blskeys")
+    hmy_wallet_store = path.join(user_home_dir, ".hmy_cli", "account-keys", active_user)
+    toolbox_location = path.join(user_home_dir, "harmony-toolbox")
+    validator_data = path.join(toolbox_location, "metadata", "validator.json")
+    password_path = path.join(harmony_dir, "passphrase.txt")
     external_ip = get_url()
-    main_menu_regular = os.path.join(toolbox_location, "src", "messages", "regularmenu.txt")
-    main_menu_full = os.path.join(toolbox_location, "src", "messages", "fullmenu.txt")
-    rpc_endpoints = ['https://api.s0.t.hmny.io', 'https://api.harmony.one', 'https://rpc.ankr.com/harmony']
+    main_menu_regular = path.join(toolbox_location, "src", "messages", "regularmenu.txt")
+    rpc_endpoints = ["https://api.s0.t.hmny.io", "https://api.harmony.one", "https://rpc.ankr.com/harmony"]
     rpc_endpoints_max_connection_retries = 10
-    hmy_tmp_path = '/tmp/hmy'
-    harmony_tmp_path = '/tmp/harmony'
-    
+    hmy_tmp_path = "/tmp/hmy"
+    harmony_tmp_path = "/tmp/harmony"
+
     @staticmethod
     def get_working_endpoint(endpoints):
         for endpoint in endpoints:
             try:
                 response = requests.get(endpoint, timeout=5)
                 if response.status_code == 200:
                     return endpoint
```

### Comparing `harmony_toolbox-1.0.8/src/toolbox/library.py` & `harmony_toolbox-1.1.0/src/toolbox/library.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     dotenv.set_key(env_file, key_name, update_name)
     load_var_file(env_file)
     return
 
 
 # loader intro splash screen
 def loader_intro():
-    subprocess.run("clear")
     print(Fore.GREEN)
     print_stars()
     p = f"""
                     ____ ____ ____ ____ _________ ____ ____ ____ ____           
                     ||E |||a |||s |||y |||       |||N |||o |||d |||e ||          
                     ||__|||__|||__|||__|||_______|||__|||__|||__|||__||          
                     |/__\|/__\|/__\|/__\|/_______\|/__\|/__\|/__\|/__\|          
@@ -75,17 +74,28 @@
                             ||T |||o |||o |||l |||b |||o |||x ||                         
                             ||__|||__|||__|||__|||__|||__|||__||                         
                             |/__\|/__\|/__\|/__\|/__\|/__\|/__\|   
     """
     print(p)
 
 
+def old_toolbox_check():
+    if os.path.exists(f"{EnvironmentVariables.user_home_dir}/validatortoolbox"):
+        print_stars()
+        print(
+            Fore.GREEN
+            + "*\n* Old folder found, Exiting toolbox.\n*\n* Please renmae your ~/validatortoolbox folder to ~/harmony-toolbox and update your command paths!\n*\n* Run: cd ~/ && mv ~/validatortoolbox ~/harmony-toolbox\n*\n* After you run the move command, relaunch with: python3 ~/harmony-toolbox/src/menu.py\n*"
+        )
+        print_stars()
+        raise SystemExit(0)
+
+
 # Install Harmony ONE
 def install_hmy():
-    os.chdir(f"{EnvironmentVariables.harmony_dir}")
+    os.chdir(f"{os.environ.get('HARMONY_DIR')}")
     os.system(f"curl -LO https://harmony.one/hmycli && mv hmycli hmy && chmod +x hmy")
     print_stars()
     print("* hmy application installed.")
 
 
 # Code to update the harmony.conf after an upgrade and other text files.
 def update_text_file(fileName, originalText, newText):
@@ -96,49 +106,64 @@
 
     with open(fileName, "w") as f:
         f.write(newdata)
 
 
 # Setup a wallet, ask if they need to import one (not required but no toolbox menu without a wallet)
 def recover_wallet():
-    question = ask_yes_no(f"* Would you like to import a wallet? (YES/NO) ")
+    print_stars()
+    print("* Wallet Configuration                                                                      *")
+    print_stars()
+    question = ask_yes_no(
+        f"* If you would like to import a wallet for manual wallet actions, and for using our claim and send functions, answer yes.\n* If you only want to load your validator address for stats answer no.\n* Would you like to add your wallet to this server? (YES/NO) "
+    )
     # if yes, find recovery type
     if question:
         recovery_type()
         load_var_file(EnvironmentVariables.dotenv_file)
         print(
             f'\n* Verify the address above matches the address below:\n* Detected Wallet: {Fore.YELLOW}{environ.get("VALIDATOR_WALLET")}{Fore.GREEN}\n* If a different wallet is showing you can remove it and retry it after installation.\n*\n* .{EnvironmentVariables.hmy_app} keys remove {EnvironmentVariables.active_user}\n*\n* To restore a wallet once again, run the following:\n*\n* .{EnvironmentVariables.hmy_app} keys recover-from-mnemonic {EnvironmentVariables.active_user} {environ.get("PASS_SWITCH")}\n*'
         )
         print_stars()
         input("* Verify your wallet information above.\n* Press ENTER to continue Installation.")
     else:
-        wallet = input(
-            f"* If you'd like to use the management menu, we need a one1 address, please input your address now: "
-        )
-        set_var(EnvironmentVariables.dotenv_file, "VALIDATOR_WALLET", wallet)
-        return
+        while True:
+            wallet = input(
+                f"* If you'd like to use the management menu, we need a one1 address, please input your address now: "
+            )
+            if wallet.startswith("one1"):
+                # Re-enter the wallet to verify
+                verify_wallet = input(f"* Please re-enter your wallet address for verification: ")
+                if wallet == verify_wallet:
+                    set_var(EnvironmentVariables.dotenv_file, "VALIDATOR_WALLET", wallet)
+                    return
+                else:
+                    print("The entered wallets do not match. Please try again.")
+            else:
+                print("Invalid wallet address. It should start with 'one1'. Please try again.")
+    return
 
 
-def pull_harmony_update(harmony_dir, bls_key_file, harmony_conf):
+def pull_harmony_update(harmony_dir, harmony_conf):
     arch = os.uname().machine
     os.chdir(f"{harmony_dir}")
     if environ.get("NETWORK") == "testnet":
         os.system("curl -LO https://harmony.one/binary_testnet && mv binary_testnet harmony && chmod +x harmony")
         os.system("./harmony config dump --network testnet harmony.conf")
-        update_text_file(harmony_conf, "MaxKeys = 10", "MaxKeys = 13")
     if environ.get("NETWORK") == "mainnet":
         if arch.startswith("arm"):
             os.system("curl -LO https://harmony.one/binary-arm64 && mv binary-arm64 harmony && chmod +x harmony")
         if arch == "x86_64":
             os.system("curl -LO https://harmony.one/binary && mv binary harmony && chmod +x harmony")
-            os.system("./harmony config dump harmony.conf")
-            update_text_file(harmony_conf, "MaxKeys = 10", "MaxKeys = 13")
+        os.system("./harmony config dump harmony.conf")
+    update_text_file(harmony_conf, "MaxKeys = 10", "MaxKeys = 13")
+    update_text_file(harmony_conf, " DisablePrivateIPScan = false", " DisablePrivateIPScan = true")
     print_stars()
-    print("* harmony.conf MaxKeys modified to 13")
-    if os.path.exists(bls_key_file):
+    print("* harmony.conf MaxKeys modified to 13 & DisablePrivateIPScan set to true.")
+    if os.path.isdir(f"{os.environ.get('HARMONY_DIR')}/blskey.pass"):
         update_text_file(harmony_conf, 'PassFile = ""', f'PassFile = "blskey.pass"')
         print("* blskey.pass found, updated harmony.conf")
     print_stars()
     print(f"* Harmony {environ.get('NETWORK')} application installed & ~/harmony/harmony.conf created. ")
     return
 
 
@@ -154,15 +179,15 @@
                 return line[9:]
             count += 1
 
 
 # build list of installs
 def get_folders():
     folders = {}
-    if os.path.exists(f"{EnvironmentVariables.user_home_dir}/harmony/harmony.conf"):
+    if os.path.exists(f"{os.environ.get('HARMONY_DIR')}/harmony.conf"):
         port = find_port(f"harmony")
         folders["harmony"] = port
         print(f"* Found ~/harmony folder, on port {port}")
         print_stars()
     if os.path.exists(f"{EnvironmentVariables.user_home_dir}/harmony0/harmony.conf"):
         port = find_port(f"harmony0")
         folders["harmony0"] = port
@@ -281,41 +306,36 @@
             + "  *** Offline *** "
             + Style.RESET_ALL
             + Fore.GREEN
         )
 
 
 def set_wallet_env():
-    if environ.get("NODE_WALLET") == "true":
-        if not environ.get("VALIDATOR_WALLET"):
-            output = subprocess.getoutput(
-                f"{EnvironmentVariables.hmy_app} keys list | grep {EnvironmentVariables.active_user}"
-            )
-            output_stripped = output.lstrip(EnvironmentVariables.active_user)
-            output_stripped = output_stripped.strip()
-            set_var(EnvironmentVariables.dotenv_file, "VALIDATOR_WALLET", output_stripped)
-            return output_stripped
-        else:
-            load_var_file(EnvironmentVariables.dotenv_file)
-            validator_wallet = environ.get("VALIDATOR_WALLET")
-            return validator_wallet
+    load_var_file(EnvironmentVariables.dotenv_file)
+    if os.path.exists(EnvironmentVariables.hmy_wallet_store):
+        output = subprocess.getoutput(
+            f"{EnvironmentVariables.hmy_app} keys list | grep {EnvironmentVariables.active_user}"
+        )
+        output_stripped = output.lstrip(EnvironmentVariables.active_user)
+        output_stripped = output_stripped.strip()
+        set_var(EnvironmentVariables.dotenv_file, "VALIDATOR_WALLET", output_stripped)
+        return output_stripped
+    else:
+        validator_wallet = environ.get("VALIDATOR_WALLET")
+        return validator_wallet
 
 
 def get_db_size(harmony_dir, our_shard) -> str:
     harmony_db_size = subprocess.getoutput(f"du -h {harmony_dir}/harmony_db_{our_shard}")
     harmony_db_size = harmony_db_size.rstrip("\t")
-    countTrim = len(EnvironmentVariables.harmony_dir) + 13
+    countTrim = len(os.environ.get("HARMONY_DIR")) + 13
     return harmony_db_size[:-countTrim]
 
 
 def recovery_type():
-    subprocess.run("clear")
-    set_var(EnvironmentVariables.dotenv_file, "NODE_WALLET", "true")
-    passphrase_status()
-    passphrase_switch = environ.get("PASS_SWITCH")
     print_stars()
     print("* Wallet Recovery Type!                                                                     *")
     print_stars()
     print("* [0] = Mnemonic phrase recovery (aka seed phrase)                                          *")
     print("* [1] = Private Key recovery                                                                *")
     print_stars()
     menu_options = [
@@ -323,50 +343,53 @@
         "[1] - Private Key Recovery",
     ]
     terminal_menu = TerminalMenu(
         menu_options, title="* Which type of restore method would you like to use for your validator wallet?"
     )
     results = terminal_menu.show()
     if results == 0:
+        passphrase_set()
         # Mnemonic Recovery Here
         os.system(
-            f"{EnvironmentVariables.hmy_app} keys recover-from-mnemonic {EnvironmentVariables.active_user} {passphrase_switch}"
+            f"{EnvironmentVariables.hmy_app} keys recover-from-mnemonic {EnvironmentVariables.active_user} --passphrase-file passphrase.txt"
         )
         print_stars()
         set_wallet_env()
     elif results == 1:
+        passphrase_set()
         # Private Key Recovery Here
         print("* Private key recovery requires your private information in the command itself.")
         private = input("* Please enter your private key to restore your wallet: ")
         os.system(
             f"{EnvironmentVariables.hmy_app} keys import-private-key {private} {EnvironmentVariables.active_user} --passphrase"
         )
         print_stars()
         set_wallet_env()
 
 
 def passphrase_status():
     load_var_file(EnvironmentVariables.dotenv_file)
-    if environ.get("NODE_WALLET") == "true":
+    if os.path.exists(EnvironmentVariables.hmy_wallet_store):
         passphrase_set()
         set_var(
             EnvironmentVariables.dotenv_file,
             "PASS_SWITCH",
-            f"--passphrase-file {EnvironmentVariables.harmony_dir}/passphrase.txt",
+            f"--passphrase-file {os.environ.get('HARMONY_DIR')}/passphrase.txt",
         )
-    if environ.get("NODE_WALLET") == "false":
+    else:
         set_var(EnvironmentVariables.dotenv_file, "PASS_SWITCH", "--passphrase")
+    load_var_file(EnvironmentVariables.dotenv_file)
 
 
 def passphrase_set():
     if os.path.exists(EnvironmentVariables.password_path):
         return
     import getpass
 
-    print(f"* Setup {EnvironmentVariables.harmony_dir}/passphrase.txt file for use with autobidder & harmony-toolbox.")
+    print(f"* Setup {os.environ.get('HARMONY_DIR')}/passphrase.txt file for use with autobidder & harmony-toolbox.")
     print_stars()
     # take input
     while True:
         print("* ")
         password_1 = getpass.getpass(
             prompt="* Please set a wallet password for this node\n* Enter your password now: ", stream=None
         )
@@ -414,23 +437,24 @@
         print(f"File not Found  ::  {e}")
         return []
 
 
 def load_var_file(var_file):
     if os.path.exists(var_file):
         load_dotenv(var_file, override=True)
+        return False
     else:
         subprocess.run(["touch", var_file])
+        return True
 
 
 def get_shard_menu() -> None:
     if not environ.get("SHARD"):
-        subprocess.run("clear")
         print_stars()
-        print("* First Boot - Gathering more information about your server                                 *")
+        print("* Gathering more information about your server.                                             *")
         print_stars()
         print("* Which shard do you want this node run on?                                                 *")
         print_stars()
         menu_options = [
             "[0] - Shard 0",
             "[1] - Shard 1",
             "[2] - Shard 2",
@@ -438,52 +462,16 @@
         ]
         terminal_menu = TerminalMenu(menu_options, title="* Which Shard will this node operate on? ")
         our_shard = str(terminal_menu.show())
         set_var(EnvironmentVariables.dotenv_file, "SHARD", our_shard)
         return our_shard
 
 
-def get_node_type() -> None:
-    if not os.path.exists(EnvironmentVariables.hmy_wallet_store):
-        if environ.get("NODE_TYPE") == None:
-            subprocess.run("clear")
-            print_stars()
-            print("* Which type of node would you like to run on this server?                                  *")
-            print_stars()
-            print("* [0] - Standard w/ Wallet - Harmony Validator Signing Node with Wallet                     *")
-            print("* [1] - Standard No Wallet - Harmony Validator Signing Node no Wallet                       *")
-            print("* [2] - Full Node Dev/RPC - Non Validating Harmony Node                                     *")
-            print_stars()
-            menu_options = [
-                "[0] Signing Node w/ Wallet",
-                "[1] Signing Node No Wallet",
-                "[2] Full Node Non Validating Dev/RPC",
-            ]
-            terminal_menu = TerminalMenu(menu_options, title="Regular or Full Node Server")
-            results = terminal_menu.show()
-            if results == 0:
-                set_var(EnvironmentVariables.dotenv_file, "NODE_TYPE", "regular")
-                set_var(EnvironmentVariables.dotenv_file, "NODE_WALLET", "true")
-            if results == 1:
-                set_var(EnvironmentVariables.dotenv_file, "NODE_TYPE", "regular")
-                set_var(EnvironmentVariables.dotenv_file, "NODE_WALLET", "false")
-            if results == 2:
-                set_var(EnvironmentVariables.dotenv_file, "NODE_TYPE", "full")
-            subprocess.run("clear")
-            return
-        set_wallet_env()
-    if not environ.get("NODE_TYPE"):
-        set_var(EnvironmentVariables.dotenv_file, "NODE_TYPE", "regular")
-    if not environ.get("NODE_WALLET"):
-        set_var(EnvironmentVariables.dotenv_file, "NODE_WALLET", "true")
-
-
 def set_main_or_test() -> None:
     if not environ.get("NETWORK"):
-        subprocess.run("clear")
         print_stars()
         print("* Setup config not found, which blockchain does this node run on?                           *")
         print_stars()
         print("* [0] - Mainnet                                                                             *")
         print("* [1] - Testnet                                                                             *")
         print_stars()
         menu_options = [
@@ -498,34 +486,17 @@
             set_var(EnvironmentVariables.dotenv_file, "RPC_NET", "https://rpc.s0.t.hmny.io")
             set_var(EnvironmentVariables.dotenv_file, "RPC_NET_SHARD", f"https://rpc.s{environ.get('SHARD')}.t.hmny.io")
         if results == 1:
             set_var(EnvironmentVariables.dotenv_file, "NETWORK", "testnet")
             set_var(EnvironmentVariables.dotenv_file, "NETWORK_SWITCH", "b")
             set_var(EnvironmentVariables.dotenv_file, "RPC_NET", "https://rpc.s0.b.hmny.io")
             set_var(EnvironmentVariables.dotenv_file, "RPC_NET_SHARD", f"https://rpc.s{environ.get('SHARD')}.b.hmny.io")
-        subprocess.run("clear")
     return
 
 
-def get_express_status() -> None:
-    if environ.get("SETUP_STATUS") == "0":
-        subprocess.run("clear")
-        print_stars()
-        print("* Express or Manual Setup?                                                                  *")
-        print_stars()
-        print("* Would you like the turbo express setup or Manual approval of each step?                   *")
-        print_stars()
-        menu_options = [
-            "[0] - Express Install",
-            "[1] - Manual Approval",
-        ]
-        terminal_menu = TerminalMenu(menu_options, title="* Express Or Manual Setup")
-        set_var(EnvironmentVariables.dotenv_file, "EXPRESS", str(terminal_menu.show()))
-
-
 def get_wallet_address():
     print("* Signing Node, No Wallet!                                                                  *")
     print("* You are attempting to launch the menu but no wallet has been loaded, as you chose         *")
     print("* If you would like to use the menu on the server, complete the following:                  *")
     print_stars()
     print("* Edit ~/.easynode.env and add your wallet address on a new line like this example:         *")
     print("* VALIDATOR_WALLET='one1thisisjustanexamplewalletreplaceme'                                 *")
@@ -692,21 +663,17 @@
         hmy_ver = hmy_ver[62:-15]
     except subprocess.CalledProcessError:
         print(f"* Error - Website for hmy upgrade is offline, setting to offline.")
         hmy_ver = "Offline"
     return output_harmony_version.group(1)[:-2], hmy_ver
 
 
-def first_env_check(env_file, home_dir) -> None:
-    if os.path.exists(env_file):
-        load_var_file(env_file)
-    else:
-        os.system(f"touch {home_dir}/.easynode.env")
-        load_var_file(env_file)
-
+def first_env_check(env_file) -> None:
+    first_time = load_var_file(env_file)
+    return first_time
 
 def version_checks(harmony_folder):
     software_versions = {}
     software_versions["harmony_version"], software_versions["hmy_version"] = get_local_version(f"{harmony_folder}")
     software_versions["online_harmony_version"], software_versions["online_hmy_version"] = check_online_version()
     # Check versions, if matching False (No Upgrade Required), non-match True (Upgrade Required)
     if (
@@ -725,116 +692,107 @@
         software_versions["hmy_upgrade"] = "True"
     return software_versions
 
 
 def first_setup():
     # Find Shard #
     get_shard_menu()
-    # Express - no prompts for each step, Manual - prompts for each step
-    get_express_status()
-    # Get Regular validator with/without wallet or Full RPC Node
-    get_node_type()
     # Get Mainnet or Testnet
     set_main_or_test()
-    # Setup status done
-    set_var(EnvironmentVariables.dotenv_file, "SETUP_STATUS", "0")
     # Look for a harmony install or install.
     check_for_install()
     print_stars()
     return
 
 
-def recheck_vars():
-    # recheck some stuff just in case the .easynode.env isn't proper
-    load_var_file(EnvironmentVariables.dotenv_file)
-    get_shard_menu()
-    get_node_type()
-    set_main_or_test()
-    return
-
-
 # looks for ~/harmony or installs it if it's not there. Asks to overwrite if it finds it, run at your own risk.
 def check_for_install() -> str:
-    load_var_file(EnvironmentVariables.dotenv_file)
-    if not os.path.exists(EnvironmentVariables.harmony_dir):
-        print(f"* You selected Shard: {environ.get('SHARD')}. ")
-        install_harmony()
-        if environ.get("NODE_WALLET") == "true":
-            restore_wallet()
-        print_stars()
-        print("* All harmony files now installed. Database download starting now...")
-        print_stars()
-        clone_shards()
-        finish_node_install()
-    else:
+    if os.path.exists(f'{EnvironmentVariables.user_home_dir}/harmony'):
         question = ask_yes_no(
-            "* You already have a harmony folder on this system, would you like to re-run installation and rclone? (YES/NO)"
+            "* You already have a harmony folder on this system, would you like to re-run installation and rclone on this server? (YES/NO)"
         )
         if question:
             install_harmony()
-            if environ.get("NODE_WALLET") == "true":
-                restore_wallet()
+            print_stars()
+            # Wallet Setup
+            recover_wallet()
+            print_stars()
+            # Check passphrase if wallet is added
+            passphrase_status()
             print_stars()
             print("* All harmony files now installed. Database download starting now...")
             print_stars()
             clone_shards()
             finish_node_install()
+        else:
+            if os.path.isdir(f'{EnvironmentVariables.user_home_dir}/harmony'):
+                print("* Exiting Harmony Validator Toolbox\n* You already have a folder at ~/harmony.\n* Contact Easy Node for help setting up if this is an existing Harmony server.")
+            if os.path.isfile(f'{EnvironmentVariables.user_home_dir}/harmony'):
+                print("* Exiting Harmony Validator Toolbox\n* You already have a file at ~/harmony.\n* Contact Easy Node for help setting up if this is an existing Harmony server with a custom configuration.")
+            raise SystemExit(0)
+    else:
+        print(f"* You selected Shard: {environ.get('SHARD')}. ")
+        install_harmony()
+        print_stars()
+        # Wallet Setup
+        recover_wallet()
+        print_stars()
+        # Check passphrase if wallet is added
+        passphrase_status()
+        print_stars()
+        print("* All harmony files now installed. Database download starting now...")
+        print_stars()
+        clone_shards()
+        finish_node_install()
+    return
 
 
 # Installer Module
 def install_harmony() -> None:
-    # check disk space, find mounted disks
-    mntCount = 0
-    if os.path.isdir("/dev/disk/by-id/"):
-        testMnt = "/mnt"
-        for subdir, dirs, files in os.walk(testMnt):
-            for dir in dirs:
-                tester = os.path.join(subdir, dir)
-                if os.path.ismount(tester):
-                    myVolumePath = tester
-                    mntCount = mntCount + 1
-
-        # if you have more than one, we'll have to find a way to list them and let people choose
-        if mntCount > 1:
-            print("* You have multiple mounts in /mnt - Review mounts, only 1 allowed for our installer at this time!")
-            raise SystemExit(0)
-        # Checks Passed at this point, only 1 folder in /mnt and it's probably our volume (can scope this down further later)
-        if environ.get("SHARD") == "0":
-            if mntCount == 1:
-                myLongHmyPath = myVolumePath + "/harmony"
-                dotenv.set_key(EnvironmentVariables.dotenv_file, "MOUNT_POINT", myLongHmyPath)
-                print("* Creating all Harmony Files & Folders")
-                os.system(f"sudo chown {EnvironmentVariables.active_user} {myVolumePath}")
-                os.system(f"mkdir -p {myLongHmyPath}/.hmy/blskeys")
-                os.system(f"ln -s {myLongHmyPath} {EnvironmentVariables.harmony_dir}")
-            # Let's make sure your volume is mounted
-            if mntCount == 0:
-                question = ask_yes_no(
-                    "* You have a volume but it is not mounted.\n* Would you like to install Harmony in ~/harmony on your main disk instead of your volume? (Yes/No) "
-                )
-                if question:
-                    dotenv.set_key(EnvironmentVariables.dotenv_file, "MOUNT_POINT", EnvironmentVariables.harmony_dir)
-                else:
-                    raise SystemExit(0)
+    # Checks Passed at this point, only 1 folder in /mnt and it's probably our volume (can scope this down further later)
+    print_stars()
+    print("* Install Location")
+    print_stars()
+    question = ask_yes_no(f"* Would you like to install Harmony in the folder ~/harmony on your main disk? (YES/NO)")
+    if question:
+        set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f'{EnvironmentVariables.user_home_dir}/harmony')
+        print_stars()
+        print("* Creating all Harmony Files & Folders")
+        os.system(f"mkdir -p {os.environ.get('HARMONY_DIR')}/.hmy/blskeys")
+    else:
+        answer = input(
+            "* If you'd like to use an alternative location or volume we can make a symlink.\n* What is the full path to your volume? (example: /mnt/mydisk) "
+        )
+        if not os.path.exists(answer):
+            print("* That path doesn't exist, please try again.")
+            install_harmony()
+        answer2 = input("* Re-enter the path to your volume: ")
+        if answer == answer2:
+            set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{answer}/harmony")
+            print_stars()
+            print("* Creating base folder, setting ownership & creating symlink.")
+            os.system(f"sudo mkdir -p {os.environ.get('HARMONY_DIR')}")
+            os.system(f"sudo chown {EnvironmentVariables.active_user} {os.environ.get('HARMONY_DIR')}")
+            os.system(f"mkdir -p {os.environ.get('HARMONY_DIR')}/.hmy/blskeys")
+            os.system(f"ln -s {os.environ.get('HARMONY_DIR')} {EnvironmentVariables.user_home_dir}/harmony")
+
     # Setup folders now that symlink exists or we know we're using ~/harmony
     if not os.path.isdir(f"{EnvironmentVariables.user_home_dir}/.hmy_cli/account-keys/"):
         os.system(f"mkdir -p {EnvironmentVariables.user_home_dir}/.hmy_cli/account-keys/")
-    if not os.path.isdir(f"{EnvironmentVariables.harmony_dir}/.hmy/blskeys"):
+    if not os.path.isdir(f"{os.environ.get('HARMONY_DIR')}/.hmy/blskeys"):
         print("* Creating all Harmony Files & Folders")
-        os.system(f"mkdir -p {EnvironmentVariables.harmony_dir}/.hmy/blskeys")
+        os.system(f"mkdir -p {os.environ.get('HARMONY_DIR')}/.hmy/blskeys")
     # Change to ~/harmony folder
-    os.chdir(f"{EnvironmentVariables.harmony_dir}")
+    os.chdir(f"{os.environ.get('HARMONY_DIR')}")
     print_stars()
     # Install hmy
     install_hmy()
     print_stars()
     # Install harmony
-    pull_harmony_update(
-        EnvironmentVariables.harmony_dir, EnvironmentVariables.bls_key_file, EnvironmentVariables.harmony_conf
-    )
+    pull_harmony_update(os.environ.get("HARMONY_DIR"), f"{os.environ.get('HARMONY_DIR')}/harmony.conf")
     # install hmy files
     print("* Installing rclone application & rclone configuration files")
     print_stars()
     # check for working rclone site and download
     try:
         os.system("curl https://rclone.org/install.sh | sudo bash")
     except (ValueError, KeyError, TypeError):
@@ -860,76 +818,49 @@
             f"sudo cp {EnvironmentVariables.toolbox_location}/src/bin/harmony.service . && sed -i 's/serviceharmony/{EnvironmentVariables.active_user}/g' 'harmony.service' && sudo mv harmony.service /etc/systemd/system/harmony.service && sudo chmod a-x /etc/systemd/system/harmony.service && sudo systemctl enable harmony.service"
         )
 
 
 # Database Downloader
 def clone_shards():
     # Move to ~/harmony
-    os.chdir(f"{EnvironmentVariables.harmony_dir}")
+    os.chdir(f"{os.environ.get('HARMONY_DIR')}")
 
     if environ.get("SHARD") != "0":
         # If we're not on shard 0, download the numbered shard DB here.
         print(f"* Now cloning shard {environ.get('SHARD')}")
         print_stars()
         os.system(
-            f"rclone -P sync release:pub.harmony.one/{environ.get('NETWORK')}.min/harmony_db_{environ.get('SHARD')} {EnvironmentVariables.harmony_dir}/harmony_db_{environ.get('SHARD')} --multi-thread-streams 4 --transfers=32"
+            f"rclone -P sync release:pub.harmony.one/{environ.get('NETWORK')}.min/harmony_db_{environ.get('SHARD')} {os.environ.get('HARMONY_DIR')}/harmony_db_{environ.get('SHARD')} --multi-thread-streams 4 --transfers=32"
         )
         print_stars()
-        print(f"Shard {environ.get('SHARD')} completed.")
+        print(f"* Shard {environ.get('SHARD')} completed.\n* Shard 0 will be created when you start your service.")
         print_stars()
     else:
         # If we're on shard 0, grab the snap DB here.
         print("* Now cloning Shard 0, kick back and relax for awhile...")
         print_stars()
         os.system(
-            f"rclone -P -L --checksum sync release:pub.harmony.one/{environ.get('NETWORK')}.snap/harmony_db_0 {EnvironmentVariables.harmony_dir}/harmony_db_0 --multi-thread-streams 4 --transfers=32"
+            f"rclone -P -L --checksum sync release:pub.harmony.one/{environ.get('NETWORK')}.snap/harmony_db_0 {os.environ.get('HARMONY_DIR')}/harmony_db_0 --multi-thread-streams 4 --transfers=32"
         )
 
 
-# Code to restore a wallet
-def restore_wallet() -> str:
-    if environ.get("NODE_WALLET") == "true":
-        if not os.path.exists(EnvironmentVariables.hmy_wallet_store):
-            subprocess.run("clear")
-            print_stars()
-            print("* Harmony ONE Validator Wallet Import")
-            print_stars()
-            if environ.get("EXPRESS") == "1":
-                question = ask_yes_no(
-                    "\n* You will directly utilize the harmony application interface"
-                    + "\n* We do not store any pass phrases  or data inside of our application"
-                    + "\n* Respond yes to recover your validator wallet via Mnemonic phrase now or say NO to create a new wallet post-install"
-                    + "\n* Restore an existing wallet now? (YES/NO) "
-                )
-                if question:
-                    passphrase_status()
-                    recover_wallet()
-                print_stars()
-                return
-            passphrase_status()
-            recover_wallet()
-            return
-        print_stars()
-        print("* Wallet already setup for this user account")
-
-
 # is this used?
 def set_mounted_point():
     # First let's make sure your volume is mounted
     totalDir = len(os.listdir("/mnt"))
     if totalDir > 0:
         volumeMountPath = os.listdir("/mnt")
         myVolumePath = "/mnt/" + str(volumeMountPath[0])
         myLongHmyPath = myVolumePath + "/harmony"
     else:
-        myVolumePath = EnvironmentVariables.harmony_dir
+        myVolumePath = os.environ.get("HARMONY_DIR")
     if totalDir == 1:
-        dotenv.set_key(EnvironmentVariables.dotenv_file, "MOUNT_POINT", myLongHmyPath)
+        dotenv.set_key(EnvironmentVariables.dotenv_file, "HARMONY_DIR", myLongHmyPath)
     else:
-        dotenv.set_key(EnvironmentVariables.dotenv_file, "MOUNT_POINT", f"{EnvironmentVariables.harmony_dir}")
+        dotenv.set_key(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{os.environ.get('HARMONY_DIR')}")
 
 
 def finish_node_install():
     load_var_file(EnvironmentVariables.dotenv_file)
     print_stars()
     print(
         "* Installation is completed"
@@ -957,32 +888,31 @@
             + "\n* To create BLS keys run:"
             + f'\n* ./hmy keys generate-bls-keys --count 1 --shard {environ.get("SHARD")} {environ.get("PASS_SWITCH")}'
             + "\n*"
         )
     print_stars()
     print("* Thanks for using Easy Node - Validator Node Server Software Installer!")
     print_stars()
-    set_var(EnvironmentVariables.dotenv_file, "SETUP_STATUS", "1")
     raise SystemExit(0)
 
 
 def free_space_check(mount) -> str:
-    ourDiskMount = get_mount_point(mount)
+    ourDiskMount = get_HARMONY_DIR(mount)
     _, _, free = shutil.disk_usage(ourDiskMount)
     freeConverted = str(converted_unit(free))
     return freeConverted
 
 
 def server_drive_check(dot_env, directory) -> None:
-    if environ.get("MOUNT_POINT") is not None:
-        ourDiskMount = environ.get("MOUNT_POINT")
+    if environ.get("HARMONY_DIR") is not None:
+        ourDiskMount = environ.get("HARMONY_DIR")
     else:
-        dotenv.set_key(dot_env, "MOUNT_POINT", directory)
+        dotenv.set_key(dot_env, "HARMONY_DIR", directory)
         load_var_file(dot_env)
-        ourDiskMount = environ.get("MOUNT_POINT")
+        ourDiskMount = environ.get("HARMONY_DIR")
     print_stars()
     print("Here are all of your mount points: ")
     for part in disk_partitions():
         print(part)
     print_stars()
     total, used, free = shutil.disk_usage(ourDiskMount)
     total = str(converted_unit(total))
@@ -1026,24 +956,32 @@
             if device == "none":
                 device = ""
             ntuple = disk_ntuple(device, mountpoint, fstype)
             retlist.append(ntuple)
     return retlist
 
 
-def get_mount_point(pathname):
+def get_HARMONY_DIR(pathname):
     pathname = os.path.normcase(os.path.realpath(pathname))
     parent_device = path_device = os.stat(pathname).st_dev
     while parent_device == path_device:
-        mount_point = pathname
+        HARMONY_DIR = pathname
         pathname = os.path.dirname(pathname)
-        if pathname == mount_point:
+        if pathname == HARMONY_DIR:
             break
         parent_device = os.stat(pathname).st_dev
-    return mount_point
+    return HARMONY_DIR
+
+
+def refresh_stats() -> str:
+    print(Fore.GREEN)
+    print_stars()
+    print(f"* Getting the latest local & blockchain information now, one moment while we load...")
+    print_stars()
+    return
 
 
 def converted_unit(n):
     symbols = ("K", "M", "G", "T", "P", "E", "Z", "Y")
     prefix = {}
     for i, s in enumerate(symbols):
         prefix[s] = 1 << (i + 1) * 10
@@ -1186,28 +1124,14 @@
 def menu_ubuntu_updates() -> str:
     question = ask_yes_no(f"* Are you sure you would like to proceed with Linux apt Upgrades? (Y/N) ")
     if question:
         run_ubuntu_updater()
         input("* OS Updates completed, press ENTER to return to the main menu. ")
 
 
-def menu_error() -> None:
-    subprocess.run("clear")
-    print_stars()
-    print(
-        "* "
-        + Fore.RED
-        + "WARNING"
-        + Fore.GREEN
-        + ": Only numbers are possible, please try your selection on the main menu once again.\n* Press enter to return to the menu."
-    )
-    print_stars()
-    return
-
-
 def menu_reboot_server() -> str:
     question = ask_yes_no(
         Fore.RED
         + "WARNING: YOU WILL MISS BLOCKS WHILE YOU REBOOT YOUR ENTIRE SERVER.\n\n"
         + "Reconnect after a few moments & Run the Validator Toolbox Menu again with: python3 ~/harmony-toolbox/start.py\n"
         + Fore.WHITE
         + "Are you sure you would like to proceed with rebooting your server?\n\nType 'Yes' or 'No' to continue"
```

### Comparing `harmony_toolbox-1.0.8/src/toolbox/toolbox.py` & `harmony_toolbox-1.1.0/src/toolbox/toolbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,71 +24,95 @@
     string_stars,
     set_var,
     free_space_check,
     server_drive_check,
     all_sys_info,
     coming_soon,
     menu_ubuntu_updates,
-    menu_error,
     menu_reboot_server,
     finish_node,
     pull_harmony_update,
     version_checks,
     harmony_service_status,
-    loader_intro,
     get_folders,
     validator_stats_output,
-    get_db_size
+    get_db_size,
+    first_setup,
+    update_text_file,
+    get_shard_menu,
+    set_main_or_test,
+    recover_wallet,
+    refresh_stats,
+    passphrase_status
 )
 
 
 def parse_flags(parser):
+    print_stars()
     # Add the arguments
     parser.add_argument(
         "-s",
         "--stats",
         action="store_true",
         help="Run your stats if Harmony is installed and running.",
     )
     
     parser.add_argument(
+        "-u",
+        "--upgrade",
+        action="store_true",
+        help="Upgrade your Harmony binary if an upgrade is available.",
+    )
+
+    parser.add_argument(
         "-c",
         "--collect",
         action="store_true",
         help="Collect your rewards to your validator wallet",
     )
-    
+
     parser.add_argument(
         "-cs",
         "--collect-send",
         action="store_true",
         help="Collect your rewards to your validator wallet and send them to your rewards wallet",
     )
+    
+    parser.add_argument(
+        "-i",
+        "--install",
+        action="store_true",
+        help="Install Harmony ONE and hmy CLI if not installed.",
+    )
 
     args = parser.parse_args()
 
-    subprocess.run("clear")
     print(Fore.RESET)
 
+    if args.install:
+        first_setup()
+        
+    if args.upgrade:
+        update_harmony_app()
+
     if args.stats:
         run_multistats()
         finish_node()
-        
+
     if args.collect:
         rewards_collector(EnvironmentVariables.hmy_app, True)
         finish_node()
-        
+
     if args.collect_send:
         rewards_collector(EnvironmentVariables.hmy_app, True, True)
         finish_node()
 
 
 def run_multistats():
-    loader_intro()
-    refresh_stats(1)
+    refresh_stats()
     folders = get_folders()
     validator_stats_output(folders)
     return
 
 
 def collect_rewards(networkCall):
     os.system(
@@ -98,15 +122,21 @@
 
 def send_rewards(networkCall, sendAmount, rewards_wallet):
     os.system(
         f"{networkCall} transfer --amount {sendAmount} --from {environ.get('VALIDATOR_WALLET')} --from-shard 0 --to {rewards_wallet} --to-shard 0 --gas-price 100 {environ.get('PASS_SWITCH')}"
     )
 
 
-def rewards_collector(rpc, bypass = False, send_out_rewards = False, rewards_wallet = environ.get('REWARDS_WALLET'), validator_wallet = environ.get('VALIDATOR_WALLET')) -> None:
+def rewards_collector(
+    rpc,
+    bypass=False,
+    send_out_rewards=False,
+    rewards_wallet=environ.get("REWARDS_WALLET"),
+    validator_wallet=environ.get("VALIDATOR_WALLET"),
+) -> None:
     print("* Harmony ONE Rewards Collection")
     print_stars()
     if bypass == False:
         question = ask_yes_no(
             f"*\n* For your validator wallet {validator_wallet}\n* You have {get_rewards_balance(rpc, validator_wallet)} $ONE pending.\n* Would you like to collect your rewards on the Harmony mainnet? (YES/NO) "
         )
         bypass = True
@@ -152,108 +182,63 @@
     try:
         load_1, load_5, load_15 = os.getloadavg()
         sign_percentage = get_sign_pct()
         total_balance = get_wallet_balance(environ.get("VALIDATOR_WALLET"))
         remote_data_shard_0, local_data_shard, remote_data_shard = menu_validator_stats()
     except (ValueError, KeyError, TypeError) as e:
         print(f"* Error fetching data: {e}")
-    subprocess.run("clear")
     # Print Menu
     print_stars()
     print(
         f'{Fore.GREEN}* Validator Toolbox for {Fore.CYAN}Harmony ONE{Fore.GREEN} Validators by Easy Node   v{environ.get("EASY_VERSION")}{Fore.WHITE}   https://easynode.pro {Fore.GREEN}*'
     )
     print_stars()
     print(
         f'* Your validator wallet address is: {Fore.RED}{str(environ.get("VALIDATOR_WALLET"))}{Fore.GREEN}\n* Your $ONE balance is:             {Fore.CYAN}{str(round(total_balance, 2))}{Fore.GREEN}\n* Your pending $ONE rewards are:    {Fore.CYAN}{str(round(get_rewards_balance(EnvironmentVariables.rpc_endpoints, environ.get("VALIDATOR_WALLET")), 2))}{Fore.GREEN}\n* Server Hostname & IP:             {Fore.BLUE}{EnvironmentVariables.server_host_name}{Fore.GREEN} - {Fore.YELLOW}{EnvironmentVariables.external_ip}{Fore.GREEN}'
     )
     harmony_service_status()
     print(
-        f'* Epoch Signing Percentage:         {Style.BRIGHT}{Fore.GREEN}{Back.BLUE}{sign_percentage} %{Style.RESET_ALL}{Fore.GREEN}\n* Current disk space free: {Fore.CYAN}{free_space_check(EnvironmentVariables.harmony_dir): >6}{Fore.GREEN}\n* Current harmony version: {Fore.YELLOW}{software_versions["harmony_version"]}{Fore.GREEN}, has upgrade available: {software_versions["harmony_upgrade"]}\n* Current hmy version: {Fore.YELLOW}{software_versions["hmy_version"]}{Fore.GREEN}, has upgrade available: {software_versions["hmy_upgrade"]}'
+        f'* Epoch Signing Percentage:         {Style.BRIGHT}{Fore.GREEN}{Back.BLUE}{sign_percentage} %{Style.RESET_ALL}{Fore.GREEN}\n* Current disk space free: {Fore.CYAN}{free_space_check(os.environ.get("HARMONY_DIR")): >6}{Fore.GREEN}\n* Current harmony version: {Fore.YELLOW}{software_versions["harmony_version"]}{Fore.GREEN}, has upgrade available: {software_versions["harmony_upgrade"]}\n* Current hmy version: {Fore.YELLOW}{software_versions["hmy_version"]}{Fore.GREEN}, has upgrade available: {software_versions["hmy_upgrade"]}'
     )
     print_stars()
     if environ.get("SHARD") != "0":
         print(
-            f"* Note: Running on shard {environ.get('SHARD')}, Shard 0 is no longer needed locally and should be under 300MB\n* Remote Shard 0 Epoch: {remote_data_shard_0['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard_0['result']['shard-chain-header']['number'])}, Local Shard 0 Size: {get_db_size(EnvironmentVariables.harmony_dir, '0')}"
+            f"* Note: Running on shard {environ.get('SHARD')}, Shard 0 is no longer needed locally and should be under 300MB\n* Remote Shard 0 Epoch: {remote_data_shard_0['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard_0['result']['shard-chain-header']['number'])}, Local Shard 0 Size: {get_db_size(os.environ.get('HARMONY_DIR'), '0')}"
         )
         print(
             f"* Remote Shard {environ.get('SHARD')} Epoch: {remote_data_shard['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard['result']['shard-chain-header']['number'])}"
         )
         print(
-            f"*  Local Shard {environ.get('SHARD')} Epoch: {local_data_shard['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(local_data_shard['result']['shard-chain-header']['number'])}, Local Shard {environ.get('SHARD')} Size: {get_db_size(EnvironmentVariables.harmony_dir, environ.get('SHARD'))}"
+            f"*  Local Shard {environ.get('SHARD')} Epoch: {local_data_shard['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(local_data_shard['result']['shard-chain-header']['number'])}, Local Shard {environ.get('SHARD')} Size: {get_db_size(os.environ.get('HARMONY_DIR'), environ.get('SHARD'))}"
         )
     if environ.get("SHARD") == "0":
         print(
             f"* Remote Shard {environ.get('SHARD')} Epoch: {remote_data_shard_0['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard_0['result']['shard-chain-header']['number'])}"
         )
         print(
             f"*  Local Shard {environ.get('SHARD')} Epoch: {local_data_shard['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(local_data_shard['result']['shard-chain-header']['number'])}"
         )
     print(
         f"* CPU Load Averages: {round(load_1, 2)} over 1 min, {round(load_5, 2)} over 5 min, {round(load_15, 2)} over 15 min"
     )
     print_stars()
 
 
-def menu_topper_full() -> None:
-    try:
-        load_1, load_5, load_15 = os.getloadavg()
-        remote_data_shard_0, local_data_shard, remote_data_shard = menu_validator_stats()
-    except (ValueError, KeyError, TypeError) as e:
-        print(f"* Error fetching data: {e}")
-    subprocess.run("clear")
-    # Print Menu
-    print_stars()
-    print(
-        f'{Fore.GREEN}* Validator Toolbox for Harmony ONE Validators by Easy Node   v{environ.get("EASY_VERSION")}{Fore.WHITE}   https://easynode.pro {Fore.GREEN}*'
-    )
-    print_stars()
-    print(
-        f"* Server Hostname & IP:             {Fore.BLUE}{EnvironmentVariables.server_host_name}{Fore.GREEN} - {Fore.YELLOW}{EnvironmentVariables.external_ip}{Fore.GREEN}"
-    )
-    harmony_service_status()
-    print(
-        f'* Current disk space free: {Fore.CYAN}{free_space_check(EnvironmentVariables.harmony_dir): >6}{Fore.GREEN}\n* Current harmony version: {Fore.YELLOW}{environ.get("HARMONY_VERSION")}{Fore.GREEN}, has upgrade available: {environ.get("HARMONY_UPGRADE_AVAILABLE")}\n* Current hmy version: {Fore.YELLOW}{environ.get("HMY_VERSION")}{Fore.GREEN}, has upgrade available: {environ.get("HMY_UPGRADE_AVAILABLE")}'
-    )
-    print(
-        f"* Remote Shard {environ.get('SHARD')} Epoch: {remote_data_shard_0['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard_0['result']['shard-chain-header']['number'])}"
-    )
-    print(
-        f"*  Local Shard {environ.get('SHARD')} Epoch: {local_data_shard['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(local_data_shard['result']['shard-chain-header']['number'])}"
-    )
-    print(
-        f"* CPU Load Averages: {round(load_1, 2)} over 1 min, {round(load_5, 2)} over 5 min, {round(load_15, 2)} over 15 min"
-    )
-    print_stars()
-
-
 def menu_regular(software_versions) -> None:
     menu_topper_regular(software_versions)
     for x in return_txt(EnvironmentVariables.main_menu_regular):
         x = x.strip()
         try:
             x = eval(x)
         except SyntaxError:
             pass
         if x:
             print(x)
 
 
-def menu_full() -> None:
-    menu_topper_full()
-    for x in return_txt(EnvironmentVariables.main_menu_full):
-        x = x.strip()
-        try:
-            x = eval(x)
-        except SyntaxError:
-            pass
-        if x:
-            print(x)
-
-
 def get_wallet_json(wallet: str) -> str:
     test_or_main = environ.get("NETWORK")
     try:
         response = requests.get(f"https://api.stake.hmny.io/networks/{test_or_main}/validators/{wallet}")
         response.raise_for_status()
         # access JSOn content
         json_response = response.json()
@@ -335,104 +320,69 @@
 
 
 def set_reserve_total(reserve_total):
     set_var(EnvironmentVariables.dotenv_file, "GAS_RESERVE", reserve_total)
 
 
 def drive_check() -> None:
-    server_drive_check(EnvironmentVariables.dotenv_file, EnvironmentVariables.harmony_dir)
+    server_drive_check(EnvironmentVariables.dotenv_file, os.environ.get("HARMONY_DIR"))
     return
 
 
 def run_check_balance() -> None:
     menu_check_balance(EnvironmentVariables.rpc_endpoints, environ.get("VALIDATOR_WALLET"))
 
 
-def run_full_node() -> None:
-    menu_options = {
-        # 0: finish_node,
-        1: refresh_stats,
-        2: coming_soon,
-        3: coming_soon,
-        4: coming_soon,
-        5: coming_soon,
-        6: coming_soon,
-        7: set_rewards_wallet,
-        8: menu_service_stop_start,
-        9: menu_service_restart,
-        10: harmony_binary_upgrade,
-        11: hmy_cli_upgrade,
-        12: menu_ubuntu_updates,
-        13: drive_check,
-        14: coming_soon,
-        15: all_sys_info,
-        999: menu_reboot_server,
-    }
-    while True:
-        load_var_file(EnvironmentVariables.dotenv_file)
-        menu_full()
-        if environ.get("HARMONY_UPGRADE_AVAILABLE") == "True":
-            print(
-                f"* The harmony binary has an update available, Option #10 will upgrade you but you may miss a block while it restarts.\n"
-            )
-            print_stars()
-        if environ.get("HMY_UPGRADE_AVAILABLE") == "True":
-            print(
-                f"* The hmy binary has an update available, Option #11 will upgrade you but you may miss a block while it restarts.\n"
-            )
-            print_stars()
-        try:
-            option = int(input("Enter your option: "))
-        except ValueError:
-            menu_error()
-            run_full_node(environ.get("NODE_TYPE"))
-        if option == 0:
-            return finish_node()
-        subprocess.run("clear")
-        menu_options[option]()
-
-
 def bingo_checker():
-    os.system(f"grep BINGO {EnvironmentVariables.harmony_dir}/latest/zerolog-harmony.log | tail -10")
+    os.system(f"grep BINGO {os.environ.get('HARMONY_DIR')}/latest/zerolog-harmony.log | tail -10")
     print_stars()
     print("* Press enter to return to the main menu.")
     print_stars()
     input()
 
 
 def run_rewards_collector() -> None:
-    rewards_collector(
-        EnvironmentVariables.hmy_app
-    )
+    rewards_collector(EnvironmentVariables.hmy_app)
     return
 
 
 def safety_defaults() -> None:
+    # default settings section
+    set_var(EnvironmentVariables.dotenv_file, "EASY_VERSION", EnvironmentVariables.easy_version)
     if environ.get("GAS_RESERVE") is None:
         set_var(EnvironmentVariables.dotenv_file, "GAS_RESERVE", "5")
     if environ.get("REFRESH_TIME") is None:
         set_var(EnvironmentVariables.dotenv_file, "REFRESH_TIME", "30")
     if environ.get("REFRESH_OPTION") is None:
         set_var(EnvironmentVariables.dotenv_file, "REFRESH_OPTION", "True")
-    if environ.get("HARMONY_FOLDER") is None:
+    if environ.get("HARMONY_DIR") is None:
         if os.path.isdir(f"{EnvironmentVariables.user_home_dir}/harmony"):
-            set_var(EnvironmentVariables.dotenv_file, "HARMONY_FOLDER", f"{EnvironmentVariables.user_home_dir}/harmony")
-        elif os.path.exists(f"{EnvironmentVariables.user_home_dir}/harmony"):
+            set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{EnvironmentVariables.user_home_dir}/harmony")
+            return
+        elif os.path.isfile(f"{EnvironmentVariables.user_home_dir}/harmony"):
             try:
-                subprocess.run(f"{EnvironmentVariables.user_home_dir}/harmony --version", check=True)
-                set_var(
-                    set_var(EnvironmentVariables.dotenv_file, "HARMONY_FOLDER", f"{EnvironmentVariables.user_home_dir}")
-                )
+                subprocess.run(f"{EnvironmentVariables.user_home_dir}/harmony -V", check=True)
+                set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{EnvironmentVariables.user_home_dir}")
+                return
             except subprocess.CalledProcessError as e:
-                print("* Harmony not found, contact Easy Node for custom configs.")
+                print(
+                    "* Well this is odd, somehow harmony was not found.\n*\n* You can add the HARMONY_DIR variable to your ~/.easynode.env file\n* Example default location: HARMONY_DIR = /home/serviceharmony/harmony\n*\n* Or contact Easy Node for custom configuration help."
+                )
                 raise SystemExit(0)
         else:
-            print("* Harmony not found, contact Easy Node for custom configs.")
-            raise SystemExit(0)
-    set_var(EnvironmentVariables.dotenv_file, "EASY_VERSION", EnvironmentVariables.easy_version)
+            first_setup()
+    # always set conf to 13 keys, shard max
+    if os.path.exists(EnvironmentVariables.harmony_conf):
+        update_text_file(EnvironmentVariables.harmony_conf, "MaxKeys = 10", "MaxKeys = 13")
+    passphrase_status()
+    get_shard_menu()
+    set_main_or_test()
+    if environ.get("VALIDATOR_WALLET") is None:
+        # Recover wallet or have them add address
+        recover_wallet()
 
 
 def refresh_toggle() -> None:
     if environ.get("REFRESH_OPTION") == "True":
         answer = ask_yes_no(f"* Refresh is currently enabled. Would you like to disable it? (Y/N) ")
         if answer:
             set_var(EnvironmentVariables.dotenv_file, "REFRESH_OPTION", "False")
@@ -463,27 +413,27 @@
                 allowNegative=False,
             )
             set_var(EnvironmentVariables.dotenv_file, "REFRESH_TIME", str(delay_time[0]))
     load_var_file(EnvironmentVariables.dotenv_file)
     return
 
 
-def refresh_status_option():
+def update_stats_option():
     if environ.get("REFRESH_OPTION") == "True":
         print(
-            f"*  20 - Disable auto-refresh      - Disable Refresh or Change Delay Timer: {str(environ.get('REFRESH_TIME'))} seconds"
+            f"*  20 - Disable auto-update       - Disable Refresh or Change Delay Timer: {str(environ.get('REFRESH_TIME'))} seconds"
         )
     else:
-        print(f"*  20 - Enable Auto refresh       - Enable Refresh Timeout")
+        print(f"*  20 - Enable Auto update        - Enable Update Timer")
 
 
 def start_regular_node() -> None:
     # Check online versions of harmony & hmy and compare to our local copy.
-    refresh_stats(1)
-    software_versions = version_checks(environ.get("HARMONY_FOLDER"))
+    refresh_stats()
+    software_versions = version_checks(environ.get("HARMONY_DIR"))
     run_regular_node(software_versions)
 
 
 def run_regular_node(software_versions) -> None:
     menu_options = {
         0: finish_node,
         1: refresh_stats,
@@ -525,15 +475,14 @@
                     timeout=int(environ.get("REFRESH_TIME")),
                     resetOnInput=True,
                     allowNegative=False,
                 )
                 if timedOut:
                     start_regular_node()
                 else:
-                    subprocess.run("clear")
                     print_stars()
                     menu_options[option]()
                     if option != 1:
                         start_regular_node()
             except KeyError:
                 print(f"* Bad option, try again. Press enter to continue.")
                 print_stars()
@@ -543,15 +492,14 @@
             try:
                 option, timedOut = timedInteger(
                     "* Auto refresh disabled, Enter your menu choice: ",
                     timeout=-1,
                     resetOnInput=True,
                     allowNegative=False,
                 )
-                subprocess.run("clear")
                 print_stars()
                 menu_options[option]()
                 if option != 1:
                     start_regular_node()
             except KeyError:
                 print(f"* Bad option, try again. Press enter to continue.")
                 print_stars()
@@ -569,15 +517,15 @@
             f"*   9 - Restart Harmony Service   - {Back.RED}{Fore.YELLOW}WARNING: You will miss blocks during a restart!{Style.RESET_ALL}{Fore.GREEN}"
         )
     else:
         print(f"*   8 - Start Harmony Service")
 
 
 def make_backup_dir() -> str:
-    folder_name = f'{EnvironmentVariables.harmony_dir}/harmony_backup/{datetime.now().strftime("%Y%m%d%H%M")}'
+    folder_name = f'{os.environ.get("HARMONY_DIR")}/harmony_backup/{datetime.now().strftime("%Y%m%d%H%M")}'
     os.system(f"mkdir -p {folder_name}")
     return folder_name
 
 
 def hmy_cli_upgrade():
     question = ask_yes_no(
         "* Are you sure you would like to proceed with updating the Harmony CLI file?\n\nType 'Yes' or 'No' to continue"
@@ -592,49 +540,49 @@
         os.system(f"{EnvironmentVariables.hmy_app} version")
         print_stars()
         set_var(EnvironmentVariables.dotenv_file, "HMY_UPGRADE_AVAILABLE", "False")
         input("* Update completed, press ENTER to return to the main menu. ")
 
 
 def update_harmony_app():
-    os.chdir(f"{EnvironmentVariables.harmony_dir}")
+    os.chdir(f"{os.environ.get('HARMONY_DIR')}")
     print_stars()
     print("Currently installed version: ")
     os.system("./harmony -V")
     folder_name = make_backup_dir()
     os.system(
-        f"cp {EnvironmentVariables.harmony_dir}/harmony {EnvironmentVariables.harmony_dir}/harmony.conf {folder_name}"
+        f"cp {os.environ.get('HARMONY_DIR')}/harmony {os.environ.get('HARMONY_DIR')}/harmony.conf {folder_name}"
     )
     print_stars()
     print("Downloading current harmony binary file from harmony.one: ")
     print_stars()
     pull_harmony_update(
-        EnvironmentVariables.harmony_dir, EnvironmentVariables.bls_key_file, EnvironmentVariables.harmony_conf
+        os.environ.get("HARMONY_DIR"), EnvironmentVariables.harmony_conf
     )
     print_stars()
     print("Updated version: ")
     os.system("./harmony -V")
     if environ.get("SHARD") != "0":
         size = 0
-        for path, dirs, files in os.walk(f"{EnvironmentVariables.harmony_dir}/harmony_db_0"):
+        for path, dirs, files in os.walk(f"{os.environ.get('HARMONY_DIR')}/harmony_db_0"):
             for f in files:
                 fp = os.path.join(path, f)
                 size += os.path.getsize(fp)
             if size >= 400000000:
                 question = ask_yes_no(
                     Fore.WHITE
                     + "* Are you sure you would like to proceed with upgrading and trimming database 0?\n\nType 'Yes' or 'No' to continue"
                 )
                 if question:
                     os.system("sudo service harmony stop")
                     os.system(
-                        f"mv {EnvironmentVariables.harmony_dir}/harmony_db_0 {EnvironmentVariables.harmony_dir}/harmony_db_0_old"
+                        f"mv {os.environ.get('HARMONY_DIR')}/harmony_db_0 {os.environ.get('HARMONY_DIR')}/harmony_db_0_old"
                     )
                     os.system("sudo service harmony start")
-                    os.system(f"rm -r {EnvironmentVariables.harmony_dir}/harmony_db_0_old")
+                    os.system(f"rm -r {os.environ.get('HARMONY_DIR')}/harmony_db_0_old")
                 else:
                     print("Skipping removal of 0, but it's no longer required, fyi!")
             else:
                 print("Your database 0 is already trimmed, enjoy!")
     os.system("sudo service harmony restart")
     print_stars()
     print("Harmony Service is restarting, waiting 10 seconds for restart.")
@@ -657,16 +605,18 @@
         print(f"* Remote Shard 0 Offline, Error {e}")
     try:
         local_shard = [f"{EnvironmentVariables.hmy_app}", "blockchain", "latest-headers"]
         result_local_shard = run(local_shard, stdout=PIPE, stderr=PIPE, universal_newlines=True)
         local_data_shard = json.loads(result_local_shard.stdout)
     except (ValueError, KeyError, TypeError) as e:
         print(
-            f"* Local Server Offline, restart your service or troubleshoot the issue by running the following in your ~/harmony directory:\n* ./harmony -c harmony.conf, Error: {e}"
+            f"* Local Server Offline\n*\n* Run troubleshooting, See our documents site for info on how to manually troubleshoot:\n* https://docs.easynode.pro/harmony/post#validator-toolbox-troubleshooting\n*"
         )
+        print_stars()
+        finish_node()
 
     if environ.get("SHARD") != "0":
         remote_shard = [
             f"{EnvironmentVariables.hmy_app}",
             "blockchain",
             "latest-headers",
             f'--node=https://api.s{environ.get("SHARD")}.{environ.get("NETWORK_SWITCH")}.hmny.io',
@@ -677,41 +627,31 @@
             return remote_data_shard_0, local_data_shard, remote_data_shard
         except (ValueError, KeyError, TypeError):
             return
 
     return remote_data_shard_0, local_data_shard, None
 
 
-def refresh_stats(clear=0) -> str:
-    print(Fore.GREEN)
-    if clear == 0:
-        subprocess.run("clear")
-    print_stars()
-    print(f"* Getting the latest local & blockchain information now, one moment while we load...")
-    print_stars()
-    return
-
-
 def shard_stats(our_shard) -> str:
     our_uptime = subprocess.getoutput("uptime")
-    db_0_size = get_db_size(EnvironmentVariables.harmony_dir, "0")
+    db_0_size = get_db_size(os.environ.get("HARMONY_DIR"), "0")
     if our_shard == "0":
         print(
             f"""
     * Uptime :: {our_uptime}\n\n Harmony DB 0 Size  ::  {db_0_size}
     {string_stars()}
         """
         )
     else:
         print(
             f"""
     * Uptime :: {our_uptime}
     *
     * Harmony DB 0 Size  ::  {db_0_size}
-    * Harmony DB {our_shard} Size  ::   {get_db_size(EnvironmentVariables.harmony_dir, str(our_shard))}
+    * Harmony DB {our_shard} Size  ::   {get_db_size(os.environ.get("HARMONY_DIR"), str(our_shard))}
     *
     *
     {string_stars()}
         """
         )
```

