<h1>Active Directory: Group Policy Management</h1>

<h2>Objective</h2>
<p>In this lab, I will be utilizing a Virtual Machine sandbox to simulate the tasks and managements of help desk specialist. I will be using Virtual Box, Active Directory, Windows Server 2022, and Windows 10 for this lab. Here, I will be demonstrating the tasks of Group Policy Management. Group Policy Management allows the admin to configure the settings for for all computers on a network.   <p>
<h3>Materials</h3>
<ul>
  <li>Virtual Box</li>
  <li>Active Directory</li>
  <li>Windows Server 2022</li>
  <li>Windows 10</li>
</ul>

<h3>Task: Restrict Desktop Wallpaer</h3>
<p>We need to make sure the clients cannot change the wallpaper on their work computers.</p>

<h3>Procedure</h3>

<p>Access Group Policy Management. Underneath your domain, create a GPO (Group Policy Object). Since this policy will prevent users from changing the wallpaper, I willbe naming this GPO Wallpaper Policy. </p>
<img width="535" height="341" alt="Screenshot 2026-07-27 125828" src="https://github.com/user-attachments/assets/aae723d8-6d2a-43d4-8184-2dd2aa0fee21" />

<p>Now we will edit this policy. Because this will apply to all users on the network, this will be under User Configuration and policies. </p>
<img width="535" height="341" alt="Screenshot 2026-07-27 130342" src="https://github.com/user-attachments/assets/dffc7b59-e93e-48f9-834b-45e7aae7b03c" />
<p> Now, Under Policies, we will open the the Administrative Template folder and then Desktop folder. </p>
<img width="535" height="341" alt="Screenshot 2026-07-27 130923" src="https://github.com/user-attachments/assets/5dcce0cc-ab6e-4d27-8673-9f5e3bd2acdb" />
<p>Within this folder, I will select "Desktop Wallpaper" and then enable configuration. I then set a wallpaper as admin. This shall not be changed by any user.  </p>
<img width="345" height="341" alt="Screenshot 2026-07-27 133236" src="https://github.com/user-attachments/assets/4a3f9392-fa94-481c-a792-90562574669d" />

