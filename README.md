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

- Windows 10</b> (22H2)

<h2>List of Prerequisites</h2>

- Download [osTicket-Installation-Files.zip](https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD) and unzip onto Desktop
- Enable Internet Information Services (IIS)
- Install PHP Manager
- Install MySQL
- Install C++ Redistributable
- Configure permissions and install osTicket

<h2>Installation Steps</h2>

<p>
<img width="1124" height="631" alt="image" src="https://github.com/user-attachments/assets/6f1d6493-2d84-4bd7-a5a5-fdbc0fbf42e3" />
</p>
<p>
Download the osTicket installation files referenced from the Prerequisities section above. Once downloaded, unzip the files onto your Desktop. Inside the folder, you should see the files as shown in the above image.
</p>
<br />

<p>
<img width="1073" height="866" alt="image" src="https://github.com/user-attachments/assets/94f73c24-580a-4a51-bf1a-6a52bb26fd33" />

</p>
<p>
Go to Control Panel. Select Programs. Select Turn Windows features on or off. Navigate to Internet Information Services and check the box. Expand the drop-down by clicking the + icon next to it. Expand World Wide Web Services and then expand Application Development Features. Check the box for CGI. Click OK. Allow time for the installation to complete and for the changes to be applied.
</p>
<br />

<p>
<img width="1120" height="635" alt="image" src="https://github.com/user-attachments/assets/2373876a-8e91-496c-b8c2-e7fc659e439f" />

</p>
<p>
Navigate to the os-Ticket-Installation-Files folder. Double-click on the PHPManagerForIIs_V1.5.0 file. Follow through the prompts, selecting next and agreeing to the terms and conditions to install.  
</p>
<br />

<p>
<img width="1123" height="627" alt="image" src="https://github.com/user-attachments/assets/eb82bfe6-d982-419f-96a4-1d2d5722117b" />

</p>
<p>
Go back to the to the os-Ticket-Installation-Files folder. Double-click on the rewrite_amd64_en-US file. Follow through the prompts, selecting next and agreeing to the terms and conditions to install. 
</p>
<br />

<p>
<img width="1712" height="725" alt="image" src="https://github.com/user-attachments/assets/fa1c3f39-5f9b-4d26-aea8-405c3e86fe98" />

</p>
<p>
Create a folder on your C drive labeled PHP. Navigate back to the os-Ticket-Installation-Files folder. Extract the php-7.3.8-nts-Win32-VC15-x86 file into the newly created PHP folder.
</p>
<br />

<p>
<img width="871" height="334" alt="image" src="https://github.com/user-attachments/assets/8734bda3-3062-44ee-951a-285f1ab43044" />

</p>
<p>
Within the os-Ticket-Installation-Files folder, double-click the VC_redist.x86 file to install, agree to the terms.
</p>
<br />

<p>
<img width="973" height="630" alt="image" src="https://github.com/user-attachments/assets/2596b0c6-2ede-4ba4-bc15-f6cccf7fb78d" />

</p>
<p>
Within the os-Ticket-Installation-Files folder, double-click the mysql-5.5.62-win32 file. Follow through the prompts to install (NOTE: Select the Typical install). Once prompted, select Finish, confirming the box is checked to launch the Configuration Wizard.
</p>
<br />

<p>
<img width="504" height="382" alt="image" src="https://github.com/user-attachments/assets/1de8ed90-c6b2-4cfb-b3f8-7923a1d49a8d" />
</p>
<p>
Now with the Congiuration Wizard open, select Next. Select the Standard Configuration and hit Next. Leave everything as-is on the next window and hit Next. Enter the root password as 'root' and retype to confirm. Select Next and then Execute.
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
