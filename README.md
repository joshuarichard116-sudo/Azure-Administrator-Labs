# Azure Administrator (AZ-104) Labs

Hands-on labs covering the Microsoft **AZ-104: Azure Administrator** skills. Each lab is written up as a breakdown: the goal, what I built, how I checked it works, and what I learned. That way this repo is both a study record and a portfolio.

> Related project: [Meridian Steel — Access Governance & RBAC](https://github.com/joshuarichard116-sudo/meridian-steel-access-governance), a hybrid AD/Entra build that covers much of Domain 1 in a realistic scenario.

## Progress

Check items off as labs are completed and written up. Each one links to its folder.

### Domain 1: Manage Azure identities and governance (20–25%)
- [ ] Users and groups in Microsoft Entra ID (incl. dynamic groups, bulk operations)
- [ ] Self-service password reset & licensing
- [ ] Azure RBAC: built-in roles, custom role, assignments at different scopes
- [ ] Azure Policy: assign built-in policy, initiative, remediation
- [ ] Resource locks, tags, management groups, cost management & budgets

### Domain 2: Implement and manage storage (15–20%)
- [ ] Storage accounts: redundancy, access tiers, lifecycle management
- [ ] Blob containers, SAS tokens, stored access policies, access keys
- [ ] Azure Files: file shares, identity-based access, snapshots
- [ ] Network access: storage firewall, private endpoint / service endpoint
- [ ] AzCopy & Storage Explorer

### Domain 3: Deploy and manage Azure compute resources (20–25%)
- [ ] ARM templates / Bicep: deploy and modify
- [ ] Virtual machines: sizes, disks, availability sets/zones, encryption
- [ ] Virtual Machine Scale Sets
- [ ] Containers: Azure Container Instances, Container Apps, Container Registry
- [ ] App Service: plans, deployment slots, scaling, backups

### Domain 4: Implement and manage virtual networking (15–20%)
- [ ] Virtual networks, subnets, peering
- [ ] Network Security Groups & Application Security Groups
- [ ] Azure Bastion, service endpoints, private endpoints
- [ ] Azure DNS (public & private zones)
- [ ] Load Balancer (internal & public)
- [ ] User-defined routes & Network Watcher troubleshooting

### Domain 5: Monitor and maintain Azure resources (10–15%)
- [ ] Azure Monitor: metrics, Log Analytics, KQL queries
- [ ] Alerts & action groups
- [ ] VM Insights / Network Watcher
- [ ] Azure Backup: Recovery Services vault, backup policies, restore
- [ ] Azure Site Recovery

*Domain weights follow Microsoft's published AZ-104 study guide. Check it for the current version.*

## Repository layout

```
.
├── README.md
├── docs/
│   └── LAB-TEMPLATE.md        ← copy this for every new lab
├── 01-identity-governance/
├── 02-storage/
├── 03-compute/
├── 04-networking/
└── 05-monitoring/
```

Each lab gets its own folder, e.g. `02-storage/lab-01-storage-account-redundancy/README.md`, with screenshots in an `images/` subfolder.

## Lab hygiene

- **Clean up after every lab:** delete the resource group so leftover resources don't run up costs.
- **Set a budget alert** on the subscription before starting.
- **Never commit secrets:** no keys, SAS tokens, connection strings or passwords. Blur subscription and tenant IDs in screenshots.
