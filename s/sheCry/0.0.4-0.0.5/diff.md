# Comparing `tmp/sheCry-0.0.4.tar.gz` & `tmp/sheCry-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheCry-0.0.4.tar", last modified: Tue Aug  1 08:25:56 2023, max compression
+gzip compressed data, was "sheCry-0.0.5.tar", last modified: Tue Aug  1 08:28:45 2023, max compression
```

## Comparing `sheCry-0.0.4.tar` & `sheCry-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:25:56.657404 sheCry-0.0.4/
--rw-rw-rw-   0        0        0    35821 2023-07-31 18:14:15.000000 sheCry-0.0.4/LICENSE.md
--rw-rw-rw-   0        0        0     9532 2023-08-01 08:25:56.651403 sheCry-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     8885 2023-08-01 08:25:41.000000 sheCry-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 08:25:56.658411 sheCry-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      909 2023-08-01 08:05:48.000000 sheCry-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:25:56.649403 sheCry-0.0.4/sheCry.egg-info/
--rw-rw-rw-   0        0        0     9532 2023-08-01 08:25:56.000000 sheCry-0.0.4/sheCry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-08-01 08:25:56.000000 sheCry-0.0.4/sheCry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:25:56.000000 sheCry-0.0.4/sheCry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:25:56.000000 sheCry-0.0.4/sheCry.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 08:28:45.382835 sheCry-0.0.5/
+-rw-rw-rw-   0        0        0    35821 2023-07-31 18:14:15.000000 sheCry-0.0.5/LICENSE.md
+-rw-rw-rw-   0        0        0     9505 2023-08-01 08:28:45.375834 sheCry-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8858 2023-08-01 08:28:27.000000 sheCry-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:28:45.382835 sheCry-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-08-01 08:28:40.000000 sheCry-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:28:45.373833 sheCry-0.0.5/sheCry.egg-info/
+-rw-rw-rw-   0        0        0     9505 2023-08-01 08:28:45.000000 sheCry-0.0.5/sheCry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-08-01 08:28:45.000000 sheCry-0.0.5/sheCry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:28:45.000000 sheCry-0.0.5/sheCry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:28:45.000000 sheCry-0.0.5/sheCry.egg-info/top_level.txt
```

### Comparing `sheCry-0.0.4/LICENSE.md` & `sheCry-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sheCry-0.0.4/PKG-INFO` & `sheCry-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheCry
-Version: 0.0.4
+Version: 0.0.5
 Summary: SHE Cryptography is architectured by Tahsin Ahmed.
 Home-page: 
 Author: Tahsin Ahmed
 Keywords: cryptography,encryption,decryption,SHE,SHE cryptography,Symmetric Hybrid Encryption,Symmetric Hybrid Encryption cryptography,sheCry
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
@@ -28,46 +28,41 @@
 Nowadays, security has become one of the most burning and sensitive issues. Confidential data is being stolen by malicious attackers rapidly. To prevent this kind of act, many security measures have been established. But “Cryptography” plays the most crucial part when we call for security. This is so because cryptography is used to protect enterprise information and communication from cyber threats through the use of codes. For example, AES and RSA are the gold standards. They are very popular and still vastly used in many renowned organizations as well as in the government. But the drawback is, AES is hardware and software dependent. So, we need to design it according to hardware and software systems. As a result, this implementation increases time and cost. Also, the attacker uses a “Side Channel Attack” to break AES. As a result, it becomes vulnerable. AES performs great in 256 bits keys and is faster in powerful devices. But if it is used in a low computational powered device then we have to use fewer bits (e.g. 64 bits), or the device could not handle the calculation of larger numbers. Thus, AES performs badly in this criterion. If we use fewer bits in AES, then a “Correlation Power Analysis Attack” is possible. So, it is not worth using AES in low computational powered devices. Whereas, RSA is slow due to its large mathematical calculation with large numbers and asymmetric mechanism. As a result, RSA fails to perform in terms of speed and low computational power. Also, the world is switching to lightweight technology day by day. IOT is the best example of it. But to secure those less powerful electronics, there is no such effective cryptographic system yet. Also, breaching the confidential data of the government and the corporate world is a very old topic and it still remains a rapid concern. So, we really need to innovate a new cryptographic algorithm that gives better results in low-power electronics and performs faster, and gives better security in sharing data. This is where lightweight cryptography SHE comes to play.
 
 ----------------------------
 **Solution Statement**
 ----------------------------
 * **Environment Independency:** SHE is reliable on any platform weather it is for software or hardware. So, developer does not need to hassle with cryptographic system while designing a software or hardware. Thus, it decreases a developer's production time as well.
 
