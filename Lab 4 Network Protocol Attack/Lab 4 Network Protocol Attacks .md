\# Lab 4: Network Protocol Attacks (MITM)



\### 1. Objective



To understand and perform Man-in-the-Middle (MITM) attacks by exploiting insecure network protocols and capturing sensitive authentication data.





\### 2. Tools Used



* &nbsp;Responder
* Ettercap
* Wireshark
* &nbsp;TryHackMe AttackBox





\### 3. Concepts Covered



* &nbsp;ARP Spoofing
* &nbsp;SMB Relay Attack
* &nbsp;NTLM Hash Capture
* &nbsp;Network Traffic Analysis





\### 4. Tasks Performed



* &nbsp;Performed ARP spoofing using Ettercap
* &nbsp;Captured NTLM authentication hashes using Responder
* &nbsp;Analyzed intercepted traffic using Wireshark
* &nbsp;Observed SMB and authentication-based attacks



\### 5. Attack Simulation Log



| Attack ID| Technique | Target IP       | Status  | Result      |

|----------|-----------|-----------------|---------|-------------|

| 015      | SMB Relay | 192.168.1.200   | Success | NTLM Hash   |



\### 6. MITM Summary



A Man-in-the-Middle attack was performed by spoofing ARP traffic between the victim and gateway. Responder was used to capture NTLM hashes during authentication. Wireshark helped analyze SMB traffic, highlighting risks associated with unsecured network protocols.





