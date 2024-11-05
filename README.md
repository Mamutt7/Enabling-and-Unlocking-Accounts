# Lab-5.3-Enabling-and-Unlocking-Accounts
In this home lab, I will simulate a locked-out user account after many failed attempts to log in (incorrect password) and unlock the account within Active Directory as an admin. I will also configure the Account Lockout Threshold in Group Policy and observe logs.


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