-
 * **Cost Effectiveness**: In 2007, about 10% of the average IT budget was spent on energy, and energy costs for IT were expected to rise to 50% by 2010. However, the cost of power supply generally depends on the maximum possible power that could be used at any one time. If a CPU needs to calculate a larger number for a cryptographical system, it needs more power and more efficiency to compute in a very short time. As a result, this increases costs most of the time. To reduce cost, many electronic products choose to use a much lighter system. This is where the SHE cryptographic system plays a major role. It reduces the clock rate when it processes large numbers of cryptographical computations. Thus, it reduces cost.
 
-
 * **Better Security**: No doubt SHE gives better security. It encrypts and decrypts with ChaCha20 algorithm, checks integrity with Poly1305 algorithm and authenticates user with DHKE protocol. In short, SHE Cryptography completely satisfies the CIA triad of a security system.
 
-
 * **Faster Speed & Low Latency**: SHE is a stream cipher version of symmetric cryptography. As a result, it encrypts and decrypts the message instantaneously after doing XOR. It can calculate 128 bits and 256 bits easily or sometimes even larger. So, a user should not face any problem if he wants to communicate with others, or wants to download and upload a content.
 
-
 * **Power Loss Reduction**: CPU gets always hot for its cryptographic system, because this kind of system does massive mathematical computation. As a result, sometimes PSU (Power Supply Unit) could not supply such power that required to perform the task efficiently. So, overloading power causes the systems goes down sometimes or burns the CPU circuit. But the lightweight architecture of SHE, it requires less power to perform its mathematical computation and reduce power loss problems.
 
 --------------------------------
 **Ideal Applications To Use**
 --------------------------------
 * **Low Power Electronics**: Networking devices like PAN, LAN, WAN devices can use this system easily. Not only Mobile but also Watches can use this cryptography efficiently. However, technology like IOT which is one of the most booming electronics nowadays, is also a less power consumption tech product. As a result, it must need lightweight cryptography like SHE to perform securely, faster, and more efficiently without any interruption.
 
-
 * **Government and Business Communication**: SHE cryptography is applicable to sharing confidential data between government and business agents. This cryptography ensures the total CIA triad (Confidentiality, Integrity and Availability) of security. Also, SHE gives strong protection against malicious attacks (e.g. MITM Attack) because of its Diffie-Hellman key exchange protocol. So, this cryptography is reliable in government and business communication.
 
-
 * **Database Encryption**: In database systems, governments and organizations rely on vendors, but there is no guarantee that the data is protected. SHE can be implemented to store data into ciphertext with the DHKE protocol. As a result, any unauthorized person or third party organization won’t be able to use our confidential data unethically.
 
-
 * **Banking**: Many online banking and payment applications require the verification of personally identifiable information before proceeding with their transactions. It helps in predicting the correct information to prevent fraudulent activities and cybercrime. This is where SHE can easily authenticate users in the money transaction system, such as credit or debit card transactions or online banking sessions.
 
 ----------------------------
 **Installation**
 ----------------------------
 To install this project in your local server -
 
-`pip install sheCry`
+```bash
+pip install sheCry
+```
 
 ----------------------------
 **Program Utilization**
 ----------------------------
 * A user inputs the length of private keys and generated shared keys.
 * A user inputs message.
 * Generates prime number according to Fermat Prime Number Theorem.
@@ -85,8 +80,8 @@
 * Anyone can use this cryptography for free only for education, research, and further development purpose.
 
 --------------------------------
 **Do You Want To Know Me?**
 --------------------------------
 * **Call**: +8801818832925
 * **Email**: tahsin.ahmed@g.bracu.ac.bd
