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

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Item 1 Azure account
- Item 2 Web browser and internet
- Item 3 Payment method
- Item 4 Basic setup knowledege
- Item 5

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
sign in to the Azure portal. In the seach type "virtual machine" and select it and then click "create" > "Azure virtual machine" </p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure VM settings (subscription, resource group, Vm name, Region,Image,Authentication Type,Username,Password/SSH Key. When choosing Disks choose the OS disk type (eg.SSD) and Adjust for the disk size needed. For Networking select an existing vitual network or create your own , assign a public ip to it and configure a Network security group to allow neccesary orts like SSH or Linux. </p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Review and create: Review all your configurations, click "create" yo deploy the Vm, once the deploymeny is complete, click "go to resource" to acess your virtual machine </p>
<br />
