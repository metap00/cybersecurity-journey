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

     ### DOMAIN 1.3 Describe cloud service types

    Shared responsibility model:
    (NETWORKING, STORAGE, SERVERS, VIRTUALIZATION, OS, MIDDLEWARE, RUNTIME, DATA, APPLICATIONS)
    
    - On-premises means all responsiblities are yours. Private cloud lives here.
    - IaaS (Infrastructure as a Service) = CSP takes on NETWORKING, STORAGE, SERVER AND VIRTUALIZATION -> CSP provides building blocks, like networking, storage and compute AND manages staff , HW, and data center  (e.g. Azure Virtual Machines, Amazon EC2, GCP  Compute Engine)
   
      IaaS use cases - when to use virtual machines?

      During testing and development. VMs provide a quick and easy way to create different OS and application configurations.
      
      Test and dev teams can easily deploy and then delete the VMs when they no longer need them.
      
      When running applications in the cloud. Can provide technical and financial benefits, as when an application might need to handle fluctuations in demand.
      
      Shutting down VMs when you don't need them or quickly starting them up to meet a sudden increase in demand means you pay only for resources you use.

      When extending your datacenter to the cloud. Can extend the capabilities of its own on-premises network by creating a virtual network in Azure and adding VMs to that virtual network.

      Makes it easier/less expensive to deploy than on-premises.

      During disaster recovery. Enables significant cost savings by using an IaaSbased approach to disaster recovery.

      Enables push button, automated VM spin up and shutdown in a disaster.

   - PaaS (Platform as a Service) = CSP takes on NETWORKING, STORAGE, SERVER, VIRTUALIZATION, OS, MIDDLEWARE, AND RUNTIME. Customer is responsible for deployment and management of apps. CSP manages provisioning, configuration, hardware, and OS. (e.g. Azure SQL Database, API Management, Azure App Service)

     Paas Use cases - when to use Paas services?

     Development framework

     PaaS provides a framework that developers can build upon to develop or customize cloud-based applications. PaaS lets developers create applications using built-in software components. Cloud features such as scalability, high-availability, and multi-tenant capability are included, reducing the amount of coding that developers must do.

     BOTTOM LINE: Reduces developer effort and increases solution quality

     Analytics or business intelligence

     Tools provided as a service with PaaS allow organizations to analyze and mine their data, finding insights and patterns and predicting outcomes. Improves forecasting, product design decisions, investment returns, and other business decisions.

BOTTOM LINE: Simplifies data analysis and improves business outcomes 

  - SaaS (Software as a Service) = Customer has some responsibility in access management and data recovery (DATA AND APPLICATIONS). Customer just configures features.
CSP is responsible for management, operation, and service availability. (e.g. Office 365, servicenow, salesforce)

  SaaS use cases - When to use SaaS services?

  Common SaaS use cases include:
  
  Email and messaging, Business productivity applications, Finance and expense tracking
  
  BOTTOM LINE: These are important utility functions not core to the company’s purpose

  SaaS enables companies to securely and reliably outsource a variety of functions so they can focus on revenue generation.
 
# DOMAIN 2 Describe Azure Architecture and Services

  ### DOMAIN 2.1 Describe the core architectural components of Azure

  - Azure Geography = A discrete market, typically containing two or more regions, that preserves data residency and compliance boundaries
  - Azure Regions = A set of datacenters deployed within a latency-defined perimeter and connected through a dedicated regional low-latency network.
  - Azure Sovereign Regions = Special regions that you might need to for compliance or legal purposes: Government (Fed govt, DoD) -> physical and logical isolation; , China ; operated by special trustees
  - Region Pairs = A relationship between 2 Azure Regions within the same geographic region for disaster recovery purposes.


  - Management groups = Management groups provide a level of scope above subscriptions

      Each directory is given a single top-level management group called the "Root"

  - Subscriptions = Subscription is a logical container used toprovision resources in Azure

Why would I create multiple subscriptions?  

1. when subscription limits are reached 

2. to use different payment methods

3. to isolate resources between departments, projects, etc

  - Resource groups = A container that holds related resources for an Azure solution. Used to group resources that share a common resource lifecycle.
  - Resources = An entity managed by Azure, like a virtual machine, virtual network, or storage account.

<img width="1609" height="806" alt="image" src="https://github.com/user-attachments/assets/bfbd260e-afb2-4ce1-a15a-ea95258e5594" />

<img width="1606" height="789" alt="image" src="https://github.com/user-attachments/assets/08b6adc5-b879-4848-8e06-6df05213347d" />

<img width="1608" height="803" alt="image" src="https://github.com/user-attachments/assets/4cb77565-4b61-42d5-a95a-83a463356804" />

<img width="1615" height="791" alt="image" src="https://github.com/user-attachments/assets/e3527913-ae2a-4bb8-a183-5fda8986a693" />

  - Availability zones = Unique physical locations within a region with independent power, network, and cooling. Comprised of one or more datacenters. Tolerant to datacenter failures via redundancy and isolation
  - Azure datacenters = Physical buildings that contain thousands of servers and other hardware to provide cloud computing services. Azure datacenters are located all over the world and are organized into regions. Designed to be secure, reliable, and efficient, leveraging economies of scale, multi-tenant. Consists of multiple physical buildings, redundant power, ISPs, etc

  ### DOMAIN 2.2 Describe Azure compute and networking services


  
  ### DOMAIN 2.3 Describe Azure Storage Services
  ### DOMAIN 2.4 Describe Azure Identity, Access, and Security
# DOMAIN 3 Describe Azure Management and Governance 
  ### DOMAIN 3.1 Describe cost management in Azure
  ### DOMAIN 3.2 Describe features and tools in Azure for governance and compliance
  ### DOMAIN 3.3 Describe features and tools for managing and deploying Azure resources
  ### DOMAIN 3.4 Describe monitoring tools in Azure
