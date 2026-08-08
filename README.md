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
I installed Windows 11 on Virtualbox, and set it up like I did with my previous virtual machine. <br/>
<img src="https://i.imgur.com/2tcHtvy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/6SrvDxK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
To switch from dynamic to static IP address I did the following steps on both machines: went to VirtualBox network settings and switched over to Host-only Adapter (this will shut down internet connection), opened control panel and Ethernet properties, and entered costume parameters in IPv4 properties. The only parameter that changes is the IP address. <br/>
 <br />
<img src="https://i.imgur.com/qH21x6h.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/IbLUR0t.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/sa1xUom.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
To verify connectivity between both machines I headed over to CMD on Windows 11 machine and typed ping jerhunt.com (the domain name of my other machine, the which can be found by typing "whoami /?"). After the connectivity test was successful, i typed "ipconfig" on both machines to view the previously set parameters and to make sure there's no access to the internet.  <br/>
 <br />
<img src="https://i.imgur.com/6MwkTBr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 <img src="https://i.imgur.com/J7er1Ba.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
To join the machine to the domain I headed to File Explorer → right click This PC → properties → domain or workgroup → change → typed the domain jerhunt.com → entered the credentials the window asks for. I went to Users and Computers on Server 2016 and opened the Computers folder to verify that it worked.  <br/>
 <br />
<img src="https://i.imgur.com/D7co3cw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
A window saying that a restart is required will pop-up, I restarted the machine. Meanwhile it was restarting, from the Server 2016 machine I allowed remote connections via system properties. Finally, in Windows 11 machine I headed over to Remote Desktop Connection, typed the Server 2016 IP address, and entered my credentials. If it works, a window will appear to confirm the changes. After this, I obtained access to the domain. <br/>
 <br />
<img src="https://i.imgur.com/Dhz8OIQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
<img src="https://i.imgur.com/XdKehc8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
