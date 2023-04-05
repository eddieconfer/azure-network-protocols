<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />



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

- I created two vm's in Microsoft Azure. One vm was running Windows 10 and the other vm was running Linux (Ubuntu).
- I had the Windows 10 vm constantly ping the Linux vm using ping -t.
- I used Wireshark to show ICMP traffic.
- I then used Wireshark to observe other types of traffic including SSH, DHCP, DNS,and RDP.

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/kiztAGW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Using Wireshark I watched ICMP traffic between the two vms'.
</p>
<br />

<p>
<img src="https://i.imgur.com/erw50IE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I then denied ICMP traffic using the firewall on Microsft Azure.
</p>
<br />

<p>
<img src="https://i.imgur.com/rT6K2OZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Finally, I observed SSH traffic between the two vms' using Wireshark.
</p>
<br />
