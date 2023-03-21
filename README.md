<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Created Domain Controller VM and Client VM (Domain Controller will host Active Directory)
- Changed the Domain Controllers private IP address to "Static"
- Allowed Domain Controller to receive connection from Client 
- Installed Acitve Direcory on Domain Controller
- Changed Client VM DNS server to Domain Controllers private IP address
- Added Client VM to the Active Directory 

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/l66FbNC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Inside Azure Microsoft, we changed the Domain Controller Virtual Machine's private IP address to "Static" in network configurations.
</p>
<br />

<p>
<img src="https://i.imgur.com/FrVWmNR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Inside Azure Microsoft, we changed the Client Virtual Machine's DNS server to the Domain Controller VM's private IP address, which now has Active Directory installed.
</p>
<br />

<p>
<img src="https://i.imgur.com/Noblzzl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We added our Client Virtual Machine to the Active Directory inside our Domain Controller VM.
</p>
<br />
