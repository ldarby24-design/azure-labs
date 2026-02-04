# Azure Administrator Labs & Demos

> **Documentation Repository for Microsoft Azure Administrator (AZ-104) Certification**

This repository contains comprehensive lab guides, demonstration walkthroughs, and proof-of-work screenshots for the Microsoft Azure Administrator certification. Each lab provides hands-on experience with detailed step-by-step instructions, while demos offer quick instructor-style walkthroughs of key concepts.

---

## 📋 Repository Structure

```
Azure-Labs/
├── Labs/
│   ├── Lab01/                      # Manage Microsoft Entra ID Identities
│   ├── Lab02a/                     # Manage Subscriptions and RBAC
│   ├── Lab02b/                     # Manage Governance via Azure Policy
│   ├── Lab03b/                     # Manage Azure Resources by Using ARM Templates
│   ├── Lab04/                      # Implement Virtual Networking
│   ├── Lab05/                      # Implement Intersite Connectivity
│   ├── Lab06/                      # Implement Network Traffic Management
│   ├── Lab07/                      # Manage Azure Storage
│   ├── Lab08/                      # Manage Virtual Machines
│   ├── Lab09a/                     # Implement Web Apps
│   ├── Lab09b/                     # Implement Azure Container Instances
│   ├── Lab09c/                     # Implement Azure Container Apps
│   ├── Lab10/                      # Implement Data Protection
│   └── Lab11/                      # Implement Monitoring
│
└── Demos/
    ├── Demo01/                     # Administer Identity
    ├── Demo02/                     # Administer Governance and Compliance
    ├── Demo03/                     # Administer Azure Resources
    ├── Demo04/                     # Administer Virtual Networking
    ├── Demo05/                     # Administer Intersite Connectivity
    ├── Demo06/                     # Administer Network Traffic Management
    ├── Demo07/                     # Administer Azure Storage
    ├── Demo08/                     # Administer Azure Virtual Machines
    ├── Demo09/                     # Administer PaaS Compute Options
    ├── Demo10/                     # Administer Data Protection
    └── Demo11/                     # Administer Monitoring
```

### **Lab Folders Contain:**
- **Step-by-step guide** (Word document with detailed instructions)
- **Screenshots folder** with proof of completion
- **README.md** with lab-specific notes and key takeaways

### **Demo Folders Contain:**
- **Quick reference guide** (Markdown format)
- **Portal walkthrough notes**
- **Configuration highlights and best practices**

---

## 🎯 Labs vs Demos

| Type | Purpose | Duration | Detail Level | Audience |
|------|---------|----------|--------------|----------|
| **Labs** | Hands-on exercises for certification prep | 20-60 min | Comprehensive step-by-step | Self-paced learners |
| **Demos** | Quick concept walkthroughs | 5-15 min | High-level overview | Instructor-led sessions |

---

## 📚 Complete Module Guide

### **Module 1: Administer Identity**

#### 🧪 Lab 01 — Manage Microsoft Entra ID Identities
- **Time:** 30 minutes
- **Skills:** Create user accounts (internal & guest), create security groups, configure group membership
- **Key Concepts:** Tenants, user accounts, groups, assigned vs dynamic membership
- **Screenshots:** 8 required

#### 🎬 Demo 01 — Administer Identity
- **Includes:** Review tenant info, explore user accounts, create and configure groups
- **Quick Tasks:** Create new user, invite guest user, review group membership types

---

### **Module 2: Administer Governance and Compliance**

#### 🧪 Lab 02a — Manage Subscriptions and RBAC
- **Time:** 20 minutes
- **Skills:** Create management groups, assign built-in Azure roles, create custom RBAC roles, monitor role assignments
- **Key Concepts:** Management groups, role-based access control, least privilege
- **Screenshots:** 6 required

#### 🧪 Lab 02b — Manage Governance via Azure Policy
- **Time:** 30 minutes
- **Skills:** Assign tags, enforce tagging via policy, apply remediation, configure resource locks
- **Key Concepts:** Azure Policy, resource tags, compliance, resource protection
- **Screenshots:** 7 required

#### 🎬 Demo 02 — Administer Governance and Compliance
- **Includes:** Assign policies, create initiative definitions, configure RBAC, check compliance
- **Quick Tasks:** Create policy assignment, assign role to user/group, review access control

---

