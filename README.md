<br><h1 align="center">User Creation with Windows Powershell ISE</br>
<br>
<img src="https://upload.wikimedia.org/wikipedia/commons/2/2f/PowerShell_5.0_icon.png" height="250" width="275"/><img src="https://icons.veryicon.com/png/o/miscellaneous/two-color-icon-library/user-286.png" height="250" width="250"/>
</br>
</h1>
This repo will guide you through the process of creating a large number of users using Powershell ISE. Something of this scale is helpful for user creation and management within Active Directory, where you would create groups/permissions and provision them to specific users. <i>We will be using a preconfigured Windows 10 VM and a Windows Server with Active Directory set up.</i>
<br/>


<h2>Databases & Programs Used</h2>
<p>
 
- <b>Powershell ISE</b>

- <b>Active Directory</b>

</p>

<h2>Environments Used</h2>
<p>
 
- <b>Windows 10 Enterprise</b> (22H2)
- <b>Windows Server Datacenter: Azure Edition</b> (2022)


<h2 align="center">Running user creation script in Powershell ISE</h2>

<p>Access your Windows Server client, launch Powershell ISE, and create a new file. Then, copy the text in the code field here and paste it in Windows PowerShell ISE. Pressing enter will start the user creation script, creating 10,000 random users that will be accessible via Active Directory. <i>Make sure you have an OU (Organizational Unit) folder in your Active Directory that matches with <b>"_EMPLOYEES"</b> in <b>line 43</b> of the script <b>BEFORE</b> executing it. You can either change <b>"_EMPLOYEES"</b> in the script to match your OU folder or vice-versa.</i>
<br><img src="https://github.com/user-attachments/assets/d29f6d02-6402-40a2-a601-26770138f86e" height="75%" width="100%"/>
<br/>
</p>

<p>Once you're satisfied with an amount of user creations, you can stop the script and view all created users in the OU folder that you set the script to place the users in on Active Directory. Then, choose and access one of the users account properties. Keep note of this user and password (located in line 2 of Powershell ISE script we ran) for later.
<br><img src="https://github.com/user-attachments/assets/d4966dcc-3aaa-4710-b209-10078e4830a4" height="75%" width="100%"/>
<br/>
</p>

<p>Log into your Windows 10 client with administrative credentials and right-click the Windows icon > System > Remote Desktop > then click Select users that can remotely access this PC. Enter "Domain Users" in the open field and click "OK". This will effectively allow all users that we just created to access and sign into this Windows 10 client.
<br><img src="https://github.com/user-attachments/assets/d37c8277-8b0c-499d-9891-bcade8605591" height="75%" width="100%"/>
<br/>
</p>

<p>With your chosen user credentials, log back into the Windows 10 client.
<br><img src="https://github.com/user-attachments/assets/0e24b4d7-23e4-4b38-9570-43b08c7fae09" height="75%" width="100%"/>
<br/>
</p>

<p>Once you're logged in, you can right-click the Windows icon > Settings > Accounts to confirm you're logged in as a user now.
<br><img src="https://github.com/user-attachments/assets/01ccc032-ef20-4fd3-b423-e6037af84790" height="75%" width="100%"/>
<br/>
</p>

Congrats! This skips the hassle of creating several users at a time, and lets you focus more on user management.








