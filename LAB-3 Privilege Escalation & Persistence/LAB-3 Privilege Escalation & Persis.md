LAB-3: Privilege Escalation \& Persistence



\### 1. Objective



To understand Linux privilege escalation techniques and persistence mechanisms using industry-standard resources such as HackTricks, LinPEAS, and GTFOBins.



\### 2. Tools \& References Used



* HackTricks
* GTFOBins
* LinPEAS (study/reference)
* Kali Linux



\### 3. Privilege Escalation Analysis



Linux privilege escalation techniques were studied using HackTricks and GTFOBins. The find binary was analyzed using GTFOBins to understand how misconfigured SUID or sudo permissions can allow privilege escalation.



The GTFOBins documentation demonstrated how find can be abused under:



* Unprivileged context
* Sudo permissions
* SUID permissions



Relevant commands and explanations were reviewed and documented through screenshots.



\### 4. Persistence (Post-Exploitation)



Linux post-exploitation and persistence concepts were reviewed using HackTricks. Topics included:

* 
* Credential harvesting
* PAM backdooring concepts
* Environment variable abuse
* Post-exploitation techniques



No real persistence was deployed, as this lab focused on understanding concepts and documentation.



Conclusion



This lab provided practical understanding of Linux privilege escalation paths and post-exploitation persistence techniques. Proper documentation and analysis help identify misconfigurations that can lead to full system compromise.

