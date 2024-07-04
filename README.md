<h1>Azure Sentinel</h1>


<h2>Description</h2>
In this Lab, I setup Azure Sentinel (SIEM) and connected it to a live virtual machine acting as a honey pot. I observe live attacks (RDP Brute Force) from all around the world. I also used a custom PowerShell script to look up the Geolocation information of attackers and plot it on the Azure Sentinel Map.
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Azure </b>

<h2>Environments Used </h2>

- <b>Azure Virtual Machine </b>
- <b>Azure Log Analytics Workspace </b>
- <b>Azure API Management </b>
- <b>Azure Sentinel (SIEM) </b>


<h2>Program walk-through:</h2>

<p align="center">
Sign UP For Azure Subscription: <br/>
<img src="https://imgur.com/cWjCLSA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Download windows 10 ISO: <br/>
<img src="https://imgur.com/eVutJHD.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Download Server 2019 ISO: <br/>
<br />
<br />
Create A Virtual Machine For the Domain Controller: <br/>
<img src="https://imgur.com/loli7ho.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Set Up IP Addressing:  <br/>
<img src="https://imgur.com/SGKIgXT.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Install Actve Directory and Domain Services On The Domain Contoller:  <br/>
<img src="https://imgur.com/EcJRSy1.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Configure The Post Deployment Configuration To Create The Domain:  <br/>
<img src="https://imgur.com/LIWXQrP.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Create An Organizational Unit:  <br/>
<img src="https://imgur.com/WullmfJ.png" height="80%" width="80%" alt=Active Directory  Steps"/>
<br />
<br />
Create A User Account Within The Organizational Unit :  <br/>
<img src="https://imgur.com/hCrmvPX.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Make The User Account A Domain Admin Account:  <br/>
<img src="https://imgur.com/Eh45Exa.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Sign in Using the Domain Admin Account created In the Previos Step: <br/>
<img src="https://imgur.com/3EDRcKL.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Install Routing and Remote Access: <br/>
<img src="https://imgur.com/rXGVLmM.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
<img src="https://imgur.com/K3IDxTa.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Install NAT To Allow Internal Users To Access The Internet Using One Address:  <br/>
<img src="https://imgur.com/4lXMz1e.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Set Up DHCP Server On The Domain Controller:  <br/>
<img src="https://imgur.com/IxDZv7E.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configure Server Options For Router:  <br/>
<img src="https://imgur.com/ZVoFSGS.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Create A Scope:  <br/>
<img src="https://imgur.com/TE63WZA.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Configure Lease Duration:  <br/>
<img src="https://imgur.com/Tk3XWFI.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Configure DHCP Options:  <br/>
<img src="https://imgur.com/whFqPX4.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
<img src="https://imgur.com/MXF7ZDX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://imgur.com/6ZLAATX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Activate The Scope:  <br/>
<img src="https://imgur.com/mn6IOoR.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Write And Run A PowerShell script which will create 1000 users in AD: <br/>
<img src="https://imgur.com/L4EJESt.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
<img src="https://imgur.com/RcGGyFn.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Create A Windows 10 VM on Virtual Box: <br/>
<img src="https://imgur.com/f2deR3N.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
<img src="https://imgur.com/3lGO2dG.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Test Connectivity: <br/>
<img src="https://imgur.com/sBVSMPb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Rename the New VM and Join It To The Domain: <br/>
<img src="https://imgur.com/8GHrUvY.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Allow Permision To Any Of The Users Created In AD To Join The Domain: <br/>
<img src="https://imgur.com/QSgXLBd.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Confirm VM Is Added to AD users and computers: <br/>
<img src="https://imgur.com/gjmhoqD.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
Log in Using any one of names created using the PowerShell Script.: <br/>
<img src="https://imgur.com/xfdZB6G.png" height="80%" width="80%" alt"Active Directory  Steps"/>
<br />
<br />
<img src=" https://imgur.com/JpicaAX.png" height="80%" width="80%" alt="Active Directory  Steps"/>
<br />
<br />
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
