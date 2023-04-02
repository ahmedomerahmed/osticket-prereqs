p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)


<h2>Installation Steps</h2>



Step 1 - Follow my procedure (Configuring Virtual machice within Azure) 



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
<p>
Step 8 - Install osTicket V1.15.8 
<p>
<img src="https://i.imgur.com/Dzp1cjL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To install osTicket, begin by downloading it from the Installation Files Folder. Then, extract the contents of the "upload" folder and transfer them to "c:\inetpub\wwwroot". Once the transfer is complete, rename the "upload" folder to "osTicket" within the "c:\inetpub\wwwroot" directory. Do not forget to restart the server
<p>
Step 9 - Click "Browse *:80"
<p>
<img src="https://i.imgur.com/Wp3YgRa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To launch the osTicket web server in your default browser, begin by opening the IIS Manager. After that, restart the server and navigate to Sites -> Default -> osTicket. On the right-hand side, select "Browse*.80" to launch the osTicket web server in your default browser.
 <p>
Step 10 - To enable 3 extentions
<p>
<img src="https://i.imgur.com/jwOTsnQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To activate certain extensions in IIS, access Sites -> Default -> osTicket. Next, double-click on PHP Manager and choose "Disable or Enable an Extension". Enable the "php_intl.dll" and "php_opcache.dll" extensions, then do not forget refresh the osTicket web server to observe any changes. You should now see that the "Intl Extension" is enabled.
 <p>
Step 11 - Rename and Assign Permissions of ost-confiq.php
<p>
<img src="https://i.imgur.com/wkzMqbC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To configure the osTicket installation, navigate to "C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php" using the Explorer. Next, rename the file to "ost-config.php" by removing the word "sample" from the filename. After that, assign full permissions to the new "ost-config.php" file for Everyone. Disable inheritance and remove all new permissions except for "Everyone" to complete the process.
 <p>
Step 12 - Download and install HeidiSQL
<p>
<img src="https://i.imgur.com/irmoX2l.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once you've installed HeidiSQL, open the application and click on "New". The username should remain as "root". Enter the password that you chose at the beginning of the lab and click "Open" to establish a connection to the database. Next, right-click and select "Create New", then choose "Database". Enter "Osticket" as the name of the database.
  <p>
Step 13 - Setting up osticket in the browser
<p>
<img src="https://i.imgur.com/316l4qG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Return to the osTicket application and provide the necessary database information. For MySQL, use "osticket" as the database name, "root" as the username, and the password you previously selected. Once you've entered the information, click "Install". Now, osTicket installion is complete
 <p>
