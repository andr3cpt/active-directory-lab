# Module 2: User Creation and Joining
Created users in custom OUs and joined the Windows 10 Pro VM to the `lab.local` domain.


## Overview

**1. Set the TCP/IPv4 properties on Windows 10 Pro client VM :** Assigned a static IP address (`192.168.50.20`), a Subnet mask of `255.255.255.0` and a DNS address pointing to the `DC-01` DNS resolver (`192.168.50.10`)
<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/01-IPv4-config.png" alt="manual IPv4 setting" width="600" />
</p>
</details>

___

**2. Verified domain DNS resolution using 'nslookup lab.local'** confirming it resolved to `192.168.50.10`

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/02-nslookup.png" alt="nslookup test" width="600" />
</p>
</details>

___

**3. Created user within OU hierarchy in ADUC** : 'Corp -> Users -> Luke Skywalker'

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/03-user-creation.png" alt="user creation" width="600" />
</p>
</details>

___

**4. Renamed client machine to** `WIN10-PRO` **and joined it to the** 'lab.local' **domain** 

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/04-join-to-domain.png" alt="join PC to domain" width="600" />
</p>
</details>

___

**5. Moved the automatically generated** `WIN10-PRO` **computer object** from the default 'Computers' container into 'Corp -> Workstations'

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/05-add-AD-workstation.png" alt="add AD workstation" width="600" />
</p>
</details>

___


**6. Verify logon with 'lskywalker'** via CLI

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/06-logon-to-domain.png" alt="logon to domain" width="600" />
</p>
</details>

___

**7. Created another domain user Han Solo ('hsolo') inside** 'Corp -> Users'. What would Luke Skywalker be without his companion?

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/07-add-han-solo.png" alt="created another user" width="600" />
</p>
</details>
