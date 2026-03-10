# DUTY 5 - Integration + Security/RBAC + Cost + Documentation + Cleanup
**Assigned to:** [Bryan Edler]

##  SECURITY & RBAC IMPLEMENTATION

### Role Assignments (Screenshot 1)
[INSERT SCREENSHOT: IAM blade showing all team members with roles]

| Member | Role | Justification |
|--------|------|---------------|
| Yiming He | Contributor | Upload data to Blob |
| Jingjing Duan | Contributor | Create/manage ADF |
| Shan Jiang | Contributor | SQL schema management |
| Naveed Hossain | Reader | View-only for Power BI |
| [Owner] | Owner | Subscription management |

### Key Vault Configuration (if used)
[INSERT SCREENSHOT: Key Vault secrets]

##  COST MANAGEMENT

### Budget Alert Configuration (Screenshot 2)
[INSERT SCREENSHOT: Budget set to $20 with alerts]

### Service Tier Selections (Screenshot 3)
[INSERT SCREENSHOT: SQL DB showing Basic tier]
[INSERT SCREENSHOT: Storage account showing Standard tier]

### Actual Costs (Screenshot 4)
[INSERT SCREENSHOT: Cost analysis showing minimal spend]

##  INTEGRATION RUNBOOK

### Deployment Order Verification
 Duty 1 Complete - Blob storage populated
 Duty 2 Complete - ADF pipeline successful
 Duty 3 Complete - SQL views created and verified
 Duty 4 Complete - Power BI dashboard connected

### End-to-End Test Results
[INSERT SCREENSHOT: SQL query showing data in views]
[INSERT SCREENSHOT: Power BI dashboard with refreshed data]

##  CLEANUP VERIFICATION

### Before Cleanup (Screenshot 5)
[INSERT SCREENSHOT: Resource Group with all resources]

### After Cleanup (Screenshot 6)
[INSERT SCREENSHOT: Resource Group deleted confirmation]

### Cleanup Script Used
```powershell
# Executed on [DATE] at [TIME]
az group delete --name "AzureDataProject-RG" --yes
