<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This project outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Preparing Active Directory Infrastrcture in Azure
- Deploying Active Directory
- Creating Users with Powershell
- Group policies and Managing accounts

<h2>Deployment and Configuration Steps</h2>

<h2>1. Preparing Active Directory Infrastrcture in Azure</h2>
<p>
<img src="https://i.imgur.com/l4ASQyo.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/VFAiVL2.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
For this project, similar to the osTicket project, I used Microsoft Azure to create a resource group and vnet, however this time I created two virtual machines, one of them will act as a domain controller and named "dc-1" I then disable firewall so that traffic between the vms is not disrupted. The second vm will be a normal windows 10 computer in the smae region as the domain controller. I test the connection using powershell to ping the domain controller to make sure everything is prepared for further testing.
</p>
<br />

<h2>2. Deploying Active Directory</h2>
<p>
<img src="https://i.imgur.com/ojo4GUs.png" height="45%" width="45%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/2pfhuEd.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/Pe2DBil.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Dc-1 is promoted to a domain controller with a new forest. New OUs(organizational units) are created for employees and admins. Client 1 is joined to the domain. To simulate a large organization of users, a script is used to create 10000 new users taht are all given permission to log into the windows virtual machine.
</p>
<br />

<h2>3. Creating Users with Powershell</h2>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<h2>4. Group policies and Managing accounts</h2>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
