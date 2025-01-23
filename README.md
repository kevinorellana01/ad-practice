<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Active Directory Account Management</h1>
This repository demonstrates various use cases and examples for managing user accounts in Active Directory (AD). It provides step-by-step instructions on common tasks, such as account lockouts, password resets, account enabling/disabling, and log observations.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>Use Cases</h2>

- Account Lockouts
  - How to configure account lockout policies via Group Policy.
  - Simulating account lockouts by attempting multiple failed login attempts.
  - Unlocking a locked account and resetting the password.

- Enabling and Disabling Accounts
  - Disabling and enabling a user account within Active Directory.
  - Observing the behavior and error messages when attempting to log in with a disabled account.

- Log Observations
  - How to observe and analyze security logs from both the Domain Controller and client machine.
  - Identifying failed login attempts, account lockouts, and other relevant events in the logs.

<h2>Instructions</h2>

1. Getting Started
- Log in to the Domain Controller (dc-1) using an administrator account.
- Ensure you have a user account created in Active Directory for testing purposes.
2. Configuring Account Lockout Policies
- Open the Group Policy Management Console (GPMC) and configure the Account Lockout Policy to lock the account after 5 failed login attempts.
- Test by attempting 6 failed logins with a bad password.
3. Account Lockout Behavior
- Observe that the account locks after the 5th failed attempt.
- Unlock the account and reset the password for testing.
4. Enabling and Disabling Accounts
- Disable a user account in Active Directory.
- Attempt to log in with the disabled account and observe the error message.
- Re-enable the account and attempt to log in again.
5. Observing Logs
- View the security logs on the Domain Controller to see the details of login attempts and account lockouts.
- Check the client machine’s event logs for any relevant information regarding login failures.

<h2>Purpose</h2>
The purpose of this repository is to provide hands-on examples and insights into managing Active Directory accounts. It highlights practical scenarios that demonstrate how to configure policies, manage account states, and troubleshoot login issues using various tools and technologies. This repository is designed to help IT professionals and system administrators gain a deeper understanding of Active Directory management.
