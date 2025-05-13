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

<!-- Step 1 -->
<p><strong>Step 1:</strong> Create a Windows 10 Azure VM and log in via Remote Desktop.</p>
<p align="center">
  <img src="https://i.imgur.com/step1img1.png" height="80%" width="80%" alt="Azure VM Setup"/>
</p>
<br />

<!-- Step 2 -->
<p><strong>Step 2:</strong> Download and unzip the osTicket Installation Files to the desktop.</p>
<p align="center">
  <img src="https://i.imgur.com/step2img1.png" height="80%" width="80%" alt="Download osTicket files"/>
</p>
<br />

<!-- Step 3 -->
<p><strong>Step 3:</strong> Install/enable IIS with CGI enabled.</p>
<p align="center">
  <img src="https://i.imgur.com/step3img1.png" height="80%" width="80%" alt="IIS Setup 1"/>
  <img src="https://i.imgur.com/step3img2.png" height="80%" width="80%" alt="IIS Setup 2"/>
</p>
<br />

<!-- Step 4 -->
<p><strong>Step 4:</strong> Install PHP Manager for IIS.</p>
<p align="center">
  <img src="https://i.imgur.com/step4img1.png" height="80%" width="80%" alt="PHP Manager Install"/>
</p>
<br />

<!-- Step 5 -->
<p><strong>Step 5:</strong> Create directory <code>C:\PHP</code>.</p>
<p align="center">
  <img src="https://i.imgur.com/step5img1.png" height="80%" width="80%" alt="Create PHP Directory"/>
</p>
<br />

<!-- Step 6 -->
<p><strong>Step 6:</strong> Unzip PHP and install VC_redist.x86.</p>
<p align="center">
  <img src="https://i.imgur.com/step6img1.png" height="80%" width="80%" alt="Unzip PHP"/>
  <img src="https://i.imgur.com/step6img2.png" height="80%" width="80%" alt="Install VC_redist"/>
</p>
<br />

<!-- Step 7 -->
<p><strong>Step 7:</strong> Install MySQL and set root credentials.</p>
<p align="center">
  <img src="https://i.imgur.com/step7img1.png" height="80%" width="80%" alt="MySQL Install"/>
</p>
<br />

<!-- Step 8 -->
<p><strong>Step 8:</strong> Open IIS as Admin and register PHP.</p>
<p align="center">
  <img src="https://i.imgur.com/step8img1.png" height="80%" width="80%" alt="Register PHP in IIS"/>
</p>
<br />

<!-- Step 9 -->
<p><strong>Step 9:</strong> Unzip osTicket, move to IIS root, rename folder.</p>
<p align="center">
  <img src="https://i.imgur.com/step9img1.png" height="80%" width="80%" alt="Unzip osTicket"/>
  <img src="https://i.imgur.com/step9img2.png" height="80%" width="80%" alt="Copy to wwwroot"/>
  <img src="https://i.imgur.com/step9img3.png" height="80%" width="80%" alt="Rename Folder"/>
  <img src="https://i.imgur.com/step9img4.png" height="80%" width="80%" alt="IIS View"/>
  <img src="https://i.imgur.com/step9img5.png" height="80%" width="80%" alt="Step 9 Screenshot 5"/>
  <img src="https://i.imgur.com/step9img6.png" height="80%" width="80%" alt="Step 9 Screenshot 6"/>
</p>
<br />

<!-- Step 10 -->
<p><strong>Step 10:</strong> Reload IIS.</p>
<p align="center">
  <img src="https://i.imgur.com/step10img1.png" height="80%" width="80%" alt="Reload IIS 1"/>
  <img src="https://i.imgur.com/step10img2.png" height="80%" width="80%" alt="Reload IIS 2"/>
</p>
<br />

<!-- Continue for Step 11–16 as needed, same format -->
