# Cyber-Kill-Chain

Created a payload using msfvenom. (Weaponization) 
<img width="1440" alt="Createpayload" src="https://github.com/colejam/Network-Traffic-Analysis/assets/163930716/3ba5228a-7070-4a5d-be1c-b93c627fb837">


Apache2 webpage to host the payload for the victim to access. (Delivery)
<img width="1440" alt="Apache2" src="https://github.com/colejam/Network-Traffic-Analysis/assets/163930716/5ce5b075-3770-488a-a8ab-9711d1ffa950">



The webpage was vulnerable, allowing the attacker to exploit it. (Exploitation) The Windows 10 victim machine accesses the webpage and installs the executable file. (Installation)
<img width="1440" alt="Victimmachine" src="https://github.com/colejam/Network-Traffic-Analysis/assets/163930716/70b37117-95be-49c2-819f-272f8d8b24b9">

Created a reverse tcp shell to establish a connection with the victim machine. (C2) Used whoami to display the username of the current user who is logged into the system. (Action and Objective)
<img width="1440" alt="Meterpreter" src="https://github.com/colejam/Network-Traffic-Analysis/assets/163930716/104b69fb-4d51-40ec-a86a-421db0ad0a05">



Took the Windows Event Viewer log file and uploaded it to VirusTotal to check for malicious files.
![Virustotal](https://github.com/colejam/Network-Traffic-Analysis/assets/163930716/3a98a8dd-a3dd-401f-bd8e-6b48d206b89d)


Wireshark to investigate the http traffic. I then followed the HTTP stream and found the
Safe.exe fill that was transmitted over the network to the victim machine. It displayed the file,
user agent, and the IP address of the attacking machine.

<img width="468" alt="image" src="https://github.com/colejam/Network-Traffic-Analysis/assets/163930716/fe5e1355-370f-434b-b224-f102a3ab8f2f">
