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

![Screenshot 2025-04-24 184513](https://github.com/user-attachments/assets/9115db74-8537-42d1-a18d-7a244d3eb9c3)


From here, we are going to use 4vcpus
-Usename: Labuser / password: Cybersecurity1 -> 
-check eligibility license on the bottom left, 
-review and create!

![Screenshot 2025-04-23 210116](https://github.com/user-attachments/assets/1a1001d5-f603-47fd-a368-1f2191173203)

We are now going to deploy our Virtual machine and login through remote desktop (RDP). To do this we will extract public IP address from the VM and enter the credentials we made earlier.

![Screenshot 2025-04-24 184720](https://github.com/user-attachments/assets/ffa860b8-a80c-4c03-a39b-78ed5ccd8666)

Within the VM (osticket-vm), download the osTicket-Installation-Files.zip and unzip it onto your desktop. The folder should be called “osTicket-Installation-Files”
We will use the files in this folder to install osTicket and some of the dependencies.

![Annotation 2025-04-25 013829](https://github.com/user-attachments/assets/c95beeb2-c2db-4852-a70c-5f8c149f676f)

From here were going to enable IIS (internet information services) to do this, control panel -> programs -> programs and features >turn windows features on or off. Once clicked we are going to select IIS / world wide web services / applicaiton development features / CGI

![iis2025-04-25 022025](https://github.com/user-attachments/assets/2b2abce2-9a55-4838-b76c-ec41b64fa2a5)

Now we are going to install “osTicket-Installation-Files” folder, install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)

![php install 2025-04-25 020054](https://github.com/user-attachments/assets/193e2382-10ca-4638-8a40-9626b598db6b)

From the “osTicket-Installation-Files” folder install the Rewrite Module (rewrite_amd64_en-US.msi)

![Annotation 2025-04-25 020335](https://github.com/user-attachments/assets/269678e9-f110-4476-b301-d25917d942da)

Now from here were going to create the directory C:\PHP

![Annotation 2025-04-25 020805](https://github.com/user-attachments/assets/0b0dd6bc-a1c7-4644-b2af-a536cfa59e90)

From the “osTicket-Installation-Files” folder, unzip PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into the “C:\PHP” folder

![Annotation 2025-04-25 021003](https://github.com/user-attachments/assets/a9053efb-3df1-4498-998f-4a671294663d)

Next we will install "VC_redist.x86.exe." from the osTicket installation.

![Annotation 2025-04-25 021125](https://github.com/user-attachments/assets/509c023e-6d60-4bd1-837e-51d668a356c7)

We will now install  MySQL 5.5.62 (mysql-5.5.62-win32.msi) from the same folder. Make sure to click standard configuration and when asked for the username and password the credentials will be: username: root / password: root (make sure you do not mess this part up).

![Annotation 2025-04-25 021227](https://github.com/user-attachments/assets/7a838788-43f2-4bf8-b12b-aa83a30aefa0)

After this is completed, run IIS manager as an administrator and register the PHP from within the IIS. Once this step is completed we will "restart" it in the IIS manager.

![Annotation 2025-04-25 022417](https://github.com/user-attachments/assets/18cd5872-4fd3-4412-86c2-cf1c46e433a7)



