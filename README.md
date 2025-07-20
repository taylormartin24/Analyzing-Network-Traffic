<img width="428" height="118" alt="download" src="https://github.com/user-attachments/assets/c81e6449-1a09-4890-badc-193a67e50956" />

# Analyzing Network Traffic
I created two virtual machines in Azure and used Wireshark to analyze the network traffic between them.

## Creating the Virtual Machines
In this part of the lab, I had to create the Resource Group by giving it a name and a region location.
<img width="1281" height="676" alt="Create Resource Group" src="https://github.com/user-attachments/assets/36b00504-33a0-4348-99b1-7a15e8451b55" />

I created the Windows virtual machine by renaming it, selecting the desired image, and the network on which it will reside. Additionally, I selected the size of the virtual machine, including the number of vCPUs and the amount of memory it will have.
<img width="1280" height="675" alt="Create Windows VM" src="https://github.com/user-attachments/assets/fe7924c1-3e49-41f8-bb03-8f0309772e22" />

I created the Virtual Network on which both virtual machines will reside by changing its name.
<img width="1280" height="675" alt="Create Lab Virtual Network" src="https://github.com/user-attachments/assets/106771cc-9c47-4d9a-bee2-29b0363c96cf" />

I created the Linux virtual machine by renaming it, selecting the desired image, and the network on which it will reside. Additionally, I selected the size of the virtual machine, including the number of vCPUs and the amount of memory it will have.
<img width="1281" height="675" alt="Create Linux VM" src="https://github.com/user-attachments/assets/ab8c5fc0-d1d7-43ef-8888-a86fd34a69c2" />
