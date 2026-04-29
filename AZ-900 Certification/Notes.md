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

  - Availability = Encompasses availability of the infrastructure, applications, and services. Generally expressed as a number of 9’s, such as five nines or 99.999% availability

    !!!! Availability and uptime are often used interchangeably. Uptime simply measures the amount of time a system is running
    
  - Scalability = The ability of a system to handle growth of users or work. Refers to the ability of a system or service to handle more traffic (to scale)
  - Elasticity = The ability of a system to automatically grow and shrink based on app demand. Focuses on the ability of a system or service to scale quickly to spikes in demand

<img width="1907" height="897" alt="image" src="https://github.com/user-attachments/assets/98fce691-c0b6-48a8-815e-2cfec17a5b2b" />

  - Agility = Focuses on the speed and ease of allocating and deallocating resources. This allows for vast amounts of computing resources to be provisioned in minutes.
  - Fault Tolerance = The ability of a system to handle faults in a service like power, network, or hardware failures. Generally, refers to componentlevel failures
  - High Availability = he ability to keep services up and running for long periods of time. Generally, refers to service-level failures
  - Disaster Recovery = The ability to recover from an event which has taken down a cloud service. Generally, focuses on recovery in the event of a service or site failure
  - Reliability = The ability of a system to recover from failures and continue to function. Reliability consists of two principles: resiliency and availability. Resiliency aims to return an application to a fully functioning state after a failure occurs. The goal of availability is to provide consistent access to your application.
  - Predictability = Azure enables solutions with predictable cost and performance. The level of service and performance and the associated cost are known in advance!

    <img width="1858" height="744" alt="image" src="https://github.com/user-attachments/assets/3be9860e-6e2e-46e4-a44b-ff06a25fc71b" />

  - Governance = A set of rules and policies that guide an organization's cloud operations. To ensure data security, manage risk, control costs, and improve efficiency. Cloud features are desgined to support governance and compliance.
  - The Shared Responsibility Model explains who is responsible for security in each model and scenario
  - Manageability = There are two aspects of manageability for the cloud: WHAT and HOW
    <img width="1069" height="1215" alt="image" src="https://github.com/user-attachments/assets/87457833-dc26-4ada-8e2e-200ad7533eac" />

    





  
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
