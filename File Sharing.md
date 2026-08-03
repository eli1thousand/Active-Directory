<h1>Active Directory: File Sharing</h1>

<h2>Objective</h2>
<p>In this lab, I will be utilizing a Virtual Machine sandbox to simulate the tasks and managements of help desk specialist. I will be using Virtual Box, Active Directory, Windows Server 2022, and Windows 10 for this lab. Here, I will be demonstrating File Sharing. Here, I act as admin and in instances where a members or users must have access to a shared folders and files.   <p>
<h3>Materials</h3>
<ul>
  <li>Virtual Box</li>
  <li>Active Directory</li>
  <li>Windows Server 2022</li>
  <li>Windows 10</li>
</ul>

<h3>Task</h3>
<p>I create a shared folder in my server. I do this by opening file explorer and "This PC". In This PC, I will create a new folder, "shares" and within this folder will be a "Finance" folder. </p>
<img width="432" height="275" alt="image" src="https://github.com/user-attachments/assets/fc3863af-bba2-40c3-bab7-85ec46265315" />
<p>Now I will click on Properties. Next, I click Sharing and Advanced Sharing. </p>
<img width="250" height="323" alt="image" src="https://github.com/user-attachments/assets/cf82aba2-b7f2-4027-8d75-82afcbc71ce3" />

<p>Next we will establish the Permissions. Once the Permssions are established for who all can access what, we save the network path. This will be used to find the folder. </p>
<img width="313" height="310" alt="image" src="https://github.com/user-attachments/assets/d8ab3e61-e990-40e8-8f26-41b2cf4454a3" />

<p>Let us see if a client can access this document once the network path was searched on their machine. </p>
<img width="444" height="334" alt="image" src="https://github.com/user-attachments/assets/6ae540a8-9224-41df-af80-eba467e27984" />
<img width="444" height="403" alt="image" src="https://github.com/user-attachments/assets/89db386e-addc-4161-a264-a00d8af573bd" />

<p>Success! The client server can access the document!</p>


