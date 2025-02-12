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

<h2>Installation Steps</h2>

<p>
<img src="Screenshot 2025-02-12 064128.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 1- For this all your're going to need is a Window Virtual machine.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 064202.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 2- Go to https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD and download the zip file.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 064537.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 3-Once you download the zip file, extract it and another file should open with all the items in it.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 064931.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 4- Open Control Panel, Programs, Programs and Features then on the lift side you will see Turn window features on or off click on that.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 065031.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 5- Click on Internet Information Service also click the plus box to the left of it.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 065120.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 6-Extended the World Wide Web service folder, Application Development features, and lastly click on CGI.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 065433.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 7-Install PHPManager.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 065515.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 8-Install the rewirte AMD64.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 065910.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 9-Right click on the php-7.3.8 file and extract it into a new folder called PHP.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 070023.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 10-Install VC_redist.x86.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 070120.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 11-Install mysql after you do click next until you see this next message.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 070155.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 12-When you see this click on typical and hit next.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 070307.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 13-Click on Standard Configuration.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 070618.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 14-Now you want to open up IIS Manager as admin.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 070720.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 15-Click on PHP Manager.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 070807.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 16-After this will pop up and you want to click on the bottom where it says Register new PHP version.A new menu will pop up you want to go to the PHP file you made earlies and add the php-cgi into it.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 071101.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 17-Now you want to open the folder again and extract osTicket file.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 071742.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 18-Once you extract the file a new folder with 2 files in it will open name scripts and osticket.Go to file This PC/ C drive/inetpub/wwwroot )here you will drag the os ticket file into this folder. 
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 071958.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 19-Go back to IIS manager and on the left side click on osticket-vm/application pools/sites/default web site/osTicket) On the right click on the http folder.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 072653.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 20-Now you on the osTicket site.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 073036.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 21-Go to C drive/inetpub/wwwroot/osticket/include) find a file name C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php and change it to C:\inetpub\wwwroot\osTicket\include\ost-config.php.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 073204.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 22-After you change the name right click it and go to the Security tab then disable inheritance and then add one that goes to everyone,then edit the permissions and give it full access, click apply and ok.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
