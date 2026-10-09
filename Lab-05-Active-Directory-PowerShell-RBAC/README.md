# Lab 5 – Active Directory, PowerShell & RBAC

## Project Overview
This hands-on IAM lab demonstrates how PowerShell can be used to inspect Active Directory users, security groups, and role-based access assignments in a Windows Server 2022 domain environment.

## Lab Environment
- Windows Server 2022
- Active Directory Domain Services (AD DS)
- Windows PowerShell
- VMware Workstation Player
- Domain: jmc-local
- Domain Controller: JMC-DC01

## Objectives
- Verify Active Directory user accounts using PowerShell.
- Review security group membership.
- Validate role-based access assignments.
- Demonstrate least-privilege access management.
- Document IAM administration and verification procedures.

## PowerShell Commands Used

```powershell
Get-ADUser -Filter * | Select-Object Name, SamAccountName

Get-ADGroupMember -Identity "GG-IT-Support"

Get-ADGroupMember -Identity "GG-IT-HelpDesk"

Get-ADGroup -Identity "GG-Privileged-IT-Admins" -Properties GroupScope, GroupCategory
```

## Lab Verification
Active Directory queries identified test users and verified membership in IT Support and HelpDesk security groups. Group properties were reviewed to support RBAC validation.

## Security Concepts Demonstrated
- Identity and Access Management (IAM)
- Role-Based Access Control (RBAC)
- Least Privilege
- Active Directory Administration
- PowerShell-Based Identity Auditing

## Results
Successfully reviewed Active Directory user accounts, group memberships, and security group properties using PowerShell.

## Documentation
Supporting screenshots and lab evidence will be added to this repository.
