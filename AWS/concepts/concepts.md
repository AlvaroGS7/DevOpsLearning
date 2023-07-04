

# List of AWS Cloud General Concepts
![AWS Banner](https://tudip.com/wp-content/uploads/2019/01/awsBanner.jpg)

# INDEX

**1.** [What is AWS](#what-is-aws)

**2.** [Most Common Concepts](#most-common-concepts)

- **2.1 -** [IAM (Identity and Access Management)](#iam)
- **2.2 -** [API Gateway](#api-gateway)
- **2.3 -** [EC2 (Elastic Compute Cloud)](#ec2)
- **2.4 -** [ELB (Elastic Load Balancer)](#elb)
- **2.5 -** [ECS (Elastic Container Service)](#ecs)
- **2.6 -** [S3 (Simple Storage Service)](#s3)
- **2.7 -** [CloudFront](#cloudfront)
- **2.8 -** [RDS (Relational Database Service)](#rds)
- **2.9 -** [Glue](#glue)
- **2.10 -** [Lambda](#lambda)
- **2.11 -** [Step Functions](#step-functions)
- **2.12 -** [Kinesis](#kinesis)
- **2.13 -** [SQS (Simple Queue Service)](#sqs)
- **2.14 -** [EKS (Elastic Kubernetes Service)](#eks)
- **2.15 -** [CloudWatch](#cloudwatch)
- **2.16 -** [SNS (Simple Notification Service)](#sns)
- **2.17 -** [Sagemaker](#sagemaker)
- **2.18 -** [CloudTrail](#cloudtrail)
- **2.19 -** [SQS (Simple Queue Service)](#sqs)
- **2.20 -** [GuardDuty](#guardduty)
- **2.21 -** [Aurora](#aurora)
- **2.22 -** [EBS (Elastic Block Store)](#ebs)
- **2.23 -** [IoT Core](#iot-core)

## What is AWS

AWS (Amazon Web Services), a leading cloud computing platform, offers a comprehensive range of services and features for businesses.

Provided by Amazon, AWS provides a robust infrastructure for computing power, storage, networking, and databases. It enables users to easily build, deploy, and manage applications through its globally distributed data centers.

With AWS, users can leverage virtual machines, multiple storage options, and networking capabilities to create a flexible and scalable infrastructure that suits their needs.

AWS also offers managed database services, application services, artificial intelligence (AI) tools, and Internet of Things (IoT) services, empowering organizations to harness advanced technologies for innovation and growth.

A key strength of AWS is its commitment to security, offering services such as AWS Identity and Access Management (IAM), AWS WAF (Web Application Firewall), and AWS Key Management Service (KMS) to ensure robust security measures.

Additionally, AWS follows a pay-as-you-go pricing model, allowing businesses to optimize costs by paying only for the resources they consume.

The scalability, reliability, and cost-effectiveness of AWS make it an attractive choice for organizations of all sizes, enabling them to scale their infrastructure, increase operational efficiency, and drive digital transformation.

Here you can look for the full [AWS Documentation](https://docs.aws.amazon.com).<br><br>

# Most Common Concepts

In this block, I will explain some of the commonly used resources in AWS and how they function. AWS offers a wide range of services that cater to different needs and requirements. AWS also provides services for analytics, machine learning, security, and many other areas. Each resource has its own unique functionalities and capabilities, empowering users to build and deploy a wide variety of applications and services in a flexible and scalable manner.<br><br>

<a name="iam"></a>
## IAM (Identity and Access Management)
This resource is a web service that enables **secure management of access to AWS resources.** You can control also and manage user identities, permissions, and policies within your AWS account.

- Provides functionalities for **managing access** to AWS resources.
- **Supports roles and federation**, allowing you to grant specific permissions to AWS services and trusted entities.
- Allows you to **integrate IAM with external identity providers**, such as Active Directory, enabling users to access AWS resources with their existing credentials.
- Has **logging capabilities**, which enable monitoring and tracking of user activity within your AWS account.
- **Free to use in your AWS account**, with no additional cost beyond the usage of AWS resources.
- Is **region-specific**, meaning that user accounts, policies, and roles created in one region are not automatically available in other regions.
- **Supports cross-account access**, allowing you to grant access to your AWS resources to users from other AWS accounts.<br><br>

Here you can read more about [AWS Identity Access Management](https://docs.aws.amazon.com/iam/).<br><br>

## API Gateway
Fully managed service that enables you to **create, publish, and manage APIs (Application Programming Interfaces) for your applications** and back-end services. It acts as a front-door for your APIs, allowing you to securely expose them to external clients or internal applications.

 - You can easily **define RESTful APIs or WebSocket APIs** using its intuitive interface.
 - Supports various **authentication mechanisms** like A*WS Identity and Access Management (IAM) roles, AWS Cognito*, and custom authorizers.
 - Allows **request and response transformations**, enabling the modification of data structure, content, or headers.
 - Provides **built-in rate limiting and throttling capabilities** to protect your APIs.
 - Supports **versioning and deployment of APIs**, allowing you to manage different versions and environments without disrupting existing clients.
 - **Uses Amazon CloudFront's global network of edge locations** to provide edge-optimized endpoints by default.

Here you can read more about [API Gateway](https://docs.aws.amazon.com/apigateway/index.html).<br><br>

<a name="ec2"></a>
## EC2 (Elastic Compute Cloud)
Web service provided that **offers resizable compute capacity in the cloud**. It allows you to quickly provision virtual servers, known as EC2 instances, and run applications or services on them.
- Flexibility to choose from a **variety of instance types** based on your specific needs.
- You can easily **scale your compute capacity** up or down based on demand.
- Offers **different pricing options** to suit your workload and budget.
- You have the freedom to choose from a **wide range of operating systems** and can also install and **run your custom applications**.
- Instances can be launched in **multiple Availability Zones within a region**.
- **Instances can be launched with user data scripts**, which are executed when the instance starts.
- **You can use placement groups**, which enable low-latency network communication between instances in the same group.
- **Provides the capability to hibernate instances**.

Here you can read more about [Elastic Compute Cloud](https://docs.aws.amazon.com/ec2/index.html).<br><br>

<a name="elb"></a>
## ELB (Elastic Load Balancer)
Service that helps distribute incoming network traffic across multiple targets, such as Amazon EC2 instances, containers, and IP addresses.

There are three types of load balancers provided by AWS:
 - **Classic Load Balancer (CLB):** The original load balancer. It operates at both the request and connection level (Layer 4 and Layer 7 of the OSI model) and is suitable for simple applications.
 - **Application Load Balancer (ALB):** This load balancer operates at the application layer (Layer 7) and provides advanced routing and content-based routing capabilities.
 - **Network Load Balancer (NLB):** This load balancer operates at the transport layer (Layer 4) and is designed to handle high network throughput.

And here's some general features about ELB:
 - **ELBs can offload the SSL/TLS encryption and decryption** process.
 - **ALBs offer a feature called sticky sessions**, and can route requests from the same client to the same target for the duration of a session.
 - **You can enable Cross-zone Load Balancing for an ALB or CLB** to balance the load more evenly across instances in different AZs.
 - With ALBs, you can configure **custom error pages** for specific HTTP status codes.
 
 Here you can read more about [Elastic Load Balancers](https://docs.aws.amazon.com/elasticloadbalancing/).<br><br>

 <a name="ecs"></a>
## ECS (Elastic Container Service)
Fully managed container orchestration service that allows you to run, manage, and scale containerized applications using Docker containers.

Here's some useful features about it:

 - **You can use task definition**, a blueprint that defines how a containerized application should be deployed.
 - **ECS integrates seamlessly with ELB.**
 - **ECS offers integration with AWS Fargate** (A serverless compute engine for containers).
 - **Uses capacity providers**, which are used to define the type and amount of infrastructure resources available for running containers.
 - **Provides a task metadata endpoint** that allows containers within a task to retrieve information about themselves

 Here you can read more about [Elastic Container Service](https://docs.aws.amazon.com/elasticloadbalancing/).<br><br>
