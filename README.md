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
Now with the Configuration Wizard open, select Next. Select the Standard Configuration and hit Next. Leave everything as-is on the next window and hit Next. Enter the root password as 'root' and retype to confirm. Select Next and then Execute.
</p>
<br />

<p>
<img width="1410" height="762" alt="image" src="https://github.com/user-attachments/assets/560fc84b-37ac-46ad-98e1-6f3749dd820e" />


</p>
<p>
Open Internet Information Services (IIS) as an Admin. Double-click PHP Manager. Click Register a new PHP version. Browse to your PHP folder on the C drive. Click into it, select the php-cgi file and select Open. Click OK.
</p>
<br />

<p>
<img width="1859" height="394" alt="image" src="https://github.com/user-attachments/assets/9f9a6870-a013-4f8f-8679-17e4206a1cdd" />

</p>
<p>
Back on the IIS Manager, ensure PHP Manager is selected. On the right-pane, select Stop. Wait a few seconds and then select Start. 
</p>
<br />

<p>
<img width="741" height="391" alt="image" src="https://github.com/user-attachments/assets/5f3f1dde-e094-41eb-80b4-641982796e56" />

</p>
<p>
Now go back to the osTicket-Installation-Files folder. Extract the osTicket-v1.15.8 file. This should create a new folder of the same name with the extracted files. Double-click into the new folder, notice the upload folder. While keeping this window open, open a new File Explorer and navigate to C Drive > inetpub > wwwroot. Now drag and drop the entire upload folder to the wwwroot folder. Rename the upload folder to osTicket.
</p>
<br />

<p>
<img width="488" height="503" alt="image" src="https://github.com/user-attachments/assets/acba1afd-8117-4f5b-bb9b-4e5b8f83283b" />
</p>
<p>
Navigate back to IIS. Right-click the server as shown in the image above. Select Stop. Wait a few seconds. Then right-click again and select Start. 
</p>
<br />

<p>
<img width="1896" height="489" alt="image" src="https://github.com/user-attachments/assets/7b38b44a-4f2f-4018-8328-b5d05ee1b1c0" />

</p>
<p>
In the left-pane expand the drop-down for the server. Expand Sites, expand Default Web Sites. Select osTicket. On the right-pane select Browse. 
</p>
<br />

<p>
<img width="1511" height="868" alt="image" src="https://github.com/user-attachments/assets/feea44f5-639f-4273-9652-b6d2cbe4d428" />

</p>
<p>
You should now be at the osTicket site. Notice not all features are installed, such as PHP IMAP Extension. 
</p>
<br />

<p>
<img width="1685" height="783" alt="image" src="https://github.com/user-attachments/assets/bfef9a0a-7ea0-4898-9337-8e3e0ab9d029" />
</p>
<p>
Go back to the IIS Manager. Make sure you are selected on osTicket, double-click PHP Manager. Select Enable or disable an extension. Enable php_imap.dll. Enable php_intl.dll. Enable php_opcache.dll.
</p>
<br />

<p>
<img width="1513" height="903" alt="image" src="https://github.com/user-attachments/assets/52d43676-19ab-4d1e-8260-c88d71ebee51" />
</p>
<p>
Go back to the osTicket site, refresh your browser. Notice some of the additional features are now enabled.
</p>
<br />

<p>
<img width="727" height="148" alt="image" src="https://github.com/user-attachments/assets/b4a37d6e-efb4-44a5-94a0-f3ebebbb20d0" />
</p>
<p>
Navigate to the following in File Explorer C:\inetpub\wwwroot\osTicket\include. Rename 'ost-sampleconfig.php' to 'ost-config.php'
</p>
<br />

<p>
<img width="762" height="523" alt="image" src="https://github.com/user-attachments/assets/2df7f98b-7920-4b5b-bb3d-f98e5abc0612" />
</p>
<p>
Right-click the file, select Properties. Go to the Securitty tab. Select Advanced. Select Disable inheritance. Select Remove all inherited permissions from this object. Select Add. Choose Select a principal. Type 'everyone', select Check names, and then select OK. Check Full control and hit OK. Select Apply and hit OK. 
</p>
<br />

<p>
<img width="883" height="816" alt="image" src="https://github.com/user-attachments/assets/32e530bc-37ab-4845-ab19-7556cae5bc0e" />
</p>
<p>
Go back to the osTicket site and select Continue. Fill out the information fields under the System Settings and Admin User sections, as shown in the image above. 
</p>
<br />

<p>
<img width="596" height="459" alt="image" src="https://github.com/user-attachments/assets/2bf0dfe9-17b4-4759-b3df-cbabf6cce4ca" />
</p>
<p>
Navigate to the osTicket-Installation-Files folder. Double-click the file 'HeidiSQL_12.3.0.6589_Setup' to install. Accept the agreement and select Next. Continue to select Next for the additional prompts and hit Install. Ensure the Launch HeidiSQL box is selected and hit Finish. 
</p>
<br />

<p>
<img width="726" height="523" alt="image" src="https://github.com/user-attachments/assets/cec74bdb-3fbd-4483-9f63-a0f5f71a6f96" />
</p>
<p>
With the session manager now open, select New in the bottom-left of the window. Type 'root' for username and password and select Open. 
</p>
<br />

<p>
<img width="1362" height="780" alt="image" src="https://github.com/user-attachments/assets/28cfefb8-b4c0-430a-b3c6-a15fc3190347" />
</p>
<p>
Right-click where it says 'Unnamed' in the top-left of the HeidiSQL windows. Select Create new and then Database. Type osTicket for the database name and hit OK. 
</p>
<br />

<p>
<img width="889" height="441" alt="image" src="https://github.com/user-attachments/assets/472cd273-ef0f-4d41-aa52-1aad1f6f19c4" />
</p>
<p>
Go back to the osTicket site and fill in the Database Settings as shown in the image above. Username and password are 'root'. Select Install Now. 
</p>
<br />

<p>
<img width="1592" height="859" alt="image" src="https://github.com/user-attachments/assets/285e5557-5333-4cc1-979f-e1177473d89b" />
</p>
<p>
The installation should now be successful, confirm my seeing a screen present you with a Congratualations!
</p>
<br />


