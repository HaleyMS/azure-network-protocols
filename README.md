<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
For this project, I observed various network traffic to and from Azure Virtual Machines with Wireshark as well as experimenting with Network Security Groups. <br />


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
- Step 4: Inspect various protocols through Wireshare on Virtual Machine 1

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/vl0ei0K.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
For the first steps to this project I created two seperate virtual machines in Azure. One with a of set up of Windows 10 Pro and the other with Ubuntu Linix. Once the machines were set up, I was able to obtain the public IPv4 Address and use remote desktop to log onto to VM1 (Virtual Machine 1 with Windows 10 setup).
</p>
<br />

<p>
<img src="https://i.imgur.com/uS67oUU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once inside VM1 I was able to set up a perpetual ICMP (Internet Control Message Protocol) ping to VM2. After establishing the ICMP ping to VM2 I went to VM2's NSG and added a new rule that would deny any ICMP pings from anywhere. Checking back in to VM1 I noticed the ping had been disrupted by the firewall. With a sucessful denial I went back to VM2 to allow ICMP to come through. I was able to reestablish a connection from VM1 to VM2. 
</p>
<br />

<p>
<img src="https://i.imgur.com/5UXnEd0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Inside VM1 I was able to observe SSH (Secure Shell) protocol shown above.
</p>
<br />
<img src="https://i.imgur.com/OyHE9JL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Inside VM1 I was able to observe DHCP (Dynamic Host Configuration Protocol) protocol shown above.
</p>
<br />
<img src="https://i.imgur.com/eXWUKd0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Inside VM1 I was able to observe DNS (Domain Name System) protocol shown above.
</p>
<br />
<img src="https://i.imgur.com/aJ0Oq5T.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Inside VM1 I was able to observe Remote Desktop protocol shown above using TCP.PORT==3389.
</p>
<br />
