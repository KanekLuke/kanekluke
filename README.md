<h1>Hi, I'm Kane! <br/>Cloud / IT Professional</a></h1><br>
Below are some of the projects I've worked on.

# MunkiReport Cloud Modernization (EC2 to Azure Container Apps)

Modernized a legacy MunkiReport deployment into a cloud-native Azure architecture using Azure Container Apps + Azure Database for MySQL, with persistent storage, secure networking, and reproducible image builds.

A legacy MunkiReport environment originally deployed in 2022 was not being patched/managed and needed a modernization path that:
- Removes single-host risk
- Standardizes builds
- Improves security posture
- Enables repeatable deployments across subscriptions/environments

What I built
- Containerized MunkiReport with a repeatable Docker build (Apache/PHP + dependencies)
- Migrated data into Azure Database for MySQL (Flexible Server)
- Implemented persistent storage for app-required state
- Deployed the workload into Azure Container Apps with environment-based configuration
- Documented the full build + migration workflow for portability and handoff

Architecture
Core services
- Azure Container Apps (MunkiReport web app)
- Azure Container Registry (image storage)
- Azure Database for MySQL Flexible Server (persistent DB)
- Storage (for required persistent app files, if applicable)
- Key Vault (secrets)

Network / Security
- Private networking where possible
- RBAC for least privilege
- App config separated from build artifacts
- Secrets never stored in Git

Repo contents
- `app/docker/` – Dockerfile + container build assets
- `app/compose/` – local docker-compose dev environment
- `scripts/` – build/push/db dump+restore helpers
- `infra/` – portal steps (and optional IaC)
- `docs/` – migration notes + troubleshooting + diagrams

# Azure, Aws, Microsoft 365, Windows Server, MySQL
<b>Azure</b>
  - [Admin](https://github.com/KanekLuke/Azure-Administrator/blob/main/README.md)
(Load Balancing, Azure Resource Manager, CloudShell, Azure Functions, Azure Logic, RBAC, Route Tables, Virtual Network Service Endpoint, Cost Management)
  - [Architecture](https://github.com/KanekLuke/Azure-Architect/blob/main/README.md)
(Deploy VM using PowerShell, Custom script ext, Azure container, Metric alert, Route tables, Storage table, Storage queue, Blob storage public/private access, Azure Database for MySQL Database, Cosmos DB)
  - [Security](https://github.com/KanekLuke/Azure-Security/blob/main/README.md)
(Azure Web App Authentication, Peering, ASG, Disk encryption, Kubernetes, Resource locks, Azure SQL Database auditing, Shared access signature keys, Cosmos DB security, Azure Monitor, Application Insights and App Service logs for Web App, Security for VM, Azure Defender for SQL)

<b>AWS</b>
  - [Admin](https://github.com/KanekLuke/AWS-Administrator)
(Cost estimation, IAM user and groups, Launch Web server on VPC, Subnets, SG, EC2, EBS, connect to instance using Linux and create file system, EBS snapshot, RDS server, AMI for Auto Scaling, Load Balancing, Lambda function)
  - [Architecture](https://github.com/KanekLuke/AWS-Architect)
(Hosting static website, EFS, SG, SSH into EC2, Create RDS Database, VPC, Peering connection. Application Load Balancer, Auto Scaling Group, CloudFormation, CloudFront, Lambda, Hybrid storage and Data Migration with Storage Gateway)
  - [Security](https://github.com/KanekLuke/AWS-Security)
(Suggest security features for a company's infrastructure, Architecture improvements using Well-Architected Framework)

<b>Microsoft 365</b>
  - [Microsoft 365](https://github.com/KanekLuke/Microsoft-365-1/blob/main/README.md)
(Select 5 users to receive updates before they're released to everyone else, Use PowerShell to connect to M365, Assign license to users with PowerShell or Admin center, Create shared mailbox from Exchange Admin center and provide access to users, Create distribution list and add users, Sharing policy that only allows users in organization to share files over OneDrive, Create policy that prevents private and shared channel creation)
  - [Microsoft 365 II](https://github.com/KanekLuke/Microsoft-365-2)
(Create mailboxes, create distribution list, configure DLP, block emails with HTML, enable tenant analytics, MFA, phishing policy, safe link policy)

<b>Windows Servers</b>
  - [Windows Server](https://github.com/KanekLuke/Windows-Server)
(Install domain, Configure group policy and enforce password change, Install DHCP server, Create forwarder from DNS server, Create storage pool on virtual disk, Install Hyper-V)

<b>SQL</b>
  - [SQL](https://drive.google.com/file/d/1HepIDFoEyyy5-vjhwsDVsb0XHjm48Uyu/view?usp=sharing)
