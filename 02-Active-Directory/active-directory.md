# Active Directory Configuration

## Active Directory Domain Services

Active Directory Domain Services (AD DS) was installed on Windows Server 2025.

The server was configured as the Domain Controller for the lab environment.

## Organizational Units

Two Organizational Units were created:

```text
Accounts
Groups
```

## Users

Two test users were created inside the `Accounts` OU.

## Groups

Two test groups were created inside the `Groups` OU.

## Windows 11 Domain Join

The Windows 11 client machine was joined to the Active Directory domain controlled by `DC01`.

This allowed the client machine to operate as a domain-joined workstation in the lab environment.

## Result

The completed lab included:

- Windows Server 2025 Domain Controller
- Windows 11 Pro domain client
- `Accounts` OU
- `Groups` OU
- Test user accounts
- Test groups
- Domain-joined Windows 11 workstation
