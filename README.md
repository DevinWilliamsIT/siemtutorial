<p align="center">
</p>



<h1>Setting Up Azure Sentinel Map With Live Attackers</h1>
In this tutorial, we setup Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot. We will observe live attacks (RDP Brute Force) from all around the world. We will use a custom PowerShell script to look up the attackers Geolocation information and plot it on the Azure Sentinel Map!. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure Account
- Azure Virtual Machines
- Azure Log Analytics Workspace
- Azure Sentinel (SIEM)
- Remote Desktop
- Powershell

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)

<h2>High-Level Steps</h2>

- Create New Resource Group and Virtual Machine
- Step 2
- Step 3
- Step 4

<h2>Actions and Observations</h2>

<p>
1. Firstly, we are going to create our new Virtual Machine. 
</p>

![image](https://github.com/DevinWilliamsIT/siemtutorial/assets/155914712/c1830895-8f3f-4899-a5ed-1254e965e1e4)

<p>
  Next navigate to Networking within our Virtual Machine creation, find NIC network security group, change to advanced, create a new one and delete the default one.
</p>

![image](https://github.com/DevinWilliamsIT/siemtutorial/assets/155914712/1db7132b-c63c-4119-ae45-f6a474e6d99d)

<p>
Now we are going to add an inbound rule and change the destination port to "*", and change the priority to 100.
</p>

![image](https://github.com/DevinWilliamsIT/siemtutorial/assets/155914712/1a4e6ea9-b977-4502-9a95-afb782f19d62)

![image](https://github.com/DevinWilliamsIT/siemtutorial/assets/155914712/0e3c3e6d-92c2-4fcc-9e33-3e1b3f49a2dd)

<p>
  What this is going to do is allow all trafic from the internet into our Virtual Machine.
</p>

<p>
  Next finish and create your Virtual Machine.
</p>



<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
