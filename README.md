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

<h2>Operating Systems Used</h2>
- Windows 10 (21H2)

<h2>List of Prerequisites</h2>
- Windows 10 or Windows Server 2016+
- Internet Information Services (IIS) with CGI enabled
- PHP 7.4 – 8.1 with required extensions: `mysqli`, `gd`, `imap`, `xml`, `mbstring`, `intl`, `curl`, `fileinfo`, `zip`, `json`, `openssl`
- MySQL 5.7+ or MariaDB 10.2+
- Microsoft Visual C++ Redistributable
- IIS Rewrite Module (optional)

<h2>Installation Steps</h2>

<!-- Step 1 -->
<p><strong>Step 1:</strong> Create an Azure VM and log in with Remote Desktop.</p>
<img src="https://i.imgur.com/step1img1.png" alt="Step 1" width="80%" />

<!-- Step 2 -->
<p><strong>Step 2:</strong> Download and unzip the osTicket-Installation-Files.zip on the VM.</p>
<img src="https://i.imgur.com/step2img1.png" alt="Step 2" width="80%" />

<!-- Step 3 -->
<p><strong>Step 3:</strong> Install and enable IIS with CGI.</p>
<img src="https://i.imgur.com/step3img1.png" alt="Step 3 - Part 1" width="80%" />
<img src="https://i.imgur.com/step3img2.png" alt="Step 3 - Part 2" width="80%" />

<!-- Step 4 -->
<p><strong>Step 4:</strong> Install PHP Manager for IIS.</p>
<img src="https://i.imgur.com/step4img1.png" alt="Step 4" width="80%" />

<!-- Step 5 -->
<p><strong>Step 5:</strong> Create the directory C:\PHP.</p>
<img src="https://i.imgur.com/step5img1.png" alt="Step 5" width="80%" />

<!-- Step 6 -->
<p><strong>Step 6:</strong> Unzip PHP and install VC_redist.</p>
<img src="https://i.imgur.com/step6img1.png" alt="Step 6 - Unzip PHP" width="80%" />
<img src="https://i.imgur.com/step6img2.png" alt="Step 6 - VC_redist" width="80%" />

<!-- Step 7 -->
<p><strong>Step 7:</strong> Install MySQL and configure with root/root.</p>
<img src="https://i.imgur.com/step7img1.png" alt="Step 7" width="80%" />

<!-- Step 8 -->
<p><strong>Step 8:</strong> Open IIS and register PHP.</p>
<img src="https://i.imgur.com/step8img1.png" alt="Step 8" width="80%" />

<!-- Step 9 -->
<p><strong>Step 9:</strong> Reload IIS, unzip osTicket, and rename folder.</p>
<img src="https://i.imgur.com/step9img1.png" alt="Step 9 - IIS" width="80%" />
<img src="https://i.imgur.com/step9img2.png" alt="Step 9 - Upload" width="80%" />
<img src="https://i.imgur.com/step9img3.png" alt="Step 9 - Rename" width="80%" />
<img src="https://i.imgur.com/step9img4.png" alt="Step 9 - Copy" width="80%" />
<img src="https://i.imgur.com/step9img5.png" alt="Step 9 - Final Check 1" width="80%" />
<img src="https://i.imgur.com/step9img6.png" alt="Step 9 - Final Check 2" width="80%" />

<!-- Step 10 -->
<p><strong>Step 10:</strong> Reload IIS again.</p>
<img src="https://i.imgur.com/step10img1.png" alt="Step 10 - Reload" width="80%" />
<img src="https://i.imgur.com/step10img2.png" alt="Step 10 - Confirmation" width="80%" />

<!-- Step 11 -->
<p><strong>Step 11:</strong> Browse to osTicket in your browser.</p>
<img src="https://i.imgur.com/step11img1.png" alt="Step 11" width="80%" />

<!-- Step 12 -->
<p><strong>Step 12:</strong> Enable required PHP extensions in PHP Manager.</p>
<img src="https://i.imgur.com/step12img1.png" alt="Step 12 - Extensions" width="80%" />
<img src="https://i.imgur.com/step12img2.png" alt="Step 12 - Save Changes" width="80%" />

<!-- Step 13 -->
<p><strong>Step 13:</strong> Refresh the osTicket browser page and verify.</p>
<img src="https://i.imgur.com/step13img1.png" alt="Step 13 - Screenshot 1" width="80%" />
<img src="https://i.imgur.com/step13img2.png" alt="Step 13 - Screenshot 2" width="80%" />
<img src="https://i.imgur.com/step13img3.png" alt="Step 13 - Screenshot 3" width="80%" />
<img src="https://i.imgur.com/step13img4.png" alt="Step 13 - Screenshot 4" width="80%" />
<img src="https://i.imgur.com/step13img5.png" alt="Step 13 - Screenshot 5" width="80%" />
<img src="https://i.imgur.com/step13img6.png" alt="Step 13 - Screenshot 6" width="80%" />
<img src="https://i.imgur.com/step13img7.png" alt="Step 13 - Screenshot 7" width="80%" />
<img src="https://i.imgur.com/step13img8.png" alt="Step 13 - Screenshot 8" width="80%" />
<img src="https://i.imgur.com/step13img9.png" alt="Step 13 - Screenshot 9" width="80%" />

<!-- Step 14 -->
<p><strong>Step 14:</strong> Rename ost-config.php to enable setup.</p>
<img src="https://i.imgur.com/step14img1.png" alt="Step 14" width="80%" />

<!-- Step 15 -->
<p><strong>Step 15:</strong> Set permissions for ost-config.php.</p>
<img src="https://i.imgur.com/step15img1.png" alt="Step 15 - Permissions 1" width="80%" />
<img src="https://i.imgur.com/step15img2.png" alt="Step 15 - Permissions 2" width="80%" />
<img src="https://i.imgur.com/step15img3.png" alt="Step 15 - Permissions 3" width="80%" />
<img src="https://i.imgur.com/step15img4.png" alt="Step 15 - Permissions 4" width="80%" />

<!-- Step 16 -->
<p><strong>Step 16:</strong> Begin final osTicket setup in browser (helpdesk name, email).</p>
<img src="https://i.imgur.com/step16img1.png" alt="Step 16 - Helpdesk Name" width="80%" />
<img src="https://i.imgur.com/step16img2.png" alt="Step 16 - Email Input" width="80%" />
<img src="https://i.imgur.com/step16img3.png" alt="Step 16 - Submit Setup" width="80%" />

