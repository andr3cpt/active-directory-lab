# Module 1: Core Infrastructure & Domain Controller Setup

On WMware Fusion, I installed two VMs - Windows Server 2022 and Windows 10 Pro - in order to emulate a mini enterprise environment.


## Overview

**1. Set the** `TCP/IPv4` **properties on Windows Server :** Assigned a static IP address (`192.168.50.10`), a Subnet mask of `255.255.255.0` and a DNS address pointing to the machine itself (`127.0.0.1`), so that the server VM could resolve incoming DNS requests from the client VM 
<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/01-manual-IPv4-setting.png" alt="manual IPv4 setting" width="600" />
</p>
</details>

---

**2. Added the Active Directory Domain Services** server role via Server Manager

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/02-ADDS-server-role.png" alt="add AD DS server role" width="600" />
</p>
</details>

___


**3. Promoted the server to create a new forest named** `lab.local`

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/03-forest-creation.png" alt="forest creation" width="600" />
</p>
</details>

___

**4. Installed Active Directory Domain Services (AD DS)** which installs DNS functionality by default

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/04-ADDS-installation.png" alt="AD DS installation" width="600" />
</p>
</details>

___

**5. Renamed server to** `DC-01` **to follow good naming conventions** (and replace the standard ugly name)

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/05-rename-server-DC-01.png" alt="server rename to DC-01" width="600" />
</p>
</details>

___

**6. Checked if core services were running correctly after rebooting**

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/06-verify-core-services.png" alt="verify core services" width="600" />
</p>
</details>

___

**7. Tested DNS resolution on newly configured server**

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/07-verify-DNS-resolution.png" alt="verify DNS resolution" width="600" />
</p>
</details>
