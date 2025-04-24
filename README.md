<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b>

<h2>List of Prerequisites</h2>

- Azure Virtual Machines
- Remote desktop
- osTicket installation files
- HeidiSQL

<h2>Installation Steps</h2>

Hi there and welcome to my in-depth tutorial on how to build a ticketing system with osTicket! To being first we are going to create a virtual machine through Microsoft Azure's portal and we will proceed to create a virutal machine. We will name the VM "osTicket-Vm". Then we will select our image which will be Windows 10 pro, version 22H2 - x64 Gen2.


From here, we are going to use 4vcpus
-Usename: Labuser / password: Cybersecurity1 -> 
-check eligibility license on the bottom left, 
-review and create!

![Screenshot 2025-04-23 210116](https://github.com/user-attachments/assets/1a1001d5-f603-47fd-a368-1f2191173203)

We are now going to deploy our Virtual machine and login through remote desktop (windows). To do this we will extract public IP address from the VM and enter the credentials we made earlier.

![Screenshot 2025-04-23 210657](https://github.com/user-attachments/assets/bcc5e339-a69b-46cb-b6a0-b7102b7ce9f0)

Within the VM (osticket-vm), download the osTicket-Installation-Files.zip and unzip it onto your desktop. The folder should be called “osTicket-Installation-Files”
We will use the files in this folder to install osTicket and some of the dependencies.

















<p>
<img src="https://imgur.com/a/964ZeUH" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
