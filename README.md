# Active-Directory-deployment-and-setup
&emsp;
<p align="center">
<img src="https://imgur.com/6VrviHv.png alt="Microsoft Active Directory Logo"/>
</p>
&emsp;  
&emsp;
&emsp;
&emsp;                                                                           
<h2>Environments and Applications Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Microsoft Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems </h2>

- Windows Server 2016
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

1. Configure and deploy Virtual Machines within Azure                                                                          
2. Change IP Address to static and test connectivity via Ping                                                                          
3. Install Active Directory Domain Services and set as Domain Controller                                                                      
4. Create Users and sign in as Admin
5. Add Client to the domain
6. Create Bulk Users within PowerShell command
                                                                             
                                                                             

<h2>Action Steps</h2>
</p>                                                                     
<img src=https://imgur.com/B17d1fy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
-Change DC 1's IP Address to Static
   </p>
<br />

&emsp; 
&emsp;
&emsp;  

<img src= =https://imgur.com/v81Uq5r.png   height="80%" width="80%" alt="Disk Sanitization Steps"/>


-Ping DC1's private IP address to check connectivity. No reply.

</p>
<br />

&emsp; 
&emsp;
&emsp;


<img src= https://imgur.com/ci6raAF.png height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
  -Enable Ping ICMP4 in Firewall.
   </p>
<br />


&emsp; 
&emsp;
&emsp;
 


<img src =https://imgur.com/JtLvwG6.png height="80%" width="80%" alt="Disk Sanitization Steps"/>

  -DC1 Ping is online. 
   </p>
<br />


&emsp; 
&emsp;
&emsp;
 
 
 
<img src =https://imgur.com/FH0Hrlo.png height="80%" width="80%" alt="Disk Sanitization Steps"/>

  -Install Active Directory Domain Services and Set as Domain Controller
   </p>
<br />


&emsp; 
&emsp;
&emsp;
 
 
 
<img src=https://imgur.com/lhjat99.png height="80%" width="80%" alt="Disk Sanitization Steps"/>

 -New User Created

   </p>
<br />


&emsp; 
&emsp;
&emsp;


<img src= https://imgur.com/OIvWAs2.png height="80%" width="80%" alt="Disk Sanitization Steps"/>

- Assign John Smith to "Admin User"

   </p>
<br />


&emsp; 
&emsp;
&emsp;


 <img src= https://imgur.com/Om1Zfi2.png height="80%" width="80%" alt="Disk Sanitization Steps"/>

-Login as new admin user on Client 1. 
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

<img src=https://imgur.com/Xqi1zI2.png  height="80%" width="80%" alt="Disk Sanitization Steps"/>

-Change Client 1's DNS settings to DC1's private IP address 

  </p>
<br />


&emsp; 
&emsp;
&emsp;

<img src=https://imgur.com/ajuLOn6.png  height="80%" width="80%" alt="Disk Sanitization Steps"/>

-Added Client 1 to the domain network
&emsp;
&emsp; 
&emsp;
&emsp;
&emsp; 
&emsp;
&emsp;

Changing Client 1's DNS settings and restarting the machine above, 
allowed the client to be added to the domain since it as the same address as DC 1's private network. 

 
