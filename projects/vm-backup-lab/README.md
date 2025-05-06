# Azure VM Backup and Disaster Recovery Lab

## Overview

This lab demonstrates how to configure Azure Backup for a Windows Server VM acting as an Active Directory Domain Controller (AD/DC). The goal was to implement a basic disaster recovery strategy using Azure Recovery Services Vault and simulate the restore process.

---

## ✅ Lab Tasks Completed

1. **Created Recovery Services Vault** (`NoggLabRecoveryVault`)
2. **Enabled backup** for `WinTestD2VM01` (Windows Server Domain Controller)
3. Applied a **Standard Backup Policy** with 30-day retention
4. **Initiated a manual backup**
5. Verified backup status via the **Backup Jobs** page
6. Simulated a **VM restore preview** using the most recent restore point

---

## 📸 Key Screenshots

| Filename | Description |
|---------|-------------|
| `create-recovery-services.png` | Vault creation config (region, name, resource group) |
| `vault-deployment-success.png` | Confirmation of successful vault deployment |
| `configure-backup-policy.png` | Backup policy settings and VM selection |
| `backup-deployment-complete.png` | Confirmation of backup being linked to the VM |
| `backup-in-progress.png` | VM backup running under initial job |
| `restore-options.png` | Restore point selection and recovery options |

---

## 🧠 Concepts Demonstrated

- Azure Backup architecture and vault setup
- Standard vs Enhanced policies
- Application-consistent restore points
- Safe, non-disruptive restore simulation
- Real-world relevance for enterprise disaster recovery

---

## 🔒 Why This Matters

Backing up Active Directory domain controllers ensures minimal downtime and protects identity infrastructure. Azure's incremental backup system offers secure, cost-effective disaster recovery—even for small environments like this lab.

---

## 🧰 Tools Used

- Azure Portal
- Azure Recovery Services Vault
- Windows Server 2022 VM (AD/DC)
- GitHub for lab documentation

---

## 🗂️ Next Steps (Future Labs)

- Enable file-level restore testing
- Automate backup alerts and monitoring
- Explore on-premises PC backup using MARS agent


