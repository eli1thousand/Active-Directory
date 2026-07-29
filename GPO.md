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



<p>Access Group Policy Management. Underneath your domain, create a GPO (Group Policy Object). Since this policy will prevent users from changing the wallpaper, I willbe naming this GPO Wallpaper Policy. </p>
<img width="535" height="341" alt="Screenshot 2026-07-27 125828" src="https://github.com/user-attachments/assets/aae723d8-6d2a-43d4-8184-2dd2aa0fee21" />

<p>Now we will edit this policy. Because this will apply to all users on the network, this will be under User Configuration and policies. </p>
<img width="535" height="341" alt="Screenshot 2026-07-27 130342" src="https://github.com/user-attachments/assets/dffc7b59-e93e-48f9-834b-45e7aae7b03c" />

<p> Now, Under Policies, we will open the the Administrative Template folder and then Desktop folder. </p>
<img width="535" height="341" alt="Screenshot 2026-07-27 130923" src="https://github.com/user-attachments/assets/5dcce0cc-ab6e-4d27-8673-9f5e3bd2acdb" />

<p>Within this folder, I will select "Desktop Wallpaper" and then enable configuration. I then set a wallpaper as admin. This shall not be changed by any user.  </p>
<img width="345" height="341" alt="Screenshot 2026-07-27 133236" src="https://github.com/user-attachments/assets/4a3f9392-fa94-481c-a792-90562574669d" />

<h3>Task: Restrict USB Devices</h3>
<p>Once again, I will acess Group Policy Management and create a new GPO titled Disable USB Devices. </p>
<img width="340" height="225" alt="Screenshot 2026-07-27 134439" src="https://github.com/user-attachments/assets/64a26296-a2f7-4f9d-b2db-8999a24e6288" />

<p>This will then be edited. This GPO will be underneath Computer COnfiguration policies. Then we will select Administrative Templates and System. Withiin System, I will find and select Removable Storage Access. </p>
<img width="345" height="260" alt="Screenshot 2026-07-27 134747" src="https://github.com/user-attachments/assets/b1ef5f3a-79c5-48be-960c-da7e2385b11e" />

<p>I locate "All Removable Storage classes: Deny all access" and enable this feature. </p>
<img width="343" height="321" alt="Screenshot 2026-07-27 135434" src="https://github.com/user-attachments/assets/2b794507-ae30-416f-b144-30ab3834aca8" />

<h3>Task: Account Lockout</h3>
<p>We return to Group Policy Management where we create and edit another GPO  titled "Account Lockout Policy". However, because this policy affects the domain accounts, this policy will be underneath Default Domain Policy. </p>
<p>Because this involves authentiaction, this will be a computer configuration policy. Underneath this policy, I will navigate through Windows Settings, Security Settings, Account Policies, and then Account Lockout Policy. </p>
<img width="455" height="316" alt="Screenshot 2026-07-29 122033" src="https://github.com/user-attachments/assets/ee2bfc65-ccb3-429e-800d-61014af1eeb2" />


<p>Here, I made the lockout time 10 minutes, the threshold for incorrect passwords 3 attempts, and reset account lockout timer 5 minutes.  </p>
<img width="200" height="150" alt="Screenshot 2026-07-27 142044" src="https://github.com/user-attachments/assets/ef3df219-24ad-4c91-a734-c0cfd0f0361b" />
<img width="200" height="150" alt="Screenshot 2026-07-27 142224" src="https://github.com/user-attachments/assets/c6d06a93-fd5f-476b-8d90-edf604fc89fb" />
<img width="200" height="150" alt="Screenshot 2026-07-27 142714" src="https://github.com/user-attachments/assets/58206589-fce3-48d3-a4e3-ebe5847d89c1" />




