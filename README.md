# Azure-IAM-RBAC-Lab
Demonstration of secure identity and access management using Microsoft Entra ID and Azure RBAC in a simulated enterprise environment for FuturinCLOUD Limited.
Azure Identity & Access Management (IAM) with Role-Based Access Control (RBAC)

# Azure Identity & Access Management (IAM) with Role-Based Access Control (RBAC)

**Author:** Ezika Ifunanya Vera  
**Date:** February 2026  
**Company (Simulated):** FuturinCLOUD Limited  
**Tools Used:** Microsoft Entra ID | Azure Portal | Azure CLI | PowerShell  



##  Overview
This lab demonstrates the implementation of **secure identity and access management** using **Microsoft Entra ID** and **Azure RBAC** in a simulated enterprise setup.

**About FuturinCLOUD Limited:**  
FuturinCLOUD is a Lagos-based cloud infrastructure and cybersecurity company that helps enterprises adopt secure, scalable cloud environments.

The lab showcases user and group management, least-privilege access, and governance within Azure, aligning with **Zero-Trust** and **Least-Privilege** security principles.



##  Lab Objectives
1. Create and configure an Azure tenant for FuturinCLOUD Limited  
2. Add enterprise users with strong password and reset policies  
3. Create security groups and assign members  
4. Assign least-privilege roles (Virtual Machine Contributor) using RBAC  
5. Validate effective permissions  



##  Implementation Summary
| Step | Description | Tools |
|------|--------------|-------|
| 1 | Tenant setup and domain branding | Azure Portal |
| 2 | Created users (Vera, Aisha, Tobi) with secure policies | Entra ID/PowerShell/Azure CLI |
| 3 | Formed 3 departmental security groups | Entra ID/Powershell/Azure CLI |
| 4 | Assigned RBAC role to Technical Support group | Azure Portal |
| 5 | Verified permissions using Access Control (IAM) blade | Portal / CLI |



##  Security Principles Demonstrated
- **Least Privilege:** Roles scoped to the resource group  
- **Zero Trust:** Authentication enforced for all actions  
- **Group-Based Access:** Simplified auditing and scalability  
- **Password Hygiene:** Strong password + mandatory reset  



##  Key Takeaways
- Use **groups**, not individuals, for access management  
- Always apply **RBAC** at the smallest possible scope  
- Regularly review and audit **permissions & access logs**  



##  Skills Gained
- Microsoft Entra ID Administration  
- Azure Role-Based Access Control (RBAC)  
- Azure Resource Management  
- Security Policy Enforcement  
- PowerShell & Azure CLI Scripting  



##  Lab Screenshots
<img width="1586" height="566" alt="Resource group (2)" src="https://github.com/user-attachments/assets/785edf53-26c0-4bcc-9714-8b47c35aab42" />
<img width="1846" height="810" alt="Groups created" src="https://github.com/user-attachments/assets/fedef520-6820-48c8-97e5-b64a37226404" />
<img width="1403" height="719" alt="Users created" src="https://github.com/user-attachments/assets/de1d5580-176a-4db0-a5ea-a187791c3a6d" />
<img width="1457" height="642" alt="Assigning role to a group" src="https://github.com/user-attachments/assets/b2df7b7c-4215-4b69-be7f-96cb1468d7d3" />
<img width="1704" height="529" alt="verified the assigned role" src="https://github.com/user-attachments/assets/6a18fd30-fc3f-4b8f-9730-274e98afe514" />
<img width="1483" height="686" alt="Platform group and user showing" src="https://github.com/user-attachments/assets/cf51aa22-bedc-4162-b3df-ca4561928777" />








