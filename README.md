<p align="center">
<img width="350" height="350" alt="image" src="https://github.com/user-attachments/assets/64682542-313e-4d29-b846-fd0c2cb95e80" />
</p>

<h1>osTicket - Post-Install Configuration</h1>
In this project, I will be configuring the open-source ticketing system osTicket for use in my "osTicket-Simulation" project (installation completed in the osTicket-Install project). The the resources used and objectives of this project are listed below.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- osTicket (Open Source Ticketing System)

<h2>Operating Systems Used </h2>

- Windows 11</b> (24H2)

<h2>Configuration Objectives</h2>

- Configure Roles (for grouping permissions)
- Configure Departments (to simulate a large company with multiple IT branches)
- Configure Teams (to group agents from different departments)
- Confiure Agents (individual employees)
- Configure End-Users (customers)
- Configure SLA (to determine the severity of a ticket)
- Configure Help Topics (to better sort/classify incoming tickets)

<h2>Configuration Steps</h2>

<p>
<img width="1568" height="557" alt="image" src="https://github.com/user-attachments/assets/a7329de1-0023-41ba-8ef7-fd46b594e9de" />

</p>
<p>
To start, I loaded the osTicket Staff Control Panel from the browser of my virtual machine. Upon logging in, I was greeted with the Tickets page within the Agent Panel.
</p>
<br />

<p>
<img width="1197" height="705" alt="image" src="https://github.com/user-attachments/assets/f5d4d2b6-cc4d-4fdb-96bf-898c133c4afe" />

</p>
<p>
I then clicked the Admin Panel button in the top right of the page. Being in the Admin Panel allows for the creation of new agents, teams, roles, and departments. In addition, I can assign Agents a team, role, or department and assign permissions. In this step, I went to the Role tab under the Agents page (all within the Admin Panel) and added a new role called "Supreme Admin." I also added the description "Full permissions" as an internal note.
</p>
<br />

<p>
<img width="863" height="768" alt="image" src="https://github.com/user-attachments/assets/2086f2ea-7356-4d53-a4b8-ec00cb35b6de" />

</p>
<p>
Next, I went to the permissions tab of the Supreme Admin role and checked every box. This will ensure that any user with the Supreme Admin role will have full access to all incoming tickets. I then clicked the Add Role button to offically create the role. 
</p>
<br />

<p>
<img width="856" height="816" alt="image" src="https://github.com/user-attachments/assets/38381446-16a4-4b2a-8b70-cdce87310aa9" />

</p>
<p>
I then went to the Departments tab on the Agents page to create a new department titled "System Admins." I set the Parent value to Top-Level Deparment and kept everything else the same for now.
</p>
<br />

<p>
<img width="906" height="811" alt="image" src="https://github.com/user-attachments/assets/36793b4a-fbb1-4822-bca0-10ef7c029d5f" />

</p>
<p>
Next, I went to the Teams tab on the Agents page and created a new team called Online Banking.
</p>
<br />

<p>
<img width="927" height="782" alt="image" src="https://github.com/user-attachments/assets/c6eaa2c1-96e1-4f00-8984-f527ee8f6bf7" />

</p>
<p>
To prepare for the creation of Agents and Users, I went to the Users tab on the Settings page and unchecked the Registration Required box (I did this for the sake of ease in this project).
</p>
<br />

<p>
<img width="896" height="746" alt="image" src="https://github.com/user-attachments/assets/471997a7-5ceb-472c-9298-b888c270d7d5" />

</p>
<p>
I then went to the Agents tab on the Agents page to create an account for my helpdesk's first employee. I named the Agent "Jane Doe" and provided some filler information.
</p>
<br />

<p>
<img width="1022" height="627" alt="image" src="https://github.com/user-attachments/assets/7fde7b60-9317-4633-8f55-74f59da0d911" />

</p>
<p>
After adding the account information, I went to the access tab and made Jane part of the System Admins Department. I also gave her Supreme Admin level access and made her part of the online banking team. Finally, I clicked the create button and Jane was offically added to the helpdesk.
<br />

<p>
<img width="1215" height="660" alt="image" src="https://github.com/user-attachments/assets/703c5d52-a14d-4a36-b8e2-b7c5992dd9c7" />

</p>
<p>
I then went through the same process but for an Agent named "John Doe." I made John part of the Support Department, but set his access to view only. 
</p>
<br />

<p>
<img width="1176" height="381" alt="image" src="https://github.com/user-attachments/assets/86eae074-cce5-47ad-b88b-606472a1c3fa" />

</p>
<p>
After I clicked create for John, the helpdesk Agents were all set up for this project. 
</p>
<br />

<p>
<img width="1207" height="747" alt="image" src="https://github.com/user-attachments/assets/1cb04003-16ef-44a8-88ba-84c462fe78c2" />

</p>
<p>
I then went to the Users page and clicked the Add User button to configure an account for an end-user. I named the user Karen, put in some filler information, and clicked the Add User button. 
</p>
<br />

<p>
<img width="1178" height="463" alt="image" src="https://github.com/user-attachments/assets/4a02295a-7686-42dc-8734-90f0b2233dab" />

</p>
<p>
On the User Directory tab, you can view Karen's information, create a ticket using her account, register or delete the user, add internal notes, view previous tickets, and more. 
</p>
<br />

<p>
<img width="1197" height="786" alt="image" src="https://github.com/user-attachments/assets/eb04348a-d9fe-4ba5-a2e9-fbba8e50a431" />

</p>
<p>
Next, it was time to add some SLAs for my helpdesk. I went to the SLA tab under the Manage page, and clicked the Add New SLA Plan button. I named the first SLA "SevA" to represent the highest level of priority for incoming tickets. I gave the SLA a grace period of one hour, meaning there needs to be hourly updates on any SevA ticket. I also scheduled SevA tickets to be open 24/7, as these would be issues of great importance that need to be handled as soon as possible. Finally, I wrote a brief internal note and clicked the Add Plan button to finalize. 
</p>
<br />

<p>
<img width="1208" height="518" alt="image" src="https://github.com/user-attachments/assets/7ce2bea2-5dd9-4edd-b66d-ba1aee7295c7" />

</p>
<p>
I then proceeded to create SLAs for SevB and SevC. SevB was created for moderately high priority tickets, and SevC was created for low priority tickets. All SLA plans are viewable and changeable on the SLA tab. These plans will help organize incoming tickets based on their perceived business impact. SevC tickets will be the most common, and will likely be processed in the order they are recieved.
</p>
<br />

<p>
<img width="1197" height="766" alt="image" src="https://github.com/user-attachments/assets/1f0c7b23-e01d-4d1e-9e3f-288f51645525" />

</p>
<p>
Next, I went to the Help Topics tab in the Manage page to create some new help topics. I clicked the Add New Help Topic button and labled the new topic "Business Critical Outage." I set the parent topic as Report a Problem, and added some brief internal notes. This specific help topic is meant to be used in the case of a critical problem that has a large effect on the business as a whole. 
</p>
<br />

<p>
<img width="1196" height="782" alt="image" src="https://github.com/user-attachments/assets/e27a8957-1abf-4c5e-bac2-106f24e0bd66" />

</p>
<p>
Finally, I created four more help topics: Equipment Request, Password Reset, Personal Computer Issues, and Other. The Help Topics tab will show all of the created topics as well as some default ones, and they can be sorted and edited as needed. This concludes the Post-Install Configuration Project. 
</p>
<br />

