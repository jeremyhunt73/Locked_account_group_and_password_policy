<h1>Group policy, password policy, and account locked </h1>

<h2>Description</h2>
THe following lab consists of some fundamental policies that can be applied to users and password policies, as well as locking out a user and how to let them log back in.Policy is very important, since it sets boundaries for employees for a safer IT environment, and adding policies to passwords will enhance the computer's security in a company. Also, users not being able to log-in to a computer is one of the most common issues in IT support, so comprehending this information is valuable and it's also implemented in cybersecurity.
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
After completely disabling the user, if I try to log in as Joseph in Windows 11 machine, it won't work, and an error message will pop-up. A user can be unlocked by simply checking "unlock account" in the account tab. <br/>
 <br />
<img src="https://i.imgur.com/2G9sEGD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/3xcwyZF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/cPJ4fNT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
A very relevant policy is logon hours. In user properties I clicked account and opened logon hours. It's possible to choose at what time or date a user can log in to a computer, this is useful in work environment for safety measures. <br/>
 <br />
<img src="https://i.imgur.com/pXI3703.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 <img src="https://i.imgur.com/1dCZueT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Another useful policy is setting an end date for a user to log-in, this is usually applied to employees who's term is expected to end soon. If they try logging in after the expiration date, they will receive an error message. <br/>
 <br />
<img src="https://i.imgur.com/XFbrt31.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Some of the most crucial password policies are expiration (how long the password will be valid for) and length (minimum characters required). These are fully customizable and key to make the log-in more secure. To do this, I headed over to Group Management Policy → right-clicked default domain policy → edit → Windows settings → security settings → account policy. <br/>
 <br />
<img src="https://i.imgur.com/ZEcEeEu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
<img src="https://i.imgur.com/9zPihGR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/hU3xJJW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
If a user fails to log-in after certain amount of attempts, their account can be locked out for a set amount of time, this helps prevent brute force attacks. <br/>
 <br />
<img src="https://i.imgur.com/1o04sZb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
<img src="https://i.imgur.com/c2WZWzl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/to5P6Es.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Applied group policies can be viewed by typing "gpresults /r" and "user name_of_user /domain" in CMD. It can also be viewed in default domain policy settings in Group Policy Management (a few windows will pop-up, I just clicked add). <br/>
 <br />
<img src="https://i.imgur.com/H2ZYvn4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
<img src="https://i.imgur.com/zyd0Hwk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/O7GRnun.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

