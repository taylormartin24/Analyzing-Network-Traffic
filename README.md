<img width="428" height="118" alt="download" src="https://github.com/user-attachments/assets/c81e6449-1a09-4890-badc-193a67e50956" />

# Analyzing Network Traffic
I created two virtual machines in Azure and used Wireshark to analyze the network traffic between them.

## Technologies and Tools Used
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Windows 11 Pro
- Ubuntu Server 22.04 LTS
- Wireshark
- Windows PowerShell

## Creating the Virtual Machines
In this part of the lab, I had to create the Resource Group by giving it a name and a region location.
<img width="1281" height="676" alt="Create Resource Group" src="https://github.com/user-attachments/assets/36b00504-33a0-4348-99b1-7a15e8451b55" />

I created the Windows virtual machine by renaming it, selecting the desired image, and the network on which it will reside. Additionally, I selected the size of the virtual machine, including the number of vCPUs and the amount of memory it will have.
<img width="1280" height="675" alt="Create Windows VM" src="https://github.com/user-attachments/assets/fe7924c1-3e49-41f8-bb03-8f0309772e22" />

I created the Virtual Network on which both virtual machines will reside by changing its name.
<img width="1280" height="675" alt="Create Lab Virtual Network" src="https://github.com/user-attachments/assets/106771cc-9c47-4d9a-bee2-29b0363c96cf" />

I created the Linux virtual machine by renaming it, selecting the desired image, and the network on which it will reside. Additionally, I selected the size of the virtual machine, including the number of vCPUs and the amount of memory it will have.
<img width="1281" height="675" alt="Create Linux VM" src="https://github.com/user-attachments/assets/ab8c5fc0-d1d7-43ef-8888-a86fd34a69c2" />

## Downloading and Using Wireshark
Downloaded and Installed Wireshark.

<img width="374" height="283" alt="Download Wireshark" src="https://github.com/user-attachments/assets/35b7fd54-8851-41ee-9561-312137e57e57" />

Opened Wireshark and observed the initial network traffic.
<img width="1280" height="764" alt="Open Wireshark and Observe initial traffic" src="https://github.com/user-attachments/assets/44dda47e-ba43-4deb-aaa8-c289030646e4" />

Filtered for ICMP or Ping Traffic before I began to ping my Linux Virtual Machine.
<img width="1280" height="764" alt="filtered ping traffic before pinging" src="https://github.com/user-attachments/assets/03fd44b9-78fd-4504-b964-cb6db502d61a" />

Pinged the Linux Virtual Machine using PowerShell.
<img width="867" height="479" alt="pinged linux vm" src="https://github.com/user-attachments/assets/ad6aa2bf-ad5e-43c9-b87d-064379d20493" />

Observed the Ping traffic in Wireshark.
<img width="1280" height="764" alt="Observed ping traffic" src="https://github.com/user-attachments/assets/f609e79d-2865-4b5b-bb83-bfc5a45827ff" />

Created a perpetual ping to the Linux Virtual Machine.
<img width="867" height="479" alt="created perpetual ping" src="https://github.com/user-attachments/assets/dd22f527-6c32-4113-b92d-4d960c6dd363" />

Created a Network Security Rule to deny incoming ICMP or Ping traffic to my Linux Virtual Machine in Microsoft Azure.
<img width="1280" height="764" alt="network security rule" src="https://github.com/user-attachments/assets/007112fa-9d3b-4d26-8e73-d735552fa567" />

Observed the Ping traffic after the rule was set in place.
<img width="1280" height="764" alt="observed ping traffic after rule" src="https://github.com/user-attachments/assets/f86f7783-8b5c-473a-902c-5ab793ad73ec" />

Deleted the rule and observed the network traffic.
<img width="1280" height="764" alt="deleted rule" src="https://github.com/user-attachments/assets/4ce87a70-6dcd-4f54-ba64-1b6c41c9bfb3" />

Connected to the Linux Virtual Machine using SSH.
<img width="867" height="479" alt="connect via ssh" src="https://github.com/user-attachments/assets/2f08ad9f-a51b-4718-9031-352c638777af" />

Observed the SSH network traffic in Wireshark.
<img width="1280" height="764" alt="observe ssh traffic" src="https://github.com/user-attachments/assets/dc145a12-9b8d-4ca8-998f-f68a173b871b" />

Entered a command for a new IP address into Windows PowerShell.
<img width="867" height="479" alt="command for new ip" src="https://github.com/user-attachments/assets/af0e2e82-212b-4e4d-b565-6e4fd7fe19fe" />

Observed the DHCP traffic in Wireshark.
<img width="1280" height="764" alt="observe dhcp" src="https://github.com/user-attachments/assets/3afafaba-07ce-4ade-9958-820f45d2b396" />

Filtered and observed RDP network traffic in Wireshark.
<img width="1280" height="764" alt="rdp traffic" src="https://github.com/user-attachments/assets/fffd90a2-848d-4659-bd8a-142634f1775a" />
