# Onyx-Ransomware
**Detection Names**
Avast (Win32:RansomX-gen [Ransom]), Combo Cleaner (IL:Trojan.MSILZilla.5554), ESET-NOD32 (A Variant Of MSIL/Filecoder.AGP), Kaspersky (HEUR:Trojan-Ransom.MSIL.Agent.gen), Microsoft (Ransom:MSIL/FileCoder.AD!MTB), 

**MD5**: cf6ff9e0403b8d89e42ae54701026c1f
**SHA256**: a7f09cfde433f3d47fc96502bf2b623ae5e7626da85d0a0130dcd19d1679af9b

**Reference:
1	https://www.pcrisk.com/removal-guides/23698-onyx-ransomware
2	https://www.bleepingcomputer.com/news/security/beware-onyx-ransomware-destroys-files-instead-of-encrypting-them/
3	https://www.tutorialjinni.com/onyx-ransomware.html
4	https://blog.malwarebytes.com/ransomware/2022/04/onyx-ransomware-destroys-files-and-also-the-criminal-circle-of-trust/
5	https://www.theregister.com/2022/04/29/onyx-ransomware-destroy-files/
6	https://www.esecurityplanet.com/threats/onyx-ransomware-destroys-files/
7	https://itigic.com/onyx-ransomware-does-not-want-to-encrypt-your-files/

**RECOMMENDATIONS:**
1.	Create rules to detect and block IOCs mentioned above in applicable security solutions - SIEM, EDR, Firewall, Proxy, Email gateway etc. to secure the network.
2.	To eliminate possible malware infections, scan your computer with legitimate antivirus software.
3.	Avoid opening attachments presented in irrelevant emails. Users can be trained to identify social engineering techniques. URL inspection within email can also help detect links leading to known malicious sites.
4.	Download software using official websites or other reliable sources. Do not use third party downloaders or other dubious tools.
5.	Do not enable macros in document attachments received via emails. A lot of malware infections rely on the action to turn ON macros.
6.	For organizations, it is advised to restrict inbound SMB Version 1 and 2 communication between client systems to prevent malware from spreading from one machine to another within the local network.
7.	Turn on the network level authentication as it offers the strongest available method for authenticating RDP communications. Otherewise, credentials are sent in clear text to a remote host or domain controller.
8.	RDP connections and outbound traffic should be monitored rigorously for much better visibility. Monitor for suspicious network traffic that could be indicative of scanning, such as large quantities originating from a single source.
9.	Harden systems and applications: This complements the principle of least privilege and can involve configuration changes, removing unnecessary rights and access, closing ports, and more. This improves system and application security and helps prevent and mitigate the potential for bugs that leave vulnerability to injection of malicious code (i.e. SQL injections), buffer overflows, etc. or other backdoors that could allow privilege escalation.
10.	Maintain offline (i.e., physically disconnected) backups of data, and regularly test backup and

