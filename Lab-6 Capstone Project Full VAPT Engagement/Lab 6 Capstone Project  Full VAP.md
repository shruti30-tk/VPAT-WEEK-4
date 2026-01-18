\# Lab 6: Capstone Project – Full VAPT Engagement



\### 1. Objective



Simulate a complete Vulnerability Assessment and Penetration Testing (VAPT) engagement following PTES methodology, including reconnaissance, exploitation, remediation, and reporting.





\### 2. Tools Used



* Kali Linux 
* Metasploit Framework  
* OpenVAS  
* Burp Suite  





\### 3. Target Environment



* Target VM: Hack The Box – Lame  
* Attack Type:Remote Code Execution (RCE)  





\### 4. Exploitation



\##1.Metasploit Module Used: exploit/unix/ftp/vsftpd\_234\_backdoor





\##2.Attack Log



| Timestamp           | Target IP      | Vulnerability | PTES Phase   |

|---------------------|--------------- |---------------|--------------|

| 2025-08-30 15:00:00 | 192.168.187.136| VSFTPD RCE    | Exploitation |







\### 5. Remediation

\- Patch vulnerable FTP service  

\- Apply least privilege principle  

\- Implement input validation  

\- Disable unnecessary services  

\- Re-scan with OpenVAS  