### **Module 3: Administer Azure Resources**

#### 🧪 Lab 03b — Manage Azure Resources Using ARM Templates
- **Time:** 50 minutes
- **Skills:** Create ARM templates, deploy via portal/PowerShell/CLI, use Bicep templates
- **Key Concepts:** Infrastructure as Code, ARM templates, Bicep, Cloud Shell
- **Screenshots:** 10 required

#### 🎬 Demo 03 — Administer Azure Resources
- **Includes:** Explore Azure Portal, use Cloud Shell, work with QuickStart templates, explore Copilot for Azure
- **Quick Tasks:** Configure portal settings, create dashboard, deploy QuickStart template, use PowerShell/Bash

---

### **Module 4: Administer Virtual Networking**

#### 🧪 Lab 04 — Implement Virtual Networking
- **Time:** 50 minutes
- **Skills:** Create virtual networks, configure subnets, create network security groups
- **Key Concepts:** VNets, subnets, NSG rules, network segmentation
- **Screenshots:** 9 required

#### 🎬 Demo 04 — Administer Virtual Networking
- **Includes:** Create VNets, configure NSGs, explore Azure DNS
- **Quick Tasks:** Create virtual network, add NSG rules, create DNS zone and records

---

### **Module 5: Administer Intersite Connectivity**

#### 🧪 Lab 05 — Implement Intersite Connectivity
- **Time:** 50 minutes
- **Skills:** Configure VNet peering, test connectivity with Network Watcher, create custom routes
- **Key Concepts:** VNet peering, Network Watcher, user-defined routes, virtual appliances
- **Screenshots:** 8 required

#### 🎬 Demo 05 — Administer Intersite Connectivity
- **Includes:** Configure VNet peering, create route tables, associate routes with subnets
- **Quick Tasks:** Set up peering between VNets, create custom routes, configure network endpoints

---

### **Module 6: Administer Network Traffic Management**

#### 🧪 Lab 06 — Implement Network Traffic Management
- **Time:** 60 minutes
- **Skills:** Implement virtual network routing, configure Azure Load Balancer, configure Application Gateway
- **Key Concepts:** Load balancing, traffic distribution, routing tables
- **Screenshots:** 11 required

#### 🎬 Demo 06 — Administer Network Traffic Management
- **Includes:** Create Azure Load Balancer, configure Application Gateway
- **Quick Tasks:** Set up load balancing rules, configure frontend/backend pools, create routing rules

---

### **Module 7: Administer Azure Storage**

#### 🧪 Lab 07 — Manage Azure Storage
- **Time:** 50 minutes
- **Skills:** Create storage accounts, configure blob containers, secure file shares, manage lifecycle policies
- **Key Concepts:** Blob storage, Azure Files, redundancy, access tiers, immutable storage
- **Screenshots:** 9 required

#### 🎬 Demo 07 — Administer Azure Storage
- **Includes:** Create storage accounts, configure blob storage, set up file shares, configure security
- **Quick Tasks:** Create containers, upload blobs, generate SAS tokens, use Storage Explorer

---

### **Module 8: Administer Virtual Machines**

#### 🧪 Lab 08 — Manage Virtual Machines
- **Time:** 50 minutes
- **Skills:** Deploy VMs, configure availability, manage VM extensions, implement auto-scaling
- **Key Concepts:** VM deployment, availability sets, scale sets, extensions
- **Screenshots:** 10 required

#### 🎬 Demo 08 — Administer Azure Virtual Machines
- **Includes:** Create VMs in portal, configure availability options, connect to VMs with Bastion
- **Quick Tasks:** Deploy Windows/Linux VM, configure scale sets, review scaling policies

---

### **Module 9: Administer PaaS Compute Options**

#### 🧪 Lab 09a — Implement Web Apps
- **Time:** 20 minutes
- **Skills:** Create web apps, configure deployment slots, swap slots, configure autoscaling
- **Key Concepts:** Azure App Service, deployment slots, scaling strategies
- **Screenshots:** 6 required

#### 🧪 Lab 09b — Implement Azure Container Instances
- **Time:** 15 minutes
- **Skills:** Deploy containers, configure container instances
- **Key Concepts:** Containers, Docker images, ACI
- **Screenshots:** 4 required