-* **Social Media**: <a href="https://www.facebook.com/ahmedinsider"> Facebook </a>
+* **Social Media**: https://www.facebook.com/ahmedinsider
```

### Comparing `sheCry-0.0.4/README.md` & `sheCry-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,46 +13,41 @@
 Nowadays, security has become one of the most burning and sensitive issues. Confidential data is being stolen by malicious attackers rapidly. To prevent this kind of act, many security measures have been established. But “Cryptography” plays the most crucial part when we call for security. This is so because cryptography is used to protect enterprise information and communication from cyber threats through the use of codes. For example, AES and RSA are the gold standards. They are very popular and still vastly used in many renowned organizations as well as in the government. But the drawback is, AES is hardware and software dependent. So, we need to design it according to hardware and software systems. As a result, this implementation increases time and cost. Also, the attacker uses a “Side Channel Attack” to break AES. As a result, it becomes vulnerable. AES performs great in 256 bits keys and is faster in powerful devices. But if it is used in a low computational powered device then we have to use fewer bits (e.g. 64 bits), or the device could not handle the calculation of larger numbers. Thus, AES performs badly in this criterion. If we use fewer bits in AES, then a “Correlation Power Analysis Attack” is possible. So, it is not worth using AES in low computational powered devices. Whereas, RSA is slow due to its large mathematical calculation with large numbers and asymmetric mechanism. As a result, RSA fails to perform in terms of speed and low computational power. Also, the world is switching to lightweight technology day by day. IOT is the best example of it. But to secure those less powerful electronics, there is no such effective cryptographic system yet. Also, breaching the confidential data of the government and the corporate world is a very old topic and it still remains a rapid concern. So, we really need to innovate a new cryptographic algorithm that gives better results in low-power electronics and performs faster, and gives better security in sharing data. This is where lightweight cryptography SHE comes to play.
 
 ----------------------------
 **Solution Statement**
 ----------------------------
 * **Environment Independency:** SHE is reliable on any platform weather it is for software or hardware. So, developer does not need to hassle with cryptographic system while designing a software or hardware. Thus, it decreases a developer's production time as well.
 
-
 * **Cost Effectiveness**: In 2007, about 10% of the average IT budget was spent on energy, and energy costs for IT were expected to rise to 50% by 2010. However, the cost of power supply generally depends on the maximum possible power that could be used at any one time. If a CPU needs to calculate a larger number for a cryptographical system, it needs more power and more efficiency to compute in a very short time. As a result, this increases costs most of the time. To reduce cost, many electronic products choose to use a much lighter system. This is where the SHE cryptographic system plays a major role. It reduces the clock rate when it processes large numbers of cryptographical computations. Thus, it reduces cost.
 
-
 * **Better Security**: No doubt SHE gives better security. It encrypts and decrypts with ChaCha20 algorithm, checks integrity with Poly1305 algorithm and authenticates user with DHKE protocol. In short, SHE Cryptography completely satisfies the CIA triad of a security system.
 
-
 * **Faster Speed & Low Latency**: SHE is a stream cipher version of symmetric cryptography. As a result, it encrypts and decrypts the message instantaneously after doing XOR. It can calculate 128 bits and 256 bits easily or sometimes even larger. So, a user should not face any problem if he wants to communicate with others, or wants to download and upload a content.
 
-
 * **Power Loss Reduction**: CPU gets always hot for its cryptographic system, because this kind of system does massive mathematical computation. As a result, sometimes PSU (Power Supply Unit) could not supply such power that required to perform the task efficiently. So, overloading power causes the systems goes down sometimes or burns the CPU circuit. But the lightweight architecture of SHE, it requires less power to perform its mathematical computation and reduce power loss problems.
 
 --------------------------------
 **Ideal Applications To Use**
 --------------------------------
 * **Low Power Electronics**: Networking devices like PAN, LAN, WAN devices can use this system easily. Not only Mobile but also Watches can use this cryptography efficiently. However, technology like IOT which is one of the most booming electronics nowadays, is also a less power consumption tech product. As a result, it must need lightweight cryptography like SHE to perform securely, faster, and more efficiently without any interruption.
 
