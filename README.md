<h1>Group policy, password policy, and account locked </h1>

<h2>Description</h2>
THe following lab consists of some fundamental policies that can be applied to users and password policies, as well as locking out a user and how to let them log back in.Policy is very important, since it sets boundaries for employees for a safer IT environment, and adding policies to passwords will enhance the computer's security in a company. Also, +users not being able to log-in to a computer is one of the most common issues in IT support, so comprehending this information is valuable.
<br />


<h2>Software Used</h2>

- <b>Latest version of VirtualBox</b> 

<h2>Environments Used </h2>

- <b>Windows Server 2016</b>
- <b>Windows 11</b>
<h2>Walk-through:</h2>

<p align="center">
I deleted Joseph and disabled this account, a user created in Server 2016 and logged in Windows 11. This user is the subject I used as a sample throughout the lab. <br/>
<img src="https://i.imgur.com/lKJQ48V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 <img src="https://i.imgur.com/hZknDzQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
After completely disabling the user, if I try to log in as Joseph in Windows 11 machine it won't work, and an error message will pop-up. <br/>
 <br />
<img src="https://i.imgur.com/2G9sEGD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
A very relevant policy is logon hours. In user properties I clicked account and opened logon hours.  <br/>
 <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 <img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
To join the machine to the domain I headed to File Explorer → right click This PC → properties → domain or workgroup → change → typed the domain jerhunt.com → entered the credentials the window asks for. I went to Users and Computers on Server 2016 and opened the Computers folder to verify that it worked.  <br/>
 <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
A window saying that a restart is required will pop-up, I restarted the machine. Meanwhile it was restarting, from the Server 2016 machine I allowed remote connections via system properties. Finally, in Windows 11 machine I headed over to Remote Desktop Connection, typed the Server 2016 IP address, and entered my credentials. If it works, a window will appear to confirm the changes. After this, I obtained access to the domain. <br/>
 <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
