# Active-Directory Deployment and Setup
&emsp;
<p align="center">
<img src="https://imgur.com/eYFnyKY.png height="20%" width="60%" alt="Disk Sanitization Steps"/>
</p>
</p>
&emsp;  
&emsp;
&emsp;
&emsp; 

**<h2> Description </h2>**
This project goes through install and action steps for Active Directory Services. I created two virtual Machines: DC1((Windows Server) and WM 2(Client). On DC-1 Active Directory is installed and a domain is created. VM 2 is used as a client PC to connect to that domain using the newly created users. The Applications and steps used are listed below. 


<h2>Environments and Applications Used</h2>

- _Microsoft Azure (Virtual Machines/Compute)_
- _Microsoft Remote Desktop_
- _Windows Server 2016_
- _Windows 10 (21H2)_                    
- _Active Directory Domain Services_
- _PowerShell_
                                           

<h3> Configuration Steps</h3>

1. Configure and deploy Virtual Machines within Azure                                                                          
2. Change IP Address to static and test connectivity via _Ping_                                                                          
3. Install _Active Directory Domain Services_ and set as _Domain Controller _                                                               
4. Create Users and sign in as Admin
5. Add users/admins to the domain                                                                             
5. Sign in as other users using their login info
5. Add Client to the domain
                                                                                      
                                                                            
<h2>Action Steps</h2>
</p>
 - Listed below are images with a step by step process of setting up Active Directory and the domain.
                                                                             
&emsp;

<img src=https://imgur.com/B17d1fy.png height="30%" width="40%" alt="Disk Sanitization Steps"/>
</p>
<p>
-Change DC 1's IP Address to Static
   </p>
<br />

&emsp; 
&emsp;
&emsp;  

<img src=https://imgur.com/rhxaKVb.png   height="50%" width="60%" alt="Disk Sanitization Steps"/>


-Pinged DC1's private IP address to check connectivity and no reply. 

</p>
<br />

&emsp; 
&emsp;
&emsp;


<img src=https://imgur.com/KrzpTRO.png height="40%" width="50%" alt="Disk Sanitization Steps"/>
  
 

  -DC1 Ping is online. Enabled Firewall settings on DC 1. 
   </p>
<br />


&emsp; 
&emsp;
&emsp;
 
 
 
<img src =https://imgur.com/FH0Hrlo.png height="45%" width="60%" alt="Disk Sanitization Steps"/>

  -Installed Active Directory Domain Services and Set as Domain Controller
   </p>
<br />


&emsp; 
&emsp;
&emsp;
 
 
 
<img src=https://imgur.com/lhjat99.png height="40%" width="50%" alt="Disk Sanitization Steps"/>

 -New User Created

   </p>
<br />


&emsp; 
&emsp;
&emsp;


<img src= https://imgur.com/OIvWAs2.png height="40%" width="50%" alt="Disk Sanitization Steps"/>

- Assigned John Smith to "Admin User"

   </p>
<br />


&emsp; 
&emsp;
&emsp;


 <img src= https://imgur.com/Om1Zfi2.png height="40%" width="50%" alt="Disk Sanitization Steps"/>

-Signed on as new admin user on Client 1. 
&emsp;
&emsp; 
&emsp;
&emsp;

After assigning the new created user to Domain Admins, the user now has login access on this device. 

  </p>
<br />


&emsp; 
&emsp;
&emsp;
&emsp; 
&emsp;
&emsp;

<img src= https://imgur.com/Xqi1zI2.png  height="30%" width="45%" alt="Disk Sanitization Steps"/>

-Changed  Client 1's DNS settings to DC1's private IP address. {Network Settings -- Change Adapters -- DNS Servers}
First in Azure I went  to my Domain Controller and got the private IP address from IP Configuration settings. Next, Client 1's DNS Server was changed to DC1's address so that it could connected to the domain.                                                                                              
                                                                                         

  </p>
<br />


&emsp; 
&emsp;
&emsp;

<img src=https://imgur.com/ajuLOn6.png  height="40%" width="50%" alt="Disk Sanitization Steps"/>

-Added Client 1 to the domain network -Changing Client 1's DNS settings and restarting the machine above, 
allowed the client to be added to the domain since it as the same address as DC 1's private network. 







**https://github.com/daltonsjones98**
 
