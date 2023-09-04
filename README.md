<p align="center">
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

<h2>List of Prerequisites</h2>

- Create Virtual Machine
- Remote Desktop into vm install all sofware needed to vm
- Download/Install needed files into Vm 
- Set up Os Ticket 


<h2>Installation Steps</h2>

![image](https://github.com/droderickb/osticket-prereqs/assets/138819497/f88ac4fd-f052-4a74-929e-da3075db327b)

Create Virtual Machine ( I chose Azure VM with Windows 10 Operating System)


![image](https://github.com/droderickb/osticket-prereqs/assets/138819497/049db991-0861-4c59-9b60-46411c36e988)

Use Remote Desktop to log into VM

<p>
  
![image](https://github.com/droderickb/osticket-prereqs/assets/138819497/56bf53ab-9b15-452e-941d-a9e08e1487a7)

</p>
<p>
Right click the start menu. Select "Run". Type "Control" for the contol panel snd press "Enter." Click on the "Program" icon and then select the "Turn windows on and off" feature. World Wide Web Services -> Application Development Features ->
[X] CGI
[X] Common HTTP Features

</p>
<br />

<p>

![image](https://github.com/droderickb/osticket-prereqs/assets/138819497/d9dfbbc5-ef4c-4aca-9f96-1fb2c0ca25ab)


</p>
<p>
After enabling IIS Windows and HTTPS features, intall and download the following files ; PHP Manager or IIS, Rewrite Module, PHP, VC Redist, MySQL, & OsTicket 
</p>
<br />

<p>

![image](https://github.com/droderickb/osticket-prereqs/assets/138819497/6f9ad069-efb8-4939-97fc-be2ccf536301)


</p>
<p>
As your installing MySql select typical setup--> launch configuration Wizard--> Standard Configuration --> Select Password (Enter password of your choice)  
</p>
<br />

![image](https://github.com/droderickb/osticket-prereqs/assets/138819497/7ce30a7f-4f96-4f05-b429-4287a4d7270a)

Open IIS as an administrator. Register PHP from within IIS. 

![image](https://github.com/droderickb/osticket-prereqs/assets/138819497/904d3897-3f8c-4639-9c09-84c48aa6075a)



Go to sites -> Default -> osTicket
On the right, click “Browse *:80”

Note that some extensions are not enabled
Go back to IIS, sites -> Default -> osTicket
Double-click PHP Manager
Click “Enable or disable an extension”
Enable: php_imap.dll
Enable: php_intl.dll
Enable: php_opcache.dll
Refresh the osTicket site in your browse, observe the changes

Rename: ost-config.php
From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
To: C:\inetpub\wwwroot\osTicket\include\ost-config.php

Assign Permissions: ost-config.php
Disable inheritance -> Remove All
New Permissions -> Everyone -> All

Continue Setting up osTicket in the browser (click Continue)
Name Helpdesk
Default email (receives email from customers)



