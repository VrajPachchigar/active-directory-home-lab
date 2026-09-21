# Lab Setup

## 1. VirtualBox Installation

Oracle VirtualBox and the VirtualBox Extension Package were installed on a Windows 11 machine.

## 2. Windows 11 Pro Virtual Machine

A Windows 11 Pro virtual machine was created in VirtualBox.

### Troubleshooting: Black Screen

During the Windows 11 installation, the virtual machine displayed a black screen.

The issue was resolved by:

1. Changing the display graphics controller to `VMSVGA`
2. Increasing video memory to `256 MB`
3. Correcting the boot order in the boot manager so the correct hard drive was selected

After these changes, the black screen issue was resolved.

## 3. Windows Server 2025

Windows Server 2025 was installed as the server virtual machine.

## 4. Server Configuration

The server was:

- Renamed to `DC01`
- Configured with VirtualBox network adapter settings
- Assigned a static IP address

The server was then prepared for Active Directory Domain Services installation.

## Lab Components

```text
Windows 11 Host
      │
      ▼
   VirtualBox
    ┌───────┴────────┐
    ▼                ▼
Windows Server    Windows 11 Pro
   DC01              Client
```
