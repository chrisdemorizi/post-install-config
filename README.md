<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
In this home lab, I will perform Sysadmin tasks on osTicket. I will use both admin and user panels to create, configure, and assign roles and ticket settings.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)

<h2>Configuration Steps</h2>

<h3>Admin/Analyst Login Page:</h3>
<p><a href="http://localhost/osTicket/scp/login.php">http://localhost/osTicket/scp/login.php</a></p>

<h3>End Users osTicket URL:</h3>
<p><a href="http://localhost/osTicket">http://localhost/osTicket</a></p>


<h3>Acknowledge Agent Panel vs Admin Panel</h3>

<p>Agent Panel</p>

![image](https://github.com/user-attachments/assets/1d6b40a2-5357-4d99-b62f-c7de624ca5e6)

<p>Admin Panel</p>

![image](https://github.com/user-attachments/assets/0dff2399-e774-4a8b-856e-c6ee968b9618)

<h3>Configure Roles (for grouping permissions)</h3>
<p>Admin Panel -> Agents -> Roles</p>
<p>Supreme Admin</p>

![image](https://github.com/user-attachments/assets/f20185e6-c92e-48a0-9441-0e881a60663e)

<h3>Configure Departments (Ticket Visibility)</h3>
<p>Admin Panel -> Agents -> Departments</p>
<p>SysAdmins</p>

![image](https://github.com/user-attachments/assets/2174401c-f97d-4235-aeae-39a24b284dfd)

<h3>Configure Teams</h3>
<p>Admin Panel -> Agents -> Teams (Pull Agents from different Departments)</p>
<p>Online Banking</p>

![image](https://github.com/user-attachments/assets/2aaafddb-f742-4def-b281-0813768502cc)

<h3>Allow anyone to create tickets</h3>
<p>Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)</p>
<p>Registration Required: Require registration and login to create tickets</p>

<h3>Configure Agents (workers)</h3>
<p>Admin Panel -> Agents -> Add New</p>
<p>Jane (Dept: SysAdmins)</p>
<p>John (Dept: Support)</p>

![image](https://github.com/user-attachments/assets/424dacba-8737-42b0-a308-2c1fcfd97e76)

<h3>Configure Users (customers)</h3>
<p>Agent Panel -> Users -> Add New</p>
<p>Emilia</p>
<p>Gojo</p>

![image](https://github.com/user-attachments/assets/0c0643a9-ada6-4918-978a-32ef6b322d68)

<h3>Configure SLA</h3>
<p>Admin Panel -> Manage -> SLA</p>
<ul>
  <li>Sev-A (Grace Period: 1 hour, Schedule: 24/7)</li>
  <li>Sev-B (Grace Period: 4 hours, Schedule: 24/7)</li>
  <li>Sev-C (Grace Period: 8 hours, Business Hours)</li>
</ul>

![image](https://github.com/user-attachments/assets/c8108e99-acf0-4f8b-9a8a-06c459a01410)

<h3>Configure Help Topics (For when users create a ticket)</h3>
<p>Admin Panel -> Manage -> Help Topics</p>
<ul>
  <li>Business Critical Outage</li>
  <li>Personal Computer Issues</li>
  <li>Equipment Request</li>
  <li>Password Reset</li>
  <li>Other</li>
</ul>

![image](https://github.com/user-attachments/assets/e93d3ac4-728a-43da-b511-6702974ea06e)

<h2>Takeaways and Key Skills Developed</h2>
In this lab, I configured osTicket by managing user roles, departments, and ticket settings. I set up roles to group permissions, defined departments for ticket visibility, and created teams by combining agents from different departments. I required user registration before ticket creation, added agents and users, and set up SLAs for different severity levels. Additionally, I created help topics to categorize tickets. This hands-on experience helped me learn to manage user roles, workflows, and settings in a ticketing system to improve help desk efficiency.