-
 * **Government and Business Communication**: SHE cryptography is applicable to sharing confidential data between government and business agents. This cryptography ensures the total CIA triad (Confidentiality, Integrity and Availability) of security. Also, SHE gives strong protection against malicious attacks (e.g. MITM Attack) because of its Diffie-Hellman key exchange protocol. So, this cryptography is reliable in government and business communication.
 
-
 * **Database Encryption**: In database systems, governments and organizations rely on vendors, but there is no guarantee that the data is protected. SHE can be implemented to store data into ciphertext with the DHKE protocol. As a result, any unauthorized person or third party organization won’t be able to use our confidential data unethically.
 
-
 * **Banking**: Many online banking and payment applications require the verification of personally identifiable information before proceeding with their transactions. It helps in predicting the correct information to prevent fraudulent activities and cybercrime. This is where SHE can easily authenticate users in the money transaction system, such as credit or debit card transactions or online banking sessions.
 
 ----------------------------
 **Installation**
 ----------------------------
 To install this project in your local server -
 
-`pip install sheCry`
+```bash
+pip install sheCry
+```
 
 ----------------------------
 **Program Utilization**
 ----------------------------
 * A user inputs the length of private keys and generated shared keys.
 * A user inputs message.
 * Generates prime number according to Fermat Prime Number Theorem.
@@ -70,8 +65,8 @@
 * Anyone can use this cryptography for free only for education, research, and further development purpose.
 
 --------------------------------
 **Do You Want To Know Me?**
 --------------------------------
 * **Call**: +8801818832925
 * **Email**: tahsin.ahmed@g.bracu.ac.bd
-* **Social Media**: <a href="https://www.facebook.com/ahmedinsider"> Facebook </a>
+* **Social Media**: https://www.facebook.com/ahmedinsider
```

### Comparing `sheCry-0.0.4/setup.py` & `sheCry-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "sheCry",
 
-    version = "0.0.4",
+    version = "0.0.5",
     
     author = "Tahsin Ahmed",
 
     description = "SHE Cryptography is architectured by Tahsin Ahmed.",
 
     long_description = open("README.md", encoding="utf-8").read(),
```

### Comparing `sheCry-0.0.4/sheCry.egg-info/PKG-INFO` & `sheCry-0.0.5/sheCry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheCry
-Version: 0.0.4
+Version: 0.0.5
 Summary: SHE Cryptography is architectured by Tahsin Ahmed.
 Home-page: 
 Author: Tahsin Ahmed
 Keywords: cryptography,encryption,decryption,SHE,SHE cryptography,Symmetric Hybrid Encryption,Symmetric Hybrid Encryption cryptography,sheCry
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
@@ -28,46 +28,41 @@
 Nowadays, security has become one of the most burning and sensitive issues. Confidential data is being stolen by malicious attackers rapidly. To prevent this kind of act, many security measures have been established. But “Cryptography” plays the most crucial part when we call for security. This is so because cryptography is used to protect enterprise information and communication from cyber threats through the use of codes. For example, AES and RSA are the gold standards. They are very popular and still vastly used in many renowned organizations as well as in the government. But the drawback is, AES is hardware and software dependent. So, we need to design it according to hardware and software systems. As a result, this implementation increases time and cost. Also, the attacker uses a “Side Channel Attack” to break AES. As a result, it becomes vulnerable. AES performs great in 256 bits keys and is faster in powerful devices. But if it is used in a low computational powered device then we have to use fewer bits (e.g. 64 bits), or the device could not handle the calculation of larger numbers. Thus, AES performs badly in this criterion. If we use fewer bits in AES, then a “Correlation Power Analysis Attack” is possible. So, it is not worth using AES in low computational powered devices. Whereas, RSA is slow due to its large mathematical calculation with large numbers and asymmetric mechanism. As a result, RSA fails to perform in terms of speed and low computational power. Also, the world is switching to lightweight technology day by day. IOT is the best example of it. But to secure those less powerful electronics, there is no such effective cryptographic system yet. Also, breaching the confidential data of the government and the corporate world is a very old topic and it still remains a rapid concern. So, we really need to innovate a new cryptographic algorithm that gives better results in low-power electronics and performs faster, and gives better security in sharing data. This is where lightweight cryptography SHE comes to play.
 
 ----------------------------
 **Solution Statement**
 ----------------------------
 * **Environment Independency:** SHE is reliable on any platform weather it is for software or hardware. So, developer does not need to hassle with cryptographic system while designing a software or hardware. Thus, it decreases a developer's production time as well.
 
