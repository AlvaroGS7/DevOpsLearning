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

Distributes incoming network traffic across multiple instances or services to ensure high availability, improve performance, and manage traffic effectively. It's a crucial component for building scalable and reliable applications on the cloud.

Helps ensure that your applications are highly available, performant, and resilient to failures. By distributing traffic intelligently, it allows you to handle varying levels of load and ensures a smooth experience for users.

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
