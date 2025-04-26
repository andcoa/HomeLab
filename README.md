# SOC Home Lab Setup

## Objective

This project outlines the process of building a SOC Home Lab. It covers the installation and configuration of virtual machines (VMs), setting up networking between VMs, and setting up Splunk and Sysmon for ingesting telemtry. The home lab is the foundation on which the other projects will be build and ran accordingly.

## Skills Learned

- Setting up and configuring virtual machines using VMware or VirtualBox.
- Configuring networking between multiple VMs to simulate real-world environments.
- Setting up Splunk and Sysmon for security event correlation.
- Understanding and applying cybersecurity attack techniques in a controlled environment.

## Tools Used

- VMware/VirtualBox: For creating and managing virtual machines.
- Windows 10, Kali Linux, Ubuntu: Operating systems used for attack and defense.
- Splunk: For centralized log management and analysis.
- Sysmon: For monitoring and generating detailed system telemetry.

Set up three Virtual Machines consisting of Kali Linux, Ubuntu, and Windows 10.

![image](https://github.com/user-attachments/assets/08835c28-8a1c-4f20-8572-f64a509fb51e)

Each machine is set up with the default NAT network settings, however they will be switched to the Internal Network and assigned static IPs to not put my host at risk when conducting Malware Analysis and Threat Hunting.

![image](https://github.com/user-attachments/assets/5b1fd014-4dda-4e98-91a4-727860b6518b)

Assigned a static IP to the Windows VM.

![image](https://github.com/user-attachments/assets/8ca81762-cdd5-461f-8369-eb6455bdc00e)

Assigned a static IP to the Kali VM.

![image](https://github.com/user-attachments/assets/e9e416e1-3cba-4f3d-a0e3-5cd46246191e)

Pinging the Kali VM from the Windows VM to check connectivity.

![image](https://github.com/user-attachments/assets/f48dfb1b-4047-4c6d-aa07-98d2da8c3cf4)


Setting up the Splunk Enterprise environment to intake logs from the Windows VM.

![image](https://github.com/user-attachments/assets/29d2a3e9-6bc8-4b62-aeb7-d22d7527e7e0)

Splunk is displaying logs from the Windows VM accordingly.

![image](https://github.com/user-attachments/assets/0db1cb81-58b6-4def-9d7d-c50c68da1b8f)

Used the following config file to set up Sysmon.

![image](https://github.com/user-attachments/assets/957cd6cc-be5c-4f65-a811-ecda2db08a3c)

Installed Sysmon using Powershell on the Windows VM with the Sysmon config above.

![image](https://github.com/user-attachments/assets/d8ead9f1-22c2-440c-a8a8-aaa96bff391a)

Confirming Sysmon was successfully installed.

![image](https://github.com/user-attachments/assets/82397391-b51a-4b2d-bf4f-4700f1202735)
![image](https://github.com/user-attachments/assets/de61a67b-ad5d-4ebc-a91e-2fdfdcc32413)








