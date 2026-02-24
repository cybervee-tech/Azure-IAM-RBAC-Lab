# Azure Identity & Access Management (IAM) with Role-Based Access Control (RBAC)
Demonstration of secure identity and access management using Microsoft Entra ID and Azure RBAC in a simulated enterprise environment for FuturinCLOUD Limited.



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

 **Azure IAM Lab  – Full Documentation**  
[Open detailed report (PDF) →](https://github.com/cybervee-tech/Azure-IAM-RBAC-Lab/blob/main/docs/Azure%20IAM%20LAB.pdf)  

**Azure CLI and PowerShell Commands Used**
[open detailed document (PDF)  →](https://github.com/cybervee-tech/Azure-IAM-RBAC-Lab/blob/main/docs/Azure%20CLI%20and%20Powershell%20commands%20.pdf)





##  Security Principles Demonstrated
- **Least Privilege:** Roles scoped to the resource group  
- **Zero Trust:** Authentication enforced for all actions  
- **Group-Based Access:** Simplified auditing and scalability  
- **Password Hygiene:** Strong password + mandatory reset

  ##  Skills Gained
- Microsoft Entra ID Administration  
- Azure Role-Based Access Control (RBAC)  
- Azure Resource Management  
- Security Policy Enforcement  
- PowerShell & Azure CLI Scripting
  



## **Recommendation** 


The following recommendations are proposed to strengthen identity and access management in a production-like FuturinCLOUD environment:

-Enable multi-factor authentication (MFA) for all users (especially admins) to protect against credential compromise.

-Implement Privileged Identity Management (PIM) to provide just-in-time and time-bound access to elevated roles instead of permanent assignments.

-Use Conditional Access policies to restrict sign-ins based on location, device compliance, or risk level.


-Regularly review role assignments using Access Reviews in Microsoft Entra ID to ensure only necessary permissions remain active.

-Adopt least-privilege at scale by creating more granular custom roles (e.g., “VM Reader” instead of Contributor) for future labs and projects.

-Centralize identity governance by integrating Microsoft Entra ID with Azure Policy to enforce RBAC standards across all resource groups and subscriptions.




  











