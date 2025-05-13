<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
<p>
  This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.
</p>

<h2>Video Demonstration</h2>
<ul>
  <li>### <a href="https://www.youtube.com">YouTube: How To Install osTicket with Prerequisites</a></li>
</ul>

<h2>Environments and Technologies Used</h2>
<ul>
  <li>Microsoft Azure (Virtual Machines/Compute)</li>
  <li>Remote Desktop</li>
  <li>Internet Information Services (IIS)</li>
</ul>

<h2>Operating Systems Used</h2>
<ul>
  <li>Windows 10 (21H2)</li>
</ul>

<h2>List of Prerequisites</h2>
<ul>
  <li>IIS with CGI enabled</li>
  <li>PHP Manager for IIS</li>
  <li>PHP 7.3.8 installed to C:\PHP</li>
  <li>MySQL 5.5.62 (root/root)</li>
  <li>VC_redist.x86</li>
</ul>

<h2>Installation Steps</h2>

<p><strong>Step 1:</strong> Create a Windows 10 Azure VM and log in via Remote Desktop.</p>
<p align="center">
  <img src="https://i.imgur.com/step1img1.png" alt="Azure VM Setup"/>
</p>

<p><strong>Step 2:</strong> Download and unzip the osTicket Installation Files to the desktop.</p>
<p align="center">
  <img src="https://i.imgur.com/step2img1.png" alt="Download osTicket files"/>
</p>

<p><strong>Step 3:</strong> Install/enable IIS with CGI enabled.</p>
<p align="center">
  <img src="https://i.imgur.com/step3img1.png" alt="IIS Setup 1"/>
</p>
<p align="center">
  <img src="https://i.imgur.com/step3img2.png" alt="IIS Setup 2"/>
</p>

<p><strong>Step 4:</strong> Install PHP Manager for IIS.</p>
<p align="center">
  <img src="https://i.imgur.com/step4img1.png" alt="PHP Manager Install"/>
</p>

<p><strong>Step 5:</strong> Create directory <code>C:\PHP</code>.</p>
<p align="center">
  <img src="https://i.imgur.com/step5img1.png" alt="Create PHP Directory"/>
</p>

<p><strong>Step 6:</strong> Unzip PHP and install VC_redist.x86.</p>
<p align="center">
  <img src="https://i.imgur.com/step6img1.png" alt="Unzip PHP"/>
</p>
<p align="center">
  <img src="https://i.imgur.com/step6img2.png" alt="Install VC_redist"/>
</p>

<p><strong>Step 7:</strong> Install MySQL and set root credentials.</p>
<p align="center">
  <img src="https://i.imgur.com/step7img1.png" alt="MySQL Install"/>
</p>

<p><strong>Step 8:</strong> Open IIS as Admin and register PHP.</p>
<p align="center">
  <img src="https://i.imgur.com/step8img1.png" alt="Register PHP in IIS"/>
</p>

<p><strong>Step 9:</strong> Unzip osTicket, move to IIS root, rename folder.</p>
<p align="center">
  <img src="https://i.imgur.com/step9img1.png" alt="Unzip osTicket"/>
</p>
<p align="center">
  <img src="https://i.imgur.com/step9img2.png" alt="Copy to wwwroot"/>
</p>
<p align="center">
  <img src="https://i.imgur.com/step9img3.png" alt="Rename Folder"/>
</p>
<p align="center">
  <img src="https://i.imgur.com/step9img4.png" alt="IIS View"/>
</p>
<p align="center">
  <img src="https://i.imgur.com/step9img5.png" alt="Step 9 Screenshot 5"/>
</p>
<p align="center">
  <img src="https://i.imgur.com/step9img6.png" alt="Step 9 Screenshot 6"/>
</p>

<p><strong>Step 10:</strong> Reload IIS.</p>
<p align="center">
  <img src="https://i.imgur.com/step10img1.png" alt="Reload IIS 1"/>
</p>
<p align="center">
  <img src="https://i.imgur.com/step10img2.png" alt="Reload IIS 2"/>
</p>

<!-- Continue same format for steps 11–16 -->
