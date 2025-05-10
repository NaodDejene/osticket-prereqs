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

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="osTicket Installation"/>
</p>
<p>
<b>Step 1:</b> Log in to your Microsoft Azure account. Go to the Virtual Machines section and create a new VM. Enter your subscription details, resource group, name, region, and choose a Windows 10 image and suitable size. Create an administrator username and password. Click "Review + Create" and then deploy the VM.
</p>
<br />

<p>
<b>Step 2:</b> After deployment, access the VM's overview page to find its public IP. Use Remote Desktop (RDP) to connect to the Windows environment.
</p>
<br />

<p>
<b>Step 3:</b> Open the Control Panel, go to "Programs and Features," then select "Turn Windows features on or off." Enable "Internet Information Services (IIS)" and its subcomponents. Click OK to install IIS.
</p>
<br />

<p>
<b>Step 4:</b> Download PHP for Windows from the official website. Extract it to a folder (e.g., C:\PHP). In IIS Manager, add a module mapping to associate `.php` files with `php-cgi.exe`. Enable required PHP extensions in `php.ini`.
</p>
<br />

<p>
<b>Step 5:</b> Install MySQL Server by downloading it from the official MySQL website. Set a root password and create a new database (e.g., `osticket_db`). Also create a user and grant it privileges to access the database.
</p>
<br />

<p>
<b>Step 6:</b> Download the latest osTicket release from the official website. Extract the contents to `C:\inetpub\wwwroot\osTicket`. Ensure the IIS user has the necessary permissions to read/write this directory.
</p>
<br />

<p>
<b>Step 7:</b> In IIS Manager, right-click "Sites" and choose "Add Website." Assign a name, set the physical path to the osTicket folder, and choose a port (default is 80). Start the website.
</p>
<br />

<p>
<b>Step 8:</b> Open your browser and navigate to the osTicket URL. Complete the setup wizard by entering helpdesk name, admin credentials, and MySQL database information. Submit the form to finish the installation.
</p>
<br />

<p>
<b>Final Setup:</b> Delete the `/setup` directory from the osTicket folder. Change the `ost-config.php` file permissions to read-only for security.
</p>
<br />

<p>
<b>Review and Create:</b> Review all your configurations, click "Create" to deploy the VM. Once deployment is complete, click "Go to Resource" to access your virtual machine.
</p>
<br />
