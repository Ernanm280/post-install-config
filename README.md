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
<img width="948" height="543" alt="Screenshot 2026-02-26 202202" src="https://github.com/user-attachments/assets/955f20e8-2be5-43cb-9c4e-aad1de18a94d" />
<img width="946" height="432" alt="Screenshot 2026-02-26 204319" src="https://github.com/user-attachments/assets/876ac459-a9a2-428a-b33a-9c60bad7afc4" />



### Step 2: Configure Departments
- Navigate to Admin Panel -> Agents -> Departments.
- Create departments for ticket visibility:
  - Example: SysAdmins
 
<img width="945" height="1098" alt="Screenshot 2026-02-26 204757" src="https://github.com/user-attachments/assets/d1fce6dc-8fc2-4a26-b17a-32f42f19a8cb" />
<img width="948" height="280" alt="Screenshot 2026-02-26 204847" src="https://github.com/user-attachments/assets/eaa2b8bc-f877-4a09-9e37-f06b62543d5e" />


### Step 3: Configure Teams
- Navigate to Admin Panel -> Agents -> Teams.
- Create a team and pull agents from different departments:
  - Example: Online Banking

<img width="936" height="662" alt="Screenshot 2026-02-26 205125" src="https://github.com/user-attachments/assets/96bd15e1-f882-445e-8227-b830417689aa" />


### Step 4: User Settings
- Navigate to Admin Panel -> Settings -> User Settings.
- Configure ticket creation settings:
  - Uncheck: Require registration and login to create tickets.  (Unregistered users can create tickets.)

<img width="675" height="674" alt="Screenshot 2026-02-26 205514" src="https://github.com/user-attachments/assets/12772c00-a1ee-4fe5-974d-e71b4b89303b" />


### Step 5: Configure Agents (Workers)
- Navigate to Admin Panel -> Agents -> Add New.
- Add agents:
  - Jane (Dept: SysAdmins)
  - John (Dept: Support)
 
<img width="953" height="470" alt="Screenshot 2026-02-26 210220" src="https://github.com/user-attachments/assets/ecf2b7d7-b7e6-4980-9035-f29bce8dc241" />
<img width="942" height="526" alt="Screenshot 2026-02-26 210615" src="https://github.com/user-attachments/assets/87188bab-e0d0-4814-8242-34251184e8bf" />
<img width="948" height="466" alt="Screenshot 2026-02-26 210745" src="https://github.com/user-attachments/assets/94891550-7264-41f7-bf69-6ea88b9a5967" />
<img width="949" height="369" alt="Screenshot 2026-02-26 210803" src="https://github.com/user-attachments/assets/f7a65a3a-5856-4a8a-b393-80969777fba1" />

### Step 6: Configure Users (Customers)
- Navigate to Agent Panel -> Users -> Add New.
- Add users:
  - Karen
  - Ken

 <img width="806" height="515" alt="Screenshot 2026-02-26 211625" src="https://github.com/user-attachments/assets/f140ac32-d3ae-4bdf-b940-9d09da1a1f8b" />
<img width="681" height="334" alt="Screenshot 2026-02-26 211819" src="https://github.com/user-attachments/assets/e07adfa3-9093-4349-8d19-d2c5be8edd0b" />

### Step 7: Configure SLA
- Navigate to Admin Panel -> Manage -> SLA.
- Create SLAs:
  - Sev-A (Grace Period: 1 hour, Schedule: 24/7)
  - Sev-B (Grace Period: 4 hours, Schedule: 24/7)
  - Sev-C (Grace Period: 8 hours, Business Hours)

<img width="953" height="397" alt="Screenshot 2026-02-26 212235" src="https://github.com/user-attachments/assets/1165e955-819d-438e-9fce-bf0848f028bd" />

### Step 8: Configure Help Topics
- Navigate to Admin Panel -> Manage -> Help Topics.
- Add help topics:
  - Business Critical Outage
  - Personal Computer Issues
  - Equipment Request
  - Password Reset
  - Other
  
<img width="628" height="624" alt="Screenshot 2026-02-26 212637" src="https://github.com/user-attachments/assets/37b01ba3-c7d0-48d6-91bb-ba67729d76a2" />
<img width="947" height="736" alt="Screenshot 2026-02-26 213226" src="https://github.com/user-attachments/assets/d8369beb-1e80-4f9c-876a-0a4ed46e2d65" />

## Conclusion
These steps complete the post-installation setup for osTicket. With these configurations, you can manage your help desk efficiently and ensure a smooth workflow for both agents and users.
