# Active Directory Home Lab & IT Support Simulation

## Project Overview

This project documents a hands-on Active Directory lab built with VirtualBox, Windows Server 2025, and Windows 11 Pro.

The lab was created to practice Active Directory administration and common IT support tasks, including user account management, group membership, domain joining, account troubleshooting, and shared-folder access.

## Environment

| Component | Configuration |
|---|---|
| Virtualization | Oracle VirtualBox |
| Server | Windows Server 2025 |
| Client | Windows 11 Pro |
| Server Name | DC01 |
| Directory Service | Active Directory Domain Services (AD DS) |
| Network | VirtualBox network adapter with a static IP configured on the server |

## Project Objectives

- Build a Windows Server and Windows 11 virtual lab environment
- Configure a Windows Server as an Active Directory Domain Controller
- Create Organizational Units, users, and groups
- Join a Windows 11 client to the domain
- Practice common Active Directory support tasks
- Troubleshoot a Windows 11 virtualization/boot display issue
- Configure shared HR folder access for an HR group

## What I Practiced

### Active Directory Administration

- Installed Active Directory Domain Services
- Configured the server as a Domain Controller
- Created `Accounts` and `Groups` Organizational Units
- Created users in the `Accounts` OU
- Created groups in the `Groups` OU
- Joined a Windows 11 client machine to the domain

### IT Support Scenarios

I simulated common Active Directory support tickets:

1. Password reset
2. Locked user account
3. Account enable/disable
4. Adding a user to a specific group
5. Shared HR folder access and mapping the folder to the client machine

## Troubleshooting Example

During Windows 11 installation in VirtualBox, the virtual machine displayed a black screen.

The issue was resolved by:

- Changing the display graphics controller to `VMSVGA`
- Increasing video memory to `256 MB`
- Correcting the boot order so the appropriate hard drive was selected

## Lab Structure

```text
Active Directory Environment
│
├── Domain Controller
│   └── DC01
│       ├── Accounts OU
│       │   └── Users
│       │
│       └── Groups OU
│           └── Security Groups
│
└── Windows 11 Client
    └── Joined to Domain
```

## IT Support Workflow Practiced

```text
User reports issue
       │
       ▼
Identify account / access problem
       │
       ▼
Check Active Directory
       │
       ├── Password issue → Reset password
       │
       ├── Account locked → Unlock account
       │
       ├── Account status → Enable / Disable
       │
       ├── Access issue → Check group membership
       │
       └── HR access → Assign HR group / map shared folder
```

## Documentation

- [Lab Setup](01-Lab-Setup/lab-setup.md)
- [Active Directory Configuration](02-Active-Directory/active-directory.md)
- [IT Support Tickets](03-IT-Support-Tickets/it-support-tickets.md)

## Skills Demonstrated

- Windows Server administration
- Active Directory administration
- User and group management
- Organizational Unit management
- Domain joining
- Account troubleshooting
- Password resets
- Account lockout troubleshooting
- Account enable/disable
- Group membership management
- Shared-folder access
- Windows virtualization troubleshooting

## Disclaimer

This is a personal lab project created for hands-on learning and portfolio purposes. User names, groups, and organizational information used in the lab are test/lab data.

## Screenshots

Screenshots can be added to the folders under `screenshots/` to provide visual evidence of the lab configuration.

Suggested screenshots:

- Windows Server `DC01`
- Active Directory Users and Computers
- `Accounts` and `Groups` OUs
- Test users and groups
- Windows 11 domain membership
- Password reset / account unlock
- HR group membership
- Mapped HR folder
