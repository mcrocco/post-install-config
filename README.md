<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles, Departments and Teams
- Configure Agents (employees)
- Configure Users (customers)
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/PThKrcw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Roles in a ticketing system are what access and permissions is set to an employee to ensure the smooth operation and management of ticket-related processes. For example, we can create a "Supreme Admin" role to give whoever is assigned this role full access and permissions, since administrators typically oversee an entire ticketing system. To do this, log in to a user admin account we created previously, select Admin Panel, then Agents and finally Roles. By clicking Add New Role, we can name it Supreme Admin, along with toggling which Permissions we want to whoever is assigned to this role. Because this is just an example of a "Supreme Admin", add all permissions and select Add Role. 

<img src="https://i.imgur.com/XPB8JFE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Departments in a ticketing system are used to categorize employees to where they handle different aspects of ticket-related processes. In osTicket, departments such as Support are created by default, which are tasked with addressing customer inquiries and issues. We can create a department called System Administrators, in which those assigned to this department are more responsible for internal staff requests and overseeing system-related problems. To create this department, go to Admin Panel, Agents, Departments and finally Add New Department. From there, you can name is System Administrators, as well as assign it a SLA and add agents to this department. 

<img src="https://i.imgur.com/ZLJsgoD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Teams in a ticketing system are used to grab "the best of the best" from each department for critical issues or periods of downage in the business. To create a team such as Level II Support, go to Admin Panel, Agents, Teams and finally Add New Team. You can also select which agents are apart of the team when creating a new team. 
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/05tqNkP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Agents in a ticketing system is another word for employees who will be responding and resolving tickets. To create an agent in osTicket, in this case it will be John Doe, go to Admin Panel, Agents, and Add New Agent. From here, fill out a name, email, along with a username and password. In addition, select Set Password and turn off "send the agent a password reset email" to input a password for this agent (This is only for lab purposes so we can login to John's account later. In real life, make sure this option stays on so the employee themselves can create a secure password). Make sure to give this agent access to the System Admins department and Supreme Admin role to work with example tickets later. 
</p>
<br />

<p>
<img src="https://i.imgur.com/aIIyw84.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Users in a ticketing system is another word for customers who are having an issue and submitting a ticket to the osTicket system. To create a user (in this example it will be Ken), go to Agent Panel, Users and then Add User. Simply put in a name and email address to create a user. 
</p>
<br />

<p>
<img src="https://i.imgur.com/ERAGM2g.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Service Level Agreements or SLAs define the agreed-upon response and resolution times for tickets raised by customers. To create SLAs in osTicket, go to Admin Panel, Manage, SLA and Add New SLA Plan. Selecting this give you the option to name the SLA, give it a grace period and schedule. For example, in the picture above an SLA called Sev-A was created with the idea that Business Critical issues will be assigned to this SLA. So, a grace period of an hour was given to Sev-A, along with a 24/7 schedule. 
</p>
<br />

<p>
<img src="https://i.imgur.com/mBPYBFN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Help Topics in a ticketing system are used by customers when creating a ticket, in which it will assist classifying and routing tickets to the correct department or support team. To create a help topic such as "Business Critical Outage" go to Admin Panel, Help Topics and then Add New Help Topic. From here you can name and give a description to this new help topic. The picture above shows examples of other help topics created through osTicket. 
</p>
<br />
