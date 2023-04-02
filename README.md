p align="center">
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

- 
- 
- 
- 
- 

<h2>Installation Steps</h2>



Step 1 - Follow my procedure (Configarted the virtual machine azure) 



Step 2 - Turn on the internet information services and CGI
<p>
<img src="https://i.imgur.com/6cpfKti.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After successfully setting up your VM, the next step is to activate IIS. To do so, go to the Control Panel and select 'Uninstall a Program'. From there, choose 'Turn Windows Features On or Off' and a list will appear. Look for Internet Information Services and enable it. Additionally, make sure to enable CGI from the world wide web.
</p>
<br />

Step 3 - Download and install PHP Manager as well as rewrite module


</p>

Step 4 - Create the directory C:\PHP
<p>
<img src="https://i.imgur.com/KvkUgSe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a folder name PHP into c drive
<p>
Step 5 - Download PHP 7.3.8 and unzip the contents in to C:\PHP
<p>
<img src="https://i.imgur.com/LvIFfYr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 After downloading, extract the folder and move it to the local disk.
<p>
Step 6 - Download and install VC_redist.x86.exe. and MySQL 5.5.62
<p>
<img src="https://i.imgur.com/iuLWzkE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Make sure to remember the password

Step 7 - Register PHP from within IIS 
<p>
<img src="https://i.imgur.com/TwFyaQf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To register a new version of PHP, run IIS with administrator privileges and access PHP Manager. In the "PHP Setup" area, locate and click "Register New PHP version", then search for the PHP folder you recently added to the "Program Files (x86)/PHP" directory. Open the folder and select the "php-cgi.exe" file.
Step 8 - Install osTicket V1.15.8 
<p>
<img src="https://i.imgur.com/Dzp1cjL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To install osTicket, begin by downloading it from the Installation Files Folder. Then, extract the contents of the "upload" folder and transfer them to "c:\inetpub\wwwroot". Once the transfer is complete, rename the "upload" folder to "osTicket" within the "c:\inetpub\wwwroot" directory.
<p>
Step 9 - 
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
 <p>
Step 9 - 
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
 <p>
Step 9 - 
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
 <p>
Step 9 - 
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
