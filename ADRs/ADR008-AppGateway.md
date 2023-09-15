# Architectural Decision Record
## Date
9/13/23 

## Title
App Gateway Implementation for Road Warrior

## Status
Accepted

## Context 
The Road Warrior will experiencing high volumes of traffic. Azure App Gateway will be entry point for our application to handle incoming traffic and distribute it to backend services. 

## Decision Drivers
- Native Integration: Azure App Gateway is a native Azure service, which means it seamlessly integrates with other Azure services such as Azure Front Door, Azure CDN, and Azure Web Apps. This allows us to build a comprehensive and scalable application architecture utilizing the Azure ecosystem. 
- Load Balancing: Azure App Gateway provides built-in load balancing capabilities, allowing us to distribute incoming traffic evenly across multiple backend servers. This helps to improve the overall performance and scalability of our application. 
- SSL Termination: App Gateway can handle SSL/TLS termination, relieving the backend services from the overhead of SSL/TLS encryption and decryption. This simplifies the configuration and management of SSL certificates and enhances the performance of the backend services. 
- Web Application Firewall (WAF): Azure App Gateway includes built-in WAF capabilities to protect our application from common web vulnerabilities and attacks. It provides features such as threat detection, prevention, and custom rule sets, enhancing the security of our application. 
- URL Routing: App Gateway allows us to configure URL-based routing, enabling us to direct incoming requests to specific backend services based on the requested URL path. This helps to achieve better flexibility and modularity in our application design. 
- Autoscaling: Azure App Gateway supports autoscaling based on demand, allowing us to handle high traffic volumes efficiently. This ensures that our application can handle increased traffic without manual intervention or performance degradation. 
- Centralized Management: Using Azure App Gateway allows us to have a centralized management point for our application's traffic routing, SSL termination, load balancing, and security policies. This simplifies the administration and maintenance of our application infrastructure.

## Decision
Approved. By adopting Azure App Gateway, we expect to achieve improved load balancing, SSL termination, URL routing, security, autoscaling, and centralized management for our application hosted on Azure. 
We acknowledge the constraints associated with the usage of Azure App Gateway and we are committed to providing the necessary resources and support to mitigate them successfully

## Consequences
- Cost: Utilizing Azure App Gateway incurs additional costs, including the gateway itself, backend server instances, and data transfer. We need to evaluate the cost implications and ensure it aligns with our budget and requirements. 
- Learning Curve: Implementing and configuring Azure App Gateway requires a learning curve for the development and operations team. We need to allocate resources for training and knowledge acquisition.
- Operational Complexity: Azure App Gateway introduces additional complexity to our infrastructure setup and management. We need to ensure that our team has the necessary skills and expertise to effectively configure, monitor, and troubleshoot the gateway. 
