<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Enabling and Unlocking Accounts using Active Directory Deployed in the Cloud (Azure)</h1>
In this home lab, I will simulate a locked-out user account after many failed attempts to log in (incorrect password) and unlock the account within Active Directory as an admin. I will also configure the Account Lockout Threshold in Group Policy and observe logs.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

Dealing with Account Lockouts

Get logged into dc-1

Pick a random user account you created previously

Configure Group Policy to Lockout the account after 5 attempts:

How To Configure Account Lockout Threshold in Group Policy

 ![image](https://github.com/user-attachments/assets/f77227a0-5f02-4711-907f-911a9937ecc4)


Attempt to log in with it 6 times with a bad password

Observe that the account has been locked out within Active Directory

Unlock the account

Reset the password

Attempt to login with it

 ![image](https://github.com/user-attachments/assets/31034cff-fd89-4bdc-b5b7-19204a748e60)


Enabling and Disabling Accounts

Disable the same account in Active Directory

Attempt to login with it, observe the error message

Re-enable the account and attempt to login with it.

![image](https://github.com/user-attachments/assets/d22ca58e-e019-4199-8de8-6a279f01b94e)
 


Observing Logs

Observe the logs in the Domain Controller

Observe the logs on the client Machine

 ![image](https://github.com/user-attachments/assets/12f9f634-8afd-439f-9b83-d34dca61dda4)

<h2>Takeaways and Key Skills Developed</h2>
In this project, I gained hands-on experience managing user accounts in Active Directory within a cloud environment on Microsoft Azure. I learned how to configure the Account Lockout Threshold using Group Policy, simulating a scenario where an account is locked after multiple failed login attempts and then unlocking it as an admin. I also explored disabling and re-enabling accounts, resetting passwords, and troubleshooting access issues. By observing logs on both the Domain Controller and client machines, I learned how to track and address user login problems. Working with Azure Virtual Machines and Remote Desktop helped me practice managing a cloud-based environment and remote administration. Overall, this project gave me valuable skills in Active Directory management, security settings, and log analysis, which are essential as I continue working toward becoming a Cloud Support Engineer.
