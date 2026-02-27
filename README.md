<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>

This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.

Admin/Analyst Login Page: [Admin Login](http://localhost/osTicket/scp/login.php)

End Users osTicket URL: [End Users Ticketing Page](http://localhost/osTicket)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Set up roles and permissions for agents and users.
- Configure ticket visibility and help desk functionality.
- Establish SLAs to define response times for tickets.
- Enhance user experience by organizing help topics.
- Secure the osTicket system with proper permissions and user settings.

<h2>Configuration Steps</h2>

### Step 1: Configure Roles
- Navigate to Admin Panel -> Agents -> Roles.
- Create a role:
  - Supreme Admin

<img width="595" alt="Screenshot 2025-01-23 at 10 47 37 AM" src="https://github.com/user-attachments/assets/dd1f2373-7147-4a4d-9b20-565ea0f363ff" />
<img width="632" alt="Screenshot 2025-01-23 at 10 47 22 AM" src="https://github.com/user-attachments/assets/9e2b8b13-ffb1-479f-aed5-64f45d590379" />


### Step 2: Configure Departments
- Navigate to Admin Panel -> Agents -> Departments.
- Create departments for ticket visibility:
  - Example: SysAdmins
 
<img width="578" alt="Screenshot 2025-01-23 at 10 49 51 AM" src="https://github.com/user-attachments/assets/1e219835-21a6-4987-a193-937a87d7f9b1" />

 
### Step 3: Configure Teams
- Navigate to Admin Panel -> Agents -> Teams.
- Create a team and pull agents from different departments:
  - Example: Online Banking

<img width="558" alt="Screenshot 2025-01-23 at 10 50 11 AM" src="https://github.com/user-attachments/assets/7b0e4f93-e614-400c-b7a0-67e3f7f7e308" />

### Step 4: User Settings
- Navigate to Admin Panel -> Settings -> User Settings.
- Configure ticket creation settings:
  - Uncheck: Unregistered users can create tickets.
  - Require registration and login to create tickets.

<img width="537" alt="Screenshot 2025-01-23 at 10 51 11 AM" src="https://github.com/user-attachments/assets/bf61aa9b-d246-40fb-ab72-19a0e4fe4d7e" />

### Step 5: Configure Agents (Workers)
- Navigate to Admin Panel -> Agents -> Add New.
- Add agents:
  - Jane (Dept: SysAdmins)
  - John (Dept: Support)
 
<img width="500" alt="Screenshot 2025-01-23 at 10 52 40 AM" src="https://github.com/user-attachments/assets/3bd02a07-516c-487c-a125-8b9a63159fca" />
<img width="559" alt="Screenshot 2025-01-23 at 10 52 56 AM" src="https://github.com/user-attachments/assets/39bfc106-1a9a-4085-a932-47dc1b35a8d2" />
<img width="572" alt="Screenshot 2025-01-23 at 10 53 43 AM" src="https://github.com/user-attachments/assets/ecde1247-be9a-443e-a808-c0897ccfe4cc" />
<img width="534" alt="Screenshot 2025-01-23 at 10 53 57 AM" src="https://github.com/user-attachments/assets/ea57ba21-029f-4ed5-9540-9316843e3849" />


### Step 6: Configure Users (Customers)
- Navigate to Agent Panel -> Users -> Add New.
- Add users:
  - Karen
  - Ken

 <img width="668" alt="Screenshot 2025-01-23 at 10 55 11 AM" src="https://github.com/user-attachments/assets/206151c8-f6ce-4b02-8867-5b4d5f942857" />
<img width="626" alt="Screenshot 2025-01-23 at 10 55 39 AM" src="https://github.com/user-attachments/assets/b5f4d93b-8314-44a9-9734-0b552e120a3c" />


### Step 7: Configure SLA
- Navigate to Admin Panel -> Manage -> SLA.
- Create SLAs:
  - Sev-A (Grace Period: 1 hour, Schedule: 24/7)
  - Sev-B (Grace Period: 4 hours, Schedule: 24/7)
  - Sev-C (Grace Period: 8 hours, Business Hours)

<img width="657" alt="Screenshot 2025-01-23 at 10 56 37 AM" src="https://github.com/user-attachments/assets/b3e82dc9-8f86-4376-af93-d00097f34cf6" />
<img width="630" alt="Screenshot 2025-01-23 at 10 56 50 AM" src="https://github.com/user-attachments/assets/5e57a1cf-44ed-406d-aa0b-1f7cadac2343" />
<img width="655" alt="Screenshot 2025-01-23 at 10 57 01 AM" src="https://github.com/user-attachments/assets/65d45620-f0e4-4d95-a572-2b114a2920c4" />


### Step 8: Configure Help Topics
- Navigate to Admin Panel -> Manage -> Help Topics.
- Add help topics:
  - Business Critical Outage
  - Personal Computer Issues
  - Equipment Request
  - Password Reset
  - Other
  <img width="638" alt="Screenshot 2025-01-23 at 10 57 35 AM" src="https://github.com/user-attachments/assets/1c6ceb7d-2df0-4f65-9190-456ce9a422a9" />
<img width="615" alt="Screenshot 2025-01-23 at 10 58 15 AM" src="https://github.com/user-attachments/assets/20cf716b-9eb3-49f2-95ad-7a9db573dca1" />


## Conclusion
These steps complete the post-installation setup for osTicket. With these configurations, you can manage your help desk efficiently and ensure a smooth workflow for both agents and users.
