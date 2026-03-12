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



---

## ✅ **Screenshot Checklist for Budget Alerts**

| # | Screenshot | Caption | Status |
|---|------------|---------|--------|
| 1 | Cost Management + Billing navigation | *Navigating to Cost Management* | ⬜ |
| 2 | Budgets page | *Budgets section in Cost Management* | ⬜ |
| 3 | Create budget button | *Starting budget creation* | ⬜ |
| 4 | Basic configuration (scope, amount) | *Setting $20 budget at resource group scope* | ⬜ |
| 5 | Alert conditions with multiple thresholds | *Configuring 50%, 80%, 90%, 100%, 120% alerts* | ⬜ |
| 6 | Action Group configuration | *Email recipients for all team members* | ⬜ |
| 7 | Review and create page | *Final budget review before creation* | ⬜ |
| 8 | Budget list showing created budget | *Completed budget in list view* | ⬜ |
| 9 | Cost analysis with budget overlay | *Spending trend against budget* | ⬜ |
| 10 | Sample alert email (optional) | *Example of notification received* | ⬜ |

---

## ⚠️ **Important Notes for Your Project**

1. **Cost data latency**: Azure cost data can take 24-48 hours to appear, so alerts aren't real-time [citation:7]
2. **No automatic shutdown**: Budget alerts only notify; they don't stop resources [citation:4]
3. **Multiple thresholds recommended**: Since alerts fire only once per threshold, having multiple (50%, 80%, 90%, 100%) gives you progressive warnings [citation:10]
4. **Test before demo**: Send a test alert to verify all team members receive notifications

Would you like me to help with any other aspect of your cost management documentation?

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
