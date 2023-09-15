# Architectural Decision Record
## Date
09/13/23

## Title
Hosting Road Warrior on Azure Cloud with Cosmos DB

## Status
Accepted

## Context 
Please also refer to [ADR02](https://github.com/WKMindSpartans/2023Katas/blob/main/ADRs/ADR002-Platform%20.md) and [ADR03](https://github.com/WKMindSpartans/2023Katas/blob/main/ADRs/ADR003-Storage.md)
- Azure is a leading cloud provider known for its robust infrastructure and wide range of services. 
- Cosmos DB is a globally distributed, multi-model database service provided by Azure. 
- Hosting Road Warrior on Azure with Cosmos DB will leverage its scalability, reliability, and integration capabilities. 
- Azure offers various services and tools that align with our requirements for Road Warrior.

## Decision Drivers 
- Azure Integration: Azure provides seamless integration with Cosmos DB, Azure DevOps, Azure Active Directory, Azure Monitor, and other Microsoft tools and services, enhancing development, security, monitoring, and data management aspects of Road Warrior. 
- Scalability: Azure Cosmos DB offers elastic scalability, enabling us to handle increasing data volumes and user demands while ensuring optimal performance. 
- Reliability: With its globally distributed data centers and comprehensive redundancy measures, Cosmos DB provides high availability and improved reliability for Road Warrior. 
- Cost-efficiency: Azure offers flexible pricing models for both Cosmos DB and other Azure services, enabling us to optimize costs based on usage and requirements. 
- Multi-model Database: Cosmos DB supports various data models, including key-value, document, graph, and columnar, providing flexibility and accommodating diverse data storage needs of Road Warrior. 
- Developer-Friendly Environment: Azure provides a user-friendly interface, extensive documentation, and a strong developer community, making it easier for our team to develop, deploy, and manage Road Warrior.

## Decision
Approved. 
- The Road Warrior will be hosted on the Azure cloud platform using Azure App Service for web application deployment and management. 
- Azure Cosmos DB will be utilized as the database service for storing and managing app data, providing globally distributed, multi-model database capabilities. 
- Azure Key Vault will be used for securely storing and managing sensitive application secrets, such as API keys and connection strings. 
- Azure Application Insights will be integrated for monitoring the app's performance, detecting issues, and gaining insights into user behavior. 
- Azure Blob Storage will be used for storing files and media assets related to the Road Warrior. 

## Consequences
- Dependency on Azure as the cloud provider and Cosmos DB as the database service, requiring familiarity and expertise in Azure services and tools. 
- Additional configuration and management overhead specific to the Azure environment and Cosmos DB. 
- Improved scalability, reliability, and cost-efficiency compared to maintaining on-premises infrastructure. 
- Enhanced development capabilities and integration options with other Azure services. 
- Flexibility in data modeling and storage options with Cosmos DB. 

## Justification 
Hosting Road Warrior on Azure cloud with Cosmos DB aligns with our decision drivers and provides numerous advantages. Azure's seamless integration with Cosmos DB, Azure App Service, and other services, along with Cosmos DB's scalability, reliability, multi-model database capabilities, and global distribution, make it a suitable choice. Utilizing services like Azure App Service, Cosmos DB, Azure Blob Storage, Azure Key Vault, and Azure Application Insights ensures a robust and secure hosting environment for the app. While there may be some considerations regarding Azure-specific configurations, Cosmos DB provides the flexibility and scalability needed for storing and managing app data. The benefits of Azure and Cosmos DB outweigh the potential drawbacks, making them optimal choices for hosting Road Warrior.

