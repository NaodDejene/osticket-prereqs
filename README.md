<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
<p>
  This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.
</p>

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

<p><strong>Step 1:</strong> Create a Windows 10 Azure VM and log in to it via Remote Desktop.</p>
<p>
  <img src="https://imgur.com/JPFRNYh.png" height="80%" width="80%" alt="Azure VM Setup"/>
</p>

<p><strong>Step 2:</strong> Download and unzip the osTicket Installation Files to your desktop.</p>
<p>
  <img src="https://imgur.com/Lvv6deU.png" height="80%" width="80%" alt="Download osTicket"/>
</p>

<p><strong>Step 3:</strong> enable IIS along with CGI enabled.</p>
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
<!-- Step 5 -->
<p><strong>Step 5:</strong> From the “osTicket-Installation-Files” folder, unzip PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into the “C:\PHP” folder.</p>
<p><img src="https://i.imgur.com/SbiOQ8P.png" width="80%" alt="Unzip PHP"/></p>
<p><img src="https://i.imgur.com/OL038XQ.png" width="80%" alt="C PHP Directory"/></p>

<!-- Step 6 -->
<p><strong>Step 6:</strong> From the “osTicket-Installation-Files” folder, install the VC_redist.x86.exe.</p>
<p><img src="https://i.imgur.com/ODvFju4.png" width="80%" alt="Install VC Redist"/></p>

<!-- Step 7 -->
<p><strong>Step 7:</strong> From the “osTicket-Installation-Files” folder, install MySQL verssion 5.5.62 (mysql-5.5.62-win32.msi).<br>
Use Typical Setup and  then Launch Configuration Wizard and then Standard Configuration.<br>
Username: <code>root</code> | Password: <code>root</code></p>
<p><img src="https://i.imgur.com/yRz3nQZ.png" width="80%" alt="Install MySQL"/></p>

<!-- Step 8 -->
<p><strong>Step 8:</strong> Open IIS as an Administrator. Register PHP from within IIS  (PHP Manager → C:\PHP\php-cgi.exe), then reload IIS (Stop/Start).</p>
<p><img src="https://i.imgur.com/yrb3c8f.png" width="80%" alt="IIS Admin"/></p>
<p><img src="https://i.imgur.com/0Bnf3aS.png" width="80%" alt="Register PHP"/></p>
<p><img src="https://i.imgur.com/jj8M3WX.png" width="80%" alt="PHP Path"/></p>
<p><img src="https://i.imgur.com/xKRQG2r.png" width="80%" alt="Reload IIS"/></p>
<p><img src="https://i.imgur.com/hbbVv1o.png" width="80%" alt="IIS View"/></p>

<!-- Step 9 -->
<p><strong>Step 9:</strong> From the “osTicket-Installation-Files” folder, unzip the one that says “osTicket-v1.15.8.zip”.<br>
Copy the “upload” folder into <code>c:\inetpub\wwwroot</code> and rename it to “osTicket”.</p>
<p><img src="https://i.imgur.com/a0l4CuL.png" width="80%" alt="Unzip osTicket"/></p>
<p><img src="https://i.imgur.com/SNfYXZe.png" width="80%" alt="Copy Upload Folder"/></p>
<p><img src="https://i.imgur.com/7c60jb8.png" width="80%" alt="Rename to osTicket"/></p>

<!-- Step 10 -->
<p><strong>Step 10:</strong> Reload the IIS (Stop and Start the server again).</p>
<p><img src="https://i.imgur.com/1QqLJCa.png" width="80%" alt="Reload IIS"/></p>
<p><img src="https://i.imgur.com/rzn1O0r.png" width="80%" alt="Reload View"/></p>

<!-- Step 11 -->
<p><strong>Step 11:</strong> In IIS, go to Sites ad Default Web Site  and then osTicket.And On the right click “Browse *:80”.</p>
<p><img src="https://i.imgur.com/X74UvNz.png" width="80%" alt="Browse osTicket"/></p>

