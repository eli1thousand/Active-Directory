<h1>Active Directory: Network Mapping</h1>

<h2>Objective</h2>
<p>In this lab, I will be utilizing a Virtual Machine sandbox to simulate the tasks and managements of help desk specialist. I will be using Virtual Box, Active Directory, Windows Server 2022, and Windows 10 for this lab. Here, I will be demonstrating network mapping. This allows certain users to shared access to folders and files within a network.   <p>
<h3>Materials</h3>
<ul>
  <li>Virtual Box</li>
  <li>Active Directory</li>
  <li>Windows Server 2022</li>
  <li>Windows 10</li>
</ul>

<h3>Task</h3>
<p>The monthly information for the upcoming quarter is here. We will need all managers of the departments to be able to access this folder.</p>

<h3>Procedure</h3>

<h4>Server</h4>
<p> On Server PC, we are going to access File Explorer. On This PC, we are going to select and add a mapped network. This will be titled Managers. The location for this folder will be \\Piedmont-PC\Managers. </p>
<img width="468" height="345" alt="Netmap1" src="https://github.com/user-attachments/assets/4fce06e4-cfe2-41ad-a14f-cea9040325a3" />
<p> We are going to right-click the folder and then go to Properties and then Sharing. We will then check the "Share this folder" box so sharing is possible.</p>
<img width="475" height="371" alt="Netmap2" src="https://github.com/user-attachments/assets/0e726853-cc2c-44ea-9e7b-1aebf15b1ac5" />
<p>Now we name this folder. I will stick with the name MANAGERS. Next, we need to grant permissions. Here we will add all of the managers who need access to this folder. Here, I only gave them access to read what is inside the folder. It is imperative that you remove "Everyone" when adding the proper users. </p>
<img width="475" height="353" alt="Netmap4" src="https://github.com/user-attachments/assets/1d5e3f9d-28dc-4a7a-a111-1237ee50b0cd" />



<p>Now, we are going to access Group Policy Management in Windows Administrative Tools. Underneath the domain, we are going add a new Group Policy Object. This will be titled "Mapped Drives". </p> 
<img width="500" height="345" alt="Netmap2 1" src="https://github.com/user-attachments/assets/5b133ff4-0011-454b-bcd6-559dae52aa3f" />
<p>Next, we are going to edit this GPO so the configuration corresponds to the correct tabs The mapped drive will be under User & Preferences.</p> 
<img width="500" height="345" alt="Netmap2 2" src="https://github.com/user-attachments/assets/ed68c56d-2eb8-4222-82e8-d3668abc1119" />
<p>Here, under User Preferences, we will then select Windows Settings and then open Drive Maps</p>
<img width="500" height="345" alt="Netmap2 3" src="https://github.com/user-attachments/assets/736bb0f8-e769-42f1-ae23-da30e220aced" />
<p>Now, we will create a new Mapped Drive. The location of this will be \\Piedmont-PC\Managers.  </p>
<img width="500" height="345" alt="Netmap2 4" src="https://github.com/user-attachments/assets/f842526e-8c94-4ae8-9893-1087101ab7fb" />
<p>Once this network map is created, we now go to our GP Management. Under GPO, our Drive Mapped folder should be present. We drag this map into each OU that possesses the users with access to this folder.</p>
<img width="500" height="345" alt="netmap2 5" src="https://github.com/user-attachments/assets/a38f2b14-1b6d-4869-9168-a721814883e1" />

<h4>Client</h4>
<p>On the Client PC, we are going to log on as the manager of Finance, Donatello. We are going to access File and Explorer. We can see that the map has now been shared with Donatello's PC.</p> 
<img width="501" height="345" alt="Screenshot 2026-07-10 195212" src="https://github.com/user-attachments/assets/74c662c1-66b6-4c27-bf98-162ba6f6ff52" />

