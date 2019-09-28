# Migration Strategies
- Rehost 
- Refactor
- Rearchitect
- Rebuild

# Prepare Azure for Migration Assessment
- Your Azure account needs permissions to create the migrate project
- You need permissions to register the Azure Migrate appliance
- You need role assignment permissions assigned to the migrate resource group for Azure Migrate to create a Key Vault to manage access keys to your replication storage account

# Prepare On-premises VMware for Migration Assessment
- Verify VMware server requirements and ensure required ports are on VCenter servers (443)
- Azure Migrate needs access to VCenter through a read-only account
- Verify appliance settings and ensure your account has permissions to create a VM using an OVA file

# Prepare On-premises Hyper-V for Migration Assessment
- Verify host settings/requirements and ensure required ports are open, WinRm ports 5985, 5986
- Enable PowerShell remoting on hosts->Enable-PSRemoting -force
- Enable CredSSP on hosts

# Azure Migrate
- Used to assess on-premises VMware and Hyper-V workloads 
- Providing sizing and cost estimates 
- Identifies affecting dependencies (Need agent install)
- Requires the Azure Migrate appliance

# Azure Migrate Steps
- Download and configure appliance
- Start Discovery
- Create assessment
- Start Replication

# Data Migration Assistant
- Assess on-premises SQL Server instances 
- Discover compatibility issues of migrating to Azure SQL database 
- Detect partially supported and unsupported features 
- Upload assessment results to Azure Migrate 
- Migrate on-premises SQL instances

# Migrate VMware VMs to Azure (agentless) - Preview
- Prepare VMs for migration
- Add the Azure Migration Server Migration tool
- Discover VMs you want to migrate
- Start replicating VMs
- Run a test migration to make sure everything's working as expected
- Run a full VM migration

# Migrate VMware VMs to Azure (agent-based)
- Set up the source environment, and deploy an Azure Migrate replication appliance for agent-based migration
- Set up the target environment for migration
- Set up a replication policy
- Enable replication
- Run a test migration to make sure everything's working as expected
- Run a full migration to Azure

# Links
https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/getting-started/migrate

















