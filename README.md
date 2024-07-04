<h1>Honeypot Lab</h1>


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
<img src="https://imgur.com/cWjCLSA.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
Configure Virtual Machine: <br/>
<img src="https://imgur.com/UK39VJM.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
Configure An Inbound Rule For The Firewall To Allow Everything Into the VM: <br/>
<img src="https://imgur.com/uTBdXez.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
 <img src="https://imgur.com/0IJNoIs.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Create A Log Analytics Workspace: <br/>
<img src="https://imgur.com/tVdd9K2.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
<img src="https://imgur.com/x5HpxTr.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
Allow Logs To Be Collected form VM TO Log Analytics Workspace : <br/>
<img src="https://imgur.com/Vy5b8XQ.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
<img src="https://imgur.com/s6YGSAO.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
<img src="https://imgur.com/ziRu0c8.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
Connect Log Analytics Workspace To VM :  <br/>
<img src="https://imgur.com/M24Pkwh.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
 Setup Azure Sentinel:  <br/>
<img src="https://imgur.com/cDf1rbS.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
<img src="https://imgur.com/0uEZjl0.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
Log into VM Using Remote Desktop:  <br/>
<img src="https://imgur.com/2LD5y9l.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
<img src="https://imgur.com/bfsUXGc.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
Turn Off Windows Firewall On VM:  <br/>
<img src="https://imgur.com/LJwvM0x.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
<img src="https://imgur.com/4ekykGX.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
<img src="https://imgur.com/8xBEAxR.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
 <img src="https://imgur.com/TXWz87M.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
Write A Custom PowerShell Script To Get Attackers  The Geo Data :  <br/>
<img src="https://imgur.com/tTrsSh1.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
Obtain AN API KEY To get Geolocation Data:  <br/>
<img src="https://imgur.com/ZlKSanr.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
Run Script To Get Geo Data From Attackers: <br/>
<img src="https://imgur.com/khnA2aP.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
Create custom log In Log Analytics Workspace To Bring In The custom log: <br/>
<img src="https://imgur.com/zc8kuuY.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
<img src="https://imgur.com/nrU8jtZ.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
<img src="https://imgur.com/i6Nptgu.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
<img src="https://imgur.com/ulDMCrk.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
 Add A New Workbook to Azure Sentinel and Add A Query by To Create Custom Fields and Extract The Fields From The custom Log Data:  <br/>
<img src="https://imgur.com/QOscRyR.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
<img src="https://imgur.com/1GPEo19.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
Setup map in sentinel with Latitude and Longitude or Country:  <br/>
<img src="https://imgur.com/htWXNTj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe Attacks And The Attackers  Geolocation On The Map:  <br/>
<img src="https://imgur.com/5x8iHGs.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
<img src="https://imgur.com/HhY9EL8.png" height="80%" width="80%" alt="Honeypot Steps"/>
<br />
<br />
<img src="https://imgur.com/KauqyXA.png" height="80%" width="80%" alt="Honeypot Steps"/>
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
