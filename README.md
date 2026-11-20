# Active Directory Home Lab

A system administration lab focused on deploying, managing, and securing a Windows Server Active Directory environment using both GUI tools and PowerShell.<br />


## Lab Setup

| Item | Details |
| :--- | :--- |
| **Environment** | VMware Fusion on macOS |
| **Domain Controller (`DC-01`)** | Windows Server 2022 |
| **Client VMs (`WIN10-PRO`, `WIN-DHCP`)** | Windows 10 Pro |
| **Domain Name** | `lab.local` |

`WIN10-PRO` is joined to `lab-local` via static IP; `WIN-DHCP` is joined to the domain via a DHCP lease by the domain.


## Modules

| # | Name |
| :--- | :--- |
| **1** | [Core Infrastructure and Domain Controller Setup](docs/01-dc-setup/01-dc-setup.md) |
| **2** | [User Creation and Client Join (static IPv4)](docs/02-user-creation-and-client-join-static-IPv4/02-user-creation-and-client-join-static-IPv4.md)|
| **3** | [User Lockout Management](docs/03-user-lockout-management/03-user-lockout-management.md) |
| **4** | [Password Policy and Delegation](docs/04-pswd-policy-and-delegation/04-pswd-policy-and-delegation.md) |
| **5** | [Shares and Permissions](docs/05-shares-and-permissions/05-shares-and-permissions.md) |
| **6** | [Drive Mapping](docs/06-drive-mapping/06-drive-mapping.md) |
| **7** | [Group Policy and Workstation Hardening](docs/07-GPO-workstation-hardening/07-GPO-workstation-hardening.md) |
| **8** | [DHCP Configuration and Client Join (DHCP lease)](docs/08-DHCP-config-and-join-lease/08-DHCP-config-and-join-lease.md) |

