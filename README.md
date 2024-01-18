<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, I observed various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

https://imgur.com/a/i8JWet2

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Step 1: Created Virtual Machines in Azure.
- Step 2: Log in to Virtual Machine (VM1 with Windows 10 Pro setup) with remote desktop
- Step 3: Configure VM2 Firewall Protocols to disrupt inbound ICMP
- Step 4: Inspect various protocols with RDP (Remote Desktop Protocol) on Virtual Machine 1

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/vl0ei0K.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
For the first steps to this project I created two seperate virtual machines in Azure. One with a of set up of Windows 10 Pro and the other with Ubuntu Linix. Once the machines were set up, I was able to obtain the public IPv4 Address use remote desktop to log onto to VM1 (Virtual Machine 1 with Windows 10 setup).
</p>
<br />

<p>
<img src="https://i.imgur.com/uS67oUU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