#### 🧪 Lab 09c — Implement Azure Container Apps
- **Time:** 15 minutes
- **Skills:** Create container apps, configure container app environments
- **Key Concepts:** Container Apps, serverless containers, managed environments
- **Screenshots:** 4 required

#### 🎬 Demo 09 — Administer PaaS Compute Options
- **Includes:** Configure App Service plans, create web apps, deploy containers, work with Container Apps
- **Quick Tasks:** Create App Service, deploy Docker container to ACI, configure Container App

---

### **Module 10: Administer Data Protection**

#### 🧪 Lab 10 — Implement Data Protection
- **Time:** 50 minutes
- **Skills:** Configure Recovery Services vault, implement VM backup, enable VM replication with Site Recovery
- **Key Concepts:** Azure Backup, disaster recovery, Site Recovery, backup policies
- **Screenshots:** 8 required

#### 🎬 Demo 10 — Administer Data Protection
- **Includes:** Backup Azure file shares, backup virtual machines, configure Recovery Services vault
- **Quick Tasks:** Create vault, configure backup policies, enable VM backup

---

### **Module 11: Administer Monitoring**

#### 🧪 Lab 11 — Implement Monitoring
- **Time:** 40 minutes
- **Skills:** Create alerts, configure action groups, use Log Analytics queries, configure alert processing rules
- **Key Concepts:** Azure Monitor, alerts, action groups, KQL queries, insights
- **Screenshots:** 7 required

#### 🎬 Demo 11 — Administer Monitoring
- **Includes:** Configure Azure alerts, work with Log Analytics, use KQL queries
- **Quick Tasks:** Create alert rules, set up action groups, query logs with KQL

---

## 🚀 Getting Started

