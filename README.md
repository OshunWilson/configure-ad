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

- Setup Resources in Azure
- Ensure Connectivity between the client and Domain Controller
- Install Active Directory
- Create an Admin and Normal User Account in AD
- Join Client-1 to your domain (mydomain.com)
- Setup Remote Desktop for non-administrative users on Client-1
- Create a bunch of additional users and attempt to log into client-1 with one of the users

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/SGnQyMq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Setup Resources In Azure by creating my VM Domain controller (Windows 10).
</p>
<br />

<p>
<img src="https://i.imgur.com/oaEpVLx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Ensure Connectivity between the Client & DC (Domain controller) by Remote Desktop into my VM and "Ping" with command

- Domain Controller is server/computer that has Active Directory installed in it.

</p>
<br />

<p>
<img src="https://i.imgur.com/8efUT9b.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Installed Active Directory.
</p>
<br />

<p>
<img src="https://i.imgur.com/w2hASI9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Promote as a DC (Domain Controller) by setting up a new forest.
</p>
<br />

<p>
<img src="https://i.imgur.com/PMWj9aV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create an Admin/Normal User Account In Active Directory.
</p>
<br />

<p>
<img src="https://i.imgur.com/PP3Y9My.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Joined Client 1 to domain.
</p>
<br />

<p>
<img src="https://i.imgur.com/Ik9FisW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the Azure Portal, I set Client-1’s DNS settings to the DC’s Private IP address.
  
  - DNS (Domain Name System) turns domain names into IP addresses
  
  - DC (Domain Controller)
  
</p>
<br />

<p>
<img src="https://i.imgur.com/vfoxY7i.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Setup Remote Desktop for non-administrative users on Client-1 VM.
</p>
<br />

<p>
<img src="https://i.imgur.com/4cZwKUB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Created a bunch of additional users.

</p>
<br />
