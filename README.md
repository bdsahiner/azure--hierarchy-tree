**Azure Platform / Global Infrastructure**
  │
  ├─ **Azure Regions**
  │    └─ **Availability Zones**
  │
  └─ **Azure Account / Enrollment**
       │
       └─ **Microsoft Entra ID Tenant**
            │
            ├─ **Identities & Access Components:**
            │    ├─ Users
            │    ├─ Groups
            │    │    ├─ Security Groups
            │    │    ├─ Mail-enabled Security Group
            │    │    ├─ Microsoft 365 Groups
            │    │    │    └─ Group Members
            │    │    ├─ Assigned Group Members
            │    │    └─ Dynamic Group Members
            │    ├─ Applications
            │    │    └─ Service Principal
            │    │         └─ Managed Identities
            │    ├─ Devices
            │    ├─ Roles
            │    │    ├─ Microsoft Entra ID Roles
            │    │    └─ Azure RBAC Roles
            │    ├─ Microsoft Entra Conditional Access
            │    ├─ Microsoft Entra Self-Service Password Reset (SSPR)
            │    ├─ Microsoft Entra Privileged Identity Management (PIM)
            │    ├─ Microsoft Entra multifactor authentication (MFA)
            │    └─ Azure AD Identity Protection
            │
            └─ **Tenant Root Group**
                 │
                 ├─ **Management Group**
                 │    ├─ Azure Policy
                 │    ├─ Azure Blueprints
                 │    └─ Azure Resource Locks
                 │
                 └─ **Management Group**
                      │
                      └─ **Subscription**
                           ├─ Azure Policy
                           ├─ Azure Blueprints
                           ├─ Azure Resource Manager (ARM)
                           └─ Azure Resource Locks
                           │
                           └─ **Resource Group**
                                ├─ Azure Policy
                                ├─ Azure Blueprints
                                ├─ Azure Resource Locks
                                ├─ Azure Tags
                                ├─ **Compute Resources:**
                                │    ├─ Virtual Machine (VM)
                                │    │    ├─ Availability Set
                                │    │    ├─ Network Interface Card (NIC)
                                │    │    ├─ Managed Disks
                                │    │    ├─ Just-In-Time (JIT) VM Access
                                │    │    └─ VM Extensions:
                                │    │         ├─ Azure Custom Script Extension
                                │    │         ├─ Desired State Configuration (DSC) Extension
                                │    │         └─ Azure Performance Diagnostics VM Extension
                                │    ├─ Virtual Machine Scale Set (VMSS)
                                │    ├─ Proximity Placement Group
                                │    ├─ Azure Kubernetes Service (AKS) Cluster
                                │    │    └─ Node Pool
                                │    ├─ Azure App Service
                                │    │    └─ Application Logging Feature
                                │    ├─ Azure Container Instance (ACI)
                                │    └─ Azure Container Registry (ACR)
                                │         ├─ Azure Container Registry Tasks
                                │         └─ Azure Container Registry Content Trust
                                │
                                ├─ **Storage Resources:**
                                │    ├─ Azure Storage Platform
                                │    │    └─ Azure Storage Account
                                │    │         ├─ **Types of Storage Accounts:**
                                │    │         │    ├─ Standard general-purpose v2
                                │    │         │    ├─ Standard general-purpose v1
                                │    │         │    ├─ Blob Storage (account type)
                                │    │         │    ├─ Premium block blobs
                                │    │         │    ├─ Premium file shares
                                │    │         │    └─ Premium page blobs
                                │    │         ├─ **Redundancy Options:**
                                │    │         │    ├─ Locally redundant storage (LRS)
                                │    │         │    ├─ Geo-redundant storage (GRS)
                                │    │         │    ├─ Read-access geo-redundant storage (RA-GRS)
                                │    │         │    ├─ Zone-redundant storage (ZRS)
                                │    │         │    ├─ Geo-zone-redundant storage (GZRS)
                                │    │         │    └─ Read-access geo-zone-redundant storage (RA-GZRS)
                                │    │         ├─ **Secure Access to Storage Accounts:**
                                │    │         │    ├─ Microsoft Entra integration
                                │    │         │    ├─ Identity-based authentication over SMB for Azure Files
                                │    │         │    ├─ Authorization with Shared Key
                                │    │         │    └─ Authorization using Shared Access Signatures (SAS)
                                │    │         ├─ **Encryption:**
                                │    │         │    ├─ Encryption at rest
                                │    │         │    │    └─ Customer-managed keys
                                │    │         │    └─ Client-side encryption
                                │    │         ├─ Blob Container
                                │    │         │    └─ Blob
                                │    │         │         ├─ Premium Block Blob
                                │    │         │         └─ Access Tiers:
                                │    │         │              ├─ Hot
                                │    │         │              ├─ Cool
                                │    │         │              ├─ Cold
                                │    │         │              └─ Archive
                                │    │         │         └─ AzCopy
                                │    │         ├─ File Share
                                │    │         │    └─ AzCopy
                                │    │         ├─ Table
                                │    │         │    └─ AzCopy
                                │    │         ├─ Queue
                                │    │         │    └─ AzCopy
                                │    │         └─ Storage Account Workloads:
                                │    │              ├─ Cloud native
                                │    │              ├─ Analytics
                                │    │              ├─ High-performance computing (HPC)
                                │    │              ├─ Backup and archive
                                │    │              └─ Machine learning and artificial intelligence (ML/AI)
                                │    ├─ Azure Disks
                                │    ├─ Azure Elastic SAN
                                │    ├─ Azure Container Storage
                                │    ├─ Azure Data Lake Storage Gen2 (ADLS Gen2)
                                │    ├─ Azure File Sync
                                │    │    ├─ Storage Sync Service
                                │    │    └─ Sync Group
                                │    │         ├─ Cloud Endpoint
                                │    │         └─ Server Endpoint
                                │    ├─ Azure NetApp Files
                                │    │    ├─ Access
                                │    │    ├─ Managed via
                                │    │    ├─ Redundancy
                                │    │    ├─ Security
                                │    │    └─ Active Directory Domain Services integration
                                │    ├─ Azure Managed Lustre
                                │    └─ Data Transfer Options
                                │         └─ Azure Import/Export Service Job
                                │
                                ├─ **Networking Resources:**
                                │    ├─ Azure Virtual Network
                                │    │    ├─ Subnet
                                │    │    ├─ VNet Peering
                                │    │    ├─ Route Table / User-Defined Routes (UDRs)
                                │    │    └─ Service Endpoints
                                │    ├─ Azure Load Balancer
                                │    │    ├─ Public Load Balancer
                                │    │    └─ Internal Load Balancer
                                │    ├─ Azure DDoS Protection
                                │    ├─ Azure Firewall
                                │    ├─ Azure Firewall Manager
                                │    ├─ Azure Bastion
                                │    ├─ Azure Private Link
                                │    │    └─ Private Endpoints
                                │    ├─ Azure Traffic Manager
                                │    │    └─ Routing methods
                                │    ├─ Azure Network Watcher
                                │    │    ├─ Monitoring Tools:
                                │    │    │    ├─ Topology
                                │    │    │    └─ Connection monitor
                                │    │    ├─ Network Diagnostic Tools:
                                │    │    │    ├─ IP flow verify
                                │    │    │    ├─ NSG diagnostics
                                │    │    │    ├─ Next hop
                                │    │    │    ├─ Effective security rules
                                │    │    │    ├─ Connection troubleshoot
                                │    │    │    ├─ Packet capture
                                │    │    │    └─ VPN troubleshoot
                                │    │    └─ Traffic Tools:
                                │    │         ├─ Flow logs
                                │    │         │    ├─ NSG flow logs
                                │    │         │    └─ Virtual network flow logs
                                │    │         └─ Traffic analytics
                                │    ├─ Azure Network Function Manager
                                │    ├─ Azure ExpressRoute
                                │    ├─ Azure Virtual WAN
                                │    ├─ Azure VPN Gateway
                                │    │    └─ Site-to-site VPN connection
                                │    ├─ Routing preference
                                │    ├─ Azure CDN
                                │    ├─ Azure Front Door
                                │    │    └─ Attributes
                                │    ├─ Azure Application Gateway
                                │    ├─ Azure Web Application Firewall (WAF)
                                │    ├─ Azure DNS
                                │    │    ├─ Public DNS Zone
                                │    │    └─ Private DNS Zone
                                │    ├─ Internet Analyzer
                                │    ├─ Azure NAT Gateway
                                │    ├─ Azure Programmable Connectivity
                                │    ├─ Public IP Address
                                │    └─ Network Security Group (NSG)
                                │
                                ├─ **Database Resources:**
                                │    ├─ Azure SQL Database
                                │    ├─ Azure Database for PostgreSQL/MySQL/MariaDB
                                │    ├─ Azure Cosmos DB
                                │    └─ Azure Cache for Redis
                                │
                                ├─ **Messaging & Integration Resources:**
                                │    ├─ Azure Service Bus
                                │    └─ Azure Event Grid
                                │
                                ├─ **Analytics & AI/ML Resources:**
                                │    ├─ Azure Synapse Analytics
                                │    │    └─ Custom detection logic using Azure Synapse Analytics
                                │    ├─ Azure Data Factory
                                │    ├─ Univariate Anomaly Detection
                                │    └─ Multivariate Anomaly Detection
                                │
                                ├─ **Security & Governance Resources:**
                                │    ├─ Microsoft Entra Domain Services (Azure AD DS)
                                │    ├─ Azure Key Vault
                                │    └─ Azure Defender for Cloud
                                │
                                ├─ **Monitoring & Management Resources:**
                                │    ├─ Log Analytics Workspace
                                │    │    └─ Log Analytics in Azure Monitor
                                │    ├─ Alert rules
                                │    ├─ Action groups
                                │    ├─ Azure Advisor
                                │    ├─ Azure Monitor Private Link Scope (AMPLS)
                                │    ├─ Data Collection Rule (DCR)
                                │    ├─ Recovery Services Vault
                                │    │    ├─ Azure Site Recovery
                                │    │    ├─ MARS Agent
                                │    │    └─ Microsoft Azure Backup Server (MABS) / System Center DPM
                                │    ├─ IT Service Management Connector (ITSMC)
                                │    └─ Azure Migrate Project
                                │
                                └─ **Other Common Resources:**
                                     ├─ Azure Functions App
                                     └─ Azure Event Hubs
                                     │
                                     └─ Resource
