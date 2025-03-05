<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://youtu.be/uGysc4upuX0?si=Gstctb-qhEmDrVLl)

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

- Install Wireshark
- Ping second Virtual machine using Powershell
- Observe Icmp Packet traffic
- Observe ssh packet traffic

<h2>Actions and Observations</h2>

![Vmlab9](https://github.com/user-attachments/assets/0b175c8f-3a41-40e4-9d93-c5eb0e3f85d8)


<p>
<img src="" height="80%" width="80%" alt="Ping Success"/>
</p>
<p>
Using Windows Powershell, Pinged second virtual machine with successful results.
</p>
<br />

![Vmlab18](https://github.com/user-attachments/assets/96768f38-7618-445d-a86f-b81e500335b5)


<p>
<img src="" height="80%" width="80%" alt="Observing DHCP traffic"/>
</p>
<p>
Using Wireshark, filter for DHCP traffic. Upon running ipconfig /renew, the DHCP traffic will appear.
</p>
<br />

![Vmlab19](https://github.com/user-attachments/assets/96e12cb3-6c20-4683-a884-880dc229c53f)


<p>
<img src="" height="80%" width="80%" alt="Observing DNS Traffic"/>
</p>
<p>
Using wireshark, to filter for DNS traffic only, use your windows 10 pc to run nslookup. Look up an IP address and the DNS traffic will appear in wireshark.
</p>
<br />

![vmlab20](https://github.com/user-attachments/assets/47429463-788e-4a10-8e36-50178617c84f)


<p>
<img src="" height="80%" width="80%" alt="Observing RDP Traffic"/>
</p>
<p>
In Wireshark. filter for RDP traffic only. The traffic should be non-stop as RDP traffic is constant.
</p>
<br />
