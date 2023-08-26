# List of Google Cloud Platform General Concepts
![Google Banner](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_images/GCP_CloudCovered_3.jpg)

# INDEX
**1.** [What is GCP](#what-is-gcp)

**2.** [Most Common Concepts](#most-common-concepts)

-   **2.1 -** [IAM (Identity and Access Management)](#iam)
-   **2.2 -** [Cloud Endpoints](#cloud-endpoints)
-   **2.3 -** [Compute Engine](#compute-engine)
-   **2.4 -** [Load Balancing](#load-balancing)
-   **2.5 -** [Google Kubernetes Engine (GKE)](#gke)
-   **2.6 -** [Cloud Storage](#cloud-storage)
-   **2.7 -** [Cloud CDN](#cloud-cdn)
-   **2.8 -** [Cloud SQL](#cloud-sql)
-   **2.9 -** [Dataflow](#dataflow)
-   **2.10 -** [Cloud Functions](#cloud-functions)
-   **2.11 -** [Cloud Composer](#cloud-composer)
-   **2.12 -** [Pub/Sub](#pub-sub)
-   **2.13 -** [Datastream](#datastream)
-   **2.14 -** [GKE Autopilot](#gke-autopilot)
-   **2.15 -** [Cloud Monitoring](#cloud-monitoring)
-   **2.16 -** [Cloud Pub/Sub Lite](#pub-sub-lite)
-   **2.17 -** [AI Platform](#ai-platform)
-   **2.18 -** [Cloud Audit Logs](#cloud-audit-logs)
-   **2.19 -** [Cloud Security Command Center](#security-command-center)
-   **2.20 -** [Cloud Spanner](#cloud-spanner)
-   **2.21 -** [Persistent Disk](#persistent-disk)
-   **2.22 -** [Cloud IoT Core](#cloud-iot-core)
<br><br>
# What is Google Cloud Platform (GCP)

GCP furnishes a **robust foundation for computing power, storage, networking, and databases**. This platform facilitates the effortless creation, deployment, and management of applications through its globally distributed network of data centers.

Through GCP, users can **make virtual machines, diverse storage choices, and advanced networking features to construct a malleable and scalable infrastructure** tailored to their requirements.

GCP **offers managed database services, application solutions, cutting-edge artificial intelligence (AI) tools, and services for the Internet of Things (IoT)**. These offerings empower organizations to leverage advanced technologies for driving innovation and fostering growth.

One of GCP's core strengths is its **steadfast dedication to security**. It provides a suite of security services including **Google Cloud Identity and Access Management (IAM), Cloud Web Security, and Google Cloud Key Management Service (KMS)** to ensure robust security protocols.

The scalability, dependability, and cost-efficiency of GCP position it as an appealing choice for entities of all sizes, enabling them to seamlessly expand their infrastructure, enhance operational efficiency, and navigate the realms of digital transformation.<br><br>

# Most Common Concepts
  
In this section, I'll introduce you to some of the **fundamental concepts within Google Cloud Platform (GCP)**, which are essential for comprehending its core components and operational capabilities. These concepts lay the groundwork for effectively building and managing your cloud resources.

For further assistance and in-depth information, you can refer to the **official documentation** available [here](https://cloud.google.com/docs).<br><br>

<a name="iam"></a>
## IAM (Identity and Access Management)
Powerful and flexible service that enables you to manage access to resources within Google Cloud Platform (GCP). 

IAM allows you to **control who has what level of access to which resources, ensuring the security and confidentiality** of your cloud-based applications and data.

 It's a fundamental component of GCP's security model, allowing you to implement the principle of least privilege and follow the principle of granting the minimum necessary permissions to perform a task.

 - Supports the use of **conditions** to specify constraints on when a policy binding should be applied.
 - **Actions and changes to IAM policies are logged**, allowing you to track who made changes and when.
 - A **policy binding associates a role with a list of members (principals)**, granting them the permissions defined by that role.
 - **Permissions are individual actions that can be granted to principals.** Each role is composed of one or more permissions.
 - **Roles define a set of permissions that determine what actions a principal can perform on specific resources.**
 - **Principals are entities that can make API requests to Google Cloud resources.**

Here you can find more about [Google Cloud IAM](https://cloud.google.com/iam/docs?hl=es-419)<br><br>

<a name="cloud-endpoints"></a>
## Cloud Endpoints

Google Cloud Endpoints helps developers **create, deploy, protect, and monitor APIs** for applications hosted on Google Cloud. **Designed to make it easier to build scalable and secure APIs**, handling many of the complexities associated with API development, such as authentication, authorization, monitoring, and deployment.

**Helps streamline the process of developing, deploying, and managing APIs**, allowing developers to focus more on building features and functionality for their applications.

 - Allows you to **design, deploy, and manage APIs using the OpenAPI Specification (OAS)**, formerly known as **Swagger.**
 - **Supports various authentication methods**, including Google Identity Platform, Firebase Authentication, and API keys.
 - Makes it easy to deploy your API to Google Cloud using Google *Kubernetes Engine (GKE) or App Engine* standard environment.
 - You can **monitor your API's usage and performance** through Google Cloud's monitoring and logging tools.
 - Integrates with Google Cloud's API analytics service, which provides insights into your API's usage patterns, user engagement, and other relevant metrics.
 - **Generates client libraries for various programming languages**, making it easier for developers to integrate and use your API in their applications.
 - **You can also implement custom authentication** using bearer tokens for scenarios that require more advanced authentication mechanisms.

Here you can find more about [Google Cloud Endpoints](https://cloud.google.com/endpoints/docs?hl=es-419)<br><br>


<a name="compute-engine"></a>
## Compute Engine

**Provides virtual machine (VM) instances for running applications.** It's an Infrastructure as a Service (IaaS) offering that allows you to create and manage virtual machines in the Google Cloud environment. Widely used for a variety of use cases, including **web hosting, application deployment, data processing, machine learning**, and more.

 - **Enables you to create, customize, and manage virtual machines** that run on Google's infrastructure.
 - You can **quickly scale your virtual machine instances up or down** based on your application's demands.
 - Provides a **range of predefined machine types** optimized for various use cases, such as general-purpose computing, memory-intensive applications, and high-performance computing.
 - Virtual machine instances on Compute Engine **can be attached to persistent disks for storing data.**
 - You can use **predefined images** provided by Google or create custom images to use as templates for your VM instances
 - Offers networking features like **Virtual Private Cloud (VPC), load balancing, and firewalls.**
 - In addition to general-purpose VMs, Compute Engine **offers instances with GPU (Graphics Processing Unit) and TPU (Tensor Processing Unit) accelerators.**
 - Offers the option of **sole tenancy**, where you can have dedicated physical servers for your VM instances.

Here you can find more about [Google Cloud Compute Engine](https://cloud.google.com/compute/docs?hl=es-419)<br><br>

<a name="load-balancing"></a>
## Load Balancing

**Distributes incoming network traffic across multiple instances or services to ensure high availability, improve performance, and manage traffic effectively.** It's a crucial component for building scalable and reliable applications on the cloud. By distributing traffic intelligently, **it allows you to handle varying levels of load** and ensures a smooth experience for users.

The different types of Load Balancing scenarios are:
 - **Global Load Balancing**: Software-defined, fully distributed load balancer that directs traffic to backend instances across multiple regions.
 - **HTTP(S) Load Balancing**: It can distribute traffic to backend instances or services based on advanced criteria such as URL path, host, and header values. It supports content-based routing, SSL termination, and cookie-based session affinity.
 - **TCP/UDP Load Balancing**: Used for non-HTTP(S) traffic. It can distribute TCP and UDP traffic to backend instances or services based on IP address and port.
 - **Internal Load Balancing**: Used to distribute traffic within a Virtual Private Cloud (VPC) network, making it accessible only to instances within the same network.
 - **Network Load Balancing**: Regional load balancer that operates at Layer 4 (transport layer) and can distribute traffic based on IP protocol data.

Here's some facts and utilities about Load Balancing:
 - **Work seamlessly with Google Cloud's auto-scaling capabilities.**
 - **Global load balancers use Anycast IP addresses**, meaning that they advertise the same IP address across multiple regions.
 - **Global load balancers distribute traffic across multiple regions**, improving latency and providing disaster recovery capabilities.
 - **HTTP(S) Load Balancing supports routing traffic based on URL paths, headers, and other attributes**, allowing for sophisticated traffic management.
 - Load balancers **can use session affinity (sticky sessions)** to route subsequent requests from a client to the same backend instance, maintaining session context.

Here you can find more about [Google Cloud Load Balancing](https://cloud.google.com/load-balancing/docs?hl=es-419)<br><br>

<a name="gke"></a>
## Google Kubernetes Engine (GKE)

**Kubernetes is an open-source container orchestration platform that automates the deployment, scaling, and management of containerized applications.** GKE simplifies the process of deploying and managing Kubernetes clusters, making it easier for developers to run containerized applications in a production environment.

 - **Abstracts the underlying infrastructure and handles many of the operational aspects** of managing Kubernetes clusters.
 - **Leverages containers to package applications and their dependencies**, making it easier to ensure consistency across different environments and simplifying the deployment process.
 - **Allows you to define different node pools within** a cluster with varying machine types, sizes, and configurations.
 - **Google Container Registry allows you to store and manage Docker container images.**
 - **With Anthos, Google's hybrid and multi-cloud platform, you can manage GKE clusters across on-premises, Google Cloud, and other cloud providers from a single dashboard.**
 - GKE **can automatically detect and repair unhealthy nodes**, ensuring that your applications continue running without manual intervention.

Here you can find more about [Google Kubernetes Engine (GKE)](https://cloud.google.com/kubernetes-engine/docs?hl=es-419)<br><br>

<a name="cloud-storage"></a>
## Google Cloud Storage

**Allows you to store and retrieve a wide variety of data, ranging from small files to large datasets, in a highly available and secure manner.** Is versatile and widely used for various purposes, including backup and recovery, data archival, serving static website content, sharing large datasets, and more.

 - **Uses an object storage model**, where data is organized into containers called "buckets".
 - Buckets and objects within Google Cloud Storage **are accessible from anywhere on the internet**, making it suitable for serving content to users globally.
 - **Is designed for high durability**, ensuring that your data is redundantly stored across multiple locations.
 - **Offers different storage classes to accommodate various use cases and access patterns.**
 - **You can set up lifecycle policies to automatically transition objects between storage classes** or delete them after a specified period.
 - **Access to Google Cloud Storage objects and buckets is controlled through Identity and Access Management (IAM) policies.**
 - **Offers encryption at rest to safeguard your data.**
 - **You can access your Google Cloud Storage data through the Google Cloud Console**, command-line tools, RESTful APIs, and client libraries in various programming languages.

Here you can find more about [Google Cloud Storage](https://cloud.google.com/storage/docs?hl=es-419)<br><br>

<a name="cloud-cdn"></a>
## Google Cloud CDN
Google Cloud CDN (**Content Delivery Network**) aims to enhance the performance, reliability, and scalability of your applications by **delivering content and assets to users from globally distributed edge servers.** 

CDNs are **designed to reduce latency and improve load times for websites and applications** by caching content closer to the user, thereby reducing the distance data has to travel.

It's particularly **useful for websites and services with a global user base**, where reducing latency and improving load times are critical factors in providing a good user experience.

 - **Caches content at these edge locations**, storing copies of your assets like images, videos, stylesheets, and more.
 - When a user requests content, the CDN **delivers it from the closest edge location**, minimizing latency and network congestion.
 - While traditional CDNs are excellent for caching static content, Google Cloud CDN is also **capable of accelerating dynamic content.**
 - Provides **SSL/TLS termination at the edge.**
 - Uses **Anycast IP addresses**, which means that multiple edge locations share the same IP address.
 - **Supports the modern HTTP/2 protocol.**
 - Additionally, it **supports Brotli compression,** which is a more efficient compression algorithm for reducing the size of web assets. 
 - **Allows you to set up cache invalidation rules based on URL patterns.**

Here you can find more about [Google Cloud CDN](https://cloud.google.com/cdn/docs?hl=es-419)<br><br>

<a name="cloud-sql"></a>
## Google Cloud SQL
Managed **relational database service** that **allows you to set up, operate, and scale relational databases** without the need to manage the underlying infrastructure.

**Simplifies the management of relational databases**, making it a suitable choice for various use cases, from small applications to large-scale projects that require high availability, scalability, and security.
- Supports multiple database engines, including:
	-   **MySQL:** A popular open-source RDBMS.
	-   **PostgreSQL:** A powerful open-source relational database system.
	-   **SQL Server:** A Microsoft-developed RDBMS.

Here's some features about Google Cloud SQL:

- Google **handles many of the routine database management tasks** such as patch management, backups, replication, failover, and scaling.
- **Performs automated backups** of your database.
- **Read replicas** allow you to offload read traffic from the primary instance.
- Enables **point-in-time recovery**, allowing you to restore your database to a specific point in time.
- **Lets you modify database engine behavior using flags.**
- Offers a **serverless option for MySQL databases.**

Here you can find more about [Google Cloud SQL](https://cloud.google.com/sql/docs?hl=es-419)<br><br>

<a name="dataflow"></a>
## Google Cloud Dataflow
**Stream and batch data processing service** that enables developers to **process and analyze data in real-time and in batch,** making it easier to build data pipelines for various use cases such as *ETL (Extract, Transform, Load), analytics, and machine learning.*

**Allows developers to focus on their data processing logic, simplifies the development of data processing pipelines** by abstracting infrastructure management, providing a unified programming model, and supporting both stream and batch processing.

 - **Supports both stream processing (real-time) and batch processing (batch-oriented)** paradigms within the same programming model.
 - Is built on top of the **Apache Beam open-source project.**
 - **Automatically scales resources** based on the volume of data and the complexity of your processing logic.
 - **Offers a serverless execution environment** where you don't need to worry about provisioning or managing infrastructure.
 - **Provides built-in support for windowing and time-based processing.**
 - **Includes connectors to various data sources and sinks**, including *Google Cloud Storage, BigQuery, Pub/Sub,* and more.
 - **Flex Templates** allow you to package your Dataflow pipeline into a reusable template, making it easier to deploy the same pipeline with different configurations.
 - **Supports stateful processing**, which enables you to maintain and update state information across data elements in your pipeline.

Here you can find more about [Google Cloud Dataflow](https://cloud.google.com/dataflow/docs?hl=es-419)<br><br>

<a name="cloud-functions"></a>
## Google Cloud Functions
Serverless compute service that allows developers to build and deploy event-driven functions that automatically scale as needed without requiring the management of underlying infrastructure.

Powerful tool for building event-driven, serverless applications and workflows. It's particularly useful for tasks that need to respond quickly to changes in data, perform lightweight processing, and integrate with other Google Cloud services.<br>
 - Can be triggered by events from various sources, such as:
	-   **Cloud Storage:** Respond to changes in objects within a storage bucket.
	-   **Cloud Pub/Sub:** React to messages published to a pub/sub topic.
	-   **HTTP:** Create HTTP-triggered functions to respond to HTTP requests.
	-   **Firestore:** Trigger functions based on changes in Firestore documents.
	-   **Firebase Authentication:** Trigger functions when users are authenticated or their profiles are updated.

Here's some features about Google Cloud Functions:

 -  **You don't need to manage servers or infrastructure.**
 - **Supports multiple programming languages**, including *Node.js, Python, Go, and Java.* This flexibility allows you to use the language you're most comfortable with.
 - Cloud Functions are **stateless by design**, meaning they don't store persistent state.
 - You can configure your Cloud Functions to **respond to specific event conditions.**
 - By default, **limits the number of concurrent invocations per function** to ensure efficient resource utilization.
 - Cloud Functions can be **categorized as background functions (triggered by events) or HTTP functions (triggered by HTTP requests).**

Here you can find more about [Google Cloud Functions](https://cloud.google.com/functions/docs?hl=es-419)<br><br>