-
 * **Cost Effectiveness**: In 2007, about 10% of the average IT budget was spent on energy, and energy costs for IT were expected to rise to 50% by 2010. However, the cost of power supply generally depends on the maximum possible power that could be used at any one time. If a CPU needs to calculate a larger number for a cryptographical system, it needs more power and more efficiency to compute in a very short time. As a result, this increases costs most of the time. To reduce cost, many electronic products choose to use a much lighter system. This is where the SHE cryptographic system plays a major role. It reduces the clock rate when it processes large numbers of cryptographical computations. Thus, it reduces cost.
 
-
 * **Better Security**: No doubt SHE gives better security. It encrypts and decrypts with ChaCha20 algorithm, checks integrity with Poly1305 algorithm and authenticates user with DHKE protocol. In short, SHE Cryptography completely satisfies the CIA triad of a security system.
 
-
 * **Faster Speed & Low Latency**: SHE is a stream cipher version of symmetric cryptography. As a result, it encrypts and decrypts the message instantaneously after doing XOR. It can calculate 128 bits and 256 bits easily or sometimes even larger. So, a user should not face any problem if he wants to communicate with others, or wants to download and upload a content.
 
-
 * **Power Loss Reduction**: CPU gets always hot for its cryptographic system, because this kind of system does massive mathematical computation. As a result, sometimes PSU (Power Supply Unit) could not supply such power that required to perform the task efficiently. So, overloading power causes the systems goes down sometimes or burns the CPU circuit. But the lightweight architecture of SHE, it requires less power to perform its mathematical computation and reduce power loss problems.
 
 --------------------------------
 **Ideal Applications To Use**
 --------------------------------
 * **Low Power Electronics**: Networking devices like PAN, LAN, WAN devices can use this system easily. Not only Mobile but also Watches can use this cryptography efficiently. However, technology like IOT which is one of the most booming electronics nowadays, is also a less power consumption tech product. As a result, it must need lightweight cryptography like SHE to perform securely, faster, and more efficiently without any interruption.
 
-
 * **Government and Business Communication**: SHE cryptography is applicable to sharing confidential data between government and business agents. This cryptography ensures the total CIA triad (Confidentiality, Integrity and Availability) of security. Also, SHE gives strong protection against malicious attacks (e.g. MITM Attack) because of its Diffie-Hellman key exchange protocol. So, this cryptography is reliable in government and business communication.
 
-
 * **Database Encryption**: In database systems, governments and organizations rely on vendors, but there is no guarantee that the data is protected. SHE can be implemented to store data into ciphertext with the DHKE protocol. As a result, any unauthorized person or third party organization won’t be able to use our confidential data unethically.
 
-
 * **Banking**: Many online banking and payment applications require the verification of personally identifiable information before proceeding with their transactions. It helps in predicting the correct information to prevent fraudulent activities and cybercrime. This is where SHE can easily authenticate users in the money transaction system, such as credit or debit card transactions or online banking sessions.
 
 ----------------------------
 **Installation**
 ----------------------------
 To install this project in your local server -
 
-`pip install sheCry`
+```bash
+pip install sheCry
+```
 
 ----------------------------
 **Program Utilization**
 ----------------------------
 * A user inputs the length of private keys and generated shared keys.
 * A user inputs message.
 * Generates prime number according to Fermat Prime Number Theorem.
@@ -85,8 +80,8 @@
 * Anyone can use this cryptography for free only for education, research, and further development purpose.
 
 --------------------------------
 **Do You Want To Know Me?**
 --------------------------------
 * **Call**: +8801818832925
 * **Email**: tahsin.ahmed@g.bracu.ac.bd
-* **Social Media**: <a href="https://www.facebook.com/ahmedinsider"> Facebook </a>
+* **Social Media**: https://www.facebook.com/ahmedinsider
```

