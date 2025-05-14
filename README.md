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
<p>
  <img src="https://imgur.com/JPFRNYh.png" height="80%" width="80%" alt="Azure VM Setup"/>
</p>

<p><strong>Step 2:</strong> Download and unzip the osTicket Installation Files to the desktop.</p>
<p>
  <img src="https://imgur.com/Lvv6deU.png" height="80%" width="80%" alt="Download osTicket"/>
</p>

<p><strong>Step 3:</strong> Install/enable IIS with CGI enabled.</p>
<p>
  <img src="https://i.imgur.com/aiTDfNa.png" height="80%" width="80%" alt="Enable IIS"/>
</p>
<p>
  <img src="https://i.imgur.com/Y3U96Cq.png" height="80%" width="80%" alt="CGI Feature"/>
</p>

<p><strong>Step 4:</strong> Install PHP Manager for IIS.</p>
<p>
  <img src="https://i.imgur.com/Q8ZTRZ9.png" height="80%" width="80%" alt="PHP Manager"/>
</p>

<p><strong>Step 5:</strong> Create directory <code>C:\PHP</code>.</p>
<p>
  <img src="https://i.imgur.com/HnDcKy7.png" height="80%" width="80%" alt="Create PHP Directory"/>
</p>

<p><strong>Step 6:</strong> Unzip PHP and install VC_redist.x86.</p>
<p>
  <img src="https://i.imgur.com/P33mH0n.png" height="80%" width="80%" alt="Unzip PHP"/>
</p>
<p>
  <img src="https://i.imgur.com/SbiOQ8P.png" height="80%" width="80%" alt="Install VC Redist"/>
</p>

<p><strong>Step 7:</strong> Install MySQL and set root credentials.</p>
<p>
  <img src="https://i.imgur.com/OL038XQ.png" height="80%" width="80%" alt="Install MySQL"/>
</p>

<p><strong>Step 8:</strong> Open IIS as Admin and register PHP.</p>
<p>
  <img src="https://i.imgur.com/ODvFju4.png" height="80%" width="80%" alt="Register PHP in IIS"/>
</p>

<p><strong>Step 9:</strong> Unzip osTicket, move to IIS root, rename folder.</p>
<p>
  <img src="https://i.imgur.com/yRz3nQZ.png" height="80%" width="80%" alt="Unzip osTicket"/>
</p>
<p>
  <img src="https://imgur.com/3fe816bc-7ff9-4d81-9d6c-a2f3180d4696.png" height="80%" width="80%" alt="Move osTicket"/>
</p>
<p>
  <img src="https://i.imgur.com/yrb3c8f.png" height="80%" width="80%" alt="Rename osTicket Folder"/>
</p>
<p>
  <img src="https://i.imgur.com/0Bnf3aS.png" height="80%" width="80%" alt="osTicket Directory"/>
</p>
<p>
  <img src="https://i.imgur.com/jj8M3WX.png" height="80%" width="80%" alt="IIS Setup"/>
</p>
<p>
  <img src="https://i.imgur.com/xKRQG2r.png" height="80%" width="80%" alt="Permissions Setup"/>
</p>
<p>
  <img src="https://i.imgur.com/hbbVv1o.png" height="80%" width="80%" alt="IIS Folder Structure"/>
</p>

<p><strong>Step 10:</strong> (Image missing or not specified)</p>

<p><strong>Step 11:</strong> Browse osTicket site from IIS.</p>
<p>
  <img src="https://i.imgur.com/SNfYXZe.png" height="80%" width="80%" alt="Browse osTicket"/>
</p>
<p>
  <img src="https://i.imgur.com/7c60jb8.png" height="80%" width="80%" alt="osTicket Welcome"/>
</p>

<p><strong>Step 12:</strong> Enable required PHP extensions (imap, intl, opcache).</p>
<p>
  <img src="https://i.imgur.com/1QqLJCa.png" height="80%" width="80%" alt="Enable PHP Extensions"/>
</p>

<p><strong>Step 13:</strong> Refresh osTicket site and rename config file.</p>
<p>
  <img src="https://i.imgur.com/rzn1O0r.png" height="80%" width="80%" alt="Rename Config"/>
</p>
<p>
  <img src="https://i.imgur.com/X74UvNz.png" height="80%" width="80%" alt="Refresh osTicket"/>
</p>

<p><strong>Step 14:</strong> Assign file permissions to ost-config.php.</p>
<p>
  <img src="https://i.imgur.com/UWNBtqk.png" height="80%" width="80%" alt="Permissions 1"/>
</p>
<p>
  <img src="https://i.imgur.com/t7yzcCz.png" height="80%" width="80%" alt="Permissions 2"/>
</p>
<p>
  <img src="https://i.imgur.com/jcYkMoe.png" height="80%" width="80%" alt="Permissions 3"/>
</p>
<p>
  <img src="https://i.imgur.com/Dq2Wm5q.png" height="80%" width="80%" alt="Permissions 4"/>
</p>
<p>
  <img src="https://i.imgur.com/xhGzW9y.png" height="80%" width="80%" alt="Permissions 5"/>
</p>
<p>
  <img src="https://i.imgur.com/9sDdDua.png" height="80%" width="80%" alt="Permissions 6"/>
</p>
<p>
  <img src="https://i.imgur.com/4gDoxXU.png" height="80%" width="80%" alt="Permissions 7"/>
</p>
<p>
  <img src="https://i.imgur.com/6wQ6vyK.png" height="80%" width="80%" alt="Permissions 8"/>
</p>
<p>
  <img src="https://i.imgur.com/TGq3ahs.png" height="80%" width="80%" alt="Permissions 9"/>
</p>
<p>
  <img src="https://i.imgur.com/AZzbIYs.png" height="80%" width="80%" alt="Permissions 10"/>
</p>

<p><strong>Step 15:</strong> Continue browser setup with helpdesk name and default email.</p>
<p>
  <img src="https://i.imgur.com/IrbMD39.png" height="80%" width="80%" alt="Helpdesk Setup"/>
</p>

<p><strong>Step 16:</strong> Install HeidiSQL, create DB session, and install osTicket.</p>
<p>
  <img src="https://i.imgur.com/nJNCgsO.png" height="80%" width="80%" alt="HeidiSQL Setup"/>
</p>
<p>
  <img src="https://i.imgur.com/8zmGRjB.png" height="80%" width="80%" alt="osTicket DB Setup"/>
</p>
<p><strong>Step 17:</strong> Continue setting up osTicket in the browser.</p>
<p>
  MySQL Database: <code>osTicket</code><br/>
  MySQL Username: <code>root</code><br/>
  MySQL Password: <code>root</code><br/>
  Click “Install Now!”
</p>
<p>
  <img src="https://i.imgur.com/tAzLcJj.png" height="80%" width="80%" alt="osTicket MySQL Setup 1"/>
</p>
<p>
  <img src="https://i.imgur.com/b86fYyy.png" height="80%" width="80%" alt="osTicket MySQL Setup 2"/>
</p>
<p>
  <img src="https://i.imgur.com/em4Tx2f.png" height="80%" width="80%" alt="osTicket MySQL Setup 3"/>
</p>
