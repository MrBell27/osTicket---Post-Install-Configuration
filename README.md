<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments & Teams
- Configure Agents & Users
- Configure SLA (service learning agreements)
- Configure Helpdesk Topics

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/jSyQqvE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
1. We will create roles as Admin and distributing them to Agents on the Helpdesk team. To see more information about roles checkout this link https://docs.osticket.com/en/latest/Admin/Agents/Roles.html . Go to the Admin Panel, click agents and then roles. We can now 'Add New Role'. You can name it Supreme Admin or whatever you want for this practice lab. Then go to permissions and you will see 'Tickets, Tasks, Knowledgbase' just select everything from each of those groups and then click Add Role. This user of Supreme Admin will be able to do everything and assign permissions to others. 
</p>
<br />

<p>
<img src="https://i.imgur.com/x85AaS2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
2. Next we will create a 'Department'. The departments will determine how the tickets get placed depending on the issue at hand. Go to Admin Panel, Agents and then Department and add a new department. Only make the changes you see in the image. We will configure the SLA's later. Scroll down an click create department. To learn more about departments you can checkout this link https://docs.osticket.com/en/latest/Admin/Agents/Departments.html

2.1 Now we will create our 'Teams', which will allow us to get agents from different departments to fix issues. Go to Admin panel, Agents, Teams and then Add new team. You can name your team 'Level II Support'. Click on members and you can add yourself to this team for now since we have not created other memebers yet. https://docs.osticket.com/en/latest/Admin/Agents/Teams.html
<br />

<p>
<img src="https://i.imgur.com/DYxhphC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
3.0 Now lets create 'Agents', these are the helpdesk individuals that will help solve tickets. Go to Admin panel, Agents and click add new agent. You can name your agents whatsveer you choose. Just remeber their credentials for when we need it to log in as them and respond to tickets. Create a name, email and username. Then click set password to create a password for your Agent. Uncheck both boxes, create password and press ok. Go to Access and set department to 'System Administrators' and the role will be 'Supreme Admin' and go to teams and set to Level II Support that we created. Click create and go back to Agents and follow the same steps to create a new Agent. This time under the Acess tab the department will be 'Support' and the role will be 'Expanded access'. https://docs.osticket.com/en/latest/Admin/Agents/Agents.html
</p>
<br />

<p>
<img src="https://i.imgur.com/hMAn0Qv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
3.1 We will create our users for this step. Users are the individuals that will create the tickets and send to the Agents for their IT needs. Go to Agent Panel, users and add new user. This is a pretty simple setup. Just add a name of your choosing and an email address like the one in the image. We will create 2 users, so repeat the process again. To learn more about Users you can refer to this link: https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html
</p>
<br />


<p>
<img src="https://i.imgur.com/0hxK4i5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
4.0 For this step we will be creating the SLA's (service level agreement). These are pretty much an agreed upon document between the company and provider saying that they will respond to certain issues within a given timeframe at all times and or will have the issue resolved or machines up and running. Go to Admin Panel, manage, SLA and click 'Add New SLA Plan'. We will create 3: SEV A put 1 hour grace period, 24/7 schedule. SEV B put 4 hours grace period, 24/7 schedule. SEV C put 8 hours grace period, Mon-Fri schedule. Here is a link to learn more about SLA's: https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html
</p>
<br />


<p>
<img src="https://i.imgur.com/z50Zte3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
5.0 Now we can configure Helpdesk Topics. These can be log-in issues, needing equipment etc etc. Go to Admin Panel, Manage and Help Topics so we can add 4 new help topics. We will just add the Topic names and leave everything else as is for each topic. 1. Business Critical Outage, 2.Personal COmputer Issues, 3. Equipment Request and 4. Password Reset. THIS WILL CONCLUDE THIS PORTION OF THE LAB! CONGARTS ON MAKING IT THIS FAR!
</p>
<br />
