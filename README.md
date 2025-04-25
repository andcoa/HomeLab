# SOC Home Lab Setup

Set up three Virtual Machines consisting of Kali Linux, Ubuntu, and Windows 10.

![image](https://github.com/user-attachments/assets/08835c28-8a1c-4f20-8572-f64a509fb51e)

Each machine is set up with the default NAT network settings, however they will be switched to the Internal Network and assigned static IPs to not put my host at risk when conducting Malware Analysis and Threat Hunting.

![image](https://github.com/user-attachments/assets/9fe046f2-784b-436b-ab09-12471447aae5)


Setting up the Splunk Enterprise environment to intake logs from the Windows Virtual Machine.

![image](https://github.com/user-attachments/assets/29d2a3e9-6bc8-4b62-aeb7-d22d7527e7e0)

Splunk is displaying logs from the Windows VM accordingly.

![image](https://github.com/user-attachments/assets/0db1cb81-58b6-4def-9d7d-c50c68da1b8f)

Used the following config file to set up Sysmon.

![image](https://github.com/user-attachments/assets/957cd6cc-be5c-4f65-a811-ecda2db08a3c)

Installed Sysmon using Powershell on the Windows VM with the Sysmon config above.

![image](https://github.com/user-attachments/assets/d8ead9f1-22c2-440c-a8a8-aaa96bff391a)

Confirming Sysmon was succesfully installed.

![image](https://github.com/user-attachments/assets/82397391-b51a-4b2d-bf4f-4700f1202735)
![image](https://github.com/user-attachments/assets/de61a67b-ad5d-4ebc-a91e-2fdfdcc32413)








