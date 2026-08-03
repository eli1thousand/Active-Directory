<h1>Active Directory: Password Resetting</h1>

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
<p>Leather Face once again forgot his password to his work PC. This is a reoccuring issue so Mr. Face may need to be able to change his password to something simple and remomorable. </p>
<p>To begin, we are going to access Users and Computers</p>
<img width="425" height="217" alt="image" src="https://github.com/user-attachments/assets/24663b4a-aaab-472c-be40-8d415c578aae" />

<p>Now we are going to locate the user. Leatherface is located under Doctors. Here I will select his user profile and right-click it. u</p>
<img width="439" height="342" alt="image" src="https://github.com/user-attachments/assets/aa8dae40-5718-4208-8743-6b7590c2f7ef" />

<p>Leatherface is now given a temporary password that will allow him to sign-in and create a new password for his account. </p>
<img width="432" height="275" alt="image" src="https://github.com/user-attachments/assets/5b608a99-610d-4595-8cab-a71d87a6060c" />
<img width="432" height="275" alt="Screenshot 2026-07-29 141710" src="https://github.com/user-attachments/assets/d8c59e15-e791-45be-8f12-ae5b1476c465" />

<h3>PowerShell</h3>
<p>A more efficient way of resetting passwords is through PowerShell. Utilizing the command Set-ADAccountPassword followed by the name and -Reset. You are able to change and update passwords from the PS Window. Here, we are going to change GhostFace's password. </p>
<img width="432" height="275" alt="image" src="https://github.com/user-attachments/assets/2d24eb7c-f143-4fdc-8f94-5881d96ac7d1" />

<p>To allow the user to update their password, you will run the command Set-ADUser </p>
<img width="432" height="275" alt="image" src="https://github.com/user-attachments/assets/54575309-2180-4fc6-8349-85af19d56bf6" />
<img width="432" height="275" alt="Screenshot 2026-08-03 191848" src="https://github.com/user-attachments/assets/5c516071-b245-463c-8412-f874a923fe5a" />

<p>Ghostface can now log in!</p>
<img width="432" height="275" alt="Screenshot 2026-08-03 191928" src="https://github.com/user-attachments/assets/e2fa385e-62c6-4769-8d3c-a0b4a94de62b" />
