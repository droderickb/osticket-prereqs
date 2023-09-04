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

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Installation Steps</h2>

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

