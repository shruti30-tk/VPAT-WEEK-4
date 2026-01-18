\# Lab 5: Mobile Application Testing



\### 1. Objective



Perform security testing on Android applications using static analysis, dynamic analysis, and inter-process communication (IPC) testing to identify potential vulnerabilities.







\### 2. Tools Used



* MobSF – Static analysis of APKs  
* Frida – Dynamic function hooking and runtime instrumentation  
* Drozer – Android IPC and component testing  





\### 3. Activities



\## 1. Static Analysis (MobSF)



* &nbsp;Uploaded `test.apk` to MobSF  
* &nbsp;Analyzed app for insecure data storage and misconfigurations  





Vulnerability Log



| Test ID | Vulnerability     | Severity| Target App |

|---------|----------------- |----------|------------|

| 016     | Insecure Storage | High     | test.apk   |







\## 2. Dynamic Testing (Frida)



* &nbsp;Hooked authentication-related functions  
* Bypassed login validation at runtime  



Summary (50 words)



Frida was used to dynamically hook authentication functions and modify return values at runtime. This allowed bypassing login checks without valid credentials, highlighting weak client-side security and improper reliance on local authentication mechanisms.







\## 3. IPC Testing (Drozer)



* Enumerated exported activities and services  
* Tested permissions and IPC component security  





\### 4. Results 

* MobSF static analysis  
* Frida dynamic testing
* Drozer IPC testing 
