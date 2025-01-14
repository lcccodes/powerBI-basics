# powerBI-basics
Some notes on using Microsoft Power BI for beginners.

<b>What is PowerBI?</b>

"Microsoft Power BI is a suite of tools and services within Microsoft Fabric that data analysts can use to build interactive data visualizations" (Microsft Learn, 2025). It's particularly good for enterprise-scale business analytics because it is "an integrated solution that can support complex data modeling, interactive reporting, and secure sharing" (Microsoft Learn, 2025).

So, there are many tools for doing data visualization, but this one is well-suited for larger business environments.

<b>The Difference Between PowerBI Desktop, PowerBI Service, and PowerBI mobile apps</b>

The bulk of your work with PowerBI as a designer or analyst will be in PowerBI desktop, which is a Microsoft Windows application and sits locally. Desktop is where you will import data, construct models and then the reports.

PowerBI Service sits on the cloud and is where you upload your reports so others can interact and share them (in accordance with permissions set).

PowerBI on various mobile devices is primarily just for accessing the reports and dashboards hosted on PowerBI service.

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This project.....s.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- PHP Manager
- C++ Redistributable
- MySQL
- osTicket
- HeidiSQL

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>List of Prerequisites</h2>

- IIS
- PHP Manager
- "rewrite module"
- "C++ Redistributable"
- MySQL
- HeidiSQL (DB client)


<h2>Installation Steps</h2>
<p>There are actually quite a few prerequisites to install, but the steps are easy.</p>

![image](https://github.com/lcccodes/osticket-install/assets/171904823/a18f124b-b556-48cc-b05f-a47f8918f77b)


<p>
Installing and configuring IIS (Internet Information Services) which will act as the webserver on which osTicket will run.
</p>
<br />

<p>
Next, you'll need PHP manager. 

![image](https://github.com/lcccodes/osticket-install/assets/171904823/ca3981b7-66c0-4830-a2b9-89c3ecb02d9d)


</p>
<p>
PHP manager needs to be installed before you try to install php_7.3.8 (or latest).
</p>
<br />

<p>
Then install the "rewrite module" (does something behind the scenes in osTicket).

![image](https://github.com/lcccodes/osticket-install/assets/171904823/2cc07698-d5c7-4f34-ab8b-42557e31875b)


</p>
<p>
This one is really quick. After this, you install the C++ Redistributable, then MySQL Server.
</p>
<br />

<p>
You can use HeidiSQL as the DB client with MySQL server (install HeidiSQL once osTicket is ready).

  ![image](https://github.com/lcccodes/osticket-install/assets/171904823/ceeba0a8-a85a-4d69-b1ec-c4724ed48dff)

</p>
<p>
Choose "standard configuration" when installing MySQL server.
</p>
<br />

<p>
osTicket is the last to install.

  ![image](https://github.com/lcccodes/osticket-install/assets/171904823/ceeba0a8-a85a-4d69-b1ec-c4724ed48dff)

</p>
<p>
Once osTicket is installed, you need to reload IIS and then enable extensions for osTicket.
</p>
<br />

<p>
In IIS, find PHP Manager. Right click on the extension needed or find "enable" on the right hand menu.

![image](https://github.com/lcccodes/osticket-install/assets/171904823/d7f82afc-a664-4112-9682-51ddeb65662d)


</p>
<p>
  ...
</p>
<br />

<p>
Install and set up HeidiSQL DB client.

 ![image](https://github.com/lcccodes/osticket-install/assets/171904823/a6944c9c-3919-4ee3-9957-51a496e4bebd)


</p>
<p>
You'll need to create a new database for osTicket (call it "osTicket"), and enter the information from the MySQL database.</p>
<br />

Make sure to read on to Part 2 for the 
[Post-Installation Configuration](https://github.com/lcccodes/post-install-config).
