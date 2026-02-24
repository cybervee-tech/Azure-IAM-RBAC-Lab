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

  
# Azure IAM / RBAC Lab Commands


# 1️ Login to Azure
az login

# 2️ Create a new user: Tobi Okeke
az ad user create \
  --display-name "Tobi Okeke" \
  --user-principal-name tobi.okeke@ezikaifunanya98gmail.onmicrosoft.com \
  --password "TempPass123!" \
  --force-change-password-next-login true \
  --job-title "Technical Support & Response Analyst" \
  --department "Technical Support"

# 3️ Create a new group
az ad group create \
  --display-name "Technical Support Group" \
  --mail-nickname "TechSupportGrp"

# 4️ Add the user to the group
az ad group member add \
  --group "Technical Support Group" \
  --member-id $(az ad user show --id tobiokeke@ezikaifunanya98gmail.onmicrosoft.com --query objectId -o tsv)

# 5️  Verify group membership
az ad group member list \
  --group "Technical Support Group" \
  --query "[].displayName" \
  -a table



 **Azure IAM Lab  – Full Documentation**  
[Open detailed report (PDF) →](https://github.com/cybervee-tech/Azure-IAM-RBAC-Lab/blob/main/docs/Azure%20IAM%20LAB.pdf)  
(12 pages including screenshots, steps, challenges & results)








