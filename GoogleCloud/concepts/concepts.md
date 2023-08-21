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

# What is Google Cloud Platform (GCP)

GCP furnishes a **robust foundation for computing power, storage, networking, and databases**. This platform facilitates the effortless creation, deployment, and management of applications through its globally distributed network of data centers.

Through GCP, users can **make virtual machines, diverse storage choices, and advanced networking features to construct a malleable and scalable infrastructure** tailored to their requirements.

GCP **offers managed database services, application solutions, cutting-edge artificial intelligence (AI) tools, and services for the Internet of Things (IoT)**. These offerings empower organizations to leverage advanced technologies for driving innovation and fostering growth.

One of GCP's core strengths is its **steadfast dedication to security**. It provides a suite of security services including **Google Cloud Identity and Access Management (IAM), Cloud Web Security, and Google Cloud Key Management Service (KMS)** to ensure robust security protocols.

The scalability, dependability, and cost-efficiency of GCP position it as an appealing choice for entities of all sizes, enabling them to seamlessly expand their infrastructure, enhance operational efficiency, and navigate the realms of digital transformation.

# Most Common Concepts
  
In this section, I'll introduce you to some of the **fundamental concepts within Google Cloud Platform (GCP)**, which are essential for comprehending its core components and operational capabilities. These concepts lay the groundwork for effectively building and managing your cloud resources.

For further assistance and in-depth information, you can refer to the **official documentation** available [here](https://cloud.google.com/docs).

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
