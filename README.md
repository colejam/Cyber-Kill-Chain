# Network-Traffic-Analysis

* **Weaponization**: Created a malicious payload using msfvenom to create a reverse TCP shell payload.
* **Delivery**: The payload was hosted on a webpage using Apache2, enabling the victim machine to download it.
* **Exploitation & Installation**: The victim accessed the vulnerable webpage and installed the malicious executable.
* **Command & Control (C2)**: Once the executable was installed, I established a reverse TCP connection back to the attacker machine using a Meterpreter shell.
* **Actions & Objectives**: I then used the whoami command to confirm the victim's user credentials.
* **VirusTotal Analysis**: I extracted a Windows Event Viewer log from the victim machine and uploaded it to VirusTotal to check for any malicious indicators in the files.
* **Network Traffic Analysis**: Utilized Wireshark to monitor HTTP traffic and followed the HTTP stream. In this stream, I identified the transmission of the payload file (Safe.exe) to the victim machine, including details like the file, user agent, and IP address of the attacker machine.

<img width="1440" alt="Createpayload" src="https://github.com/colejam/Network-Traffic-Analysis/assets/163930716/3ba5228a-7070-4a5d-be1c-b93c627fb837">



<img width="1440" alt="Apache2" src="https://github.com/colejam/Network-Traffic-Analysis/assets/163930716/5ce5b075-3770-488a-a8ab-9711d1ffa950">




<img width="1440" alt="Victimmachine" src="https://github.com/colejam/Network-Traffic-Analysis/assets/163930716/70b37117-95be-49c2-819f-272f8d8b24b9">


<img width="1440" alt="Meterpreter" src="https://github.com/colejam/Network-Traffic-Analysis/assets/163930716/104b69fb-4d51-40ec-a86a-421db0ad0a05">



![Virustotal](https://github.com/colejam/Network-Traffic-Analysis/assets/163930716/3a98a8dd-a3dd-401f-bd8e-6b48d206b89d)



<img width="468" alt="image" src="https://github.com/colejam/Network-Traffic-Analysis/assets/163930716/fe5e1355-370f-434b-b224-f102a3ab8f2f">
