## Study Notes
I ll take notes going through all of the Domains.
# DOMAIN 1 Describe Cloud Concepts
  ### DOMAIN 1.1 Describe Cloud Computing
  
  Cloud computing is the delivery of computing services over the internet Expands the traditional IT offerings to include services like: Internet of Things (IoT), Machine Learning (ML), Artificial Intelligence (AI). Enables organizations to quickly expand their compute footprint without the need to build a datacenter
  
  Benefits of Cloud Computing: Cloud is cost-effective, global, secure, scalable, elastic, and always current. Allows organizations to transfer risk, operational responsability, and to focus on innovation.
  
  -> Public Cloud: Everything runs on your cloud provider's hardware. Advantages include scalability, agility, PAYG, no maintenance, and low skills. Use to skip building your own datacenter.
  
  -> Private Cloud: A cloud environment in your own datacenter. Advantages include legacy support, control, and compliance. Use when you need more control.
  
  -> Hybrid Cloud: Combines public and private clouds, allowing you to run your apps in the right location. Advantages include flexibility in legacy, compliance, and scalability scenarios.
  
  Economies of scale = The ability to do things more efficiently or at a lower-cost per unit when operating at a larger scale.
  
  Capital Expenditure (CapEx) = is the spending of money on physical infrastructure up front. Associated with legacy on-premises datacenter scenarios.
  
  Operational Expenditure (OpEx) = is spending money on services or products now and being billed as you go. Associated with public cloud consumption (pay-as-you-go).
  
  Consumption-based model = Pay for what you use, typically per unit of time or capacity (per-minute, per-GB, per-execution).
  
  Fixed price model = You provision resources and pay for those instances whether you use them or not. Ensures predictable costs for your cloud services.
  
  Serverless arhitecture = a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers. hosted as a pay-as-you-go model based on use. Resources are stateless, servers ephemeral and often capable of being triggered. (e.g. Function-as-Service)

  Serverless vs Paas (Platform as a Service) in terms of responsiblity:
<img width="1539" height="860" alt="image" src="https://github.com/user-attachments/assets/fc2a7d2c-83c1-47eb-8fcc-6f55e7ae19d0" />

  Word association to Servereless: 

  -> Logic App = A cloud service that helps you schedule, automate, and orchestrate tasks, business processes, and workflows. You can choose from a gallery of hundreds of prebuilt connectors for MSFT & 3rd party services. Logic App is the foundation for Power Automate (MS Flow).


  -> Functions = An event driven, compute-on-demand experience that extends the existing Azure application platform with capabilities to implement code triggered by events occurring in Azure as well as on-premises systems. This enables billing per execution rather than by time.

  -> Event Grid = Enables you to easily manage events across many different Azure services and applications. Once a subscription is created, Event Grid will PUSH events to the configured destination. Makes it easy for any developer to utilize the “push” model instead of the inefficient “pull” across their Serverless architecture. Like Azure Functions, it is ‘pay per use’


  
  ### DOMAIN 1.2 Describe the benefits of using cloud services
  ### DOMAIN 1.3 Describe Cloud Service Types
# DOMAIN 2 Describe Azure Architecture and Services
  ### DOMAIN 2.1 Describe the core architectural components of Azure
  ### DOMAIN 2.2 Describe Azure compute and networking services
  ### DOMAIN 2.3 Describe Azure Storage Services
  ### DOMAIN 2.4 Describe Azure Identity, Access, and Security
# DOMAIN 3 Describe Azure Management and Governance 
  ### DOMAIN 3.1 Describe cost management in Azure
  ### DOMAIN 3.2 Describe features and tools in Azure for governance and compliance
  ### DOMAIN 3.3 Describe features and tools for managing and deploying Azure resources
  ### DOMAIN 3.4 Describe monitoring tools in Azure
