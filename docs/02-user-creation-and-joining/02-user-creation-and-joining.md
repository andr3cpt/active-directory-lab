# Module 2: User Creation and Joining
Create users in custom OUs and join the Windows 10 Pro VM to the `lab.local` domain.


## Overview

**1. Set the** `TCP/IPv4` **properties on Windows 10 Pro client VM :** Assign a static IP address (`192.168.50.20`), a Subnet mask of `255.255.255.0` and a DNS address pointing to the `DC-01` DNS resolver (`192.168.50.10`)
<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/01-IPv4-config.png" alt="manual IPv4 setting" width="600" />
</p>
</details>

___

**2. Verify domain DNS resolution using** `nslookup lab.local` confirming it resolves to `192.168.50.10`

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/02-nslookup.png" alt="nslookup test" width="600" />
</p>
</details>

___

**3. Create user within OU hierarchy in ADUC** : `Corp` -> `Users` -> `Luke Skywalker`

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/03-user-creation.png" alt="user creation" width="600" />
</p>
</details>

___

**4. Rename client machine to** `WIN10-PRO` **and join it to the** `lab.local` **domain** 

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/04-join-to-domain.png" alt="join PC to domain" width="600" />
</p>
</details>

___

**5. Move the automatically generated** `WIN10-PRO` **computer object** from the default `Computers` container into `Corp` -> `Workstations` (standard enterprise practice)

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/05-add-AD-workstation.png" alt="add AD workstation" width="600" />
</p>
</details>

___


**6. Verify logon with** `lskywalker` **via CLI**

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/06-verify-logon.png" alt="verify logon to domain" width="600" />
</p>
</details>

___

**7. Create another domain user** `Han Solo` (`hsolo`) inside `Corp` -> `Users`
<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/07-add-han-solo.png" alt="created another user" width="600" />
</p>
</details>
