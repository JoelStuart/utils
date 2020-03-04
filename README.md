# Utility Scripts

... for making life easy.

### Invoke-USQLRequest.ps1
    Powershell script for saving or viewing USQL queries as PS Tables or CSV files
        Use case: 
            - Extract USQL data from a tenant in a standard format
        
### move-dashboard.ps1 (needs to be renamed copy-Dashboard)
    Powershell script for moving Dynatrace Managed Dashboards between Managed clusters or tenants
        Use case: 
            - After creating a standard report, copying it to another tenant to share value

### assign-syntheticClusterLocation.ps1
    Powershell script for assigning a Synthetic Location to a Dynatrace Managed Synthetic Cluster Node
        Use case: 
            - Providing a better system to add new cluster synthetic nodes - currently there's no UI

### run-clusterWide.ps1
    Powershell script for running arbitary code against a collection of Dynatrace tenants.
        Use case: 
            - Copying a new standard Dashboard to all tenants in a cluster or customer environment
            - Exporting Config from all tenants in a cluster or customer environment
            - Gathering Audit logs from all tenants in a cluster or customer environment
            - Creating a new token for use by a data ingestion group across the customer environment
            - Use any of the other scripts above across multiple tenants

## Goals

* Have a single repo with utility scripts I use personally with Dynatrace.
* Move to using ENV vars where possible to reduce the amount of input required with each script.
* 