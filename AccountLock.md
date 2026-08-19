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

<p>Here I set the account lockout to 1 attempt. </p>
<img width="1007" height="696" alt="image" src="https://github.com/user-attachments/assets/6e1b1406-11a9-4b6f-82ef-b4de9d21e7e2" />
