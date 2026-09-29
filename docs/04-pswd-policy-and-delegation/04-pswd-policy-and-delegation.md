# Module 4: Password Policy and Delegation
Delegated password reset capabilities to the Helpdesk group. Domain password policies were configured via the **Default Domain Policy** at the domain root. Implementing advanced, granular rules remains outside the scope of this lab.

## Overview

**1. Configured Domain Password Policy**: Navigated to `Default Domain Policy` → `Account Policies` → `Password Policy` in GPMC to set a maximum password age...

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/01-max-pwsd-age.png" alt="set max password age" width="600" />
</p>
</details>

___


**2. ...and a minimum password length**

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/02-min-pswd-length.png" alt="set min password length" width="600" />
</p>
</details>

___


**3. Attempted to assign a non-compliant password** to newly created user `lorgana`

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/03-ADDS-min-length-warning.png" alt="ADDS min length warning.png" width="600" />
</p>
</details>

___

**4. Created new Security Groups** and assigned members to each:
- `lskywalker` to `SG-Finance-RW`
- `lorgana` to `SG-Helpdesk-RW`
- `hsolo` to `SG-IT-RW`


<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/04-security-groups-creation.png" alt="security groups creation" width="600" />
</p>
</details>

___

**5. Executed the Delegation of Control Wizard** on the `Corp/Users` OU

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/05-delegation-group.png" alt="delegation group" width="600" />
</p>
</details>

___

**6. Granted** `SG-Helpdesk-RW` **permission to reset user passwords and force changes at next logon**

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/06-set-pswd-delegation.png" alt="set password management delegation" width="600" />
</p>
</details>

___


**7. Enabled Advanced Features in ADUC to verify explicit** `Reset password` **rights** under `Corp/Users` -> `Properties`-> `Security`
<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/07-user-security-list.png" alt="user security list" width="600" />
</p>
</details>