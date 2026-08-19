<h1>Active Directory: Account Lockout Durations</h1>

<h2>Objective</h2>
<p>In this lab, I will be utilizing a Virtual Machine sandbox to simulate the tasks and managements of help desk specialist. I will be using Virtual Box, Active Directory, Windows Server 2022, and Windows 10 for this lab. Here, I will be demonstrating password resetting. Here, I act as admin and in instances where a member forgets their password, I simply reset their passwords so they are able to log onto their account.    <p>
<h3>Materials</h3>
<ul>
  <li>Virtual Box</li>
  <li>Active Directory</li>
  <li>Windows Server 2022</li>
  <li>Windows 10</li>
</ul>

<h3>Task</h3>
<p>We need to make sure no one has access all the time. Configure an account lockout policy.</p>

<h4>Procedures</h4>
<p>First I will locate Account Policies by opening Group Policy Management terminal. Next I will locate and edit Default Domain Policy, Underneath Computer Configuration, I will then select Policies, Window Settings, Security Settings, Account Policy, and finally Account Lockout Policy</p>

<img width="1023" height="652" alt="image" src="https://github.com/user-attachments/assets/c5c2734c-35f3-4dd7-8db7-c073d4e920e3" />

<p>Here I set the account lockout to 1 attempt because we're strict around here!. </p>
<img width="1007" height="696" alt="image" src="https://github.com/user-attachments/assets/6e1b1406-11a9-4b6f-82ef-b4de9d21e7e2" />

<p>Now I will force this update by running the command GPUDATE /FORCE in command prompt.</p>
<img width="971" height="527" alt="Screenshot 2026-08-19 091955" src="https://github.com/user-attachments/assets/ceebf99c-f949-42aa-8e99-f1b3aa360b46" />

<p>Now we will have Michael test if the lockout is effective and it is!.</p>
<img width="1022" height="760" alt="Screenshot 2026-08-19 092249" src="https://github.com/user-attachments/assets/d4db542c-3c6c-4958-8c34-a8e61b555faa" />

<p>After 3 minutes of account lockout, Michael should now be able to try again to log in.</p>
<img width="1010" height="777" alt="image" src="https://github.com/user-attachments/assets/35bacda4-f5af-4b01-ba64-0c8cf1578e18" />
