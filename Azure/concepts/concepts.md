## List of Azure Cloud General Concepts
![Azure IMG](https://www.xpand-it.com/wp-content/uploads/2021/05/Banner_Azure_1920x500.png)

# INDEX
**1.-** [What is Azure](#what-is-azure-cloud)

**2.-** [Most Common Concepts](#most-common-concepts)

- **2.1 -** [Active Directory](#active-directory)
- **2.2 -** [API Management](#api-management)
- **2.3 -** [App Service](#app-service)
- **2.4 -** [Application Gateway](#application-gateway)
- **2.5 -** [Batch](#batch)
- **2.6 -** [Cognitive Services](#cognitive-services)
- **2.7 -** [Content Delivery Network](#content-delivery-network)
- **2.8 -** [Cosmos DB](#cosmos-db)
- **2.9 -** [Data Factory](#data-factory)
- **2.10 -** [Data Lake Storage](#data-lake-storage)
- **2.11 -** [Databricks](#databricks)
- **2.12 -** [Event Grid](#event-grid)
- **2.13 -** [Event Hubs](#event-hubs)
- **2.14 -** [Functions](#functions)
- **2.15 -** [Kubernetes Service](#kubernetes-service)
- **2.16 -** [Logic Apps](#logic-apps)
- **2.17 -** [Machine Learning](#machine-learning)
- **2.18 -** [Monitor](#monitor)
- **2.19 -** [Service Bus](#service-bus)
- **2.20 -** [Sentinel](#sentinel)
- **2.21 -** [SQL Database](#sql-database)
- **2.22 -** [Storage](#storage)
- **2.23 -** [IoT Hub](#iot-hub)

# What is Azure Cloud
Azure Cloud, provided by **Microsoft**, offers computing power, storage, networking, databases, AI, IoT, and analytics. 

Users can easily build, deploy, and manage applications using Microsoft-managed data centers worldwide. It provides virtual machines, various storage options, and networking capabilities, offering a flexible infrastructure for businesses.

Azure also offers managed databases, app services, AI tools, and IoT services, enabling organizations to leverage advanced technologies for innovation. 

One of Azure's notable features is its strong focus on security, with measures such as Azure Active Directory, Azure Security Center, and Azure Key Vault. Moreover, Azure follows a pay-as-you-go model, allowing businesses to optimize costs. 

This scalability and cost-effectiveness make Azure an attractive choice for organizations of all sizes, empowering them to scale infrastructure, increase efficiency, and drive digital transformation.<br><br>

# Most Common Concepts
In this section, I'll explain some of the most common concepts in Azure Cloud, to understand its key components and functionalities. These concepts serve as building blocks for creating and managing your cloud resources efficiently.

If you need more help after reading, you can read the official doc [here](https://learn.microsoft.com/en-us/azure/?product=popular).<br><br>

## Active Directory
  
**Cloud-based identity and access management service**. Serves as a central directory for managing user identities, authentication, and authorization in services and other integrated applications. Here's some useful aspects about Azure Directory:
 - **Single Sign-On (SSO)**, allows users to access multiple applications and services with a single set of credentials.
 - **Application Integration** with various cloud-based and on-premises applications, such as *Microsoft 365, Azure services, Software-as-a-Service (SaaS) applications etc.*
 - **Azure AD Connect**, tool that enables synchronization of on-premises Active Directory with Azure AD.
 - **Multi-Tenant Support**, allows organizations to manage identities and provide services to external users, such as business partners or customers.
 - **B2B and B2C Scenarios**, Business-to-Business allows organizations to share resources with external users. Business-to-Customers enables organizations to provide identity and access management for customer.
 - Allows organizations to add **conditional access** controls based on conditions such as user location, device type, or risk level.
 - **Provides good security features**, including threat detection, risk-based authentication, and integration with *Azure Active Directory Identity Protection.*
You can read more about Azure AD [here](https://learn.microsoft.com/en-us/azure/active-directory/).<br><br>

## API Management
**Allows organizations to manage, secure, and publish APIs** (Application Programming Interfaces) to both internal and external developers.
Here's some interesting utilities:

 - Acts as a **centralized gateway for APIs**, allowing organizations to expose, manage, and secure their APIs through a single interface.
 - Supports some **authentication mechanisms** like *OAuth, API keys, and client certificates.*
 - Includes a **customizable developer portal** that enables devs to discover, explore, and consume APIs.
 - Offers analytics and monitoring features to **track API usage**, performance, and health.
 - **Integrates with other Azure services**, such as *Azure Functions, Logic Apps, and Azure Active Directory.*

You can read more about Azure API Management [here](https://learn.microsoft.com/en-us/azure/api-management/).<br><br>

## App Service
**Allows developers to build, deploy, and scale web, mobile, and API applications** without having to worry about managing the underlying infrastructure. App Service simplifies the process of deploying and managing applications. Works as a PaaS (Platform as a Service).

 - **Supports different deployment options**, including code deployment from *Git, Azure DevOps*, or other source control systems.
 - **Offers automatic scaling based on application demand.**
 - **Has integration with Azure DevOps** and other popular DevOps tools.
 - **Built-in authentication and authorization capabilities**, including *Azure Active Directory* integration and social identity providers like *Microsoft, Google, Facebook, and Twitter.*

You can read more about Azure App Service [here](https://learn.microsoft.com/en-us/azure/app-service/).<br><br>

## Application Gateway
**A web traffic load balancer and application delivery controller.** It provides advanced load balancing capabilities, SSL termination, and web application firewall (WAF) functionalities. 

 - **Distributes incoming web traffic across multiple backend servers** to ensure optimal resource utilization and improved application performance.
 - **Acts as an SSL/TLS termination point.**
 - **Built-in web application firewall.**
 - **Allows traffic routing** to different backend servers based on URL paths.
 - **Continuously monitors the health of backend servers** by periodically sending health probes.
 - **Supports URL rewriting**, allowing modification of incoming requests before forwarding them to backend servers.

You can read more about Azure Application Gateway [here](https://learn.microsoft.com/en-us/azure/application-gateway/).<br><br>

## Batch
**Cloud-based job scheduling service**, you can distribute your tasks across a pool of VMs and easily scale resources up or down. Here's some useful things about it:
 - Allows you to **divide your workload** into smaller tasks that can run in parallel.
 - You can **choose from a wide range of VM configurations** to meet your specific requirements.
 - **You define a pool of VMs** with specific configurations and sizes, and Azure Batch automatically provisions and manages the VMs for you.
 - **Integration with Docker**, allowing you to package your applications and dependencies into Docker containers.
 - **Easy input and output data transfer** for your jobs using Azure Storage or Azure Data Lake Storage.
 
 You can read more about Azure Batch [here](https://learn.microsoft.com/bs-latn-ba/azure/batch/).<br><br>
 
## Cognitive Services
**Collection of cloud-based artificial intelligence (AI) APIs and services**, designed to help developers incorporate pre-built AI capabilities into their applications without needing extensive knowledge or expertise in AI or machine learning.
 - Offers a wide array of AI capabilities, including **vision, speech, language, knowledge, and search.**
 - **The vision services include capabilities like image recognition**, object detection, image analysis, optical character recognition (OCR), face detection, and emotion recognition.
 - **The speech services provide speech recognition**, text-to-speech, and speech translation capabilities.
 - **The language services encompass natural language understanding (NLU)**, natural language processing (NLP), and text analytics.
 - **The knowledge services focus on knowledge exploration and discovery**.
 - **The search services offer capabilities for web and image search**, autosuggest, spell check, and entity search.

 You can read more about Azure Cognitive Services [here](https://learn.microsoft.com/en-us/azure/cognitive-services/).<br><br>
 
## Content Delivery Network
**Distributed network of servers strategically located around the world with the purpose to deliver web content**, such as images, videos, JavaScript files, and other static or dynamic content, to users more efficiently and quickly.
 - **Works by caching content in multiple edge servers** located closer to end users.
 - **Has a global reach** with servers distributed across various geographic locations.
 - **Provides scalability** to handle increased traffic and sudden spikes in demand.
 - Includes security features to **protect against distributed denial-of-service (DDoS) attacks**

 You can read more about Azure Content Delivery Network [here](https://azure.microsoft.com/en-in/products/cdn).<br><br>

## Cosmos DB
**Globally distributed multi-model database service** designed to provide fast and scalable access to data, ensuring high availability and low latency across the globe.
 - **Offers a globally distributed architecture**, allowing you to replicate your data across multiple Azure regions.
 - **Supports multiple data models**, including key-value, document, graph, column-family, and tabular.
 - D**esigned to scale horizontally**, allowing you to handle massive amounts of data and traffic.
 - **Provides  a 99.999% uptime SLA** (Service Level Agreement).
 - **Offers low latency data access.**
 - **Supports multiple APIs**, including SQL (DocumentDB), MongoDB, Cassandra, Gremlin, and Table API.

 You can read more about Azure Cosmos DB [here](https://learn.microsoft.com/en-us/azure/cosmos-db/).<br><br>
 
## Data Factory
 **Cloud-based data integration service** that allows you to orchestrate and automate the movement and transformation of data across various sources and destinations.
 
 - **Enables you to connect and integrate data from various sources**, both on-premises and in the cloud.
 - **Offers a visual interface for designing and managing data pipelines.**
 - **Provides seamless data movement between on-premises and cloud environments.**
 - **Supports data transformation and processing** capabilities using Azure Databricks, Azure HDInsight, and Azure Machine Learning.
 - **Allows you to schedule and automate the execution of data pipelines.**

 You can read more about Azure Data Factory [here](https://learn.microsoft.com/en-us/azure/data-factory/).<br><br>
   
## Data Lake Storage
**Scalable and secure cloud-based storage service** designed to store and analyze massive amounts of unstructured and structured data.
 - **Optimized for storing large volumes of data**, including structured, semi-structured, and unstructured data.
 - **Can handle petabytes of data** and provide high throughput for data-intensive workloads.
 - **Integration with various Azure analytics services**, such as Azure Databricks, Azure Synapse Analytics (formerly SQL Data Warehouse), and Azure HDInsight.
 - **Has two generations, Gen1 and Gen2:**
	 - Gen1 offers a distributed file system with Hadoop-compatible APIs.
	 - Gen2 builds on top of Azure Blob Storage, providing a combination of the Hadoop Distributed File System (HDFS) and Blob storage capabilities.

You can read more about Azure Data Lake Storage (GEN1) [here](https://learn.microsoft.com/en-us/azure/data-lake-store/).
You can read more about Azure Data Lake Storage (GEN2) [here](https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-introduction).<br><br>
  
## Data Bricks
**Enables teams to collaborate and build data-driven applications**, perform big data analytics, and implement machine learning workflows. Combines Apache Spark, an open-source distributed computing system, with an optimized version of Databricks' Unified Analytics Platform.
 - **Uses the power of Apache Spark**, a popular distributed data processing and analytics engine.
 - **Offers a collaborative environment** that allows data engineers, data scientists, and analysts to work together seamlessly.
 - **Provides built-in machine learning capabilities** that simplify the development and deployment of machine learning models.
 - **Supports real-time streaming analytics** using Spark Streaming and Structured Streaming.
 - **Has Delta Lake**, an open-source storage layer built on top of Azure Databricks.
 - **Enables you to automate and schedule data workflows** using notebooks, jobs, and pipelines.

 You can read more about Azure Data Bricks [here](https://learn.microsoft.com/en-us/azure/databricks/).<br><br>
 
## Event Grid
**Eventing service that simplifies the development and management of event-driven architectures** by enabling the routing and delivery of events from various sources to interested subscribers.
 - **Enables the implementation of event-driven architectures.**
 - **Supports a wide range of event sources and publishers.**
 - **Supports events of different types**, including system-defined events and custom events.
 - **Allows you to define event subscriptions and specify filtering rules** to route events to the appropriate subscribers.
 - **Guarantees at least once delivery of events to subscribers.**
 - **Can integrate with on-premises systems and other cloud providers** ,making it suitable for hybrid and multi-cloud scenarios.
 - **Can integrate with on-premises systems and other cloud providers** ,making it suitable for hybrid and multi-cloud scenarios.

 You can read more about Azure Event Grid [here](https://learn.microsoft.com/en-us/azure/event-grid/).<br><br>

## Event Hubs
**Highly scalable and real-time data streaming platform** designed to handle large volumes of event data from various sources and enable real-time analytics, monitoring, and data ingestion.
 - **Distributed event streaming platform that enables the ingestion**, retention, and processing of event data.
 - **Supports both event publishers and event consumers.**
 - **Scales horizontally to handle high event throughput.**
 - **Provides configurable event retention periods**, allowing you to define how long event data should be stored.
 - **Uses data partitioning** to distribute event data across multiple storage units called partitions.
 - **Offers built-in geo-disaster recovery capabilities.**
 - **Offers built-in geo-disaster recovery capabilities.**

 You can read more about Azure Event Hubs [here](https://learn.microsoft.com/en-us/azure/event-hubs/).<br><br>

## Functions
**Serverless compute service** that allows developers to build and deploy small, event-driven functions that respond to various triggers, such as HTTP requests, timers, message queues, and more.

 - **Follows the serverless computing model**, where you don't need to provision or manage servers or infrastructure.
 - **Designed to be event-driven**, meaning they respond to events or triggers.
 - **Supports multiple programming languages**, including *C#, JavaScript (Node.js), Python, PowerShell, and TypeScript.*
 - **Provides a streamlined development experience.**
 - **Supports a wide range of triggers and bindings.**
 - **Can be executed in both stateful and stateless modes:**
	 - In *stateless mode*, functions do not maintain any persistent state between invocations.
	 - In *stateful mode*, functions can maintain their execution state across invocations.

 You can read more about Azure Functions [here](https://learn.microsoft.com/en-us/azure/azure-functions/).<br><br>

## Kubernetes Service
**Managed container orchestration service** that simplifies the deployment, management, and scaling of containerized applications using Kubernetes.

 - **Allows you to deploy containerized applications** quickly and easily.
 - **Supports automatic scaling** based on resource usage metrics.
 - Ensures high availability of your applications by **distributing your workloads** across multiple nodes.
 - **Integrates with Azure Monitor**, enabling you to gain insights into the performance and health of your Kubernetes cluster and applications.
 - **You can use features like CI/CD pipelines and GitOps** to streamline your development and release processes.
 - **Supports hybrid and multi-cloud scenarios.**
 - Supports Azure Private Link, which enables you to securely access your AKS cluster over a private network connection.
 - Integrates with Azure Dev Spaces, a tool that enables developers to rapidly iterate and debug their applications running in Kubernetes.

You can read more about Azure Kubernetes Service [here](https://learn.microsoft.com/en-us/azure/aks/).<br><br>

## Logic Apps
**Allows you to design and automate workflows** and integrate various systems, services, and applications together.

 - **Enables you to automate processes and workflows** by visually
   designing them using a drag-and-drop interface.
 - **Provides a wide range of connectors** to interact with various services
   and systems, both within Azure and outside of it.
 - **Can be extended with custom code** using Azure Functions or Azure API Management.
 - **Includes built-in transformations and mapping capabilities** to transform data between different formats like JSON, XML, CSV, and more.
 - **Supports version control and deployment management** through Azure DevOps.
 - **Offers an Integration Service Environment**, which provides a dedicated and isolated environment for running your workflows.
 - **You can also build custom connectors for Logic Apps.**
 - **Supports the fan-out/fan-in pattern**, which enables parallel processing and aggregation of data.

You can read more about Azure Logic Apps [here](https://learn.microsoft.com/en-us/azure/logic-apps/).<br><br>

## Machine Learning
**Enables you to build, deploy, and manage machine learning models at scale.** Offers a good set of tools and services to support the end-to-end machine learning lifecycle.

 - **You can use Jupyter notebooks, Python scripts, or visual interfaces** like Azure Machine Learning Studio to create and experiment with machine learning models.
 - **Includes AutoML**, a feature that automates the process of model selection and hyperparameter tuning.
 - **Offers utilities for data preparation and feature engineering.**
 - **You can easily train models on large datasets** using scalable compute resources.
 - **Supports MLOps practices**, which involve applying DevOps principles to machine learning workflows.
 - **Includes a drag-and-drop visual interface called Designer.**
 - **Supports the *Open Neural Network Exchange (ONNX)* format**, which allows you to easily import and export models across different frameworks and platforms.
 - **Integrates easily with Azure Databricks.**

You can find more about Az Machine Learning [here](https://learn.microsoft.com/en-us/azure/machine-learning/?view=azureml-api-2).<br><br>

## Monitor
**Cloud-based monitoring and diagnostics service** that provides wide monitoring capabilities for Azure resources, applications, and infrastructure

 - **Collects and analyzes metrics and logs from various Azure resources**,
   including virtual machines, databases, storage accounts, and more.
 - **Includes Application Insights**, a feature that helps monitor the performance and usage of your applications.
 - **Allows you to set up alerts** based on customizable thresholds and conditions.
 - **Integrates with Azure Autoscale**, allowing you to automatically adjust the capacity of your resources based on demand.
 - **Includes specific features for monitoring containerized workloads.**
 - **Supports integration with popular third-party monitoring tools** and services.
 - **Includes Action Groups**, which allow you to define a set of actions to be executed when an alert is triggered.
 - **Uses a powerful query language called Kusto Query Language (KQL)**, also known as Azure Data Explorer (ADX).
 - **Has the Service Map feature** provides a visual representation of the dependencies and connections between different components of your application or service.

You can find more about Az Monitor [here](https://learn.microsoft.com/en-us/azure/azure-monitor/).<br><br>

## Service Bus
**A messaging service** that enables reliable communication and coordination between different applications and services running on various platforms and devices.
 - **Supports two fundamental messaging patterns:**
	 - **The publish-subscribe** pattern allows publishers to send messages to a topic and subscribers can receive those messages selectively based on their interests.
	 - **The queuing** pattern enables reliable and ordered message delivery to a single receiver.
 - **Acts as a message broker**, decoupling senders and receivers of messages.
 - **Supports durable message queues**, which guarantee message delivery and provide first-in, first-out (FIFO) semantics.
 - **Provides a dead-letter queue** where messages that cannot be delivered to their intended destinations are moved.
 - **Allows messages of up to 1 MB in size.**
 - **Supports message compression.**
 - **You can schedule messages to be delivered at a specific time.**

You can read the full Azure Service Bus documentation [here](https://learn.microsoft.com/en-us/azure/service-bus-messaging/).<br><br>

## Sentinel
Cloud-native **security information and event management (SIEM) service** that provides intelligent security analytics and threat intelligence to help organizations.

 - **Ingests and collects security data from various sources**, including logs, events, and alerts generated by Azure services, third-party solutions, and on-premises infrastructure.
 - **Uses advanced analytics and machine learning techniques** to detect security threats and identify potential vulnerabilities.
 - **Provides automation and orchestration capabilities** to streamline security operations.
 - **Allows you to create custom analytics rules.**
 - **Introduces  Fusion**, that allows you to combine different types of data and security signals to create an analysis of potential threats.
 - **Uses Microsoft's threat intelligence and research** to provide early detection of emerging threats, including zero-day vulnerabilities.
 - **Can create custom hunting queries using Kusto Query Language (KQL).**

You can read the full Azure Sentinel documentation [here](https://learn.microsoft.com/en-us/azure/sentinel/).<br><br>

## SQL Database
**Managed, cloud-based relational database service** that provides a scalable and fully managed platform for hosting SQL Server databases.

 - **Built on the same SQL Server database engine**, providing compatibility with on-premises SQL Server.
 - **Enables hybrid connectivity scenarios**, allowing you to securely connect and synchronize data between on-premises SQL Server instances and Azure SQL Database.
 - **Supports advanced development capabilities** such as JSON support, spatial data, graph data, and full-text search.
 - **Provides built-in scalability options** to handle variable workloads.
	 - Offers the **Hyperscale** service tier, specifically designed for large-scale, mission-critical workloads.
 - **Provides transparent data encryption at rest**, which automatically encrypts data files and backups.
 - **Supports Always Encrypted.**
 - **Uses intelligent query processing** capabilities that optimize query performance.
 - **Has Query Store**, a powerful feature that captures and retains query execution plans and performance metrics.

You can read the full Azure SQL Database documentation [here](https://learn.microsoft.com/en-us/azure/azure-sql/?view=azuresql).<br><br>

## Storage
**Scalable and highly available cloud storage service** which provides a reliable and secure platform for storing and accessing various types of data, such as files, blobs, tables, and queues.

 - **Azure Blob Storage**, designed for storing unstructured data, such as text files, images, videos, and logs.
 - **File Storage**, enables you to create file shares in the cloud that can be accessed by multiple clients simultaneously.
 - **Table Storage**, a NoSQL key-value store that offers schemaless storage for structured data.
 - **Storage Explorer**, is a graphical user interface (GUI) tool that allows you to easily manage and interact with Azure Storage resources.
 - **Supports blob versioning**, which allows you to maintain and access previous versions of a blob.
 - **Can be used to host static websites.** You can upload HTML, CSS, JavaScript, and other web assets.
 - **Provides Shared Access Signatures**, which are secure tokens that grant limited access rights to your storage resources.

You can read the full Azure Storage documentation [here](https://learn.microsoft.com/en-us/azure/storage/blobs/).<br><br>

