<img align="right" src="img/homelab.jpg" width="250">  Ansible managed homelab
==================

Playbooks, inventories and config files used with Ansible to manage my small homelab.
This is still ongoing project and currently I'm waiting for more equipment to expand my network. 
Currently all services are running on multiple Raspberry Pi devices:
  - Honeypot
  - Network-Attached Storage
  - Web server
  - CTF lab
More about them:
<br clear="tight"/>
------------


- Honeypot (RPi Zero 2)		- Ubuntu server connected to Internet to catch common and automated scans or indicators of compromise. Runs listener that spoof signatures and keeps open ports for FTP, SSH, Telnet, VNC, RDP protocols.
  
![ports](img/honey3.jpg?raw=true "open ports")

Configured PSAD and Snort in IDS mode, logs any attacks attempts, while Splunk forwarder sends logs to indexer hosted on my PC.
On average, honeypot detects approximately 20000 malicious activities per day with SSH password spraying attack on the lead. Most attacks come from China, United Kingdom and India.
![events1](img/honey1.jpg?raw=true "events1")
![events2](img/honey2.jpg?raw=true "events2")

------------


- NAS (RPi 3B) 		- Hosting ownCloud as private network-attached storage server, accessible within my local network. 

![nas](img/nas.jpg?raw=true "nas")

------------

tbd...
