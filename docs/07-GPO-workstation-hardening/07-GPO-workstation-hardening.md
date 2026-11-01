# Module 7: Enterprise Group Policy & Workstation Hardening
Use Group Policy Objects (GPOs) to lock down domain-joined Windows 10 endpoints by restricting access to administrative settings.

## Overview

**1. Create a new GPO within the Group Policy Management Console**:
- Right click on `Corp` → `Create a GPO in this domain, and Link it here...` → name it `GPO-Workstation-Hardening`
- Right click on `GPO-Workstation-Hardening` → `Edit`

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/01-new-hardening-GPO.png" alt="new hardening GPO" width="600" />
</p>
</details>

___


**2. Prevent the authenticated user from accessing the command prompt**:
- Navigate to `User Configuration` → `Policies` → `Administrative Settings` → `System`
- Open `Prevent access to the command prompt` and select `Enable`

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/02-prevent-command-prompt-access.png" alt="prevent command prompt access" width="600" />
</p>
</details>

___


**3. Prevent the authenticated user from accessing the Control Panel and PC Settings**:
- Navigate to `User Configuration` → `Policies` → `Administrative Settings` → `Control Panel`
- Open `Prohibit access to Control Panel and and PC settings` and select `Enable`

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/03-prevent-control-panel-access.png" alt="prevent control panel access" width="600" />
</p>
</details>

___


**4. While logged on as a domain user, try opening the command prompt...**

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/04-command-prompt-disabled.png" alt="command prompt disabled" width="600" />
</p>
</details>

___


**5. ...as well as the Control Panel**:

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/05-control-panel-restriction-error.png" alt="control panel restriction error" width="600" />
</p>
</details>

___