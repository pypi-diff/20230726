# Comparing `tmp/AshCrypt-3.0.2.tar.gz` & `tmp/AshCrypt-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AshCrypt-3.0.2.tar", last modified: Tue Jul 25 15:02:41 2023, max compression
+gzip compressed data, was "AshCrypt-3.0.3.tar", last modified: Wed Jul 26 12:15:10 2023, max compression
```

## Comparing `AshCrypt-3.0.2.tar` & `AshCrypt-3.0.3.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/AshCrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    38088 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/AshCrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/AshCrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/AshCrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/AshCrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/AshCrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/AshCrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/AshCrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20174 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:15:10.059177 AshCrypt-3.0.3/
+drwxrwxrwx   0        0        0        0 2023-07-26 12:15:10.022992 AshCrypt-3.0.3/AshCrypt/
+-rw-rw-rw-   0        0        0      287 2023-07-23 12:24:36.000000 AshCrypt-3.0.3/AshCrypt/README.md
+-rw-rw-rw-   0        0        0       84 2023-07-25 14:30:46.000000 AshCrypt-3.0.3/AshCrypt/__init__.py
+-rw-rw-rw-   0        0        0     6816 2023-07-23 12:35:47.000000 AshCrypt-3.0.3/AshCrypt/clicrypt.py
+-rw-rw-rw-   0        0        0     7330 2023-07-23 12:24:36.000000 AshCrypt-3.0.3/AshCrypt/crypt.py
+-rw-rw-rw-   0        0        0     9213 2023-07-25 14:30:46.000000 AshCrypt-3.0.3/AshCrypt/database.py
+-rw-rw-rw-   0        0        0     3985 2023-07-23 12:24:36.000000 AshCrypt-3.0.3/AshCrypt/filecrypt.py
+-rw-rw-rw-   0        0        0    40295 2023-07-26 11:32:12.000000 AshCrypt-3.0.3/AshCrypt/gui.py
+-rw-rw-rw-   0        0        0      499 2023-07-23 12:24:36.000000 AshCrypt-3.0.3/AshCrypt/qr.py
+-rw-rw-rw-   0        0        0     1802 2023-07-23 12:24:36.000000 AshCrypt-3.0.3/AshCrypt/textcrypt.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:15:10.046995 AshCrypt-3.0.3/AshCrypt/unittests/
+-rw-rw-rw-   0        0        0       31 2023-07-23 12:24:36.000000 AshCrypt-3.0.3/AshCrypt/unittests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:15:10.054377 AshCrypt-3.0.3/AshCrypt/unittests/__pycache__/
+-rw-rw-rw-   0        0        0      179 2023-07-25 15:00:15.000000 AshCrypt-3.0.3/AshCrypt/unittests/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5785 2023-07-25 15:00:15.000000 AshCrypt-3.0.3/AshCrypt/unittests/__pycache__/unittest_crypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3357 2023-07-23 12:24:36.000000 AshCrypt-3.0.3/AshCrypt/unittests/unittest_crypt.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:15:10.039993 AshCrypt-3.0.3/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0     1314 2023-07-26 12:15:09.000000 AshCrypt-3.0.3/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      544 2023-07-26 12:15:09.000000 AshCrypt-3.0.3/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 12:15:09.000000 AshCrypt-3.0.3/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-26 12:15:09.000000 AshCrypt-3.0.3/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-26 12:15:09.000000 AshCrypt-3.0.3/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-07-21 19:57:01.000000 AshCrypt-3.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1314 2023-07-26 12:15:10.058076 AshCrypt-3.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    20545 2023-07-25 14:43:26.000000 AshCrypt-3.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-26 12:15:10.060193 AshCrypt-3.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1667 2023-07-26 12:05:40.000000 AshCrypt-3.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `AshCrypt-3.0.2/AshCrypt/clicrypt.py` & `AshCrypt-3.0.3/AshCrypt/clicrypt.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,233 +1,233 @@
-from AshCrypt import filecrypt as af
-from AshCrypt import textcrypt as at
-import os.path
-import sys
-
-
-print('Welcome to the CLI')
-
-commands = 'Commands : \n' \
-           '\tq: to quit the program \n' \
-           '\tc : view commands\n' \
-           '\te: for encryption\n' \
-           '\td : for decryption\n' \
-           '\tef : to encrypt a file\n' \
-           '\tdf : to decrypt a file\n'
-
-global key
-
-
-def input_selection(q=None, c=None, e=None, d=None, ef=None, df=None):
-    global encflag, decFlag, file_decFlag, file_encFlag
-    if q == 1:
-        sys.exit()
-    if c == 1:
-        print(commands)
-    if e == 1:
-        file_decFlag = False
-        file_encFlag = False
-        decFlag = False
-        encflag = True
-        enc_f()
-    if d == 1:
-        file_decFlag = False
-        file_encFlag = False
-        encflag = False
-        decFlag = True
-        dec_f()
-    if ef == 1:
-        decFlag = False
-        encflag = False
-        file_decFlag = False
-        file_encFlag = True
-        file_enc()
-    if df == 1:
-        encflag = False
-        decFlag = True
-        file_encFlag = False
-        file_decFlag = True
-        file_dec()
-    else:
-        pass
-
-
-def input_wrap(inp):
-    inp = inp.lower()
-    if inp == 'c':
-        input_selection(c=1)
-        return 'c'
-    if inp == 'q':
-        input_selection(q=1)
-        return 'q'
-    if inp == 'e':
-        input_selection(e=1)
-        return 'e'
-    if inp == 'd':
-        input_selection(d=1)
-        return 'd'
-    if inp == 'ef':
-        input_selection(ef=1)
-        return 'ef'
-    if inp == 'df':
-        input_selection(df=1)
-        return 'df'
-    else:
-        return None
-
-
-def intro():
-    while True:
-        print('Program started running..')
-        print('Press c to view commands : ')
-        while True:
-            n = input("Press..\n")
-            input_wrap(n)
-
-
-def keysetup():
-    outer = True
-    inner = True
-    while outer:
-        global key
-        key = ''
-        i = input('Do you have a key ?(y/n) : ')
-        input_wrap(i)
-        if i.lower() == 'n':
-            print("Here's your key : ")
-            key = at.Crypt.genkey()
-            print(key)
-            inner = False
-            outer = False
-        elif i.lower() == 'y':
-            while inner:
-                print('insert your key here : ')
-                kk = input()
-                input_wrap(kk)
-                if at.Crypt.keyverify(kk) == 1:
-                    print('Key selected\n')
-                    key = kk
-                    inner = False
-                    outer = False
-                else:
-                    print('Enter a valid key !\n')
-
-
-encflag = True
-
-
-def enc_f():
-    keysetup()
-    while encflag:
-        print()
-        global key
-        print("press c to view commands.. ")
-        message = input('Encrypt a message : ')
-        input_wrap(message)
-        a = at.Crypt(message, key=key)
-        enc = a.encrypt()
-        if (enc[0]) == 1:
-            print("Success ! Here's the message : ")
-            print('\t', enc[1], '\n')
-        else:
-            print('Error occurred during the encryption process\n')
-
-
-decFlag = True
-
-
-def dec_f():
-    keysetup()
-    while decFlag:
-        print()
-        global key
-        print("press c to view commands.. ")
-        message = input('Decrypt a message : ')
-        input_wrap(message)
-        a = at.Crypt(message, key=key)
-        dec = a.decrypt()
-        if (dec[0]) == 1:
-            print("Success ! Here's the message : ")
-            print('\t', dec[1], '\n')
-        else:
-            print('Error occurred during the decryption process\n')
-
-
-file_encFlag = True
-
-
-file_decFlag = True
-
-
-def file_dec():
-    keysetup()
-    while file_decFlag:
-        print()
-        global key
-        pre = input(
-            "Running file decryption mode..\nPress the known commands or 'Enter' to continue.. : ")
-        print()
-        input_wrap(pre)
-        if pre == '':
-            print("You can use the commands AFTER entering the file name.. ")
-            filename = input('Enter full file name to be Decrypted : ')
-            target = af.CryptFile(filename, key)
-            a = target.decrypt()
-            if a == 1:
-                print('File successfully decrypted + removed .crypt extension')
-                print(f'File is now named {os.path.splitext(filename)[0]}')
-            if a == 2:
-                print('Cannot decrypt the file  when it is already empty')
-            if a == 3:
-                print(
-                    f'The file named : "{filename}" does not exists , try specifying the whole sys path')
-            if a == 0:
-                print(
-                    'Error in the decryption process. Check if the the file is distorted or it might just be '
-                    'decrypted already')
-            if a == 4:
-                print('Unknown Error has occurred ( system related ) \n')
-            if a == 5:
-                print('ERROR : Key is Not 256-bit')
-            if a == 6:
-                print('ERROR : File is already decrypted')
-            elif a == 7:
-                print('ERROR : Given a directory instead of a file')
-
-
-def file_enc():
-    keysetup()
-    while file_encFlag:
-        print()
-        global key
-        pre = input(
-            "Running file encryption mode..\nPress the known commands or 'Enter' to continue.. : ")
-        print()
-        input_wrap(pre)
-        if pre == '':
-            print("You can use the commands AFTER entering the file name.. ")
-            filename = input('Enter full file name to be Encrypted : ')
-            target = af.CryptFile(filename, key)
-            a = target.encrypt()
-            if a == 1:
-                print("File successfully encrypted + added '.crypt' extension")
-                print(f"File is now named : '{filename}.crypt' ")
-            if a == 2:
-                print('Cannot encrypt the file  when it is already empty')
-            if a == 3:
-                print(
-                    f'The file named : "{filename}" does not exists , try specifying the whole sys path')
-            if a == 0:
-                print(
-                    'Error in the encryption process. Check if the the file is distorted')
-            elif a == 4:
-                print('Unknown Error has occurred\n')
-            if a == 5:
-                print('ERROR : Key is Not 256-bit')
-            if a == 6:
-                print('ERROR : File is already encrypted')
-            elif a == 7:
-                print('ERROR : Given a directory instead of a file')
-
-
-if __name__ == '__main__':
-    intro()
+from AshCrypt import filecrypt as af
+from AshCrypt import textcrypt as at
+import os.path
+import sys
+
+
+print('Welcome to the CLI')
+
+commands = 'Commands : \n' \
+           '\tq: to quit the program \n' \
+           '\tc : view commands\n' \
+           '\te: for encryption\n' \
+           '\td : for decryption\n' \
+           '\tef : to encrypt a file\n' \
+           '\tdf : to decrypt a file\n'
+
+global key
+
+
+def input_selection(q=None, c=None, e=None, d=None, ef=None, df=None):
+    global encflag, decFlag, file_decFlag, file_encFlag
+    if q == 1:
+        sys.exit()
+    if c == 1:
+        print(commands)
+    if e == 1:
+        file_decFlag = False
+        file_encFlag = False
+        decFlag = False
+        encflag = True
+        enc_f()
+    if d == 1:
+        file_decFlag = False
+        file_encFlag = False
+        encflag = False
+        decFlag = True
+        dec_f()
+    if ef == 1:
+        decFlag = False
+        encflag = False
+        file_decFlag = False
+        file_encFlag = True
+        file_enc()
+    if df == 1:
+        encflag = False
+        decFlag = True
+        file_encFlag = False
+        file_decFlag = True
+        file_dec()
+    else:
+        pass
+
+
+def input_wrap(inp):
+    inp = inp.lower()
+    if inp == 'c':
+        input_selection(c=1)
+        return 'c'
+    if inp == 'q':
+        input_selection(q=1)
+        return 'q'
+    if inp == 'e':
+        input_selection(e=1)
+        return 'e'
+    if inp == 'd':
+        input_selection(d=1)
+        return 'd'
+    if inp == 'ef':
+        input_selection(ef=1)
+        return 'ef'
+    if inp == 'df':
+        input_selection(df=1)
+        return 'df'
+    else:
+        return None
+
+
+def intro():
+    while True:
+        print('Program started running..')
+        print('Press c to view commands : ')
+        while True:
+            n = input("Press..\n")
+            input_wrap(n)
+
+
+def keysetup():
+    outer = True
+    inner = True
+    while outer:
+        global key
+        key = ''
+        i = input('Do you have a key ?(y/n) : ')
+        input_wrap(i)
+        if i.lower() == 'n':
+            print("Here's your key : ")
+            key = at.Crypt.genkey()
+            print(key)
+            inner = False
+            outer = False
+        elif i.lower() == 'y':
+            while inner:
+                print('insert your key here : ')
+                kk = input()
+                input_wrap(kk)
+                if at.Crypt.keyverify(kk) == 1:
+                    print('Key selected\n')
+                    key = kk
+                    inner = False
+                    outer = False
+                else:
+                    print('Enter a valid key !\n')
+
+
+encflag = True
+
+
+def enc_f():
+    keysetup()
+    while encflag:
+        print()
+        global key
+        print("press c to view commands.. ")
+        message = input('Encrypt a message : ')
+        input_wrap(message)
+        a = at.Crypt(message, key=key)
+        enc = a.encrypt()
+        if (enc[0]) == 1:
+            print("Success ! Here's the message : ")
+            print('\t', enc[1], '\n')
+        else:
+            print('Error occurred during the encryption process\n')
+
+
+decFlag = True
+
+
+def dec_f():
+    keysetup()
+    while decFlag:
+        print()
+        global key
+        print("press c to view commands.. ")
+        message = input('Decrypt a message : ')
+        input_wrap(message)
+        a = at.Crypt(message, key=key)
+        dec = a.decrypt()
+        if (dec[0]) == 1:
+            print("Success ! Here's the message : ")
+            print('\t', dec[1], '\n')
+        else:
+            print('Error occurred during the decryption process\n')
+
+
+file_encFlag = True
+
+
+file_decFlag = True
+
+
+def file_dec():
+    keysetup()
+    while file_decFlag:
+        print()
+        global key
+        pre = input(
+            "Running file decryption mode..\nPress the known commands or 'Enter' to continue.. : ")
+        print()
+        input_wrap(pre)
+        if pre == '':
+            print("You can use the commands AFTER entering the file name.. ")
+            filename = input('Enter full file name to be Decrypted : ')
+            target = af.CryptFile(filename, key)
+            a = target.decrypt()
+            if a == 1:
+                print('File successfully decrypted + removed .crypt extension')
+                print(f'File is now named {os.path.splitext(filename)[0]}')
+            if a == 2:
+                print('Cannot decrypt the file  when it is already empty')
+            if a == 3:
+                print(
+                    f'The file named : "{filename}" does not exists , try specifying the whole sys path')
+            if a == 0:
+                print(
+                    'Error in the decryption process. Check if the the file is distorted or it might just be '
+                    'decrypted already')
+            if a == 4:
+                print('Unknown Error has occurred ( system related ) \n')
+            if a == 5:
+                print('ERROR : Key is Not 256-bit')
+            if a == 6:
+                print('ERROR : File is already decrypted')
+            elif a == 7:
+                print('ERROR : Given a directory instead of a file')
+
+
+def file_enc():
+    keysetup()
+    while file_encFlag:
+        print()
+        global key
+        pre = input(
+            "Running file encryption mode..\nPress the known commands or 'Enter' to continue.. : ")
+        print()
+        input_wrap(pre)
+        if pre == '':
+            print("You can use the commands AFTER entering the file name.. ")
+            filename = input('Enter full file name to be Encrypted : ')
+            target = af.CryptFile(filename, key)
+            a = target.encrypt()
+            if a == 1:
+                print("File successfully encrypted + added '.crypt' extension")
+                print(f"File is now named : '{filename}.crypt' ")
+            if a == 2:
+                print('Cannot encrypt the file  when it is already empty')
+            if a == 3:
+                print(
+                    f'The file named : "{filename}" does not exists , try specifying the whole sys path')
+            if a == 0:
+                print(
+                    'Error in the encryption process. Check if the the file is distorted')
+            elif a == 4:
+                print('Unknown Error has occurred\n')
+            if a == 5:
+                print('ERROR : Key is Not 256-bit')
+            if a == 6:
+                print('ERROR : File is already encrypted')
+            elif a == 7:
+                print('ERROR : Given a directory instead of a file')
+
+
+if __name__ == '__main__':
+    intro()
```

