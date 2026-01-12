# Azure VM Labs

## Overview

This repository documents my hands-on experience using Microsoft Azure to deploy and manage virtual machines (VMs) and related cloud infrastructure. These labs were completed in a live Azure environment using the Free Tier and Pay-As-You-Go resources.

## Learning Goals

- Deploy Linux and Windows VMs using the Azure Portal
- Configure VM networking (NSGs, subnets, IP addressing)
- Connect via SSH and RDP
- Install and configure basic services inside VMs
- Set up monitoring, auto-shutdown, and tagging
- Practice Azure Role-Based Access Control (RBAC)

## Labs Completed

### 1. Deploy Ubuntu VM

- Created Ubuntu Server 22.04 LTS VM using B1s SKU
- Configured custom inbound SSH rule on NSG
- Connected via SSH and installed Apache web server
- Verified public IP web access via browser

See: `screenshots/ubuntu-web.png`

---

### 2. Deploy Windows Server VM

- Provisioned Windows Server 2019 Datacenter
- Enabled RDP access with NSG rule
- Installed Active Directory Domain Services (ADDS)
- Set up local admin users inside the VM

See: `screenshots/windows-server-rdp.png`

---

### 3. Use Azure Cloud Shell + Resource Group Automation

- Created resource group, VNet, and subnet using Azure CLI

```bash
az group create --name LabRG --location eastus
az network vnet create --name LabVNet --resource-group LabRG --subnet-name LabSubnet