<!-- Step 12 -->
<p><strong>Step 12:</strong> If any of PHP extensions are missing, enable them:</p>
<ul>
  <li>In IIS, double-click PHP Manager</li>
  <li>Click “Enable or disable an extension”</li>
  <li>Enable: <code>php_imap.dll</code>, <code>php_intl.dll</code>, <code>php_opcache.dll</code></li>
</ul>
<p>Refresh osTicket browser page.</p>
<p><img src="https://i.imgur.com/UWNBtqk.png" width="80%" alt="Enable Extensions"/></p>
<p><img src="https://i.imgur.com/t7yzcCz.png" width="80%" alt="PHP Extensions"/></p>

<!-- Step 13 -->
<p><strong>Step 13:</strong> Make sure that you Rename and configure the config file:</p>
<ul>
  <li>Rename: <code>ost-sampleconfig.php</code> → <code>ost-config.php</code></li>
  <li>Path: <code>C:\inetpub\wwwroot\osTicket\include</code></li>
  <li>Disable inheritance → Remove all permissions</li>
  <li>Add permission: Everyone → Full Control</li>
</ul>
<p><img src="https://i.imgur.com/jcYkMoe.png" width="80%" alt="Rename Config"/></p>
<p><img src="https://i.imgur.com/Dq2Wm5q.png" width="80%" alt="Permission 1"/></p>
<p><img src="https://i.imgur.com/xhGzW9y.png" width="80%" alt="Permission 2"/></p>
<p><img src="https://i.imgur.com/9sDdDua.png" width="80%" alt="Permission 3"/></p>
<p><img src="https://i.imgur.com/4gDoxXU.png" width="80%" alt="Permission 4"/></p>
<p><img src="https://i.imgur.com/6wQ6vyK.png" width="80%" alt="Permission 5"/></p>
<p><img src="https://i.imgur.com/TGq3ahs.png" width="80%" alt="Permission 6"/></p>
<p><img src="https://i.imgur.com/AZzbIYs.png" width="80%" alt="Permission 7"/></p>
<p><img src="https://i.imgur.com/IrbMD39.png" width="80%" alt="Permission 8"/></p>

<!-- Step 14 -->
<p><strong>Step 14:</strong> Now you want to Continue to the  osTicket setup in the browser. Set your Helpdesk name and your default email (this is where customer messages go).</p>
<p><img src="https://i.imgur.com/nJNCgsO.png" width="80%" alt="Helpdesk Config"/></p>

<!-- Step 15 -->
<p><strong>Step 15:</strong> Install HeidiSQL.</p>
<ul>
  <li>Open HeidiSQL</li>
  <li>Create new session with the username: <code>root</code> and password: <code>root</code></li>
  <li>Create a database called <code>osTicket</code></li>
</ul>
<p><img src="https://i.imgur.com/8zmGRjB.png" width="80%" alt="HeidiSQL 1"/></p>
<p><img src="https://i.imgur.com/7T9AyE4.png" width="80%" alt="HeidiSQL 2"/></p>
<p><img src="https://i.imgur.com/pBSkf1j.png" width="80%" alt="HeidiSQL 3"/></p>
<p><img src="https://i.imgur.com/LEonddO.png" width="80%" alt="HeidiSQL 4"/></p>

<!-- Step 16 -->
<p><strong>Step 16:</strong> Continue setup in the browser:</p>
<ul>
  <li>MySQL Database: <code>osTicket</code></li>
  <li>Username: <code>root</code></li>
  <li>Password: <code>root</code></li>
  <li>Click “Install Now!”</li>
</ul>
<p><img src="https://i.imgur.com/tAzLcJj.png" width="80%" alt="osTicket DB Setup 1"/></p>
<p><img src="https://i.imgur.com/b86fYyy.png" width="80%" alt="osTicket DB Setup 2"/></p>
<p><img src="https://i.imgur.com/em4Tx2f.png" width="80%" alt="osTicket DB Setup 3"/></p>
