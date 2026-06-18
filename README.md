<h1>Hybrid Identity Lab : AD + Entra ID Integration</h1>


<h2>Description</h2>
This project demonstrates the integration of on-premises Active Directory Domain Services (AD DS) with Microsoft Entra ID (formerly Azure AD), creating a hybrid identity environment that mirrors real-world enterprise IT setups. The goal is to build a functional lab to manage users, groups, and policies across both cloud and on-premises resources.
<br />



<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>
Environment & Cost Considerations --


For this lab, I chose the **Standard E2s v7** VM size for all virtual machines (Domain Controller and Client). I made this decision for the following reasons:

1.  **Performance Requirements:** A domain controller running Active Directory, DNS, and handling user authentication requires a stable level of performance. The 2 vCPUs and 16 GiB of RAM offered by the E2s v7 size meet the minimum recommendations for a smooth, responsive lab environment.

2.  **Cost Awareness:** The Standard D2s v3 is a cost-effective choice that balances sufficient performance with a reasonable hourly rate, demonstrating an understanding of operational budget management in Azure.
<br />
<p align="center">
VM Size: <br/>
<img src="https://i.imgur.com/1v0Wh5M.png" height="80%" width="80%" alt="VM Size Selection"/>
<br />
<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
