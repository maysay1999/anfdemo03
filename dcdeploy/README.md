# Create a new Windows VM and create a new AD Forest, Domain and DC for ANF Hands-on


## Description
This template will deploy a new VM (along with a new VNet and Load Balancer) and will configure it as a Domain Controller and create a new forest and domain. No public IP is assigned.  You must use Bastion to connect this VM. 


## Components
- 1 Virtual Machine as Active Directory Domain Service domain controller.
  - Default VM size: Standard_DS2_v3
  - OS: Windows Server 2019 Datacenter
  - 1 Nic with static virtual network IP Address: 192.168.81.4
  - 1 OS disk and 1 Data disk - Managed Disks. 
- 1 Virtual Network.
  - IP Range: 192.168.81.0/24
  - 1 subnet: 192.168.81.0/25
  - DNS: 192.168.81.4


## Deployment
Click the button below to deploy

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2maysay1999%2anfdemo03%2master%2dcdeploy%2Fazuredeploy.json" target="_blank">
    <img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.png"/>
</a>

