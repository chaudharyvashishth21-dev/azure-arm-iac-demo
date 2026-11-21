# Azure Fundamentals (AZ-900) — Infrastructure as Code (ARM Template)

A declarative **Azure Resource Manager (ARM)** JSON template demonstrating core Microsoft Azure architecture, storage, networking, and governance concepts from the **AZ-900** curriculum.

## Architecture Overview

```text
Subscription (Billing & Access Boundary)
 └── Resource Group (Lifecycle Container)
      ├── Virtual Network (10.0.0.0/16)
      │    └── Subnet: snet-app (10.0.1.0/24)
      └── Storage Account (StorageV2 | Hot Tier | Standard_LRS)
           ├── Resource Tags (Project, Environment)
           └── Resource Lock (CanNotDelete)