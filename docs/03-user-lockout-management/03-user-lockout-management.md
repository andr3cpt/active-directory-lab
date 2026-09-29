# Module 3: User Lockout Management
Implement a standard security policy to lock the user out if they attempt to enter a password too many times. 

## Overview

**1. In the Group Policy Management Editor**: Set an account **lockout threshold** of 3 attempts, after which the user is locked out and can only be unlocked by the admin
<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/01-set-lockout-threshold.png" alt="set lockout threshold" width="600" />
</p>
</details>

___

**2. On the CLI, make sure to update the server machine so that the new policy can take effect...**

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/02-server-policy-update.png" alt="server policy update" width="600" />
</p>
</details>

___

**3. ...as well as on the client machine**

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/03-client-policy-update.png" alt="client policy update" width="600" />
</p>
</details>

___

**4. Enter wrong password enough times to trigger the lockout for the user** `hsolo`

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/04-user-lockout.png" alt="user lockout screen" width="600" />
</p>
</details>

___

**5. Unlock the user** `hsolo` **from the ADUC dashboard**

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/05-user-unlock.png" alt="ADUC-user-unlock" width="600" />
</p>
</details>

___


**6. The account can be searched and unlocked via the CLI as well**

<details>
<summary>View Screenshot</summary>
<br />
<p align="center">
  <img src="assets/06-powershell-user-unlock.png" alt="powershell user unlock" width="600" />
</p>
</details>