### Comparing `AshCrypt-3.0.2/AshCrypt/crypt.py` & `AshCrypt-3.0.3/AshCrypt/crypt.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-"""This module provides classes and functions for AES-256 encryption and decryption"""
-
-
-from typing import Union
-import hmac as hmc
-import base64
-import os
-import struct
-import bcrypt
-from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import hashes, hmac
-from cryptography.hazmat.primitives import padding
-
-
-class IterationsOutofRangeError(Exception):
-    """Exception raised when iterations come to be out of range usually due to message tampering
-    where the bytes representing the KDF iterations get touched"""
-
-    def __init__(self, num: any) -> None:
-        self.display = f'Iterations must be between 50 and 100000. RECEIVED : {num} '
-        super().__init__(self.display)
-
-
-class Enc:
-    """Class to encrypt data of either type bytes or strings"""
-
-    def __init__(self, message: Union[str, bytes], mainkey: str) -> None:
-        if isinstance(message, str):
-            self.message = message.encode()
-        elif isinstance(message, bytes):
-            self.message = message
-
-        self.mainkey = mainkey
-        self._iv = os.urandom(16)
-        self.salt = os.urandom(16)
-        self.pepper = os.urandom(16)
-        self.iterations = 50
-        if self.iterations < 50 or self.iterations > 100000:
-            raise IterationsOutofRangeError(self.iterations)
-        self.enc_key = self.derkey(self.mainkey, self.salt, self.iterations)
-        self.hmac_key = self.derkey(self.mainkey, self.pepper, self.iterations)
-
-    @staticmethod
-    def derkey(mainkey: str, salt_pepper: bytes, iterations: int) -> bytes:
-        """AES Key & HMAC derivation function"""
-        return bcrypt.kdf(
-            password=mainkey.encode('UTF-8'),
-            salt=salt_pepper,
-            desired_key_bytes=32,
-            rounds=iterations)
-
-    @staticmethod
-    def genkey() -> str:
-        """Generates a random 256-bit key as a hex string."""
-        return os.urandom(32).hex()
-
-    def mode(self):
-        """Returns AES Cipher Block Chaining (CBC) mode with the chosen initialization vector"""
-        return modes.CBC(self._iv)
-
-    def cipher(self):
-        """Creates AES cipher object using the encryption key and CBC mode"""
-        return Cipher(
-            algorithms.AES(
-                key=self.enc_key),
-            mode=self.mode(),
-            backend=default_backend())
-
-    def cipher_encryptor(self):
-        """Returns the encryptor for the AES cipher"""
-        return self.cipher().encryptor()
-
-    def padded_message(self) -> bytes:
-        """Pads the message to a multiple of the block size using PKCS#7 padding"""
-        padder = padding.PKCS7(128).padder()
-        return padder.update(self.message) + padder.finalize()
-
-    def ciphertext(self) -> bytes:
-        """Encrypts the padded message using AES and returns the ciphertext"""
-        return self.cipher_encryptor().update(self.padded_message()) + \
-            self.cipher_encryptor().finalize()
-
-    def hmac(self) -> bytes:
-        """Computes the HMAC-SHA512 of the ciphertext"""
-        _hmac = self.hmac_key
-        _hmac = hmac.HMAC(_hmac, hashes.SHA512())
-        _hmac.update(self.ciphertext())
-        return _hmac.finalize()
-
-    def setup_iterations(self) -> bytes:
-        """Packs the number of iterations into bytes using the 'big-endian' format"""
-        iters_bytes = struct.pack('!I', self.iterations)
-        return iters_bytes
-
-    def enc_to_bytes(self) -> bytes:
-        """Returns the encrypted data as bytes in the form 'HMAC' -> 'IV'
-        -> 'Salt value' -> 'pepper value' -> 'iterations' -> 'ciphertext """
-        return self.hmac() + self._iv + self.salt + self.pepper + \
-            self.setup_iterations() + self.ciphertext()
-
-    def enc_to_str(self) -> str:
-        """Returns a URL safe base 64 encoded string of the encrypted data"""
-        return base64.urlsafe_b64encode(self.enc_to_bytes()).decode('UTF-8')
-
-
-class MessageTamperingError(Exception):
-    """Raised when any part of the message gets tampered with. DISCARD THE MESSAGE"""
-
-    def __init__(self) -> None:
-        self.display = 'HMAC mismatch ! Message has been TAMPERED with ,\n' \
-                       ' or Possible key difference'
-        super().__init__(self.display)
-
-
-class Dec:
-    """Class to decrypt data of either type bytes or strings"""
-
-    def __init__(self, message: Union[str, bytes], mainkey: str) -> None:
-        if isinstance(message, str):
-            mess = message.encode('UTF-8')
-            self.message = base64.urlsafe_b64decode(mess)
-        elif isinstance(message, bytes):
-            self.message = message
-        self.key = mainkey
-        self.rec_hmac = self.message[:64]
-        self.rec_iv = self.message[64:80]
-        self.rec_salt = self.message[80:96]
-        self.rec_pepper = self.message[96:112]
-        self.rec_iterations = struct.unpack('!I', self.message[112:116])[0]
-        if self.rec_iterations < 50 or self.rec_iterations > 100000:
-            raise IterationsOutofRangeError(self.rec_iterations)
-        self.rec_ciphertext = self.message[116:]
-        self.dec_key = Enc.derkey(self.key, self.rec_salt, self.rec_iterations)
-        self.hmac_k = Enc.derkey(
-            self.key,
-            self.rec_pepper,
-            self.rec_iterations)
-        if self.verify_hmac() is False:
-            raise MessageTamperingError()
-
-    def calculated_hmac(self) -> bytes:
-        """Computes the HMAC-SHA512 of the received ciphertext"""
-        _hmac = self.hmac_k
-        _hmac = hmac.HMAC(_hmac, hashes.SHA512())
-        _hmac.update(self.rec_ciphertext)
-        return _hmac.finalize()
-
-    def verify_hmac(self) -> bool:
-        """Verifies the received HMAC-SHA512 against the calculated HMAC"""
-        return hmc.compare_digest(self.calculated_hmac(), self.rec_hmac)
-
-    def mode(self):
-        """Returns the AES Cipher Block Chaining (CBC) mode with the received  IV"""
-        return modes.CBC(self.rec_iv)
-
-    def cipher(self):
-        """Creates an AES cipher object using the decryption key and CBC mode"""
-        return Cipher(
-            algorithms.AES(
-                key=self.dec_key),
-            mode=self.mode(),
-            backend=default_backend())
-
-    def cipher_decryptor(self):
-        """Returns the decryptor for the AES cipher"""
-        return self.cipher().decryptor()
-
-    def pre_unpadding_dec(self) -> bytes:
-        """Decrypts the received ciphertext and returns the pre-unpadded data"""
-        return self.cipher_decryptor().update(self.rec_ciphertext) + \
-            self.cipher_decryptor().finalize()
-
-    def unpadded_m(self) -> bytes:
-        """Unpads the pre-unpadded data and returns the original message """
-        unpadder = padding.PKCS7(128).unpadder()
-        return unpadder.update(self.pre_unpadding_dec()) + unpadder.finalize()
-
-    def dec_to_bytes(self) -> bytes:
-        """Returns the decrypted message as bytes"""
-        return self.unpadded_m()
-
-    def dec_to_str(self) -> str:
-        """Returns the decrypted message as a UTF-8 encoded string"""
-        return self.unpadded_m().decode('UTF-8')
+"""This module provides classes and functions for AES-256 encryption and decryption"""
+
+
+from typing import Union
+import hmac as hmc
+import base64
+import os
+import struct
+import bcrypt
+from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hashes, hmac
+from cryptography.hazmat.primitives import padding
+
+
+class IterationsOutofRangeError(Exception):
+    """Exception raised when iterations come to be out of range usually due to message tampering
+    where the bytes representing the KDF iterations get touched"""
+
+    def __init__(self, num: any) -> None:
+        self.display = f'Iterations must be between 50 and 100000. RECEIVED : {num} '
+        super().__init__(self.display)
+
+
+class Enc:
+    """Class to encrypt data of either type bytes or strings"""
+
+    def __init__(self, message: Union[str, bytes], mainkey: str) -> None:
+        if isinstance(message, str):
+            self.message = message.encode()
+        elif isinstance(message, bytes):
+            self.message = message
+
+        self.mainkey = mainkey
+        self._iv = os.urandom(16)
+        self.salt = os.urandom(16)
+        self.pepper = os.urandom(16)
+        self.iterations = 50
+        if self.iterations < 50 or self.iterations > 100000:
+            raise IterationsOutofRangeError(self.iterations)
+        self.enc_key = self.derkey(self.mainkey, self.salt, self.iterations)
+        self.hmac_key = self.derkey(self.mainkey, self.pepper, self.iterations)
+
+    @staticmethod
+    def derkey(mainkey: str, salt_pepper: bytes, iterations: int) -> bytes:
+        """AES Key & HMAC derivation function"""
+        return bcrypt.kdf(
+            password=mainkey.encode('UTF-8'),
+            salt=salt_pepper,
+            desired_key_bytes=32,
+            rounds=iterations)
+
+    @staticmethod
+    def genkey() -> str:
+        """Generates a random 256-bit key as a hex string."""
+        return os.urandom(32).hex()
+
+    def mode(self):
+        """Returns AES Cipher Block Chaining (CBC) mode with the chosen initialization vector"""
+        return modes.CBC(self._iv)
+
+    def cipher(self):
+        """Creates AES cipher object using the encryption key and CBC mode"""
+        return Cipher(
+            algorithms.AES(
+                key=self.enc_key),
+            mode=self.mode(),
+            backend=default_backend())
+
+    def cipher_encryptor(self):
+        """Returns the encryptor for the AES cipher"""
+        return self.cipher().encryptor()
+
+    def padded_message(self) -> bytes:
+        """Pads the message to a multiple of the block size using PKCS#7 padding"""
+        padder = padding.PKCS7(128).padder()
+        return padder.update(self.message) + padder.finalize()
+
+    def ciphertext(self) -> bytes:
+        """Encrypts the padded message using AES and returns the ciphertext"""
+        return self.cipher_encryptor().update(self.padded_message()) + \
+            self.cipher_encryptor().finalize()
+
+    def hmac(self) -> bytes:
+        """Computes the HMAC-SHA512 of the ciphertext"""
+        _hmac = self.hmac_key
+        _hmac = hmac.HMAC(_hmac, hashes.SHA512())
+        _hmac.update(self.ciphertext())
+        return _hmac.finalize()
+
+    def setup_iterations(self) -> bytes:
+        """Packs the number of iterations into bytes using the 'big-endian' format"""
+        iters_bytes = struct.pack('!I', self.iterations)
+        return iters_bytes
+
+    def enc_to_bytes(self) -> bytes:
+        """Returns the encrypted data as bytes in the form 'HMAC' -> 'IV'
+        -> 'Salt value' -> 'pepper value' -> 'iterations' -> 'ciphertext """
+        return self.hmac() + self._iv + self.salt + self.pepper + \
+            self.setup_iterations() + self.ciphertext()
+
+    def enc_to_str(self) -> str:
+        """Returns a URL safe base 64 encoded string of the encrypted data"""
+        return base64.urlsafe_b64encode(self.enc_to_bytes()).decode('UTF-8')
+
+
+class MessageTamperingError(Exception):
+    """Raised when any part of the message gets tampered with. DISCARD THE MESSAGE"""
+
+    def __init__(self) -> None:
+        self.display = 'HMAC mismatch ! Message has been TAMPERED with ,\n' \
+                       ' or Possible key difference'
+        super().__init__(self.display)
+
+
+class Dec:
+    """Class to decrypt data of either type bytes or strings"""
+
+    def __init__(self, message: Union[str, bytes], mainkey: str) -> None:
+        if isinstance(message, str):
+            mess = message.encode('UTF-8')
+            self.message = base64.urlsafe_b64decode(mess)
+        elif isinstance(message, bytes):
+            self.message = message
+        self.key = mainkey
+        self.rec_hmac = self.message[:64]
+        self.rec_iv = self.message[64:80]
+        self.rec_salt = self.message[80:96]
+        self.rec_pepper = self.message[96:112]
+        self.rec_iterations = struct.unpack('!I', self.message[112:116])[0]
+        if self.rec_iterations < 50 or self.rec_iterations > 100000:
+            raise IterationsOutofRangeError(self.rec_iterations)
+        self.rec_ciphertext = self.message[116:]
+        self.dec_key = Enc.derkey(self.key, self.rec_salt, self.rec_iterations)
+        self.hmac_k = Enc.derkey(
+            self.key,
+            self.rec_pepper,
+            self.rec_iterations)
+        if self.verify_hmac() is False:
+            raise MessageTamperingError()
+
+    def calculated_hmac(self) -> bytes:
+        """Computes the HMAC-SHA512 of the received ciphertext"""
+        _hmac = self.hmac_k
+        _hmac = hmac.HMAC(_hmac, hashes.SHA512())
+        _hmac.update(self.rec_ciphertext)
+        return _hmac.finalize()
+
+    def verify_hmac(self) -> bool:
+        """Verifies the received HMAC-SHA512 against the calculated HMAC"""
+        return hmc.compare_digest(self.calculated_hmac(), self.rec_hmac)
+
+    def mode(self):
+        """Returns the AES Cipher Block Chaining (CBC) mode with the received  IV"""
+        return modes.CBC(self.rec_iv)
+
+    def cipher(self):
+        """Creates an AES cipher object using the decryption key and CBC mode"""
+        return Cipher(
+            algorithms.AES(
+                key=self.dec_key),
+            mode=self.mode(),
+            backend=default_backend())
+
+    def cipher_decryptor(self):
+        """Returns the decryptor for the AES cipher"""
+        return self.cipher().decryptor()
+
+    def pre_unpadding_dec(self) -> bytes:
+        """Decrypts the received ciphertext and returns the pre-unpadded data"""
+        return self.cipher_decryptor().update(self.rec_ciphertext) + \
+            self.cipher_decryptor().finalize()
+
+    def unpadded_m(self) -> bytes:
+        """Unpads the pre-unpadded data and returns the original message """
+        unpadder = padding.PKCS7(128).unpadder()
+        return unpadder.update(self.pre_unpadding_dec()) + unpadder.finalize()
+
+    def dec_to_bytes(self) -> bytes:
+        """Returns the decrypted message as bytes"""
+        return self.unpadded_m()
+
+    def dec_to_str(self) -> str:
+        """Returns the decrypted message as a UTF-8 encoded string"""
+        return self.unpadded_m().decode('UTF-8')
```

### Comparing `AshCrypt-3.0.2/AshCrypt/database.py` & `AshCrypt-3.0.3/AshCrypt/database.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,274 +1,274 @@
-from dataclasses import dataclass, field
-from typing import Union, Generator
-from datetime import datetime
-import sqlite3
-import os
-
-
-@dataclass
-class Database:
-    dbname: str = field()
-    tablename: str = field(default='Classified')
-    conn: sqlite3.Connection = field(init=False, repr=False)
-    c: sqlite3.Cursor = field(init=False, repr=False)
-
-    def __post_init__(self):
-        self.conn = sqlite3.connect(self.dbname)
-        self.c = self.conn.cursor()
-
-    @property
-    def size(self) -> Union[int, tuple]:         # Size in MB #
-        try:
-            with self.conn:
-                self.c.execute(
-                    'SELECT page_count * page_size FROM pragma_page_count() , pragma_page_size')
-                size_info = self.c.fetchone()
-                size = size_info[0] / 1024 / 1024
-                return size
-        except sqlite3.Error as e:
-            return -1, e
-
-    @property
-    def last_mod(self) -> Union[datetime, tuple]:
-        try:
-            time_stat = datetime.fromtimestamp(os.stat(self.dbname).st_mtime)
-            return time_stat
-
-        except OSError as e:
-            return 0, e
-
-    @property
-    def default_routing(self) -> str:
-        return f'DEFAULT ROUTING ALL METHODS TO "{self.tablename}"'
-
-    def query(self, *querys: str) -> list:
-        result = []
-        for i, query in enumerate(querys):
-            if not isinstance(query, str):
-                result.append({f'query {i}': (-1, TypeError)})
-            try:
-                with self.conn:
-                    self.c.execute(query)
-                    if self.c.rowcount == 1:
-                        result.append(
-                            {f'query {i}': ['SUCCESS', self.c.fetchone()]})
-                    else:
-                        result.append(
-                            {f'query {i}': ['SUCCESS', self.c.fetchall()]})
-
-            except sqlite3.Error as e:
-                result.append({f'query {i}': ('FAILURE', e.__str__())})
-        return result
-
-    def addtable(self, optional_tablename=None) -> Union[int, tuple]:
-        if optional_tablename is None:
-            try:
-                with self.conn:
-                    self.c.execute(
-                        f"CREATE TABLE IF NOT EXISTS {self.tablename} "
-                        "(ID INTEGER PRIMARY KEY, Name Text , Content BLOB ,Key TEXT )")
-                return 11
-            except sqlite3.Error as e:
-                return -1, e
-
-        else:
-            try:
-                with self.conn:
-                    self.c.execute(
-                        f"CREATE TABLE IF NOT EXISTS {optional_tablename} "
-                        "(ID INTEGER PRIMARY KEY,"
-                        "Name TEXT ,"
-                        "Content BLOB ,"
-                        "Key TEXT )")
-                    self.tablename = optional_tablename
-                return 1
-
-            except sqlite3.Error as e:
-                return 0, e
-
-    def insert(self, name, content, key,
-               optional_table_name=None) -> Union[int, tuple]:
-        if optional_table_name is None:
-            try:
-                with self.conn:
-                    self.c.execute(
-                        f"INSERT INTO {self.tablename} (Name , Content ,Key) VALUES (? , ? , ?) ",
-                        (name,
-                         content,
-                         key))
-
-                return 11
-            except sqlite3.Error as e:
-                return -1, e
-
-        else:
-            try:
-                with self.conn:
-                    self.c.execute(
-                        f"INSERT INTO {optional_table_name} (Name, Content ,Key) VALUES (? , ? , ?) ",
-                        (name,
-                         content,
-                         key))
-                return 1
-            except sqlite3.Error as e:
-                return 0, e
-
-    def update(
-            self,
-            column_name: str,
-            new_column_val: str,
-            idd: int,
-            optional_table_name=None) -> Union[int, tuple]:
-        if optional_table_name is None:
-            try:
-                with self.conn:
-                    self.c.execute(
-                        f'UPDATE {self.tablename} SET {column_name} = ? WHERE ID = ? ',
-                        (new_column_val,
-                         idd))
-                    return 11
-
-            except sqlite3.Error as e:
-                return -1, e
-
-        else:
-            try:
-                with self.conn:
-                    self.c.execute(
-                        f'UPDATE {optional_table_name} SET {column_name} = ? WHERE ID = ? ',
-                        (new_column_val,
-                         idd))
-                    return 1
-
-            except sqlite3.Error as e:
-                return 0, e
-
-    def content(self, optional_tablename=None) -> Union[Generator, tuple]:
-        if optional_tablename is None:
-            try:
-                with self.conn:
-                    self.c.execute(f'SELECT * FROM {self.tablename} ')
-                    for row in self.c.fetchall():
-                        yield row
-
-            except sqlite3.Error as e:
-                return -1, e
-
-        else:
-            try:
-                with self.conn:
-                    self.c.execute(f'SELECT * FROM {optional_tablename} ')
-                    for row in self.c.fetchall():
-                        yield row
-
-            except sqlite3.Error as e:
-                return 0, e
-
-    def content_by_id(
-            self, idd: int, optional_tablename=None) -> Union[Generator, tuple]:
-        if optional_tablename is None:
-            try:
-                with self.conn:
-                    self.c.execute(
-                        f'SELECT * FROM {self.tablename} WHERE ID = ? ', (idd,))
-                    for row in self.c.fetchall():
-                        yield row
-
-            except sqlite3.Error as e:
-                return -1, e
-
-        else:
-            try:
-                with self.conn:
-                    self.c.execute(
-                        f'SELECT * FROM {optional_tablename} WHERE ID = ? ', (idd,))
-                    for row in self.c.fetchall():
-                        yield row
-
-            except sqlite3.Error as e:
-                return 0, e
-
-    def show_contents(self, *optional_tablenames) -> Union[Generator, tuple]:
-        if optional_tablenames:
-            try:
-                for arg in optional_tablenames:
-                    with self.conn:
-                        self.c.execute(f'SELECT * FROM {arg} ')
-                        for row in self.c.fetchall():
-                            yield {arg: row}
-
-            except sqlite3.Error as e:
-                return -1, e
-
-        else:
-            try:
-                with self.conn:
-                    self.c.execute(f'SELECT * FROM {self.tablename} ')
-                    for row in self.c.fetchall():
-                        yield {self.tablename: row}
-
-            except sqlite3.Error as e:
-                return 0, e
-
-    def show_tables(self) -> Union[Generator, tuple]:
-        try:
-            with self.conn:
-                self.c.execute(
-                    "SELECT name FROM sqlite_master WHERE type= 'table' ")
-                for row in self.c.fetchall():
-                    yield row
-
-        except sqlite3.Error as e:
-            return 0, e
-
-    def dropall(self) -> Union[int, tuple]:
-        try:
-            with self.conn:
-                self.c.execute(
-                    "SELECT name FROM sqlite_master WHERE type= 'table' ")
-                for table in self.c.fetchall():
-                    self.c.execute(f'DROP TABLE {table[0]}')
-                return 1
-
-        except sqlite3.Error as e:
-            return 0, e
-
-    def drop_table(self, *table_names) -> Union[int, tuple]:
-        if table_names:
-            try:
-                for arg in table_names:
-                    with self.conn:
-                        self.c.execute(f"DROP TABLE {arg}")
-                return 1
-            except sqlite3.Error as e:
-                return -1, e
-
-        else:
-            try:
-                with self.conn:
-                    self.c.execute(f'DROP TABLE {self.tablename}')
-                    return 1
-
-            except sqlite3.Error as e:
-                return 0, e
-
-    def drop_content(self, idd, optional_table_name=None) -> Union[int, tuple]:
-        if optional_table_name is None:
-            try:
-                with self.conn:
-                    self.c.execute(
-                        f'DELETE FROM {self.tablename} WHERE ID = {idd}')
-                return 11
-
-            except sqlite3.Error as e:
-                return -1, e
-
-        else:
-            try:
-                with self.conn:
-                    self.c.execute(
-                        f'DELETE FROM {optional_table_name} WHERE ID = {idd}')
-                return 1
-
-            except sqlite3.Error as e:
-                return 0, e
+from dataclasses import dataclass, field
+from typing import Union, Generator
+from datetime import datetime
+import sqlite3
+import os
+
+
+@dataclass
+class Database:
+    dbname: str = field()
+    tablename: str = field(default='Classified')
+    conn: sqlite3.Connection = field(init=False, repr=False)
+    c: sqlite3.Cursor = field(init=False, repr=False)
+
+    def __post_init__(self):
+        self.conn = sqlite3.connect(self.dbname)
+        self.c = self.conn.cursor()
+
+    @property
+    def size(self) -> Union[int, tuple]:         # Size in MB #
+        try:
+            with self.conn:
+                self.c.execute(
+                    'SELECT page_count * page_size FROM pragma_page_count() , pragma_page_size')
+                size_info = self.c.fetchone()
+                size = size_info[0] / 1024 / 1024
+                return size
+        except sqlite3.Error as e:
+            return -1, e
+
+    @property
+    def last_mod(self) -> Union[datetime, tuple]:
+        try:
+            time_stat = datetime.fromtimestamp(os.stat(self.dbname).st_mtime)
+            return time_stat
+
+        except OSError as e:
+            return 0, e
+
+    @property
+    def default_routing(self) -> str:
+        return f'DEFAULT ROUTING ALL METHODS TO "{self.tablename}"'
+
+    def query(self, *querys: str) -> list:
+        result = []
+        for i, query in enumerate(querys):
+            if not isinstance(query, str):
+                result.append({f'query {i}': (-1, TypeError)})
+            try:
+                with self.conn:
+                    self.c.execute(query)
+                    if self.c.rowcount == 1:
+                        result.append(
+                            {f'query {i}': ['SUCCESS', self.c.fetchone()]})
+                    else:
+                        result.append(
+                            {f'query {i}': ['SUCCESS', self.c.fetchall()]})
+
+            except sqlite3.Error as e:
+                result.append({f'query {i}': ('FAILURE', e.__str__())})
+        return result
+
+    def addtable(self, optional_tablename=None) -> Union[int, tuple]:
+        if optional_tablename is None:
+            try:
+                with self.conn:
+                    self.c.execute(
+                        f"CREATE TABLE IF NOT EXISTS {self.tablename} "
+                        "(ID INTEGER PRIMARY KEY, Name Text , Content BLOB ,Key TEXT )")
+                return 11
+            except sqlite3.Error as e:
+                return -1, e
+
+        else:
+            try:
+                with self.conn:
+                    self.c.execute(
+                        f"CREATE TABLE IF NOT EXISTS {optional_tablename} "
+                        "(ID INTEGER PRIMARY KEY,"
+                        "Name TEXT ,"
+                        "Content BLOB ,"
+                        "Key TEXT )")
+                    self.tablename = optional_tablename
+                return 1
+
+            except sqlite3.Error as e:
+                return 0, e
+
+    def insert(self, name, content, key,
+               optional_table_name=None) -> Union[int, tuple]:
+        if optional_table_name is None:
+            try:
+                with self.conn:
+                    self.c.execute(
+                        f"INSERT INTO {self.tablename} (Name , Content ,Key) VALUES (? , ? , ?) ",
+                        (name,
+                         content,
+                         key))
+
+                return 11
+            except sqlite3.Error as e:
+                return -1, e
+
+        else:
+            try:
+                with self.conn:
+                    self.c.execute(
+                        f"INSERT INTO {optional_table_name} (Name, Content ,Key) VALUES (? , ? , ?) ",
+                        (name,
+                         content,
+                         key))
+                return 1
+            except sqlite3.Error as e:
+                return 0, e
+
+    def update(
+            self,
+            column_name: str,
+            new_column_val: str,
+            idd: int,
+            optional_table_name=None) -> Union[int, tuple]:
+        if optional_table_name is None:
+            try:
+                with self.conn:
+                    self.c.execute(
+                        f'UPDATE {self.tablename} SET {column_name} = ? WHERE ID = ? ',
+                        (new_column_val,
+                         idd))
+                    return 11
+
+            except sqlite3.Error as e:
+                return -1, e
+
+        else:
+            try:
+                with self.conn:
+                    self.c.execute(
+                        f'UPDATE {optional_table_name} SET {column_name} = ? WHERE ID = ? ',
+                        (new_column_val,
+                         idd))
+                    return 1
+
+            except sqlite3.Error as e:
+                return 0, e
+
+    def content(self, optional_tablename=None) -> Union[Generator, tuple]:
+        if optional_tablename is None:
+            try:
+                with self.conn:
+                    self.c.execute(f'SELECT * FROM {self.tablename} ')
+                    for row in self.c.fetchall():
+                        yield row
+
+            except sqlite3.Error as e:
+                return -1, e
+
+        else:
+            try:
+                with self.conn:
+                    self.c.execute(f'SELECT * FROM {optional_tablename} ')
+                    for row in self.c.fetchall():
+                        yield row
+
+            except sqlite3.Error as e:
+                return 0, e
+
+    def content_by_id(
+            self, idd: int, optional_tablename=None) -> Union[Generator, tuple]:
+        if optional_tablename is None:
+            try:
+                with self.conn:
+                    self.c.execute(
+                        f'SELECT * FROM {self.tablename} WHERE ID = ? ', (idd,))
+                    for row in self.c.fetchall():
+                        yield row
+
+            except sqlite3.Error as e:
+                return -1, e
+
+        else:
+            try:
+                with self.conn:
+                    self.c.execute(
+                        f'SELECT * FROM {optional_tablename} WHERE ID = ? ', (idd,))
+                    for row in self.c.fetchall():
+                        yield row
+
+            except sqlite3.Error as e:
+                return 0, e
+
+    def show_contents(self, *optional_tablenames) -> Union[Generator, tuple]:
+        if optional_tablenames:
+            try:
+                for arg in optional_tablenames:
+                    with self.conn:
+                        self.c.execute(f'SELECT * FROM {arg} ')
+                        for row in self.c.fetchall():
+                            yield {arg: row}
+
+            except sqlite3.Error as e:
+                return -1, e
+
+        else:
+            try:
+                with self.conn:
+                    self.c.execute(f'SELECT * FROM {self.tablename} ')
+                    for row in self.c.fetchall():
+                        yield {self.tablename: row}
+
+            except sqlite3.Error as e:
+                return 0, e
+
+    def show_tables(self) -> Union[Generator, tuple]:
+        try:
+            with self.conn:
+                self.c.execute(
+                    "SELECT name FROM sqlite_master WHERE type= 'table' ")
+                for row in self.c.fetchall():
+                    yield row
+
+        except sqlite3.Error as e:
+            return 0, e
+
+    def dropall(self) -> Union[int, tuple]:
+        try:
+            with self.conn:
+                self.c.execute(
+                    "SELECT name FROM sqlite_master WHERE type= 'table' ")
+                for table in self.c.fetchall():
+                    self.c.execute(f'DROP TABLE {table[0]}')
+                return 1
+
+        except sqlite3.Error as e:
+            return 0, e
+
+    def drop_table(self, *table_names) -> Union[int, tuple]:
+        if table_names:
+            try:
+                for arg in table_names:
+                    with self.conn:
+                        self.c.execute(f"DROP TABLE {arg}")
+                return 1
+            except sqlite3.Error as e:
+                return -1, e
+
+        else:
+            try:
+                with self.conn:
+                    self.c.execute(f'DROP TABLE {self.tablename}')
+                    return 1
+
+            except sqlite3.Error as e:
+                return 0, e
+
+    def drop_content(self, idd, optional_table_name=None) -> Union[int, tuple]:
+        if optional_table_name is None:
+            try:
+                with self.conn:
+                    self.c.execute(
+                        f'DELETE FROM {self.tablename} WHERE ID = {idd}')
+                return 11
+
+            except sqlite3.Error as e:
+                return -1, e
+
+        else:
+            try:
+                with self.conn:
+                    self.c.execute(
+                        f'DELETE FROM {optional_table_name} WHERE ID = {idd}')
+                return 1
+
+            except sqlite3.Error as e:
+                return 0, e
```

### Comparing `AshCrypt-3.0.2/AshCrypt/gui.py` & `AshCrypt-3.0.3/AshCrypt/gui.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,1105 +1,1131 @@
-import AshCrypt.textcrypt as At
-import AshCrypt.filecrypt as Af
-import AshCrypt.database as Ad
-import ttkbootstrap as tk
-import AshCrypt.qr as qr
-import platform
-import secrets
-import os.path
-import string
-import atexit
-import json
-import re
-
-
-'''------------------------FRAMING STARTED-------------------'''
-
-main_object = tk.Window(themename='vapor')
-main_object.resizable(False, False)
-main_object.title('AshCrypt')
-main_object.geometry('1500x800')
-
-
-databaseFrame = tk.Frame(master=main_object, width=500, height=800)
-databaseFrame.place(x=0, y=0)
-
-frameFile1 = tk.Frame(master=main_object, width=500, height=250)
-frameFile1.place(x=500, y=0)
-
-frameFile2 = tk.Frame(master=main_object, width=500, height=250)
-frameFile2.place(x=500, y=250)
-
-textFrame1 = tk.Frame(master=main_object, width=500, height=250)
-textFrame1.place(x=1000, y=0)
-
-textFrame2 = tk.Frame(master=main_object, width=500, height=250)
-textFrame2.place(x=1000, y=250)
-
-lowerFrame = tk.Frame(master=main_object, width=1000, height=260)
-lowerFrame.place(x=500, y=540)
-
-'''---------------DATABASE FRAME STARTED-----------------------'''
-
-
-databaseFrame = tk.Frame(master=main_object, height=800, width=500)
-databaseFrame.place(rely=0, relx=0)
-
-if platform.system() == 'Windows':
-    console_label = tk.Label(
-        master=databaseFrame,
-        text='DATABASE OUTPUT CONSOLE',
-        font='Terminal 15 bold')
-    console_label.place(relx=0.09, rely=0.04)
-
-    db_display_text = tk.ScrolledText(
-        width=43,
-        height=27,
-        font='terminal 13',
-        wrap='word')
-    db_display_text.place(relx=0.016, rely=0.105)
-    db_display_text.insert(tk.END, 'Waiting to fetch..')
-else:
-    console_label = tk.Label(
-        master=databaseFrame,
-        text='DATABASE OUTPUT CONSOLE',
-        font='Calibre 15 bold')
-    console_label.place(relx=0.115, rely=0.04)
-
-    db_display_text = tk.Text(
-        width=38,
-        height=22,
-        font='Calibre 13 bold',
-        wrap='word')
-    db_display_text.place(relx=0.015, rely=0.105)
-    db_display_text.insert(tk.END, 'Waiting to fetch..')
-
-
-def show_all_content():
-    global db_enable_blocker, main_db_name_var, usable_real_path, main_db_conn, db_display_text, keys_db_conn
-    if db_enable_blocker != 0:
-        db_display_text.delete('1.0', tk.END)
-        db_display_text.insert(
-            tk.END, f"Check 'output.json' in the chosen path : {usable_real_path}\n")
-        json_path = os.path.join(usable_real_path, 'output.json')
-        if swich_db_var.get() == 1:
-            conn = keys_db_conn
-        else:
-            conn = main_db_conn
-        try:
-            with open(json_path, 'w') as f:
-                buffer = {}
-                for e in conn.content():
-                    buffer['ID ' + e[0].__str__()] = [{'Filename': e[1]}, {
-                        'Content': e[2].__str__()}, {'KeyRef': e[3]}]
-                json_content = json.dumps(buffer, indent=2)
-                f.write(json_content)
-                db_display_text.insert(
-                    tk.END, f"\nSuccessfully written all table content in output.json\n"
-                    f"\nNote that this file will be deleted when the app is closed")
-        except BaseException:
-            db_display_text.insert(
-                tk.END, f"Failed to write all table content in output.json\n")
-
-
-def show_content_by_id():
-    global db_enable_blocker, main_db_conn, keys_db_conn, content_id_entry_var, usable_real_path
-    idd = content_id_entry_var.get().strip()
-    last_id = checkid()
-    if db_enable_blocker != 0:
-        if swich_db_var.get() == 1:
-            conn = keys_db_conn
-        else:
-            conn = main_db_conn
-        try:
-            if int(idd) > 0:
-                if last_id == -1:
-                    db_display_text.delete('1.0', tk.END)
-                    db_display_text.insert(
-                        tk.END, 'The table does not have any content to show')
-                elif last_id != -1:
-
-                    if int(idd) in range(1, last_id):
-                        db_display_text.delete('1.0', tk.END)
-                        to_json_path = os.path.join(
-                            usable_real_path, 'output.json')
-                        with open(to_json_path, 'w') as f:
-                            buffer = {}
-                            for e in conn.content_by_id(int(idd)):
-                                buffer['ID_' + e[0].__str__()] = [{'Filename': e[1]}, {
-                                    'Content': e[2].__str__()}, {'KeyRef': e[3]}]
-                            json_content = json.dumps(buffer, indent=2)
-                            f.write(json_content)
-                        db_display_text.insert(
-                            tk.END, f"Successful fetch !\n\nCheck the 'output.json' file in the"
-                            f" chosen path :\n\n'{usable_real_path}'")
-                    if int(idd) == last_id:
-                        db_display_text.delete('1.0', tk.END)
-                        db_display_text.insert(tk.END, 'Chosen last ID\n\n')
-                        to_json_path = os.path.join(
-                            usable_real_path, 'output.json')
-                        try:
-                            with open(to_json_path, 'w') as f:
-                                buffer = {}
-                                for e in conn.content_by_id(int(idd)):
-                                    buffer['ID_' + e[0].__str__()] = [{'Filename': e[1]}, {
-                                        'Content': e[2].__str__()}, {'KeyRef': e[3]}]
-                                json_content = json.dumps(buffer, indent=2)
-                                f.write(json_content)
-                            db_display_text.insert(
-                                tk.END, f"Successful fetch !\n\nCheck the 'output.json' file in the"
-                                f" the chosen path :\n\n'{usable_real_path}'")
-                        except BaseException:
-                            db_display_text.delete('1.0', tk.END)
-                            db_display_text.insert(
-                                tk.END, "ERROR \n\nCheck the validity of 'output.json' file"
-                                "\n\nCheck if the database is faulty\n")
-                    elif int(idd) > last_id:
-                        db_display_text.delete('1.0', tk.END)
-                        db_display_text.insert(
-                            tk.END, 'Given ID is greater than the highest available ID')
-            else:
-                db_display_text.delete('1.0', tk.END)
-                db_display_text.insert(
-                    tk.END, 'ID must be strictly greater than 0')
-        except BaseException:
-            db_display_text.delete('1.0', tk.END)
-            db_display_text.insert(tk.END, 'ID value must be a valid integer')
-
-
-def drop_content_by_id():
-    global db_enable_blocker, main_db_conn, keys_db_conn, content_id_entry_var
-    idd = content_id_entry_var.get().strip()
-    last_id = checkid()
-    if db_enable_blocker != 0:
-        if swich_db_var.get() == 1:
-            conn = keys_db_conn
-        else:
-            conn = main_db_conn
-        try:
-            if int(idd) > 0:
-                if last_id == -1:
-                    db_display_text.delete('1.0', tk.END)
-                    db_display_text.insert(
-                        tk.END, 'The table does not have any content to drop')
-                elif last_id != -1:
-
-                    if int(idd) in range(1, last_id):
-                        db_display_text.delete('1.0', tk.END)
-                        db_display_text.insert(tk.END, 'Valid ID')
-                        conn.drop_content(idd)
-                        db_display_text.insert(
-                            tk.END, f'\nDropping by ID {idd} Went successful')
-
-                    if int(idd) == last_id:
-                        db_display_text.delete('1.0', tk.END)
-                        db_display_text.insert(tk.END, 'Chosen last ID')
-                        conn.drop_content(idd)
-                        db_display_text.insert(
-                            tk.END, f'\nDropping by ID {idd} Went successful')
-
-                    elif int(idd) > last_id:
-                        db_display_text.delete('1.0', tk.END)
-                        db_display_text.insert(
-                            tk.END, 'Given ID is greater than the highest available ID')
-            else:
-                db_display_text.delete('1.0', tk.END)
-                db_display_text.insert(
-                    tk.END, 'ID must be strictly greater than 0')
-        except BaseException:
-            db_display_text.delete('1.0', tk.END)
-            db_display_text.insert(tk.END, 'ID value must be a valid integer')
-
-
-show_all_content_button = tk.Button(
-    master=databaseFrame,
-    text='SHOW ALL TABLE CONTENT',
-    command=show_all_content,
-    bootstyle='warning outline')
-show_all_content_button.place(relx=0.287, rely=0.87)
-
-
-query_clicks = 1
-
-
-def query():
-    global db_enable_blocker, main_db_conn, keys_db_conn, usable_real_path, query_clicks
-    if db_enable_blocker != 0:
-        if swich_db_var.get() == 1:
-            conn = keys_db_conn
-        else:
-            conn = main_db_conn
-        query_var = query_entry_var.get().strip()
-        if len(query_var) > 0:
-            try:
-                db_display_text.delete('1.0', tk.END)
-                json_file = os.path.join(usable_real_path, 'output.json')
-                with open(json_file, 'w') as f:
-                    query_out = conn.query(query_var)
-                    conn.addtable()
-                    json_content = json.dumps(
-                        {f'query {query_clicks}': query_out}, indent=2)
-                    query_clicks += 1
-                    f.write(json_content)
-                db_display_text.insert(
-                    tk.END, f"Ran query {query_clicks} !\n\n")
-                db_display_text.insert(
-                    tk.END, f"The result of the query is in 'output.json' file\n\n")
-            except BaseException:
-                db_display_text.delete('1.0', tk.END)
-                db_display_text.insert(
-                    tk.END, f"Failed to finish the query!\n\n")
-                db_display_text.insert(
-                    tk.END, 'Detected object that is not JSON serializable\n\n')
-                db_display_text.insert(
-                    tk.END, 'Use buttons instead if possible')
-        else:
-            db_display_text.delete('1.0', tk.END)
-            db_display_text.insert(tk.END, f"Can't query nothing\n\n")
-
-
-query_entry_var = tk.StringVar()
-query_entry = tk.Entry(
-    master=databaseFrame,
-    width=38,
-    font='Calibre 13 bold',
-    textvariable=query_entry_var)
-
-query_entry.place(relx=0.043, rely=0.742)
-
-query_button = tk.Button(
-    master=databaseFrame,
-    text='RUN QUERY',
-    command=query,
-    bootstyle='warning outline')
-query_button.place(relx=0.39, rely=0.81)
-
-
-drop_content_by_id_button = tk.Button(
-    master=databaseFrame,
-    text='DROP CONTENT BY ID',
-    command=drop_content_by_id,
-    bootstyle='warning outline')
-drop_content_by_id_button.place(relx=0.08, rely=0.93)
-
-content_id_entry_var = tk.StringVar(value=' ID')
-content_id_entry = tk.Entry(
-    master=databaseFrame,
-    textvariable=content_id_entry_var,
-    width=3,
-    font='Calibre 11')
-content_id_entry.place(relx=0.45, rely=0.93)
-
-show_content_by_id_button = tk.Button(
-    master=databaseFrame,
-    text='SHOW CONTENT BY ID',
-    command=show_content_by_id,
-    bootstyle='warning outline')
-show_content_by_id_button.place(relx=0.562, rely=0.93)
-
-
-'''----------------------LOWER FRAME STARTED------------------'''
-
-
-lowerFrame = tk.Frame(master=main_object, width=1000, height=260)
-lowerFrame.place(x=500, y=540)
-
-
-db_path_blocker = 0
-usable_real_path = ''
-
-
-def set_db_path():
-    global db_path_blocker, usable_real_path
-    path = db_path_var.get().strip()
-    if os.path.isdir(path.strip()):
-        db_path_blocker = 1
-        db_path_result_var.set('SET')
-        usable_real_path = path
-    else:
-        db_path_blocker = 0
-        db_path_result_var.set('NOT SET')
-        usable_real_path = ''
-
-
-main_db_name_blocker = 0
-db_already_exists_blocker = 0
-maindbname = ''
-
-
-def main_db_name():
-    global main_db_name_blocker,\
-        db_already_exists_blocker,\
-        usable_real_path, db_path_blocker,\
-        success_maindb_connection_blocker,\
-        main_db_conn,\
-        maindbname
-
-    dbname = main_db_name_var.get().strip()
-    if re.match(r'((^[\w(-.)?]+\.db$)|(^[\w?(-.)]\.db$))', dbname):
-        try:
-            maindbname = dbname
-            main_db_name_blocker = 1
-            main_db_name_result_var.set('SET')
-            if db_path_blocker == 1:
-                fullpath = usable_real_path
-                conn_path_db = os.path.join(usable_real_path, maindbname)
-                if os.path.isfile(
-                        fullpath +
-                        f'\\{maindbname}') or os.path.isfile(
-                        fullpath +
-                        f'/{maindbname}'):
-                    db_already_exists_blocker = 1
-                    main_db_conn = Ad.Database(conn_path_db)
-                    main_db_conn.addtable()
-                    main_db_name_result_var.set('CONNECTED')
-                    db_display_text.delete('1.0', tk.END)
-                    db_display_text.insert(
-                        tk.END, f'Connected to {maindbname}..\n\n')
-                    success_maindb_connection_blocker = 1
-                    encfiletoolbutt.state(['!disabled'])
-                    decfiletoolbutt.state(['!disabled'])
-                else:
-                    db_already_exists_blocker = 0
-                    main_db_conn = Ad.Database(conn_path_db)
-                    main_db_conn.addtable()
-                    db_display_text.delete('1.0', tk.END)
-                    db_display_text.insert(
-                        tk.END,
-                        f"Created and Connected to '{maindbname}'.. in the directory '{fullpath}'\n\n")
-                    success_maindb_connection_blocker = 1
-                    encfiletoolbutt.state(['!disabled'])
-                    decfiletoolbutt.state(['!disabled'])
-
-            else:
-                db_display_text.delete('1.0', tk.END)
-                db_display_text.insert(
-                    tk.END, f"PATH : '{db_path_var.get().strip()}' is not a valid path\n\n")
-        except BaseException:
-            db_display_text.delete('1.0', tk.END)
-            db_display_text.insert(tk.END, f"The database might be distorted")
-    else:
-        main_db_name_result_var.set('NOT SET')
-        main_db_name_blocker = 0
-
-
-def keyd_db_setup():
-    global usable_real_path,\
-        success_keysdb_connection_blocker,\
-        keys_db_conn
-    print(usable_real_path)
-    if db_path_blocker == 1 and main_db_name_blocker == 1:
-        try:
-            dbname = main_db_name_var.get().strip()
-            keys_db = dbname[:-3] + 'Keys.db'
-            dbname_keys_win = '\\' + keys_db
-            dbname_keys_unix = '/' + keys_db
-            conn_path_keys = os.path.join(usable_real_path, keys_db)
-            if db_already_exists_blocker == 1:
-                if os.path.isfile(
-                        usable_real_path +
-                        dbname_keys_win) or os.path.isfile(
-                        usable_real_path +
-                        dbname_keys_unix):
-                    keys_db_conn = Ad.Database(conn_path_keys)
-                    keys_db_conn.addtable()
-                    db_display_text.insert(
-                        tk.END, f"Connected to '{keys_db}' ..\n\n")
-                    success_keysdb_connection_blocker = 1
-                else:
-                    keys_db_conn = Ad.Database(conn_path_keys)
-                    keys_db_conn.addtable()
-                    db_display_text.insert(
-                        tk.END,
-                        f"'{keys_db}' NOT FOUND ! ==> Created and Connected to '{keys_db}' ..\n\n")
-                    success_keysdb_connection_blocker = 1
-            else:
-                keys_db_conn = Ad.Database(conn_path_keys)
-                keys_db_conn.addtable()
-                db_display_text.insert(
-                    tk.END, f"Created and Connected to '{keys_db}' ..\n\n")
-                success_keysdb_connection_blocker = 1
-        except BaseException:
-            db_display_text.delete('1.0', tk.END)
-            db_display_text.insert(
-                tk.END, f"The database might be distorted\n")
-
-
-success_maindb_connection_blocker = 0
-success_keysdb_connection_blocker = 0
-db_enable_blocker = 0
-
-
-def path_name_wrapper():
-    set_db_path()
-    main_db_name()
-    keyd_db_setup()
-    global db_enable_blocker, success_keysdb_connection_blocker, success_keysdb_connection_blocker
-    if success_keysdb_connection_blocker and success_keysdb_connection_blocker:
-        db_enable_blocker = 1
-        swich_db_toggle.state(['!disabled'])
-    else:
-        db_enable_blocker = 0
-        swich_db_toggle.state(['disabled'])
-
-
-db_path_var = tk.StringVar()
-db_path_entry = tk.Entry(master=lowerFrame,
-                         width=31,
-                         font='Calibre 14 bold',
-                         textvariable=db_path_var)
-db_path_entry.place(relx=0.03, rely=0.005)
-
-db_path_result_var = tk.StringVar(value="")
-db_path_result_entry = tk.Label(
-    master=lowerFrame,
-    font='Calibre 13 bold',
-    bootstyle='light',
-    textvariable=db_path_result_var)
-db_path_result_entry.place(relx=0.7, rely=0.022)
-
-path_label = tk.Label(master=lowerFrame,
-                      font='Calibre 13 bold',
-                      bootstyle='light',
-                      text='DATABASES PATH')
-path_label.place(relx=0.47, rely=0.022)
-
-main_database_label = tk.Label(
-    master=lowerFrame,
-    font='Calibre 13 bold',
-    bootstyle='light',
-    text='MAIN DATABASE')
-main_database_label.place(relx=0.47, rely=0.205)
-
-set_db_path_button = tk.Button(
-    master=lowerFrame,
-    text='SUBMIT PATH AND NAME',
-    width=49,
-    command=path_name_wrapper,
-    bootstyle='info outline')
-set_db_path_button.place(relx=0.031, rely=0.38)
-
-
-def checksize():
-    global db_enable_blocker, main_db_conn, keys_db_conn
-    if db_enable_blocker != 0:
-        if swich_db_var.get() == 1:
-            conn = keys_db_conn
-        else:
-            conn = main_db_conn
-        size = conn.size
-        if size < 1024:
-            db_display_text.delete('1.0', tk.END)
-            db_display_text.insert(
-                tk.END, f"Current size is {size:.5f} (MB)'\n\n")
-        if size >= 1024:
-            db_display_text.delete('1.0', tk.END)
-            db_display_text.insert(
-                tk.END, f"Current size is {(size/1024):.3f} (GB)'\n\n")
-
-
-size_button = tk.Button(
-    master=lowerFrame,
-    text='SIZE',
-    width=22,
-    command=checksize,
-    bootstyle='warning outline')
-size_button.place(relx=0.031, rely=0.58)
-
-
-def checkid():
-    global db_enable_blocker, main_db_conn, keys_db_conn
-    if db_enable_blocker != 0:
-        if swich_db_var.get() == 1:
-            conn = keys_db_conn
-        else:
-            conn = main_db_conn
-        try:
-            q = conn.query('SELECT ID FROM Classified')
-            idd = 0
-            for e in q:
-                for k, v in e.items():
-                    idd += v[-1][-1][0]
-            db_display_text.delete('1.0', tk.END)
-            db_display_text.insert(tk.END, f"Last inserted ID is : '{idd}'\n")
-            return idd
-        except BaseException:
-            db_display_text.delete('1.0', tk.END)
-            db_display_text.insert(tk.END, f"Last inserted ID is : '0'\n")
-            return -1
-
-
-id_button = tk.Button(
-    master=lowerFrame,
-    text='LAST ID',
-    width=22,
-    command=checkid,
-    bootstyle='warning outline')
-id_button.place(relx=0.247, rely=0.58)
-
-
-def check_las_mod():
-    global db_enable_blocker, main_db_conn, keys_db_conn
-    if db_enable_blocker != 0:
-        if swich_db_var.get() == 1:
-            conn = keys_db_conn
-        else:
-            conn = main_db_conn
-        db_display_text.delete('1.0', tk.END)
-        db_display_text.insert(
-            tk.END, f"Last modification at : '{conn.last_mod}'\n")
-
-
-las_mod_button = tk.Button(
-    master=lowerFrame,
-    text='LAST MODIFICATION',
-    width=49,
-    command=check_las_mod,
-    bootstyle='warning outline')
-las_mod_button.place(relx=0.031, rely=0.74)
-
-
-main_db_name_var = tk.StringVar()
-main_db_name_entry = tk.Entry(
-    master=lowerFrame,
-    width=31,
-    font='Calibre 14 bold',
-    textvariable=main_db_name_var)
-main_db_name_entry.place(relx=0.03, rely=0.192)
-
-
-main_db_name_result_var = tk.StringVar(value='')
-main_db_name_result_entry = tk.Label(
-    master=lowerFrame,
-    font='Calibre 13 bold',
-    bootstyle='light',
-    textvariable=main_db_name_result_var)
-main_db_name_result_entry.place(relx=0.7, rely=0.205)
-
-current_working_db = maindbname
-
-
-def swich_db():
-    global current_working_db
-    if db_enable_blocker != 0:
-        if swich_db_var.get() == 1:
-            switch_db_label_var.set('ON KEYS')
-            db_display_text.delete('1.0', tk.END)
-            db_display_text.insert(tk.END, f"Switched to keys database\n")
-            current_working_db = maindbname
-        else:
-            switch_db_label_var.set('ON MAIN')
-            db_display_text.delete('1.0', tk.END)
-            db_display_text.insert(tk.END, f"Back to default main database\n")
-            current_working_db = maindbname[:-3] + 'Keys.db'
-
-
-switch_db_label_var = tk.StringVar(value='SWITCH DATABASE')
-switch_db_label = tk.Label(master=lowerFrame,
-                           textvariable=switch_db_label_var,
-                           bootstyle='light',
-                           font='Calibre 13 bold')
-switch_db_label.place(relx=0.52, rely=0.39)
-
-
-swich_db_var = tk.IntVar(value=0)
-swich_db_toggle = tk.Checkbutton(bootstyle='light,squared-toggle',
-                                 master=lowerFrame,
-                                 variable=swich_db_var,
-                                 offvalue=0,
-                                 onvalue=1,
-                                 command=swich_db)
-swich_db_toggle.state(['disabled'])
-
-
-swich_db_toggle.place(relx=0.47, rely=0.413)
-
-
-'''------------TEXT DECRYPTION/ENCRYPTION STARTED--------------'''
-
-
-def encryption():
-    m = inputfield1_1.get()
-    if Af.CryptFile.keyverify(
-            mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
-        if len(m) > 200:
-            outputvar1.set('Too Long')
-        else:
-            if inputfield1_1.get():
-                progressbar.start()
-                a = At.Crypt(m, mainkeyvar.get())
-                b = a.encrypt()[1]
-                outputvar1.set(b.__str__())
-                if var1.get() == 1:
-                    qr.tqr(b)
-
-
-def decryption():
-    n = inputfield2_1.get()
-    if Af.CryptFile.keyverify(
-            mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
-        if inputfield2_1.get():
-            progressbar2.start()
-            a = At.Crypt(n, mainkeyvar.get())
-            b = a.decrypt()[1]
-            outputvar2.set(b.__str__())
-            if var2.get() == 1:
-                if not len(b) > 200:
-                    qr.tqr(b)
-
-
-def func1():
-    if var1.get() == 1:
-        label1.config(text='QR ON')
-    else:
-        label1.config(text='QR OFF')
-
-
-def func2():
-    if var2.get() == 1:
-        label2.config(text='QR ON')
-    else:
-        label2.config(text='QR OFF')
-
-
-button1 = tk.Button(
-    master=textFrame1,
-    text='ENCRYPT',
-    command=encryption,
-    bootstyle='light outline')
-button1.place(relx=0.42, rely=0.73)
-
-button2 = tk.Button(
-    master=textFrame2,
-    text='DECRYPT',
-    command=decryption,
-    bootstyle='light outline')
-button2.place(relx=0.42, rely=0.8)
-
-inputfield1_1 = tk.StringVar()
-textfield1_1 = tk.Entry(master=textFrame1,
-                        width=20,
-                        font='Calibre 11 bold',
-                        textvariable=inputfield1_1)
-textfield1_1.place(relx=0.29, rely=0.30)
-
-inputfield2_1 = tk.StringVar(value='')
-textfield2_1 = tk.Entry(
-    master=textFrame2,
-    font='Calibre 11 bold',
-    width=20,
-    textvariable=inputfield2_1)
-textfield2_1.place(relx=0.290, rely=0.38)
-
-namelabel1 = tk.Label(master=textFrame1,
-                      text='TEXT ENCRYPTION',
-                      font='Calibre 20 bold',
-                      )
-namelabel1.place(relx=0.190, rely=0.10)
-namelabel2 = tk.Label(master=textFrame2,
-                      text='TEXT DECRYPTION',
-                      font='Calibre 20 bold',
-                      )
-namelabel2.place(relx=0.190, rely=0.200)
-
-outputvar1 = tk.StringVar(value='')
-outputlabel1 = tk.Entry(master=textFrame1,
-                        textvariable=outputvar1,
-                        font='terminal 11 bold')
-outputlabel1.place(relx=0.02, rely=0.48, width=480, height=50)
-
-outputvar2 = tk.StringVar(value='')
-outputlabel2 = tk.Entry(master=textFrame2,
-                        textvariable=outputvar2,
-                        font='terminal 11 bold')
-outputlabel2.place(relx=0.02, rely=0.55, width=480, height=50)
-
-
-label1 = tk.Label(master=textFrame1, text='QR', font=('terminal', 17))
-label1.place(relx=0.2, rely=0.75)
-var1 = tk.IntVar()
-mytoolbutt3 = tk.Checkbutton(bootstyle='success , round-toggle',
-                             master=textFrame1,
-                             variable=var1,
-                             offvalue=0,
-                             command=func1)
-
-mytoolbutt3.place(relx=0.1, rely=0.77)
-
-
-label2 = tk.Label(master=textFrame2, text='QR', font=('terminal', 17))
-label2.place(relx=0.2, rely=0.82)
-var2 = tk.IntVar()
-mytoolbutt6 = tk.Checkbutton(bootstyle='success , round-toggle',
-                             master=textFrame2,
-                             variable=var2,
-                             offvalue=0,
-                             command=func2)
-
-mytoolbutt6.place(relx=0.1, rely=0.84)
-
-
-progressbar = tk.Progressbar(
-    master=textFrame1,
-    mode='indeterminate',
-    style='secondary',
-    length=100,
-)
-progressbar.place(relx=0.05, rely=0.34)
-
-progressbar2 = tk.Progressbar(
-    master=textFrame2,
-    mode='indeterminate',
-    style='secondary',
-    length=100,
-)
-progressbar2.place(relx=0.05, rely=0.42)
-
-
-'''---------FILE ENCRYPTION/DECRYPTION STARTED-------------'''
-
-
-filepathlabel = tk.Label(master=frameFile1,
-                         text='FILE PATH',
-                         font='Calibre 20 bold',
-                         )
-filepathlabel.place(relx=0.335, rely=0.10)
-
-if platform.system() == 'Windows':
-    resultvarfile = tk.StringVar(value='                 ..........')
-    resultLabelfile = tk.Label(master=frameFile1,
-                               textvariable=resultvarfile,
-                               font='terminal 13 bold')
-    resultLabelfile.place(rely=0.55)
-else:
-    resultvarfile = tk.StringVar(value='                    ..........')
-    resultLabelfile = tk.Label(master=frameFile1,
-                               textvariable=resultvarfile,
-                               font='terminal 13 bold')
-    resultLabelfile.place(rely=0.55)
-
-
-def enc_file():
-    global add_enc_to_db, main_db_conn, mainkey
-    if 1:
-        if keySelectionFlag.get() != 0:
-            filename = filenameStringVar.get().strip()
-            key = mainkey
-            target = Af.CryptFile(filename, key)
-            a = target.encrypt()
-            if a == 1:
-                filename = filename + '.crypt'
-                filenameStringVar.set(filename)
-                resultvarfile.set(
-                    '      Encrypted Successfully / added .crypt')
-                if encfiletoolbuttvar.get() == 1:
-                    with open(filename, 'rb') as f:
-                        file_content = f.read()
-                    try:
-                        main_db_conn.insert(
-                            filename, file_content, outputKeyref.get().strip())
-                    except BaseException:
-                        db_display_text.delete('1.0', tk.END)
-                        db_display_text.insert(
-                            tk.END, f"ERROR \n\nDatabase might be distorted\n")
-            if platform.system() == 'Windows':
-                if a == 2:
-                    resultvarfile.set('                 File is Empty')
-                if a == 3:
-                    resultvarfile.set("               File Doesn't Exist")
-                if a == 0:
-                    resultvarfile.set("                  Can't Encrypt")
-                if a == 4:
-                    resultvarfile.set('                     ERROR')
-                if a == 5:
-                    resultvarfile.set('          ERROR : Key is Not 512-bit')
-                if a == 6:
-                    resultvarfile.set(
-                        '       ERROR : File is already encrypted')
-                elif a == 7:
-                    resultvarfile.set(
-                        ' ERROR : Given a directory instead of a file')
-            else:
-                if a == 2:
-                    resultvarfile.set('                   File is Empty')
-                if a == 3:
-                    resultvarfile.set("                 File Doesn't Exist")
-                if a == 0:
-                    resultvarfile.set("                    Can't Encrypt")
-                if a == 4:
-                    resultvarfile.set('                       ERROR')
-                if a == 5:
-                    resultvarfile.set('            ERROR : Key is Not 512-bit')
-                if a == 6:
-                    resultvarfile.set(
-                        '         ERROR : File is already encrypted')
-                elif a == 7:
-                    resultvarfile.set(
-                        '   ERROR : Given a directory instead of a file')
-
-
-def decfile():
-    global add_dec_to_db, main_db_conn, mainkey
-    if 1:
-        if keySelectionFlag.get() != 0:
-            filename = filenameStringVar.get().strip()
-            key = mainkey
-            target = Af.CryptFile(filename, key)
-            a = target.decrypt()
-            if a == 1:
-                filename = os.path.splitext(filename)[0]
-                filenameStringVar.set(filename)
-                resultvarfile.set(
-                    '     Decrypted Successfully + removed .crypt')
-                if decfiletoolbuttvar.get() == 1:
-                    with open(filename, 'rb') as f:
-                        file_content = f.read()
-                    try:
-                        main_db_conn.insert(
-                            filename, file_content, outputKeyref.get().strip())
-                    except BaseException:
-                        db_display_text.delete('1.0', tk.END)
-                        db_display_text.insert(
-                            tk.END, f"ERROR \n\nDatabase might be distorted\n")
-            if platform.system() == 'Windows':
-                if a == 2:
-                    resultvarfile.set('                 File is Empty')
-                if a == 3:
-                    resultvarfile.set("               File Doesn't Exist")
-                if a == 0:
-                    resultvarfile.set("                 Can't Decrypt")
-                if a == 4:
-                    resultvarfile.set('                     ERROR')
-                elif a == 5:
-                    resultvarfile.set('          ERROR : Key is Not 512-bit')
-                if a == 6:
-                    resultvarfile.set(
-                        '       ERROR : File is already decrypted')
-                elif a == 7:
-                    resultvarfile.set(
-                        ' ERROR : Given a directory instead of a file')
-            else:
-                if a == 2:
-                    resultvarfile.set('                   File is Empty')
-                if a == 3:
-                    resultvarfile.set("                 File Doesn't Exist")
-                if a == 0:
-                    resultvarfile.set("                   Can't Decrypt")
-                if a == 4:
-                    resultvarfile.set('                       ERROR')
-                elif a == 5:
-                    resultvarfile.set('            ERROR : Key is Not 512-bit')
-                if a == 6:
-                    resultvarfile.set(
-                        '         ERROR : File is already decrypted')
-                elif a == 7:
-                    resultvarfile.set(
-                        '   ERROR : Given a directory instead of a file')
-
-
-encryptionfilebutton = tk.Button(
-    master=frameFile1,
-    text='ENCRYPT FILE',
-    command=enc_file,
-    bootstyle='warning outline')
-encryptionfilebutton.place(relx=0.25, rely=0.73)
-
-decryptionfilebutton = tk.Button(
-    master=frameFile1,
-    text='DECRYPT FILE',
-    command=decfile,
-    bootstyle='warning outline')
-decryptionfilebutton.place(relx=0.55, rely=0.73)
-
-filenameStringVar = tk.StringVar(value='')
-
-filenametext = tk.Entry(
-    master=frameFile1,
-    width=31,
-    font='Calibre 15 bold',
-    textvariable=filenameStringVar)
-filenametext.place(relx=0.05, rely=0.30)
-
-
-addtodbLabel = tk.Label(
-    master=frameFile1,
-    text='ADD TO DATABASE',
-    font=(
-        'Calibre',
-        11),
-    bootstyle='warning')
-addtodbLabel.place(relx=0.35, rely=0.908)
-
-add_enc_to_db = 0
-
-
-def enc_toggle_func():
-    global add_enc_to_db
-    if encfiletoolbuttvar == 1:
-        add_enc_to_db = 1
-    else:
-        add_enc_to_db = 0
-
-
-add_dec_to_db = 0
-
-
-def dec_toggle_func():
-    global add_dec_to_db
-    if decfiletoolbuttvar == 1:
-        add_dec_to_db = 1
-    else:
-        add_dec_to_db = 0
-
-
-encfiletoolbuttvar = tk.IntVar()
-encfiletoolbutt = tk.Checkbutton(bootstyle='warning , round-toggle',
-                                 master=frameFile1,
-                                 variable=encfiletoolbuttvar,
-                                 offvalue=0,
-                                 onvalue=1,
-                                 command=enc_toggle_func)
-encfiletoolbutt.state(['disabled'])
-encfiletoolbutt.place(relx=0.25, rely=0.92)
-
-
-decfiletoolbuttvar = tk.IntVar()
-decfiletoolbutt = tk.Checkbutton(bootstyle='warning , round-toggle',
-                                 master=frameFile1,
-                                 variable=decfiletoolbuttvar,
-                                 offvalue=0,
-                                 command=dec_toggle_func)
-decfiletoolbutt.state(['disabled'])
-decfiletoolbutt.place(relx=0.717, rely=0.92)
-
-
-keySelectionFlag = tk.IntVar(value=0)
-
-
-def main_key_wrapper():
-    global success_keysdb_connection_blocker, mainkey
-    if Af.CryptFile.keyverify(mainkeyvar.get().strip()) == 1:
-        mainkey = mainkeyvar.get().strip()
-        keyref_gen()
-        keyselectionvar.set('       SELECTED')
-        keySelectionFlag.set(1)
-        try:
-            if success_keysdb_connection_blocker and os.path.isfile(
-                    filenameStringVar.get().strip()):
-                keys_db_conn.insert(
-                    filenameStringVar.get().strip(),
-                    mainkey,
-                    outputKeyref.get())
-            if success_keysdb_connection_blocker and not os.path.isfile(
-                    filenameStringVar.get().strip()):
-                keys_db_conn.insert('STANDALONE', mainkey, outputKeyref.get())
-        except BaseException:
-            db_display_text.delete('1.0', tk.END)
-            db_display_text.insert(tk.END, f"Faulty Database\n")
-    else:
-        keySelectionFlag.set(0)
-        keyselectionvar.set('     NOT SELECTED')
-
-
-mainkeyLabel = tk.Label(master=frameFile2,
-                        text='MAIN KEY',
-                        font='Calibre 20 bold',
-                        bootstyle='info',
-                        )
-mainkeyLabel.place(relx=0.3, rely=0.075)
-
-
-mainkeyvar = tk.StringVar()
-mainkeyEntry = tk.Entry(master=frameFile2,
-                        font='Calibre 14 bold',
-                        textvariable=mainkeyvar,
-                        width=29
-                        )
-mainkeyEntry.place(relx=0.09, rely=0.29)
-
-
-def keyref_gen():
-    ref = '#'
-    for _ in range(6):
-        character = secrets.choice(
-            string.ascii_letters +
-            string.digits +
-            '$' +
-            '?' +
-            '&' +
-            '@' +
-            '!' +
-            '-' +
-            '+')
-        ref += character
-    outputKeyref.set(ref)
-
-
-outputKeyref = tk.StringVar(value='#XXXXXX')
-keyrefLabel = tk.Label(
-    master=frameFile2,
-    textvariable=outputKeyref,
-    bootstyle='secondary',
-    font=(
-        'terminal',
-        12))
-keyrefLabel.place(relx=0.712, rely=0.12)
-
-keySelectButton = tk.Button(
-    master=frameFile2,
-    text='SELECT KEY',
-    command=main_key_wrapper,
-    bootstyle='info outline')
-keySelectButton.place(relx=0.6725, rely=0.5)
-
-
-keyselectionvar = tk.StringVar(value='   KEY NOT SELECTED')
-keyselectionLabel = tk.Label(master=frameFile2,
-                             textvariable=keyselectionvar,
-                             bootstyle='info',
-                             font='terminal 11 bold')
-keyselectionLabel.place(relx=0.15, rely=0.465, height=50)
-
-
-def genkey():
-    keyGenVar.set(Af.CryptFile.genkey())
-
-
-keyGenVar = tk.StringVar(value='')
-keyGenEntry = tk.Entry(master=frameFile2,
-                       font='Calibre 12 bold',
-                       textvariable=keyGenVar,
-                       width=23)
-keyGenEntry.place(relx=0.1, rely=0.69)
-
-keyButton = tk.Button(master=frameFile2,
-                      text='GENERATE',
-                      command=genkey,
-                      bootstyle='success outline')
-keyButton.place(relx=0.671, rely=0.7)
-
-
-'''----------------------------STAMP STARTED ------------------------------'''
-
-
-latest_ID_key_label = tk.Label(
-    master=lowerFrame,
-    text='GitHub.com/AshGw/AES-256',
-    font='Calibre 6')
-latest_ID_key_label.place(relx=0.84, rely=0.92)
-
-'''------------------------------STAMP ENDED------------------------------'''
-
-
-def rm_json():
-    global usable_real_path
-    file = os.path.join(usable_real_path, 'output.json')
-    if os.path.exists(file):
-        os.remove(file)
-
-
-
-atexit.register(rm_json)
-
-
-if __name__ == '__main__':
-    main_object.mainloop()
+import AshCrypt.textcrypt as At
+import AshCrypt.filecrypt as Af
+import AshCrypt.database as Ad
+import ttkbootstrap as tk
+import AshCrypt.qr as qr
+import platform
+import secrets
+import os.path
+import string
+import atexit
+import json
+import re
+
+
+'''------------------------FRAMING STARTED-------------------'''
+
+main_object = tk.Window(themename='vapor')
+main_object.resizable(False, False)
+main_object.title('AshCrypt')
+main_object.geometry('1500x800')
+
+
+databaseFrame = tk.Frame(master=main_object, width=500, height=800)
+databaseFrame.place(x=0, y=0)
+
+frameFile1 = tk.Frame(master=main_object, width=500, height=250)
+frameFile1.place(x=500, y=0)
+
+frameFile2 = tk.Frame(master=main_object, width=500, height=250)
+frameFile2.place(x=500, y=250)
+
+textFrame1 = tk.Frame(master=main_object, width=500, height=250)
+textFrame1.place(x=1000, y=0)
+
+textFrame2 = tk.Frame(master=main_object, width=500, height=250)
+textFrame2.place(x=1000, y=250)
+
+lowerFrame = tk.Frame(master=main_object, width=1000, height=260)
+lowerFrame.place(x=500, y=540)
+
+'''---------------DATABASE FRAME STARTED-----------------------'''
+
+
+databaseFrame = tk.Frame(master=main_object, height=800, width=500)
+databaseFrame.place(rely=0, relx=0)
+
+if platform.system() == 'Windows':
+    console_label = tk.Label(
+        master=databaseFrame,
+        text='DATABASE OUTPUT CONSOLE',
+        font='Terminal 15 bold')
+    console_label.place(relx=0.09, rely=0.04)
+
+    db_display_text = tk.ScrolledText(
+        width=43,
+        height=27,
+        font='terminal 13',
+        wrap='word')
+    db_display_text.place(relx=0.016, rely=0.105)
+    db_display_text.insert(tk.END, 'Waiting to fetch..')
+else:
+    console_label = tk.Label(
+        master=databaseFrame,
+        text='DATABASE OUTPUT CONSOLE',
+        font='Calibre 15 bold')
+    console_label.place(relx=0.115, rely=0.04)
+
+    db_display_text = tk.Text(
+        width=38,
+        height=22,
+        font='Calibre 13 bold',
+        wrap='word')
+    db_display_text.place(relx=0.015, rely=0.105)
+    db_display_text.insert(tk.END, 'Waiting to fetch..')
+
+
+def show_all_content():
+    global db_enable_blocker, main_db_name_var, usable_real_path, main_db_conn, db_display_text, keys_db_conn
+    if db_enable_blocker != 0:
+        db_display_text.delete('1.0', tk.END)
+        db_display_text.insert(
+            tk.END, f"Check 'output.json' in the chosen path : {usable_real_path}\n")
+        json_path = os.path.join(usable_real_path, 'output.json')
+        if swich_db_var.get() == 1:
+            conn = keys_db_conn
+        else:
+            conn = main_db_conn
+        try:
+            with open(json_path, 'w') as f:
+                buffer = {}
+                for e in conn.content():
+                    buffer['ID ' + e[0].__str__()] = [{'Filename': e[1]}, {
+                        'Content': e[2].__str__()}, {'KeyRef': e[3]}]
+                json_content = json.dumps(buffer, indent=2)
+                f.write(json_content)
+                db_display_text.insert(
+                    tk.END, f"\nSuccessfully written all table content in output.json\n"
+                    f"\nNote that this file will be deleted when the app is closed")
+        except BaseException:
+            db_display_text.insert(
+                tk.END, f"Failed to write all table content in output.json\n")
+
+
+def show_content_by_id():
+    global db_enable_blocker, main_db_conn, keys_db_conn, content_id_entry_var, usable_real_path
+    idd = content_id_entry_var.get().strip()
+    last_id = checkid()
+    if db_enable_blocker != 0:
+        if swich_db_var.get() == 1:
+            conn = keys_db_conn
+        else:
+            conn = main_db_conn
+        try:
+            if int(idd) > 0:
+                if last_id == -1:
+                    db_display_text.delete('1.0', tk.END)
+                    db_display_text.insert(
+                        tk.END, 'The table does not have any content to show')
+                elif last_id != -1:
+
+                    if int(idd) in range(1, last_id):
+                        db_display_text.delete('1.0', tk.END)
+                        to_json_path = os.path.join(
+                            usable_real_path, 'output.json')
+                        with open(to_json_path, 'w') as f:
+                            buffer = {}
+                            for e in conn.content_by_id(int(idd)):
+                                buffer['ID_' + e[0].__str__()] = [{'Filename': e[1]}, {
+                                    'Content': e[2].__str__()}, {'KeyRef': e[3]}]
+                            json_content = json.dumps(buffer, indent=2)
+                            f.write(json_content)
+                        db_display_text.insert(
+                            tk.END, f"Successful fetch !\n\nCheck the 'output.json' file in the"
+                            f" chosen path :\n\n'{usable_real_path}'")
+                    if int(idd) == last_id:
+                        db_display_text.delete('1.0', tk.END)
+                        db_display_text.insert(tk.END, 'Chosen last ID\n\n')
+                        to_json_path = os.path.join(
+                            usable_real_path, 'output.json')
+                        try:
+                            with open(to_json_path, 'w') as f:
+                                buffer = {}
+                                for e in conn.content_by_id(int(idd)):
+                                    buffer['ID_' + e[0].__str__()] = [{'Filename': e[1]}, {
+                                        'Content': e[2].__str__()}, {'KeyRef': e[3]}]
+                                json_content = json.dumps(buffer, indent=2)
+                                f.write(json_content)
+                            db_display_text.insert(
+                                tk.END, f"Successful fetch !\n\nCheck the 'output.json' file in the"
+                                f" the chosen path :\n\n'{usable_real_path}'")
+                        except BaseException:
+                            db_display_text.delete('1.0', tk.END)
+                            db_display_text.insert(
+                                tk.END, "ERROR \n\nCheck the validity of 'output.json' file"
+                                "\n\nCheck if the database is faulty\n")
+                    elif int(idd) > last_id:
+                        db_display_text.delete('1.0', tk.END)
+                        db_display_text.insert(
+                            tk.END, 'Given ID is greater than the highest available ID')
+            else:
+                db_display_text.delete('1.0', tk.END)
+                db_display_text.insert(
+                    tk.END, 'ID must be strictly greater than 0')
+        except BaseException:
+            db_display_text.delete('1.0', tk.END)
+            db_display_text.insert(tk.END, 'ID value must be a valid integer')
+
+
+def drop_content_by_id():
+    global db_enable_blocker, main_db_conn, keys_db_conn, content_id_entry_var
+    idd = content_id_entry_var.get().strip()
+    last_id = checkid()
+    if db_enable_blocker != 0:
+        if swich_db_var.get() == 1:
+            conn = keys_db_conn
+        else:
+            conn = main_db_conn
+        try:
+            if int(idd) > 0:
+                if last_id == -1:
+                    db_display_text.delete('1.0', tk.END)
+                    db_display_text.insert(
+                        tk.END, 'The table does not have any content to drop')
+                elif last_id != -1:
+
+                    if int(idd) in range(1, last_id):
+                        db_display_text.delete('1.0', tk.END)
+                        db_display_text.insert(tk.END, 'Valid ID')
+                        conn.drop_content(idd)
+                        db_display_text.insert(
+                            tk.END, f'\nDropping by ID {idd} Went successful')
+
+                    if int(idd) == last_id:
+                        db_display_text.delete('1.0', tk.END)
+                        db_display_text.insert(tk.END, 'Chosen last ID')
+                        conn.drop_content(idd)
+                        db_display_text.insert(
+                            tk.END, f'\nDropping by ID {idd} Went successful')
+
+                    elif int(idd) > last_id:
+                        db_display_text.delete('1.0', tk.END)
+                        db_display_text.insert(
+                            tk.END, 'Given ID is greater than the highest available ID')
+            else:
+                db_display_text.delete('1.0', tk.END)
+                db_display_text.insert(
+                    tk.END, 'ID must be strictly greater than 0')
+        except BaseException:
+            db_display_text.delete('1.0', tk.END)
+            db_display_text.insert(tk.END, 'ID value must be a valid integer')
+
+
+show_all_content_button = tk.Button(
+    master=databaseFrame,
+    text='SHOW ALL TABLE CONTENT',
+    command=show_all_content,
+    bootstyle='warning outline')
+show_all_content_button.place(relx=0.287, rely=0.87)
+
+
+query_clicks = 1
+
+
+def query():
+    global db_enable_blocker, main_db_conn, keys_db_conn, usable_real_path, query_clicks
+    if db_enable_blocker != 0:
+        if swich_db_var.get() == 1:
+            conn = keys_db_conn
+        else:
+            conn = main_db_conn
+        query_var = query_entry_var.get().strip()
+        if len(query_var) > 0:
+            try:
+                db_display_text.delete('1.0', tk.END)
+                json_file = os.path.join(usable_real_path, 'output.json')
+                with open(json_file, 'w') as f:
+                    query_out = conn.query(query_var)
+                    conn.addtable()
+                    json_content = json.dumps(
+                        {f'query {query_clicks}': query_out}, indent=2)
+                    query_clicks += 1
+                    f.write(json_content)
+                db_display_text.insert(
+                    tk.END, f"Ran query {query_clicks} !\n\n")
+                db_display_text.insert(
+                    tk.END, f"The result of the query is in 'output.json' file\n\n")
+            except BaseException:
+                db_display_text.delete('1.0', tk.END)
+                db_display_text.insert(
+                    tk.END, f"Failed to finish the query!\n\n")
+                db_display_text.insert(
+                    tk.END, 'Detected object that is not JSON serializable\n\n')
+                db_display_text.insert(
+                    tk.END, 'Use buttons instead if possible')
+        else:
+            db_display_text.delete('1.0', tk.END)
+            db_display_text.insert(tk.END, f"Can't query nothing\n\n")
+
+
+query_entry_var = tk.StringVar()
+query_entry = tk.Entry(
+    master=databaseFrame,
+    width=38,
+    font='Calibre 13 bold',
+    textvariable=query_entry_var)
+
+query_entry.place(relx=0.043, rely=0.742)
+
+query_button = tk.Button(
+    master=databaseFrame,
+    text='RUN QUERY',
+    command=query,
+    bootstyle='warning outline')
+query_button.place(relx=0.39, rely=0.81)
+
+
+drop_content_by_id_button = tk.Button(
+    master=databaseFrame,
+    text='DROP CONTENT BY ID',
+    command=drop_content_by_id,
+    bootstyle='warning outline')
+drop_content_by_id_button.place(relx=0.08, rely=0.93)
+
+content_id_entry_var = tk.StringVar(value=' ID')
+content_id_entry = tk.Entry(
+    master=databaseFrame,
+    textvariable=content_id_entry_var,
+    width=3,
+    font='Calibre 11')
+content_id_entry.place(relx=0.45, rely=0.93)
+
+show_content_by_id_button = tk.Button(
+    master=databaseFrame,
+    text='SHOW CONTENT BY ID',
+    command=show_content_by_id,
+    bootstyle='warning outline')
+show_content_by_id_button.place(relx=0.562, rely=0.93)
+
+
+'''----------------------LOWER FRAME STARTED------------------'''
+
+
+lowerFrame = tk.Frame(master=main_object, width=1000, height=260)
+lowerFrame.place(x=500, y=540)
+
+
+db_path_blocker = 0
+usable_real_path = ''
+
+
+def set_db_path():
+    global db_path_blocker, usable_real_path
+    path = db_path_var.get().strip()
+    if os.path.isdir(path.strip()):
+        db_path_blocker = 1
+        db_path_result_var.set('SET')
+        usable_real_path = path
+    else:
+        db_path_blocker = 0
+        db_path_result_var.set('NOT SET')
+        usable_real_path = ''
+
+
+main_db_name_blocker = 0
+db_already_exists_blocker = 0
+maindbname = ''
+
+
+def main_db_name():
+    global main_db_name_blocker,\
+        db_already_exists_blocker,\
+        usable_real_path, db_path_blocker,\
+        success_maindb_connection_blocker,\
+        main_db_conn,\
+        maindbname
+
+    dbname = main_db_name_var.get().strip()
+    if re.match(r'((^[\w(-.)?]+\.db$)|(^[\w?(-.)]\.db$))', dbname):
+        try:
+            maindbname = dbname
+            main_db_name_blocker = 1
+            main_db_name_result_var.set('SET')
+            if db_path_blocker == 1:
+                fullpath = usable_real_path
+                conn_path_db = os.path.join(usable_real_path, maindbname)
+                if os.path.isfile(
+                        fullpath +
+                        f'\\{maindbname}') or os.path.isfile(
+                        fullpath +
+                        f'/{maindbname}'):
+                    db_already_exists_blocker = 1
+                    main_db_conn = Ad.Database(conn_path_db)
+                    main_db_conn.addtable()
+                    main_db_name_result_var.set('CONNECTED')
+                    db_display_text.delete('1.0', tk.END)
+                    db_display_text.insert(
+                        tk.END, f'Connected to {maindbname}..\n\n')
+                    success_maindb_connection_blocker = 1
+                    encfiletoolbutt.state(['!disabled'])
+                    decfiletoolbutt.state(['!disabled'])
+                else:
+                    db_already_exists_blocker = 0
+                    main_db_conn = Ad.Database(conn_path_db)
+                    main_db_conn.addtable()
+                    db_display_text.delete('1.0', tk.END)
+                    db_display_text.insert(
+                        tk.END,
+                        f"Created and Connected to '{maindbname}'.. in the directory '{fullpath}'\n\n")
+                    success_maindb_connection_blocker = 1
+                    encfiletoolbutt.state(['!disabled'])
+                    decfiletoolbutt.state(['!disabled'])
+
+            else:
+                db_display_text.delete('1.0', tk.END)
+                db_display_text.insert(
+                    tk.END, f"PATH : '{db_path_var.get().strip()}' is not a valid path\n\n")
+        except BaseException:
+            db_display_text.delete('1.0', tk.END)
+            db_display_text.insert(tk.END, f"The database might be distorted")
+    else:
+        main_db_name_result_var.set('NOT SET')
+        main_db_name_blocker = 0
+
+
+def keyd_db_setup():
+    global usable_real_path,\
+        success_keysdb_connection_blocker,\
+        keys_db_conn
+    print(usable_real_path)
+    if db_path_blocker == 1 and main_db_name_blocker == 1:
+        try:
+            dbname = main_db_name_var.get().strip()
+            keys_db = dbname[:-3] + 'Keys.db'
+            dbname_keys_win = '\\' + keys_db
+            dbname_keys_unix = '/' + keys_db
+            conn_path_keys = os.path.join(usable_real_path, keys_db)
+            if db_already_exists_blocker == 1:
+                if os.path.isfile(
+                        usable_real_path +
+                        dbname_keys_win) or os.path.isfile(
+                        usable_real_path +
+                        dbname_keys_unix):
+                    keys_db_conn = Ad.Database(conn_path_keys)
+                    keys_db_conn.addtable()
+                    db_display_text.insert(
+                        tk.END, f"Connected to '{keys_db}' ..\n\n")
+                    success_keysdb_connection_blocker = 1
+                else:
+                    keys_db_conn = Ad.Database(conn_path_keys)
+                    keys_db_conn.addtable()
+                    db_display_text.insert(
+                        tk.END,
+                        f"'{keys_db}' NOT FOUND ! ==> Created and Connected to '{keys_db}' ..\n\n")
+                    success_keysdb_connection_blocker = 1
+            else:
+                keys_db_conn = Ad.Database(conn_path_keys)
+                keys_db_conn.addtable()
+                db_display_text.insert(
+                    tk.END, f"Created and Connected to '{keys_db}' ..\n\n")
+                success_keysdb_connection_blocker = 1
+        except BaseException:
+            db_display_text.delete('1.0', tk.END)
+            db_display_text.insert(
+                tk.END, f"The database might be distorted\n")
+
+
+success_maindb_connection_blocker = 0
+success_keysdb_connection_blocker = 0
+db_enable_blocker = 0
+
+
+def path_name_wrapper():
+    set_db_path()
+    main_db_name()
+    keyd_db_setup()
+    global db_enable_blocker, success_keysdb_connection_blocker, success_keysdb_connection_blocker
+    if success_keysdb_connection_blocker and success_keysdb_connection_blocker:
+        db_enable_blocker = 1
+        swich_db_toggle.state(['!disabled'])
+    else:
+        db_enable_blocker = 0
+        swich_db_toggle.state(['disabled'])
+
+
+db_path_var = tk.StringVar()
+db_path_entry = tk.Entry(master=lowerFrame,
+                         width=31,
+                         font='Calibre 14 bold',
+                         textvariable=db_path_var)
+db_path_entry.place(relx=0.03, rely=0.005)
+
+db_path_result_var = tk.StringVar(value="")
+db_path_result_entry = tk.Label(
+    master=lowerFrame,
+    font='Calibre 13 bold',
+    bootstyle='light',
+    textvariable=db_path_result_var)
+db_path_result_entry.place(relx=0.7, rely=0.022)
+
+path_label = tk.Label(master=lowerFrame,
+                      font='Calibre 13 bold',
+                      bootstyle='light',
+                      text='DATABASES PATH')
+path_label.place(relx=0.47, rely=0.022)
+
+main_database_label = tk.Label(
+    master=lowerFrame,
+    font='Calibre 13 bold',
+    bootstyle='light',
+    text='MAIN DATABASE')
+main_database_label.place(relx=0.47, rely=0.205)
+
+set_db_path_button = tk.Button(
+    master=lowerFrame,
+    text='SUBMIT PATH AND NAME',
+    width=49,
+    command=path_name_wrapper,
+    bootstyle='info outline')
+set_db_path_button.place(relx=0.031, rely=0.38)
+
+
+def checksize():
+    global db_enable_blocker, main_db_conn, keys_db_conn
+    if db_enable_blocker != 0:
+        if swich_db_var.get() == 1:
+            conn = keys_db_conn
+        else:
+            conn = main_db_conn
+        size = conn.size
+        if size < 1024:
+            db_display_text.delete('1.0', tk.END)
+            db_display_text.insert(
+                tk.END, f"Current size is {size:.5f} (MB)'\n\n")
+        if size >= 1024:
+            db_display_text.delete('1.0', tk.END)
+            db_display_text.insert(
+                tk.END, f"Current size is {(size/1024):.3f} (GB)'\n\n")
+
+
+size_button = tk.Button(
+    master=lowerFrame,
+    text='SIZE',
+    width=22,
+    command=checksize,
+    bootstyle='warning outline')
+size_button.place(relx=0.031, rely=0.58)
+
+
+def checkid():
+    global db_enable_blocker, main_db_conn, keys_db_conn
+    if db_enable_blocker != 0:
+        if swich_db_var.get() == 1:
+            conn = keys_db_conn
+        else:
+            conn = main_db_conn
+        try:
+            q = conn.query('SELECT ID FROM Classified')
+            idd = 0
+            for e in q:
+                for k, v in e.items():
+                    idd += v[-1][-1][0]
+            db_display_text.delete('1.0', tk.END)
+            db_display_text.insert(tk.END, f"Last inserted ID is : '{idd}'\n")
+            return idd
+        except BaseException:
+            db_display_text.delete('1.0', tk.END)
+            db_display_text.insert(tk.END, f"Last inserted ID is : '0'\n")
+            return -1
+
+
+id_button = tk.Button(
+    master=lowerFrame,
+    text='LAST ID',
+    width=22,
+    command=checkid,
+    bootstyle='warning outline')
+id_button.place(relx=0.247, rely=0.58)
+
+
+def check_las_mod():
+    global db_enable_blocker, main_db_conn, keys_db_conn
+    if db_enable_blocker != 0:
+        if swich_db_var.get() == 1:
+            conn = keys_db_conn
+        else:
+            conn = main_db_conn
+        db_display_text.delete('1.0', tk.END)
+        db_display_text.insert(
+            tk.END, f"Last modification at : '{conn.last_mod}'\n")
+
+
+las_mod_button = tk.Button(
+    master=lowerFrame,
+    text='LAST MODIFICATION',
+    width=49,
+    command=check_las_mod,
+    bootstyle='warning outline')
+las_mod_button.place(relx=0.031, rely=0.74)
+
+
+main_db_name_var = tk.StringVar()
+main_db_name_entry = tk.Entry(
+    master=lowerFrame,
+    width=31,
+    font='Calibre 14 bold',
+    textvariable=main_db_name_var)
+main_db_name_entry.place(relx=0.03, rely=0.192)
+
+
+main_db_name_result_var = tk.StringVar(value='')
+main_db_name_result_entry = tk.Label(
+    master=lowerFrame,
+    font='Calibre 13 bold',
+    bootstyle='light',
+    textvariable=main_db_name_result_var)
+main_db_name_result_entry.place(relx=0.7, rely=0.205)
+
+current_working_db = maindbname
+
+
+def swich_db():
+    global current_working_db
+    if db_enable_blocker != 0:
+        if swich_db_var.get() == 1:
+            switch_db_label_var.set('ON KEYS')
+            db_display_text.delete('1.0', tk.END)
+            db_display_text.insert(tk.END, f"Switched to keys database\n")
+            current_working_db = maindbname
+        else:
+            switch_db_label_var.set('ON MAIN')
+            db_display_text.delete('1.0', tk.END)
+            db_display_text.insert(tk.END, f"Back to default main database\n")
+            current_working_db = maindbname[:-3] + 'Keys.db'
+
+
+switch_db_label_var = tk.StringVar(value='SWITCH DATABASE')
+switch_db_label = tk.Label(master=lowerFrame,
+                           textvariable=switch_db_label_var,
+                           bootstyle='light',
+                           font='Calibre 13 bold')
+switch_db_label.place(relx=0.52, rely=0.39)
+
+
+swich_db_var = tk.IntVar(value=0)
+swich_db_toggle = tk.Checkbutton(bootstyle='light,squared-toggle',
+                                 master=lowerFrame,
+                                 variable=swich_db_var,
+                                 offvalue=0,
+                                 onvalue=1,
+                                 command=swich_db)
+swich_db_toggle.state(['disabled'])
+
+
+swich_db_toggle.place(relx=0.47, rely=0.413)
+
+
+'''------------TEXT DECRYPTION/ENCRYPTION STARTED--------------'''
+
+
+def encryption():
+    m = inputfield1_1.get()
+    if Af.CryptFile.keyverify(
+            mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
+        if len(m) > 200:
+            outputvar1.set('Too Long')
+        else:
+            if inputfield1_1.get():
+                progressbar.start()
+                a = At.Crypt(m, mainkeyvar.get())
+                b = a.encrypt()[1]
+                outputvar1.set(b.__str__())
+                if var1.get() == 1:
+                    qr.tqr(b)
+
+
+def decryption():
+    n = inputfield2_1.get()
+    if Af.CryptFile.keyverify(
+            mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
+        if inputfield2_1.get():
+            progressbar2.start()
+            a = At.Crypt(n, mainkeyvar.get())
+            b = a.decrypt()[1]
+            outputvar2.set(b.__str__())
+            if var2.get() == 1:
+                if not len(b) > 200:
+                    qr.tqr(b)
+
+
+def func1():
+    if var1.get() == 1:
+        label1.config(text='QR ON')
+    else:
+        label1.config(text='QR OFF')
+
+
+def func2():
+    if var2.get() == 1:
+        label2.config(text='QR ON')
+    else:
+        label2.config(text='QR OFF')
+
+
+button1 = tk.Button(
+    master=textFrame1,
+    text='ENCRYPT',
+    command=encryption,
+    bootstyle='light outline')
+button1.place(relx=0.42, rely=0.73)
+
+button2 = tk.Button(
+    master=textFrame2,
+    text='DECRYPT',
+    command=decryption,
+    bootstyle='light outline')
+button2.place(relx=0.42, rely=0.8)
+
+inputfield1_1 = tk.StringVar()
+textfield1_1 = tk.Entry(master=textFrame1,
+                        width=20,
+                        font='Calibre 11 bold',
+                        textvariable=inputfield1_1)
+textfield1_1.place(relx=0.29, rely=0.30)
+
+inputfield2_1 = tk.StringVar(value='')
+textfield2_1 = tk.Entry(
+    master=textFrame2,
+    font='Calibre 11 bold',
+    width=20,
+    textvariable=inputfield2_1)
+textfield2_1.place(relx=0.290, rely=0.38)
+if platform.system() == 'Windows':
+    namelabel1 = tk.Label(master=textFrame1,
+                          text='TEXT ENCRYPTION',
+                          font='Calibre 20',
+                          )
+    namelabel1.place(relx=0.190, rely=0.10)
+    namelabel2 = tk.Label(master=textFrame2,
+                          text='TEXT DECRYPTION',
+                          font='Calibre 20',
+                          )
+    namelabel2.place(relx=0.190, rely=0.200)
+else:
+    namelabel1 = tk.Label(master=textFrame1,
+                          text='TEXT ENCRYPTION',
+                          font='Calibre 20 bold',
+                          )
+    namelabel1.place(relx=0.190, rely=0.10)
+    namelabel2 = tk.Label(master=textFrame2,
+                          text='TEXT DECRYPTION',
+                          font='Calibre 20 bold',
+                          )
+    namelabel2.place(relx=0.190, rely=0.200)
+
+
+outputvar1 = tk.StringVar(value='')
+outputlabel1 = tk.Entry(master=textFrame1,
+                        textvariable=outputvar1,
+                        font='terminal 11 bold')
+outputlabel1.place(relx=0.02, rely=0.48, width=480, height=50)
+
+outputvar2 = tk.StringVar(value='')
+outputlabel2 = tk.Entry(master=textFrame2,
+                        textvariable=outputvar2,
+                        font='terminal 11 bold')
+outputlabel2.place(relx=0.02, rely=0.55, width=480, height=50)
+
+
+label1 = tk.Label(master=textFrame1, text='QR', font=('terminal', 17))
+label1.place(relx=0.2, rely=0.75)
+var1 = tk.IntVar()
+mytoolbutt3 = tk.Checkbutton(bootstyle='success , round-toggle',
+                             master=textFrame1,
+                             variable=var1,
+                             offvalue=0,
+                             command=func1)
+
+mytoolbutt3.place(relx=0.1, rely=0.77)
+
+
+label2 = tk.Label(master=textFrame2, text='QR', font=('terminal', 17))
+label2.place(relx=0.2, rely=0.82)
+var2 = tk.IntVar()
+mytoolbutt6 = tk.Checkbutton(bootstyle='success , round-toggle',
+                             master=textFrame2,
+                             variable=var2,
+                             offvalue=0,
+                             command=func2)
+
+mytoolbutt6.place(relx=0.1, rely=0.84)
+
+
+progressbar = tk.Progressbar(
+    master=textFrame1,
+    mode='indeterminate',
+    style='secondary',
+    length=100,
+)
+progressbar.place(relx=0.05, rely=0.34)
+
+progressbar2 = tk.Progressbar(
+    master=textFrame2,
+    mode='indeterminate',
+    style='secondary',
+    length=100,
+)
+progressbar2.place(relx=0.05, rely=0.42)
+
+
+'''---------FILE ENCRYPTION/DECRYPTION STARTED-------------'''
+
+
+
+if platform.system() == 'Windows':
+    filepathlabel = tk.Label(master=frameFile1,
+                             text='FILE PATH',
+                             font='Calibre 20',
+                             )
+    filepathlabel.place(relx=0.335, rely=0.10)
+
+    resultvarfile = tk.StringVar(value='                 .............')
+    resultLabelfile = tk.Label(master=frameFile1,
+                               textvariable=resultvarfile,
+                               font='terminal 13 bold')
+    resultLabelfile.place(rely=0.55)
+else:
+    filepathlabel = tk.Label(master=frameFile1,
+                             text='FILE PATH',
+                             font='Calibre 20 bold',
+                             )
+    filepathlabel.place(relx=0.335, rely=0.10)
+    resultvarfile = tk.StringVar(value='                    ..........')
+    resultLabelfile = tk.Label(master=frameFile1,
+                               textvariable=resultvarfile,
+                               font='terminal 13 bold')
+    resultLabelfile.place(rely=0.55)
+
+
+def enc_file():
+    global add_enc_to_db, main_db_conn, mainkey
+    if 1:
+        if keySelectionFlag.get() != 0:
+            filename = filenameStringVar.get().strip()
+            key = mainkey
+            target = Af.CryptFile(filename, key)
+            a = target.encrypt()
+            if a == 1:
+                filename = filename + '.crypt'
+                filenameStringVar.set(filename)
+                resultvarfile.set(
+                    '      Encrypted Successfully / added .crypt')
+                if encfiletoolbuttvar.get() == 1:
+                    with open(filename, 'rb') as f:
+                        file_content = f.read()
+                    try:
+                        main_db_conn.insert(
+                            filename, file_content, outputKeyref.get().strip())
+                    except BaseException:
+                        db_display_text.delete('1.0', tk.END)
+                        db_display_text.insert(
+                            tk.END, f"ERROR \n\nDatabase might be distorted\n")
+            if platform.system() == 'Windows':
+                if a == 2:
+                    resultvarfile.set('                 File is Empty')
+                if a == 3:
+                    resultvarfile.set("               File Doesn't Exist")
+                if a == 0:
+                    resultvarfile.set("                  Can't Encrypt")
+                if a == 4:
+                    resultvarfile.set('                     ERROR')
+                if a == 5:
+                    resultvarfile.set('          ERROR : Key is Not 512-bit')
+                if a == 6:
+                    resultvarfile.set(
+                        '       ERROR : File is already encrypted')
+                elif a == 7:
+                    resultvarfile.set(
+                        ' ERROR : Given a directory instead of a file')
+            else:
+                if a == 2:
+                    resultvarfile.set('                   File is Empty')
+                if a == 3:
+                    resultvarfile.set("                 File Doesn't Exist")
+                if a == 0:
+                    resultvarfile.set("                    Can't Encrypt")
+                if a == 4:
+                    resultvarfile.set('                       ERROR')
+                if a == 5:
+                    resultvarfile.set('            ERROR : Key is Not 512-bit')
+                if a == 6:
+                    resultvarfile.set(
+                        '         ERROR : File is already encrypted')
+                elif a == 7:
+                    resultvarfile.set(
+                        '   ERROR : Given a directory instead of a file')
+
+
+def decfile():
+    global add_dec_to_db, main_db_conn, mainkey
+    if 1:
+        if keySelectionFlag.get() != 0:
+            filename = filenameStringVar.get().strip()
+            key = mainkey
+            target = Af.CryptFile(filename, key)
+            a = target.decrypt()
+            if a == 1:
+                filename = os.path.splitext(filename)[0]
+                filenameStringVar.set(filename)
+                resultvarfile.set(
+                    '     Decrypted Successfully + removed .crypt')
+                if decfiletoolbuttvar.get() == 1:
+                    with open(filename, 'rb') as f:
+                        file_content = f.read()
+                    try:
+                        main_db_conn.insert(
+                            filename, file_content, outputKeyref.get().strip())
+                    except BaseException:
+                        db_display_text.delete('1.0', tk.END)
+                        db_display_text.insert(
+                            tk.END, f"ERROR \n\nDatabase might be distorted\n")
+            if platform.system() == 'Windows':
+                if a == 2:
+                    resultvarfile.set('                 File is Empty')
+                if a == 3:
+                    resultvarfile.set("               File Doesn't Exist")
+                if a == 0:
+                    resultvarfile.set("                 Can't Decrypt")
+                if a == 4:
+                    resultvarfile.set('                     ERROR')
+                elif a == 5:
+                    resultvarfile.set('          ERROR : Key is Not 512-bit')
+                if a == 6:
+                    resultvarfile.set(
+                        '       ERROR : File is already decrypted')
+                elif a == 7:
+                    resultvarfile.set(
+                        ' ERROR : Given a directory instead of a file')
+            else:
+                if a == 2:
+                    resultvarfile.set('                   File is Empty')
+                if a == 3:
+                    resultvarfile.set("                 File Doesn't Exist")
+                if a == 0:
+                    resultvarfile.set("                   Can't Decrypt")
+                if a == 4:
+                    resultvarfile.set('                       ERROR')
+                elif a == 5:
+                    resultvarfile.set('            ERROR : Key is Not 512-bit')
+                if a == 6:
+                    resultvarfile.set(
+                        '         ERROR : File is already decrypted')
+                elif a == 7:
+                    resultvarfile.set(
+                        '   ERROR : Given a directory instead of a file')
+
+
+encryptionfilebutton = tk.Button(
+    master=frameFile1,
+    text='ENCRYPT FILE',
+    command=enc_file,
+    bootstyle='warning outline')
+encryptionfilebutton.place(relx=0.25, rely=0.73)
+
+decryptionfilebutton = tk.Button(
+    master=frameFile1,
+    text='DECRYPT FILE',
+    command=decfile,
+    bootstyle='warning outline')
+decryptionfilebutton.place(relx=0.55, rely=0.73)
+
+filenameStringVar = tk.StringVar(value='')
+
+filenametext = tk.Entry(
+    master=frameFile1,
+    width=31,
+    font='Calibre 15 bold',
+    textvariable=filenameStringVar)
+filenametext.place(relx=0.05, rely=0.30)
+
+
+addtodbLabel = tk.Label(
+    master=frameFile1,
+    text='ADD TO DATABASE',
+    font=(
+        'Calibre',
+        11),
+    bootstyle='warning')
+addtodbLabel.place(relx=0.35, rely=0.908)
+
+add_enc_to_db = 0
+
+
+def enc_toggle_func():
+    global add_enc_to_db
+    if encfiletoolbuttvar == 1:
+        add_enc_to_db = 1
+    else:
+        add_enc_to_db = 0
+
+
+add_dec_to_db = 0
+
+
+def dec_toggle_func():
+    global add_dec_to_db
+    if decfiletoolbuttvar == 1:
+        add_dec_to_db = 1
+    else:
+        add_dec_to_db = 0
+
+
+encfiletoolbuttvar = tk.IntVar()
+encfiletoolbutt = tk.Checkbutton(bootstyle='warning , round-toggle',
+                                 master=frameFile1,
+                                 variable=encfiletoolbuttvar,
+                                 offvalue=0,
+                                 onvalue=1,
+                                 command=enc_toggle_func)
+encfiletoolbutt.state(['disabled'])
+encfiletoolbutt.place(relx=0.25, rely=0.92)
+
+
+decfiletoolbuttvar = tk.IntVar()
+decfiletoolbutt = tk.Checkbutton(bootstyle='warning , round-toggle',
+                                 master=frameFile1,
+                                 variable=decfiletoolbuttvar,
+                                 offvalue=0,
+                                 command=dec_toggle_func)
+decfiletoolbutt.state(['disabled'])
+decfiletoolbutt.place(relx=0.717, rely=0.92)
+
+
+keySelectionFlag = tk.IntVar(value=0)
+
+
+def main_key_wrapper():
+    global success_keysdb_connection_blocker, mainkey
+    if Af.CryptFile.keyverify(mainkeyvar.get().strip()) == 1:
+        mainkey = mainkeyvar.get().strip()
+        keyref_gen()
+        keyselectionvar.set('       SELECTED')
+        keySelectionFlag.set(1)
+        try:
+            if success_keysdb_connection_blocker and os.path.isfile(
+                    filenameStringVar.get().strip()):
+                keys_db_conn.insert(
+                    filenameStringVar.get().strip(),
+                    mainkey,
+                    outputKeyref.get())
+            if success_keysdb_connection_blocker and not os.path.isfile(
+                    filenameStringVar.get().strip()):
+                keys_db_conn.insert('STANDALONE', mainkey, outputKeyref.get())
+        except BaseException:
+            db_display_text.delete('1.0', tk.END)
+            db_display_text.insert(tk.END, f"Faulty Database\n")
+    else:
+        keySelectionFlag.set(0)
+        keyselectionvar.set('     NOT SELECTED')
+
+if platform.system() == 'Windows':
+    mainkeyLabel = tk.Label(master=frameFile2,
+                            text='MAIN KEY',
+                            font='Calibre 20',
+                            bootstyle='info',
+                            )
+    mainkeyLabel.place(relx=0.3, rely=0.075)
+else:
+    mainkeyLabel = tk.Label(master=frameFile2,
+                            text='MAIN KEY',
+                            font='Calibre 20 bold',
+                            bootstyle='info',
+                            )
+    mainkeyLabel.place(relx=0.3, rely=0.075)
+
+
+
+mainkeyvar = tk.StringVar()
+mainkeyEntry = tk.Entry(master=frameFile2,
+                        font='Calibre 14 bold',
+                        textvariable=mainkeyvar,
+                        width=29
+                        )
+mainkeyEntry.place(relx=0.09, rely=0.29)
+
+
+def keyref_gen():
+    ref = '#'
+    for _ in range(6):
+        character = secrets.choice(
+            string.ascii_letters +
+            string.digits +
+            '$' +
+            '?' +
+            '&' +
+            '@' +
+            '!' +
+            '-' +
+            '+')
+        ref += character
+    outputKeyref.set(ref)
+
+
+outputKeyref = tk.StringVar(value='#XXXXXX')
+keyrefLabel = tk.Label(
+    master=frameFile2,
+    textvariable=outputKeyref,
+    bootstyle='secondary',
+    font=(
+        'terminal',
+        12))
+keyrefLabel.place(relx=0.712, rely=0.12)
+
+keySelectButton = tk.Button(
+    master=frameFile2,
+    text='SELECT KEY',
+    command=main_key_wrapper,
+    bootstyle='info outline')
+keySelectButton.place(relx=0.6725, rely=0.5)
+
+
+keyselectionvar = tk.StringVar(value='   KEY NOT SELECTED')
+keyselectionLabel = tk.Label(master=frameFile2,
+                             textvariable=keyselectionvar,
+                             bootstyle='info',
+                             font='terminal 11 bold')
+keyselectionLabel.place(relx=0.15, rely=0.465, height=50)
+
+
+def genkey():
+    keyGenVar.set(Af.CryptFile.genkey())
+
+
+keyGenVar = tk.StringVar(value='')
+keyGenEntry = tk.Entry(master=frameFile2,
+                       font='Calibre 12 bold',
+                       textvariable=keyGenVar,
+                       width=23)
+keyGenEntry.place(relx=0.1, rely=0.69)
+
+keyButton = tk.Button(master=frameFile2,
+                      text='GENERATE',
+                      command=genkey,
+                      bootstyle='success outline')
+keyButton.place(relx=0.671, rely=0.7)
+
+
+'''----------------------------STAMP STARTED ------------------------------'''
+
+
+latest_ID_key_label = tk.Label(
+    master=lowerFrame,
+    text='GitHub.com/AshGw/AES-256',
+    font='Calibre 6')
+latest_ID_key_label.place(relx=0.84, rely=0.92)
+
+'''------------------------------STAMP ENDED------------------------------'''
+
+
+def rm_json():
+    global usable_real_path
+    file = os.path.join(usable_real_path, 'output.json')
+    if os.path.exists(file):
+        os.remove(file)
+
+
+
+atexit.register(rm_json)
+
+
+if __name__ == '__main__':
+    main_object.mainloop()
```

### Comparing `AshCrypt-3.0.2/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-3.0.3/AshCrypt.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1
-Name: AshCrypt
-Version: 3.0.2
-Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
-Home-page: https://github.com/AshGw/AES-256.git
-Author: Ashref Gwader
-Author-email: AshrefGw@proton.me
-License: UNKNOWN
-Description: # Cryptography App &  Library : AES-256
-        ##  Objective ## 
-        #### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256 With No Unnecessary Complications.
-        ## Docs ## 
-        **Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository.**
-        
-        
-Keywords: Cryptography application,cryptography libraryAES-256
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: AshCrypt
+Version: 3.0.3
+Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
+Home-page: https://github.com/AshGw/AES-256.git
+Author: Ashref Gwader
+Author-email: AshrefGw@proton.me
+Keywords: Cryptography application,cryptography libraryAES-256
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Cryptography App &  Library : AES-256
+##  Objective ## 
+#### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256 With No Unnecessary Complications.
+## Docs ## 
+**Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository.**
+
```

### Comparing `AshCrypt-3.0.2/PKG-INFO` & `AshCrypt-3.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1
-Name: AshCrypt
-Version: 3.0.2
-Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
-Home-page: https://github.com/AshGw/AES-256.git
-Author: Ashref Gwader
-Author-email: AshrefGw@proton.me
-License: UNKNOWN
-Description: # Cryptography App &  Library : AES-256
-        ##  Objective ## 
-        #### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256 With No Unnecessary Complications.
-        ## Docs ## 
-        **Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository.**
-        
-        
-Keywords: Cryptography application,cryptography libraryAES-256
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: AshCrypt
+Version: 3.0.3
+Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
+Home-page: https://github.com/AshGw/AES-256.git
+Author: Ashref Gwader
+Author-email: AshrefGw@proton.me
+Keywords: Cryptography application,cryptography libraryAES-256
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Cryptography App &  Library : AES-256
+##  Objective ## 
+#### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256 With No Unnecessary Complications.
+## Docs ## 
+**Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository.**
+
```

### Comparing `AshCrypt-3.0.2/README.md` & `AshCrypt-3.0.3/README.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,371 +1,371 @@
-# Cryptography App & Library w/ AES-256
-##  Objective ## 
-#### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256.
-## Reason Behind It
-In a world where control, surveillance, and privacy violations are increasingly prevalent, the protection of individual freedom becomes crucial. 
-
-This led me to develop a set of tools in Python that leverages the AES-256 algorithm to make it easier for individuals to safeguard their data without blindly relying on third parties to do it for them. 
-
-My aim here is to make these tools accessible and user-friendly, even for individuals with a limited programming knowledge. By providing these resources, I hope to contribute to the preservation of privacy and enable individuals to take control of their own data security, so feel free to explore these tools.
-## Overview ## 
-![alt text](important/GUI.png)
-The project incorporates an App & a library called **AshCrypt** : 
-
-**App :** 
-<br>Full-fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
-<br>check [GUI](https://github.com/AshGw/AES-256#GUI) header for more info.
-
-**Library :** 
-<br>A simple, secure, and developer-oriented library for performing encryption and decryption operations on data using the AES-256 (CBC) encryption algorithm.
-<br>The core of the library is the module `crypt`
-It offers cryptographic capabilities and top security measures to safeguard
-sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
-<br>View [Features](https://github.com/AshGw/AES-256#features) Header for more details.
-
-
-
-
-
-### For Developers ###
-The project uses `crypt` module to ensure secure data encryption and decryption for files and texts while keeping it very easy and simple to use .
-view the headers for [filecrypt](https://github.com/AshGw/AES-256#filecrypt) and [textcrypt](https://github.com/AshGw/AES-256#textcrypt) to learn more.
-
-
-It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
-safe and simple manner.
-
-<br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if you're not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check [database](https://github.com/AshGw/AES-256#database-1) header to learn more.
-
-## Installation ##
-### If you want to use it as a library ###
-You can simply use **pip**
-<br>First upgrade the package installer 
-```bash
-pip install --upgrade pip 
-```
-Then install the Library 
-```bash
-pip install AshCrypt
-```
-This will install the latest version of `AshCrypt`.
-You can start using it in your code by importing its modules :
-
-```python
-from AshCrypt import crypt as ac
-```
-That's it.
-
-### Whole repo installation 
-Now if you want to get the whole repo with no manual configurations
-<br>Run this command in the Terminal
-```bash
-curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/main/important/setup.sh | bash
-```
-This will run the commands in [setup.sh](important/setup.sh).
-<br>It will clone & install all the dependencies needed on your machine and activate the development mode, inside the directory you're currently at.
-
-<details>
-<summary>Got Errors ?</summary>
-
-<h5>For Debian based systems</h5>
-
-1) Install `curl` if you don't have it already 
-```bash
-sudo apt-get install curl
-```
-2) If you're running a lightweight python version it might not include `tkinter` in the standard library so run
-```bash
-sudo apt-get update
-sudo apt-get install python3-tk 
-```
-3) If you're running `python 3.6` or older, then you might need to install `dataclasses`
-```
-pip install dataclasses
-```
-<br>Now if none of this works you might just use the docker image for this purpose, so check this [directory](Docker-build)
-</details>
-
-**After the library is installed** 
-<br>To run the GUI 
-```shell
-python -m AshCrypt.gui
-```
-
-**NOTE**:
-You  can use `clicrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints intended for use within systems where you can't use GUI's.
-
-
-To run the CLI 
-```shell
-python -m AshCrypt.clicrypt
-```
-
-## "crypt" Module ##
-The `crypt.py` Module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring security and 
-confidentiality.
-
-<br>It uses primitives from the `cryptography.py` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
-
-<br>You can check [Features](https://github.com/AshGw/AES-256#features) tag below to learn more about the security features.
-<br>You can check the [unittesting file](AshCrypt/unittests/unittest_crypt.py) to verify how it works.
-
-### Usage ##
-1) Generate a key if you don't have one already
-```python
-mainkey = Enc.genkey()
-```
-2) Before encrypting or decrypting anything, first set the arguments you want to pass, you can have an encrypted message or a  decrypted message , and a mainkey to use.
-<br>Set the correct mainkey ( 32 byte long key ) 
-```python
-mainkey = '6ce113be19e898c2b98df82b7fa8efb166928925fc05574a54eb1114c3410900'
-```
-The message can be of type string or bytes.
-<br>Normal string message :  
-```python 
-message = 'Hello There'
-```
-or a normal bytes message 
-```python
-message = b'Hello There'
-```
-or string URL safe encrypted message ( to decrypt ): 
-```python
-message = 'ZEfikRiNQ4EE1y5E-Qn4gQbo8goVpWLPstqTlgWtoRq1CK_oeMz4oelCYNpM-NZyzSIKk7DazkAUO9HcZJzWWMXR6zqRjNTN-c1Q6vRWSkj1g20oL6JbzUvEJL3xvY2-Fye1simoOAr7YP5YHAnSYAAAADIA0juak_JYQnzXQ-apJ8azahvngigFrHRg142g7OqvfA=='
-```
-or bytes type encrypted message ( to decrypt ):
-```python
-message = b'dG\xe2\x91\x18\x8dC\x81\x04\xd7.D\xf9\t\xf8\x81\x06\xe8\xf2\n\x15\xa5b\xcf\xb2\xda\x93\x96\x05\xad\xa1\x1a\xb5\x08\xaf\xe8x\xcc\xf8\xa1\xe9B`\xdaL\xf8\xd6r\xcd"\n\x93\xb0\xda\xce@\x14;\xd1\xdcd\x9c\xd6X\xc5\xd1\xeb:\x91\x8c\xd4\xcd\xf9\xcdP\xea\xf4VJH\xf5\x83m(/\xa2[\xcdK\xc4$\xbd\xf1\xbd\x8d\xbe\x17\'\xb5\xb2)\xa88\n\xfb`\xfeX\x1c\t\xd2`\x00\x00\x002\x00\xd2;\x9a\x93\xf2XB|\xd7C\xe6\xa9\'\xc6\xb3j\x1b\xe7\x82(\x05\xact`\xd7\x8d\xa0\xec\xea\xaf|'
-```
-3) Now pass the arguments accordingly. If you have a normal message and you try to decrypt it, an Exception will be raised so pass the arguments to the right classes. 
-<br><br>So first create an instance of either the `Enc` or `Dec` class. 
-<br>Here I chose to encrypt a message 
-```python
-a = Enc(message=message, mainkey=mainkey)
-```
-
-4) Now you'd have to specify the output, you can encrypt to bytes or encrypt to URL-safe strings.
-<br> Here I chose to encrypt to bytes
-```python
-output = a.enc_to_bytes()
-```
-you can also encrypt to a URL safe string
-```python
-output = a.enc_to_str()
-```
-<br> The same logic applies to the decryption process simply switch `Enc` with `Dec` and `enc_to_bytes` to `dec_to_bytes`
-That simple, that's it.
-
-
-
-
-## Features ## 
-- AES 256 CBC mode 
-- Generates a randomly secure 256-bit main key 
-- Derives the HMAC and the AES key from the mainkey using bcrypt's KDFs with a configurable number of iterations with :
-    - Salt : Random 128 bit value is generated  each time and passed to the KDF to generate the AES key
-    - Pepper : Random 128 bit value is generated  each time and passed to the KDF to generate the HMAC
-- AES Key : 256 bit
-- HMAC : 256 bit hashed using SHA512
-- Generates a random 128 bit Initialization Vector (IV) each time for the Cipher
-- PKCS7 message padding
-### Other Features :
-These focus on ease of use: 
-- No need to manipulate the input to fit, it accepts strings or bytes you can pass them right away
-- You can get a string or a bytes representation of either the encryption or the decryption result
-- In `crypt` module the key is flexible it doesn't have to be 256 bit long, it can actually be of any length but that's up to you to ensure its security, or leave it as is and use the key generation function to get secure and random keys ( although in `textcrypt` and `filecrypt` you have to use a 256 bit long key )
-- Encrypting to a string has URL-safe string representation 
-### Regarding KDFs
-Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
-<br>Im using 50 just to demonstrate the process and make it quick.
-<br>The bare minimum is 50 ( which is secure enough ), the max is 100 000, choose somewhere in between.
-<br>In my use case 50 takes around 0.5 secs while using the maximum number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
-<br>You can check how it works by checking this [Jupyter Notebook](demo/performance-check.ipynb) demo file
-
-
-## filecrypt ## 
-If you want to encrypt a file :
-1) Follow the steps above to set the key up.
-2) Create an instance of the class CryptFiles and pass 2 arguments, the first one being the target file and the second argument being the key :
-```python
-my_instance = CryptFile('target.txt', key)
-```
-```python
-my_instance = CryptFile('testDataBase.db', key)
-```
-The file can be of anything : image`.png`, movie `.mp4`,`.sqlite`  etc..
-<br>It doesn't have to just be of `.txt` extension ,can be of anything really.  
-<br>**Note** : 
-If the file is not in the working directory you can specify the whole path: 
-<br>**For windows**
-```python
-target = CryptFile('C:\\Users\\offic\\MyProjects\\SomeOtherfolder\\myfile.txt',key) 
-```
-<br>**On Mac and Linux :**
-```python
-target = CryptFile('/User/Desktop/MyProjects/SomeOtherfolder/myfile.txt',key)
-```
-3) Apply either the encryption or decryption functions to that instance :
-```python
-my_instance = CryptFile('qrv10.png',key)
-my_instance.encrypt()
-```
-you can apply `print()` on `my_instance.encrypt()`to check the result :
-<br> 1 : File successfully encrypted/decrypted + added/removed .crypt extension 
-<br> 2 : File is empty
-<br> 3 : File doesn't exist
-<br> 4 : Unknown Error usually a system related one 
-<br> 5 : Key is denied for cryptographic use
-<br> 6 : File is already encrypted/decrypted
-<br> 7 : File is not a file it's a directory
-<br> 0 : Error in enc/dec probable file distortion, tampering or wrong key
-```python
-my_instance.encrypt()
-```
-```python
-my_instance.decrypt()
-```
-
-That's it, if you follow the steps above then everything should work just fine.
-## textcrypt ## 
-Same steps above just the naming is different, and keep in mind both accept either strings or bytes 
-```python
-my_instance = Crypt('Hello Wold !',key)
-```
-```python
-my_instance.encrypt()[1]
-```
-```python
-my_instance.decrypt()[1]
-```
-The result simply returns a tuple so index `[0]` is going to be the confirmation if it's 1 then it worked, else some Error has occurred.
-<br>Index `[1]` contains the encrypted/decrypted content that's it very simple.
-
-**Note**:
-<br>Unlike the `crypt` module where if you try to decrypt a non-encrypted message you get all kinds of errors.
-
-in `filecrypt` & `textcrypt` it's simpler if you attempt to decrypt an non-encrypted message then you'll get the same message back along with an integer in this case `0` for failure.
-<br>`1`'s for success.
-<br>Non `1`'s for failure (`2`/`0.0`/`0`) each indicate different Errors. 
-
-Error handling here has no Exceptions raised just `1`'s, `0`'s & `2`'s for feedback, just to make it simple and Non-Technical.
-
-
-### QR ## 
-The `qr.py` module is used to display a qr code of the encrypted/decrypted messages to be quickly scanned and transmitted , you can use qr versions from `1` to `40` , although I recommend using `40` since it can take the maximum number of characters for small files , and `10` if you're working with the GUI which is intended for text/short messages,
-
-## database ##
-To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using an sqlite3 database
-
-Ensuring that the encrypted data remains organized and readily accessible to anyone with the right key. Any content going in must be encrypted with a key that you must keep off grid.
-
-**Note** that in `database.py` I'm using `dataclasses` module which was introduced in `python 3.7`, so make sure to install it if you have an older version.
-
-### Usage ## 
-In the module I'm providing built-in functions to make it easier to perform usual queries on Sqlite tables , by default it creates a table `Classified` with two default columns :
-
-**content** : This can be a single character or a whole movie in binary, that depends on your specific needs.
-
-**key** : This key column wasn't indeed meant to store a key itself but rather store a reference to the actual key. The key itself should be stored somewhere else safe and secure preferably off-grid and completely separate from any vulnerable devices on you can have it on a separate database stored safely away, you can even write it down on a piece of paper if you want , just make sure to rotate your keys from time to time.
-
-1) Create a connection to the database :
-```python
-conn = Database('test.db')
-```
-This would automatically set the default table name to `Classifed` if no arguments are passed to the other class functions then they would all be working on the default table name , if you want to set your default table name instead of `Classified` you can pass your table name as the second argument : 
-```python
-conn = Database('test.db','MyDefaultTable')
-```
-2) create/add the table to the database :
-```python
-conn.addtable()
-```
-Added the default table that's been set to the database,  if you want to pass an argument to the function that would create another table of your choice
-
-3) Set a reference to the key not the key itself : 
-```python
- key = '#5482A'
-```
-4) Use the connection to perform various tasks <br>
-The content can be anything post encryption bytes or string format
-```python
-content='Some Encrypted Content'
-conn.insert(content=content,key='#1E89JO', optional_table_name=None)
-```
-If the optional table name is `None` then it will insert into the default table , else it would insert into the table you specify
-
-
-5) You can check the tables you have , it returns a generator object, yields the result of each element so you must run a for loop over it
-```python
-for e in conn.show_tables():
-        print(e)
-```
-You can check the current size of the database using the size property method 
-```python
-print(conn.size) # Size of the Database in MB 
-```
-
-6) Check the module itself so you can run through all the available methods.
-<br>The methods available perform the usual operations like insertion, deletion , updating the database and more..
-
-
-7) to run more complex queries I've dedicated a query function that takes in `*queries` and returns the result fetched 
-```python
-query = 'SELECT COUNT(*) AS cc ,content FROM Classified WHERE key = "#5482A" ORDER BY cc DESC '
-print(conn.query(query))
-```
-The result fetched should look like this : 
- ```python
-[{'query 0': ['SUCCESS', [(1, 'some encrypted content of bytes or strings')]]}]
-```
-If some error has occurred while querying like : 
-```python
-query = 'SELECT COUNT(*) AS cc ,content FROM DoesntExist WHERE key = "#5482A" ORDER BY cc DESC '
-```
-The result fetched should look similar to this : 
-```python
-[{'query 0': ('FAILURE', 'no such table: DoesntExist')}]
-```
-That's it so simple !
-
-
-## GUI ##
-The GUI as mentioned above is a fully functional application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
-### Usage ###
-1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. Then insert it in the `MAINKEY` entry
-2) Now you're able to encrypt files or text (text is limited to 200 characters max)
-####  Text : 
-- You can insert some text in the entry right below the `TEXT ENCRYPTION` label.<br>The given text will be encrypted and you can choose if you want to have that text displayed as a qr code, a qr image will pop on the screen and you'll be able to scan it using your phone.
-- Insert some encrypted text below the `TEXT DECRYPTION` label.<br>The given text will be decrypted and you'd have the option to display the "plaintext" as a qr code to be scanned by other devices.
-<br>If the text cannot be decrypted it will display itself , so you might as well use this to display the key you're using as a qr code 
-
-#### Files
-- Under the `FILE PATH` label enter the file name (if it's in the current working directory) or submit the whole file path , the file can be of any type, click on `ENCRYPT FILE` Button to encrypt the given file , if the encryption turned out to be successful , you'll see a success message along with a `added .crypt extention to the file` message if the encryption wasn't successful you'll see an error message specifying the problem.<br>Note that you cannot re-encrypt a file that  has `.crypt` as extention.
-- The file name should be changed by now to `filename + '.crypt'` , if the file has .crypt extension you can go ahead and decrypt it , if the same key is used for both enc/dec operations then the result should be `success` + `removed .crypt extention` from the file.
-#### Database
-- Now you have some encrypted/decrypted files but you want to keep them stored somewhere safe, this is where the main database comes in , where you need to store your files + their content + reference to the key used for their encryption/decryption. you can specify your database by :
-1) Specifying the actual path where you want your database to be 
-2) Give it a name, it must be a valid file name that ends with `.db` .<br>
-If the database doesn't exist then a database with the name you've given will be created and automatically connected to.<br>If the given database already exists then it will automatically connect.
-3) Did I mention the keys' database ? well if you give a database file name it will also create the keys database with the same name as the database you chose plus `Keys` added to its name. This database holds the actual keys and the reference to these keys.
-<br>The only common data that these two separate databases have in common is the key reference values.  
-
-   
-**Info** Both databases have the same table called `Classified` that has 4 columns <br>`ID` which is auto generated & incremented for each piece of data that gets inserted<br>
-`Name` that holds the filename in both databases , although in the keys database if you haven't specified any file to operate on and keep selecting keys the keys name will be `STANDALONE` 
-<br>`Content` in the main db, that holds the entire content of the given file whereas for the keys db that holds the actual 256 bit encryption key.
-<br>`Key` in  both db's that holds the `KeyRef` or key reference value
-#### Usage 
-The buttons are self-explanatory so do what you see fit. the result of any task related to the databases is displayed in `DATABASE OUTPUT CONSOLE` although you can run a query anytime by writing a query and using `query` button , the result will be displayed to an `output.json` file that auto-deletes when you exit the app.
-<br>Just click buttons and check the result in the output console, it will guide you through the process.
-
-<br>To run the GUI anywhere
-```shell
-python -m AshCrypt.gui
-```
-
-
-## License ##
-This project is licensed under the [MIT LICENSE](https://github.com/AshGw/AES-256/blob/main/LICENSE).
-## Acknowledgments ##
-This cryptographic scheme is inspired by secure cryptographic practices and various open-source implementations.
-
+# Cryptography App & Library w/ AES-256
+##  Objective ## 
+#### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256.
+## Reason Behind It
+In a world where control, surveillance, and privacy violations are increasingly prevalent, the protection of individual freedom becomes crucial. 
+
+This led me to develop a set of tools in Python that leverages the AES-256 algorithm to make it easier for individuals to safeguard their data without blindly relying on third parties to do it for them. 
+
+My aim here is to make these tools accessible and user-friendly, even for individuals with a limited programming knowledge. By providing these resources, I hope to contribute to the preservation of privacy and enable individuals to take control of their own data security, so feel free to explore these tools.
+## Overview ## 
+![alt text](important/GUI.png)
+The project incorporates an App & a library called **AshCrypt** : 
+
+**App :** 
+<br>Full-fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
+<br>check [GUI](https://github.com/AshGw/AES-256#GUI) header for more info.
+
+**Library :** 
+<br>A simple, secure, and developer-oriented library for performing encryption and decryption operations on data using the AES-256 (CBC) encryption algorithm.
+<br>The core of the library is the module `crypt`
+It offers cryptographic capabilities and top security measures to safeguard
+sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
+<br>View [Features](https://github.com/AshGw/AES-256#features) Header for more details.
+
+
+
+
+
+### For Developers ###
+The project uses `crypt` module to ensure secure data encryption and decryption for files and texts while keeping it very easy and simple to use .
+view the headers for [filecrypt](https://github.com/AshGw/AES-256#filecrypt) and [textcrypt](https://github.com/AshGw/AES-256#textcrypt) to learn more.
+
+
+It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
+safe and simple manner.
+
+<br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if you're not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check [database](https://github.com/AshGw/AES-256#database-1) header to learn more.
+
+## Installation ##
+### If you want to use it as a library ###
+You can simply use **pip**
+<br>First upgrade the package installer 
+```bash
+pip install --upgrade pip 
+```
+Then install the Library 
+```bash
+pip install AshCrypt
+```
+This will install the latest version of `AshCrypt`.
+You can start using it in your code by importing its modules :
+
+```python
+from AshCrypt import crypt as ac
+```
+That's it.
+
+### Whole repo installation 
+Now if you want to get the whole repo with no manual configurations
+<br>Run this command in the Terminal
+```bash
+curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/main/important/setup.sh | bash
+```
+This will run the commands in [setup.sh](important/setup.sh).
+<br>It will clone & install all the dependencies needed on your machine and activate the development mode, inside the directory you're currently at.
+
+<details>
+<summary>Got Errors ?</summary>
+
+<h5>For Debian based systems</h5>
+
+1) Install `curl` if you don't have it already 
+```bash
+sudo apt-get install curl
+```
+2) If you're running a lightweight python version it might not include `tkinter` in the standard library so run
+```bash
+sudo apt-get update
+sudo apt-get install python3-tk 
+```
+3) If you're running `python 3.6` or older, then you might need to install `dataclasses`
+```
+pip install dataclasses
+```
+<br>Now if none of this works you might just use the docker image for this purpose, so check this [directory](Docker-build)
+</details>
+
+**After the library is installed** 
+<br>To run the GUI 
+```shell
+python -m AshCrypt.gui
+```
+
+**NOTE**:
+You  can use `clicrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints intended for use within systems where you can't use GUI's.
+
+
+To run the CLI 
+```shell
+python -m AshCrypt.clicrypt
+```
+
+## "crypt" Module ##
+The `crypt.py` Module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring security and 
+confidentiality.
+
+<br>It uses primitives from the `cryptography.py` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
+
+<br>You can check [Features](https://github.com/AshGw/AES-256#features) tag below to learn more about the security features.
+<br>You can check the [unittesting file](AshCrypt/unittests/unittest_crypt.py) to verify how it works.
+
+### Usage ##
+1) Generate a key if you don't have one already
+```python
+mainkey = Enc.genkey()
+```
+2) Before encrypting or decrypting anything, first set the arguments you want to pass, you can have an encrypted message or a  decrypted message , and a mainkey to use.
+<br>Set the correct mainkey ( 32 byte long key ) 
+```python
+mainkey = '6ce113be19e898c2b98df82b7fa8efb166928925fc05574a54eb1114c3410900'
+```
+The message can be of type string or bytes.
+<br>Normal string message :  
+```python 
+message = 'Hello There'
+```
+or a normal bytes message 
+```python
+message = b'Hello There'
+```
+or string URL safe encrypted message ( to decrypt ): 
+```python
+message = 'ZEfikRiNQ4EE1y5E-Qn4gQbo8goVpWLPstqTlgWtoRq1CK_oeMz4oelCYNpM-NZyzSIKk7DazkAUO9HcZJzWWMXR6zqRjNTN-c1Q6vRWSkj1g20oL6JbzUvEJL3xvY2-Fye1simoOAr7YP5YHAnSYAAAADIA0juak_JYQnzXQ-apJ8azahvngigFrHRg142g7OqvfA=='
+```
+or bytes type encrypted message ( to decrypt ):
+```python
+message = b'dG\xe2\x91\x18\x8dC\x81\x04\xd7.D\xf9\t\xf8\x81\x06\xe8\xf2\n\x15\xa5b\xcf\xb2\xda\x93\x96\x05\xad\xa1\x1a\xb5\x08\xaf\xe8x\xcc\xf8\xa1\xe9B`\xdaL\xf8\xd6r\xcd"\n\x93\xb0\xda\xce@\x14;\xd1\xdcd\x9c\xd6X\xc5\xd1\xeb:\x91\x8c\xd4\xcd\xf9\xcdP\xea\xf4VJH\xf5\x83m(/\xa2[\xcdK\xc4$\xbd\xf1\xbd\x8d\xbe\x17\'\xb5\xb2)\xa88\n\xfb`\xfeX\x1c\t\xd2`\x00\x00\x002\x00\xd2;\x9a\x93\xf2XB|\xd7C\xe6\xa9\'\xc6\xb3j\x1b\xe7\x82(\x05\xact`\xd7\x8d\xa0\xec\xea\xaf|'
+```
+3) Now pass the arguments accordingly. If you have a normal message and you try to decrypt it, an Exception will be raised so pass the arguments to the right classes. 
+<br><br>So first create an instance of either the `Enc` or `Dec` class. 
+<br>Here I chose to encrypt a message 
+```python
+a = Enc(message=message, mainkey=mainkey)
+```
+
+4) Now you'd have to specify the output, you can encrypt to bytes or encrypt to URL-safe strings.
+<br> Here I chose to encrypt to bytes
+```python
+output = a.enc_to_bytes()
+```
+you can also encrypt to a URL safe string
+```python
+output = a.enc_to_str()
+```
+<br> The same logic applies to the decryption process simply switch `Enc` with `Dec` and `enc_to_bytes` to `dec_to_bytes`
+That simple, that's it.
+
+
+
+
+## Features ## 
+- AES 256 CBC mode 
+- Generates a randomly secure 256-bit main key 
+- Derives the HMAC and the AES key from the mainkey using bcrypt's KDFs with a configurable number of iterations with :
+    - Salt : Random 128 bit value is generated  each time and passed to the KDF to generate the AES key
+    - Pepper : Random 128 bit value is generated  each time and passed to the KDF to generate the HMAC
+- AES Key : 256 bit
+- HMAC : 256 bit hashed using SHA512
+- Generates a random 128 bit Initialization Vector (IV) each time for the Cipher
+- PKCS7 message padding
+### Other Features :
+These focus on ease of use: 
+- No need to manipulate the input to fit, it accepts strings or bytes you can pass them right away
+- You can get a string or a bytes representation of either the encryption or the decryption result
+- In `crypt` module the key is flexible it doesn't have to be 256 bit long, it can actually be of any length but that's up to you to ensure its security, or leave it as is and use the key generation function to get secure and random keys ( although in `textcrypt` and `filecrypt` you have to use a 256 bit long key )
+- Encrypting to a string has URL-safe string representation 
+### Regarding KDFs
+Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
+<br>Im using 50 just to demonstrate the process and make it quick.
+<br>The bare minimum is 50 ( which is secure enough ), the max is 100 000, choose somewhere in between.
+<br>In my use case 50 takes around 0.5 secs while using the maximum number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
+<br>You can check how it works by checking this [Jupyter Notebook](demo/performance-check.ipynb) demo file
+
+
+## filecrypt ## 
+If you want to encrypt a file :
+1) Follow the steps above to set the key up.
+2) Create an instance of the class CryptFiles and pass 2 arguments, the first one being the target file and the second argument being the key :
+```python
+my_instance = CryptFile('target.txt', key)
+```
+```python
+my_instance = CryptFile('testDataBase.db', key)
+```
+The file can be of anything : image`.png`, movie `.mp4`,`.sqlite`  etc..
+<br>It doesn't have to just be of `.txt` extension ,can be of anything really.  
+<br>**Note** : 
+If the file is not in the working directory you can specify the whole path: 
+<br>**For windows**
+```python
+target = CryptFile('C:\\Users\\offic\\MyProjects\\SomeOtherfolder\\myfile.txt',key) 
+```
+<br>**On Mac and Linux :**
+```python
+target = CryptFile('/User/Desktop/MyProjects/SomeOtherfolder/myfile.txt',key)
+```
+3) Apply either the encryption or decryption functions to that instance :
+```python
+my_instance = CryptFile('qrv10.png',key)
+my_instance.encrypt()
+```
+you can apply `print()` on `my_instance.encrypt()`to check the result :
+<br> 1 : File successfully encrypted/decrypted + added/removed .crypt extension 
+<br> 2 : File is empty
+<br> 3 : File doesn't exist
+<br> 4 : Unknown Error usually a system related one 
+<br> 5 : Key is denied for cryptographic use
+<br> 6 : File is already encrypted/decrypted
+<br> 7 : File is not a file it's a directory
+<br> 0 : Error in enc/dec probable file distortion, tampering or wrong key
+```python
+my_instance.encrypt()
+```
+```python
+my_instance.decrypt()
+```
+
+That's it, if you follow the steps above then everything should work just fine.
+## textcrypt ## 
+Same steps above just the naming is different, and keep in mind both accept either strings or bytes 
+```python
+my_instance = Crypt('Hello Wold !',key)
+```
+```python
+my_instance.encrypt()[1]
+```
+```python
+my_instance.decrypt()[1]
+```
+The result simply returns a tuple so index `[0]` is going to be the confirmation if it's 1 then it worked, else some Error has occurred.
+<br>Index `[1]` contains the encrypted/decrypted content that's it very simple.
+
+**Note**:
+<br>Unlike the `crypt` module where if you try to decrypt a non-encrypted message you get all kinds of errors.
+
+in `filecrypt` & `textcrypt` it's simpler if you attempt to decrypt an non-encrypted message then you'll get the same message back along with an integer in this case `0` for failure.
+<br>`1`'s for success.
+<br>Non `1`'s for failure (`2`/`0.0`/`0`) each indicate different Errors. 
+
+Error handling here has no Exceptions raised just `1`'s, `0`'s & `2`'s for feedback, just to make it simple and Non-Technical.
+
+
+### QR ## 
+The `qr.py` module is used to display a qr code of the encrypted/decrypted messages to be quickly scanned and transmitted , you can use qr versions from `1` to `40` , although I recommend using `40` since it can take the maximum number of characters for small files , and `10` if you're working with the GUI which is intended for text/short messages,
+
+## database ##
+To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using an sqlite3 database
+
+Ensuring that the encrypted data remains organized and readily accessible to anyone with the right key. Any content going in must be encrypted with a key that you must keep off grid.
+
+**Note** that in `database.py` I'm using `dataclasses` module which was introduced in `python 3.7`, so make sure to install it if you have an older version.
+
+### Usage ## 
+In the module I'm providing built-in functions to make it easier to perform usual queries on Sqlite tables , by default it creates a table `Classified` with two default columns :
+
+**content** : This can be a single character or a whole movie in binary, that depends on your specific needs.
+
+**key** : This key column wasn't indeed meant to store a key itself but rather store a reference to the actual key. The key itself should be stored somewhere else safe and secure preferably off-grid and completely separate from any vulnerable devices on you can have it on a separate database stored safely away, you can even write it down on a piece of paper if you want , just make sure to rotate your keys from time to time.
+
+1) Create a connection to the database :
+```python
+conn = Database('test.db')
+```
+This would automatically set the default table name to `Classifed` if no arguments are passed to the other class functions then they would all be working on the default table name , if you want to set your default table name instead of `Classified` you can pass your table name as the second argument : 
+```python
+conn = Database('test.db','MyDefaultTable')
+```
+2) create/add the table to the database :
+```python
+conn.addtable()
+```
+Added the default table that's been set to the database,  if you want to pass an argument to the function that would create another table of your choice
+
+3) Set a reference to the key not the key itself : 
+```python
+ key = '#5482A'
+```
+4) Use the connection to perform various tasks <br>
+The content can be anything post encryption bytes or string format
+```python
+content='Some Encrypted Content'
+conn.insert(content=content,key='#1E89JO', optional_table_name=None)
+```
+If the optional table name is `None` then it will insert into the default table , else it would insert into the table you specify
+
+
+5) You can check the tables you have , it returns a generator object, yields the result of each element so you must run a for loop over it
+```python
+for e in conn.show_tables():
+        print(e)
+```
+You can check the current size of the database using the size property method 
+```python
+print(conn.size) # Size of the Database in MB 
+```
+
+6) Check the module itself so you can run through all the available methods.
+<br>The methods available perform the usual operations like insertion, deletion , updating the database and more..
+
+
+7) to run more complex queries I've dedicated a query function that takes in `*queries` and returns the result fetched 
+```python
+query = 'SELECT COUNT(*) AS cc ,content FROM Classified WHERE key = "#5482A" ORDER BY cc DESC '
+print(conn.query(query))
+```
+The result fetched should look like this : 
+ ```python
+[{'query 0': ['SUCCESS', [(1, 'some encrypted content of bytes or strings')]]}]
+```
+If some error has occurred while querying like : 
+```python
+query = 'SELECT COUNT(*) AS cc ,content FROM DoesntExist WHERE key = "#5482A" ORDER BY cc DESC '
+```
+The result fetched should look similar to this : 
+```python
+[{'query 0': ('FAILURE', 'no such table: DoesntExist')}]
+```
+That's it so simple !
+
+
+## GUI ##
+The GUI as mentioned above is a fully functional application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
+### Usage ###
+1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. Then insert it in the `MAINKEY` entry
+2) Now you're able to encrypt files or text (text is limited to 200 characters max)
+####  Text : 
+- You can insert some text in the entry right below the `TEXT ENCRYPTION` label.<br>The given text will be encrypted and you can choose if you want to have that text displayed as a qr code, a qr image will pop on the screen and you'll be able to scan it using your phone.
+- Insert some encrypted text below the `TEXT DECRYPTION` label.<br>The given text will be decrypted and you'd have the option to display the "plaintext" as a qr code to be scanned by other devices.
+<br>If the text cannot be decrypted it will display itself , so you might as well use this to display the key you're using as a qr code 
+
+#### Files
+- Under the `FILE PATH` label enter the file name (if it's in the current working directory) or submit the whole file path , the file can be of any type, click on `ENCRYPT FILE` Button to encrypt the given file , if the encryption turned out to be successful , you'll see a success message along with a `added .crypt extention to the file` message if the encryption wasn't successful you'll see an error message specifying the problem.<br>Note that you cannot re-encrypt a file that  has `.crypt` as extention.
+- The file name should be changed by now to `filename + '.crypt'` , if the file has .crypt extension you can go ahead and decrypt it , if the same key is used for both enc/dec operations then the result should be `success` + `removed .crypt extention` from the file.
+#### Database
+- Now you have some encrypted/decrypted files but you want to keep them stored somewhere safe, this is where the main database comes in , where you need to store your files + their content + reference to the key used for their encryption/decryption. you can specify your database by :
+1) Specifying the actual path where you want your database to be 
+2) Give it a name, it must be a valid file name that ends with `.db` .<br>
+If the database doesn't exist then a database with the name you've given will be created and automatically connected to.<br>If the given database already exists then it will automatically connect.
+3) Did I mention the keys' database ? well if you give a database file name it will also create the keys database with the same name as the database you chose plus `Keys` added to its name. This database holds the actual keys and the reference to these keys.
+<br>The only common data that these two separate databases have in common is the key reference values.  
+
+   
+**Info** Both databases have the same table called `Classified` that has 4 columns <br>`ID` which is auto generated & incremented for each piece of data that gets inserted<br>
+`Name` that holds the filename in both databases , although in the keys database if you haven't specified any file to operate on and keep selecting keys the keys name will be `STANDALONE` 
+<br>`Content` in the main db, that holds the entire content of the given file whereas for the keys db that holds the actual 256 bit encryption key.
+<br>`Key` in  both db's that holds the `KeyRef` or key reference value
+#### Usage 
+The buttons are self-explanatory so do what you see fit. the result of any task related to the databases is displayed in `DATABASE OUTPUT CONSOLE` although you can run a query anytime by writing a query and using `query` button , the result will be displayed to an `output.json` file that auto-deletes when you exit the app.
+<br>Just click buttons and check the result in the output console, it will guide you through the process.
+
+<br>To run the GUI anywhere
+```shell
+python -m AshCrypt.gui
+```
+
+
+## License ##
+This project is licensed under the [MIT LICENSE](https://github.com/AshGw/AES-256/blob/main/LICENSE).
+## Acknowledgments ##
+This cryptographic scheme is inspired by secure cryptographic practices and various open-source implementations.
+
```

### Comparing `AshCrypt-3.0.2/setup.py` & `AshCrypt-3.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from setuptools import setup, find_packages
-
-with open('AshCrypt/README.md', 'r') as f:
-    readme = f.read()
-
-setup(
-    name='AshCrypt',
-    version='3.0.2',
-    author='Ashref Gwader',
-    author_email='AshrefGw@proton.me',
-    python_requires='>=3.7',
-    description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
-                " with a database module to store encrypted content.",
-    long_description_content_type='text/markdown',
-    long_description=readme,
-    url='https://github.com/AshGw/AES-256.git',
-    packages=find_packages(exclude=['important', 'Docker-build', '.github', 'Executables', 'demo']),
-    package_data={
-        'AshCrypt': ['**'],
-    },
-    exclude_package_data={
-        '': ['.gitignore', 'LICENSE', 'README'],
-    },
-    install_requires=[
-        'bcrypt==4.0.1',
-        'cryptography==40.0.2',
-        'qrcode==7.4.2',
-        'ttkbootstrap==1.10.1',
-    ],
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-    ],
-    keywords=[
-        'Cryptography application',
-        'cryptography library'
-        'AES-256',
-    ],
-)
+from setuptools import setup, find_packages
+
+with open('AshCrypt/README.md', 'r') as f:
+    readme = f.read()
+
+setup(
+    name='AshCrypt',
+    version='3.0.3',
+    author='Ashref Gwader',
+    author_email='AshrefGw@proton.me',
+    python_requires='>=3.7',
+    description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
+                " with a database module to store encrypted content.",
+    long_description_content_type='text/markdown',
+    long_description=readme,
+    url='https://github.com/AshGw/AES-256.git',
+    packages=find_packages(exclude=['important', 'Docker-build', '.github', 'Executables', 'demo']),
+    package_data={
+        'AshCrypt': ['**'],
+    },
+    exclude_package_data={
+        '': ['.gitignore', 'LICENSE', 'README'],
+    },
+    install_requires=[
+        'bcrypt==4.0.1',
+        'cryptography==40.0.2',
+        'qrcode==7.4.2',
+        'ttkbootstrap==1.10.1',
+    ],
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+    ],
+    keywords=[
+        'Cryptography application',
+        'cryptography library'
+        'AES-256',
+    ],
+)
```