### Prerequisites
- **Azure Account:** Active Azure subscription ([Get a free account](https://azure.microsoft.com/free/))
- **Portal Access:** https://portal.azure.com
- **Recommended Region:** East US (most labs use this region)
- **Browser:** Modern browser with InPrivate/Incognito mode for testing

### How to Use This Repository

#### **For Labs (Detailed Practice):**

1. **Choose a Lab** from the module list above
2. **Navigate** to `Labs/LabXX/` folder
3. **Open the step-by-step guide** (Word document)
4. **Follow the instructions** carefully
5. **Take screenshots** at designated points (marked with 📸)
6. **Save screenshots** using the suggested filenames
7. **Review** your work using the built-in checklist

#### **For Demos (Quick Reference):**

1. **Select a Demo** matching the topic you're studying
2. **Navigate** to `Demos/DemoXX/` folder
3. **Review the markdown guide** for high-level steps
4. **Use as a quick refresher** before or after labs
5. **Follow along in the portal** for hands-on practice

---

## 📸 Screenshot Guidelines

Labs include screenshot markers that look like this:

> **📸 SCREENSHOT — Capture the Entra ID Overview page showing tenant information**

**When you see these markers:**

1. **Pause** your current task
2. **Capture** the full browser window (including address bar)
3. **Save** using the suggested filename format (e.g., `01_entra_id_overview.png`)
4. **Store** in your lab's screenshots folder
5. **Check off** the screenshot in your completion checklist

**Screenshot Best Practices:**
- Use full-screen browser windows for clarity
- Capture the entire portal interface
- Ensure resource names and settings are visible
- Use PNG format for best quality
- Name files sequentially with descriptive names

---

## ✅ Progress Tracking

### Lab Completion Tracker

| Lab | Module | Time | Status | Screenshots | Demo Reviewed | Notes |
|-----|--------|------|--------|-------------|---------------|-------|
| Lab 01 | Identity | 30m | ☐ | ☐ | ☐ | |
| Lab 02a | Governance | 20m | ☐ | ☐ | ☐ | |
| Lab 02b | Governance | 30m | ☐ | ☐ | ☐ | |
| Lab 03b | Resources | 50m | ☐ | ☐ | ☐ | |
| Lab 04 | Networking | 50m | ☐ | ☐ | ☐ | |
| Lab 05 | Connectivity | 50m | ☐ | ☐ | ☐ | |
| Lab 06 | Traffic Mgmt | 60m | ☐ | ☐ | ☐ | |
| Lab 07 | Storage | 50m | ☐ | ☐ | ☐ | |
| Lab 08 | VMs | 50m | ☐ | ☐ | ☐ | |
| Lab 09a | Web Apps | 20m | ☐ | ☐ | ☐ | |
| Lab 09b | Containers | 15m | ☐ | ☐ | ☐ | |
| Lab 09c | Container Apps | 15m | ☐ | ☐ | ☐ | |
| Lab 10 | Data Protection | 50m | ☐ | ☐ | ☐ | |
| Lab 11 | Monitoring | 40m | ☐ | ☐ | ☐ | |

**Total Lab Time:** ~540 minutes (~9 hours)

### Demo Completion Tracker

| Demo | Module | Reviewed | Notes |
|------|--------|----------|-------|
| Demo 01 | Identity | ☐ | |
| Demo 02 | Governance | ☐ | |
| Demo 03 | Resources | ☐ | |
| Demo 04 | Networking | ☐ | |
| Demo 05 | Connectivity | ☐ | |
| Demo 06 | Traffic Mgmt | ☐ | |
| Demo 07 | Storage | ☐ | |
| Demo 08 | VMs | ☐ | |
| Demo 09 | PaaS | ☐ | |
| Demo 10 | Data Protection | ☐ | |
| Demo 11 | Monitoring | ☐ | |

---

## 🎓 Certification Information

These labs and demos support preparation for the **Microsoft Certified: Azure Administrator Associate** certification (AZ-104).

**Exam Details:**
- **Exam Code:** AZ-104
- **Skills Measured:**
  - Manage Azure identities and governance (20-25%)
  - Implement and manage storage (15-20%)
  - Deploy and manage Azure compute resources (20-25%)
  - Implement and manage virtual networking (15-20%)
  - Monitor and maintain Azure resources (10-15%)
- **Exam Format:** Multiple choice, case studies, performance-based scenarios
- **Duration:** 100 minutes
- **Passing Score:** 700/1000
- **More Info:** [Microsoft Learn AZ-104](https://learn.microsoft.com/credentials/certifications/azure-administrator/)

**Study Strategy:**
1. **Complete all labs** in sequential order
2. **Review demos** before each lab for context
3. **Practice in your own Azure subscription** when possible
4. **Take notes** on key concepts and gotchas
5. **Review key takeaways** at the end of each lab
6. **Use Microsoft Learn** modules for additional theory

---

## 💡 Best Practices

### General Practices
- **Use Consistent Naming:** Follow Azure naming conventions (e.g., `rg-projectname-env`)
- **Document Everything:** Add notes to README files in each lab folder
- **Stay Organized:** Keep screenshots organized by lab number
- **Track Progress:** Use the completion checklist above

### Cost Management
- **Delete Resources After Each Lab:** Avoid unexpected charges
- **Use Free Tier When Possible:** Many services have free tiers
- **Set Budget Alerts:** Configure alerts for spending thresholds
- **Stop VMs When Not in Use:** Deallocate VMs to save costs
- **Clean Up Resource Groups:** Delete entire resource groups to remove all resources at once

### Lab Execution
- **Region Selection:** Use the same region throughout a lab for consistency
- **Read Carefully:** Follow each step exactly as written
- **Take Notes:** Document any issues or deviations
- **Screenshot Everything:** Better to have too many than too few
- **Verify Each Step:** Check that resources are created successfully

### Portal Navigation
- **Use Search:** The search bar is the fastest way to find resources
- **Pin Favorites:** Pin frequently used services to your sidebar
- **Use Breadcrumbs:** Navigate back using the breadcrumb trail
- **Open Multiple Tabs:** Keep documentation and portal in separate tabs

---

## 🔗 Additional Resources

### Official Microsoft Documentation
- [Azure Documentation](https://learn.microsoft.com/azure/)
- [Azure Portal](https://portal.azure.com)
- [Azure CLI Reference](https://learn.microsoft.com/cli/azure/)
- [Azure PowerShell Reference](https://learn.microsoft.com/powershell/azure/)
- [Azure Architecture Center](https://learn.microsoft.com/azure/architecture/)

### Learning Resources
- [Microsoft Learn AZ-104 Learning Path](https://learn.microsoft.com/training/courses/az-104t00)
- [AZ-104 Exam Skills Outline](https://learn.microsoft.com/credentials/certifications/resources/study-guides/az-104)
- [Azure Quickstart Templates](https://azure.microsoft.com/resources/templates/)
- [Azure Updates](https://azure.microsoft.com/updates/)

### Community & Support
- [Azure Community Support](https://learn.microsoft.com/answers/products/azure)
- [Azure Tech Community](https://techcommunity.microsoft.com/t5/azure/ct-p/Azure)
- [Azure YouTube Channel](https://www.youtube.com/c/MicrosoftAzure)
- [r/AZURE on Reddit](https://www.reddit.com/r/AZURE/)

### Practice Tools
- [Azure Pricing Calculator](https://azure.microsoft.com/pricing/calculator/)
- [Azure Speed Test](https://www.azurespeed.com/)
- [Azure Resource Explorer](https://resources.azure.com/)

---

## 🛠️ Troubleshooting

### Common Issues

**Issue:** Deployment fails due to region capacity
- **Solution:** Try a different region (West US, Central US, North Europe)
- **Alternative:** Use the "help me choose" feature for region selection

**Issue:** Feature not available in subscription
- **Solution:** Check subscription type (some features require paid subscriptions)
- **Workaround:** Review demo instead or use Microsoft Learn sandbox environments

**Issue:** Permission denied errors
- **Solution:** Ensure you have Owner or Contributor role on the subscription
- **Check:** Verify you're using the correct subscription in the portal

**Issue:** Resource name already exists
- **Solution:** Use globally unique names (add your initials or random numbers)
- **Tip:** Azure will suggest alternatives if your name is taken

**Issue:** Portal interface looks different
- **Solution:** Screenshots may be from an older portal version
- **Approach:** Look for similar options or use search to find the feature

**Issue:** Screenshots not saving properly
- **Solution:** Use Snipping Tool (Windows) or Screenshot (Mac)
- **Alternative:** Use browser extensions like Lightshot or Nimbus

**Issue:** Lab taking longer than estimated time
- **Solution:** Don't rush - accuracy is more important than speed
- **Note:** Times are estimates and may vary based on experience

---

## 📝 Important Notes

### About Labs
- All labs are designed for **East US** region unless otherwise specified
- Some features may vary based on your **subscription type**
- **Premium features** may require additional licensing or paid subscriptions
- Labs are written for the **Azure Portal** interface
- **Cloud Shell** is used for PowerShell and CLI tasks
- Resource provisioning times may vary

### About Demos
- Demos are **instructor-focused** with high-level steps
- **Not intended for certification study** (use labs instead)
- Great for **quick refreshers** or **concept review**
- Less detailed than labs - assumes Azure experience
- Can be completed in **5-15 minutes** each

### Repository Maintenance
- Labs updated to reflect current Azure Portal UI
- Demo content based on official Microsoft AZ-104 course
- Screenshots reflect February 2026 portal version
- Check for updates regularly as Azure evolves

---

## 📧 Contact & Feedback

- **GitHub Profile:** [ldarby24-design](https://github.com/ldarby24-design)
- **Repository Issues:** Use the Issues tab for questions, corrections, or suggestions
- **Pull Requests:** Contributions welcome for fixes or improvements

---

## 📜 License

This repository is for educational and certification preparation purposes. All Azure services, features, and Microsoft content are property of Microsoft Corporation. Lab and demo content adapted from official Microsoft AZ-104 course materials.

---

## 🗂️ Repository Maintenance

**Last Updated:** February 2026  
**Maintained by:** ldarby24-design  
**Lab Count:** 14 labs  
**Demo Count:** 11 demos  
**Total Content:** 25 modules

---

## 🎯 Quick Links

### For New Learners
- Start with [Lab 01](Labs/Lab01/) - Manage Entra ID Identities
- Review [Getting Started](#-getting-started) section
- Check [Prerequisites](#prerequisites)

### For Returning Students
- Review [Progress Tracking](#-progress-tracking) checklist
- Browse [Troubleshooting](#-troubleshooting) for common issues
- Check [Additional Resources](#-additional-resources)

### For Exam Preparation
- Complete all 14 labs
- Review all key takeaways
- Practice with demos for speed
- Use [Microsoft Learn](https://learn.microsoft.com/training/courses/az-104t00)

---

> 💡 **Success Tip:** Consistency is key! Aim to complete 1-2 labs per week, review the corresponding demos, and take detailed notes. This steady approach builds muscle memory for the exam and real-world scenarios.

> ⭐ **Star this repository** to keep it handy during your certification journey!
