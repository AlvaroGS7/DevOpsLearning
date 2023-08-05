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
- **2.19 -** [GuardDuty](#guardduty)
- **2.20 -** [Aurora](#aurora)
- **2.21 -** [EBS (Elastic Block Store)](#ebs)
- **2.22 -** [IoT Core](#iot-core)

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
This resource is a web service that enables **secure management of access to AWS resources.** 

You can control also and manage user identities, permissions, and policies within your AWS account.

- Provides functionalities for **managing access** to AWS resources.
- **Supports roles and federation**, allowing you to grant specific permissions to AWS services and trusted entities.
- Allows you to **integrate IAM with external identity providers**, such as Active Directory, enabling users to access AWS resources with their existing credentials.
- Has **logging capabilities**, which enable monitoring and tracking of user activity within your AWS account.
- **Free to use in your AWS account**, with no additional cost beyond the usage of AWS resources.
- Is **region-specific**, meaning that user accounts, policies, and roles created in one region are not automatically available in other regions.
- **Supports cross-account access**, allowing you to grant access to your AWS resources to users from other AWS accounts.<br><br>

Here you can read more about [AWS Identity Access Management](https://docs.aws.amazon.com/iam/).<br><br>

## API Gateway
Fully managed service that enables you to **create, publish, and manage APIs (Application Programming Interfaces) for your applications** and back-end services. 

It acts as a front-door for your APIs, allowing you to securely expose them to external clients or internal applications.

 - You can easily **define RESTful APIs or WebSocket APIs** using its intuitive interface.
 - Supports various **authentication mechanisms** like A*WS Identity and Access Management (IAM) roles, AWS Cognito*, and custom authorizers.
 - Allows **request and response transformations**, enabling the modification of data structure, content, or headers.
 - Provides **built-in rate limiting and throttling capabilities** to protect your APIs.
 - Supports **versioning and deployment of APIs**, allowing you to manage different versions and environments without disrupting existing clients.
 - **Uses Amazon CloudFront's global network of edge locations** to provide edge-optimized endpoints by default.

Here you can read more about [API Gateway](https://docs.aws.amazon.com/apigateway/index.html).<br><br>

<a name="ec2"></a>
## EC2 (Elastic Compute Cloud)
Web service provided that **offers resizable compute capacity in the cloud**. 

It allows you to quickly provision virtual servers, known as EC2 instances, and run applications or services on them.
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
Service that **helps distribute incoming network traffic across multiple targets**, such as Amazon EC2 instances, containers, and IP addresses.

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
Fully managed **container orchestration service** that allows you to run, manage, and scale containerized applications using Docker containers.

Here's some useful features about it:

 - **You can use task definition**, a blueprint that defines how a containerized application should be deployed.
 - **ECS integrates seamlessly with ELB.**
 - **ECS offers integration with AWS Fargate** (A serverless compute engine for containers).
 - **Uses capacity providers**, which are used to define the type and amount of infrastructure resources available for running containers.
 - **Provides a task metadata endpoint** that allows containers within a task to retrieve information about themselves

 Here you can read more about [Elastic Container Service](https://docs.aws.amazon.com/elasticloadbalancing/).<br><br>

<a name="s3"></a>
## S3 (Simple Storage Service)
Offers scalability, durability, and security to **store and retrieve any amount of data from anywhere on the web.** 

Used for a variety of storage use cases, **ranging from simple backup and archiving to hosting static websites** and powering data lakes for big data analytics.

Here's some useful features about S3:

 - **Offers lifecycle management capabilities**, which allow you to automate the movement of objects between different storage classes.
 - **Supports versioning**, which enables you to keep multiple versions of an object in the same bucket.
 - **Can generate event notifications** when specific actions occur, such as object creation, deletion, or restoration.
 - **Uses transfer acceleration**, that enables faster data uploads and downloads to and from S3.
 - **Provides eventual consistency** for overwrite PUTS and DELETES.
 - Allows you to retrieve only a subset of data from an object by using **SQL-like queries**.

 Here you can read more about [Simple Storage Service](https://docs.aws.amazon.com/s3/index.html).<br><br>
 
## CloudFront
A **content delivery network (CDN) service** that delivers content to users with low latency and high data transfer speeds.

Whether you are running a website, a mobile application, or an API, **CloudFront can significantly enhance the performance and user experience** of your applications by bringing content closer to your end users.

 - Offers an optional feature called **Origin Shield**, which provides an
   additional caching layer between the edge locations and your origin
   server.
 - Provides **detailed logs and real-time monitoring** capabilities.
 - Integrates with AWS Lambda through a feature called **Lambda@Edge.**
 - Provides a feature called **Geo-Restriction**, which allows you to control the countries from which your content can be accessed.
 - Supports **field-level encryption**, which enables you to encrypt specific fields in your web forms or API requests.
 - Supports **origin failover**, which allows you to set up multiple origin servers for redundancy.

 Here you can read more about [CloudFront](https://docs.aws.amazon.com/cloudfront/index.html).<br><br>

<a name="rds"></a>
## RDS (Relational Database Service)

Also called **Amazon Relational Database Service**, is a **managed database service** that simplifies the process of setting up, operating, and scaling relational databases in the cloud.

 - **Enables automated backups of your databases**, which are retained for a user-defined period.
 - **Allows you to create read replicas of your databases**, which are asynchronously replicated copies of your primary database.
 - **Supports certain extensions specific to different database engines.**
 - **Amazon Aurora**, a MySQL and PostgreSQL-compatible database engine, offers a serverless option within RDS.
 - Provides a **database proxy feature** that allows you to manage connections to your RDS databases.
 - **Offers a Data API that allows you to interact with your databases** using HTTP-based API calls instead of traditional database connections.
 
 Here you can read more about [Relational Database Service](https://docs.aws.amazon.com/rds/index.html).<br><br>
 
<a name="glue"></a>
## Glue
**A fully managed extract, transform, and load (ETL) service** pthat enables you to prepare and transform your data for analytics, data warehousing, machine learning, and other data-driven tasks.

 - Provides a **centralized metadata repository called the Data Catalog.**
 - Offers a **visual interface and built-in ETL jobs** that allow you to transform and clean your data.
 - Can **automatically discover the schema and structure of your data** by crawling the data sources.
 - Provides a **serverless execution environment** for running ETL jobs.
 - Introduces the concept of **Dynamic Frames**, which are an extension of Apache Spark DataFrames.
 - **Supports schema evolution**, allowing you to handle changes in the schema of your data over time.
 - **Supports connection sharing across multiple ETL jobs.**
 - **Offers custom classifiers**, which allow you to define your own logic for classifying and cataloging data.

 Here you can read more about [AWS Glue](https://docs.aws.amazon.com/glue/index.html).<br><br>

## Lambda
A **serverless compute service** that allows you to run your code without provisioning or managing servers, and you only pay for the compute time consumed by your code. 

AWS Lambda **supports a wide range of programming languages** and can be used for various types of applications and workloads.

 - **Functions are triggered by events** from various AWS services.
 - **Supports multiple programming languages**, including *Python, JavaScript (Node.js), Java, C#, Ruby, and Go.*
 - **Functions are stateless**, meaning they don't maintain any persistent state between invocations.
 - Provides **built-in support for several programming languages**, you can also create custom runtimes.
 - Has a feature called **provisioned concurrency**, that allows you to allocate a set number of concurrent executions to your functions.
 - Lambda **now supports running functions inside custom Virtual Private Clouds (VPCs).**
 - **Extensions are companion processes** that can run alongside your Lambda functions.

 Here you can read more about [AWS Lambda](https://docs.aws.amazon.com/lambda/index.html).<br><br>

## Step Functions

**A serverless workflow orchestration service** that allows you to coordinate and sequence multiple AWS services. With Step Functions, you can **visually define and execute workflows**, known as state machines, that model complex business processes or application workflows.

 - **Uses state machines to represent workflows.**
 - Provides **built-in execution control** capabilities. 
 - **You can define conditions, timeouts, retries, and error handling** for each state in your state machine.
 - **Supports both parallel and sequential execution** of tasks within a workflow.
 - **Enables event-driven workflows.**
 - Offers a local development and testing environment called **"Step Functions Local".**
 - **Supports the concept of nested workflows** or sub-workflows.

 Here you can read more about [Step Functions](https://docs.aws.amazon.com/step-functions/index.html).<br><br>

## Kinesis

**A suite of fully managed services** that enables real-time data streaming and processing at scale. 

**It is designed to ingest, process, and analyze large amounts of data in real-time**, allowing you to build applications that require immediate insights and responsiveness to streaming data.

There are three primary services within AWS Kinesis:

 - **Amazon Kinesis Data Streams**: Allows you to continuously capture and store streaming data from various sources, such as website clickstreams, IoT devices, log data, social media feeds, and more.
 - **Amazon Kinesis Data Firehose**: Simplifies the process of loading streaming data into storage and analytics services.
 - **Amazon Kinesis Data Analytics**: Allows you to process and analyze streaming data in real-time using standard SQL queries.

Here's some featureas about Kinesis:

 - Kinesis Data Streams allows you to **specify the retention period for your data.**
 - Offers a feature called "**Enhanced Fan-Out**" that allows you to build applications with low-latency data processing and real-time data delivery.
 - Provides **built-in support for time series data** using a feature called "time-based partitioning".
 - **Allows you to reference external data sets**, known as "reference data," within your SQL queries.
 - **Supports continuous querying**, which allows you to continuously process and analyze the incoming streaming data.
 - **Automatically maintains checkpoints** to track the processing progress of the streaming data.

 Here you can read more about [Kinesis](https://docs.aws.amazon.com/kinesis/index.html).<br><br>

<a name="sqs"></a>
## SQS (Simple Queue Service)
**Fully managed message queuing** that allows you to scale distributed systems by providing a reliable way to **send, store, and receive messages** between various software microservices.

Here's some **key features** about SQS:

 - Provides a message queue model, where **messages are sent by producers and retrieved by consumers**.
 - Is **designed to be distributed**, making it highly available and fault-tolerant. 
 - It **replicates messages across multiple availability zones**, ensuring high durability.
 - Messages sent to an SQS queue are **retained until they are explicitly deleted** by consumers or reach their maximum retention period.
 - **Offers FIFO (First-In-First-Out) queues.**
 - **Supports message deduplication**, which allows you to ensure that duplicate messages are not sent to the queue within a specific time window.
 - You can create and manage SQS queues using **AWS CloudFormation.**
 
  Here you can read more about [AWS SQS](https://docs.aws.amazon.com/sqs/index.html).<br><br>

  <a name="eks"></a>
## EKS (Elastic Kubernetes Service)
Fully managed **container orchestration service** that allows you to **deploy, manage, and scale containerized applications using Kubernetes**, an open-source container orchestration platform.

This is suitable for organizations looking to run containerized applications with Kubernetes but prefer to offload the management of the Kubernetes control plane to AWS.

 - **Takes care of the Kubernetes control plane**, which includes the API server, etcd, and other critical components.
 - **Compatible with standard Kubernetes**, which means you can use familiar Kubernetes tools and APIs to interact with the EKS cluster.
 - **Integrates with other AWS services**, such as *Amazon ECR (Elastic Container Registry)* for container image storage, *AWS IAM* for authentication, and *AWS CloudTrail* for auditing and logging.
 - Offers an option to **run Kubernetes pods on AWS Fargate**, a serverless compute engine for containers.
 - Offers **support for multiple Kubernetes versions.**
 - **Supports OpenID Connect (OIDC)** for cluster authentication.

Here you can read more about [AWS EKS](https://docs.aws.amazon.com/eks/latest/userguide/getting-started.html).<br><br>

<a name="cloudwatch"></a>
## Cloudwatch

**Monitoring and observability service** that enables you to **collect and track metrics, collect and monitor log files**, and set alarms for your AWS resources and applications in real-time.

**Fundamental tool for managing** your AWS infrastructure, providing real-time visibility and ensuring that your applications and services run smoothly.

 - **Collects and stores various metrics from AWS resources** such as *EC2 instances, RDS databases, S3 buckets*, and more. 
	 - These metrics include *CPU utilization, network traffic, disk I/O*, and custom application-specific metrics.
 - Allows you to create **customized dashboards** to visualize your metrics in real-time.
 - **Set up notifications** based on predefined thresholds for your metrics.
 - Set **retention policies** for your CloudWatch log data, determining how long it is stored and you can use Amazon S3 for long-term storage and compliance purposes.
 - Supports **cross-account access**, allowing you to collect and view metrics and logs from multiple AWS accounts in a centralized manner.
 - **CloudWatch Synthetics** enables you to monitor your application endpoints and workflows using **canaries** (configurable scripts that mimic user interactions).

Here you can read more about [AWS CloudWatch](https://docs.aws.amazon.com/cloudwatch/index.html).<br><br>

<a name="sns"></a>
## SNS (Simple Notification Service)
**Messaging service** that enables you to send messages or notifications to distributed systems, mobile devices, email, and other endpoints in a flexible and scalable manner.

Simplifies the process of sending messages to multiple recipients simultaneously, making it a valuable tool for building event-driven architectures and real-time communication applications.

Commonly used in a wide range of applications, including mobile app push notifications, email notifications, monitoring and alerting systems, and building event-driven microservices architectures.

 - **Uses topics as communication channels.**
 - Supports **multiple communication protocols**, including *HTTP/HTTPS, Amazon SQS (Simple Queue Service), SMS, email, mobile push notifications, and AWS Lambda functions.*
 - **Enables fanout messaging**, meaning you can send a single message to a topic.
 - Provides the ability to **track the delivery status** of messages to subscribers.
 - Automatically **handles SMS opt-out management**, respecting the Do Not Disturb (DND) preferences of recipients.
 - Allows you to **send mobile push notifications with custom payload data.**

Here you can read more about [AWS SNS](https://docs.aws.amazon.com/cloudwatch/index.html).<br><br>

<a name="sagemaker"></a>
## Sagemaker

**Machine learning service** that enables data scientists and developers to build, train, and deploy machine learning models at scale without the need for managing the underlying infrastructure.

Simplifies the end-to-end machine learning workflow, from data preparation to model deployment.

Widely used across various industries and applications, including recommendation systems, fraud detection, image and speech recognition, forecasting, and natural language processing.

 - Provides a managed **Jupyter Notebook environment** that allows data scientists to explore and analyze data, prototype machine learning models, and collaborate on projects.
 - Offers **data preprocessing capabilities** to clean, transform, and prepare data for training models.
 - You can **bring your own custom algorithms and libraries.**
 - Allows you to **create and manage training jobs**, which distribute and parallelize the training process across multiple instances to accelerate model training.
 - Once the model is trained, SageMaker **can host the model as an endpoint**, making it accessible for real-time predictions or batch inference. 
 - Allows you to **deploy multiple models on a single endpoint.**
 - Allows you to **bring your own Docker containers** for training and inference.

Here you can read more about [AWS Sagemaker](https://docs.aws.amazon.com/sagemaker/index.html).<br><br>

<a name="cloudtrail"></a>
## CloudTrail
**Service that enables you to monitor, log, and retain account activity** related to your AWS resources.

Provides **detailed information about actions taken by users, roles, or services** within your AWS account, making it a valuable tool for security, compliance, and operational auditing.

By providing a **detailed record of actions taken within your AWS environment**, CloudTrail helps you ensure security, track changes, troubleshoot issues, and maintain compliance with industry regulations.

 - **Records API activity**, management console actions, and other account-level activity across all AWS services.
 - **Captures management events** related to AWS management activities, such as AWS Management Console sign-ins, changes to IAM policies, and security group modifications.
 - Can be configured to **log S3 data events** at the object level.
 - Can **capture data events for AWS Lambda** functions.
 - Supports an **Event Selector feature** that allows you to choose specific events and data attributes to log.
 - Can enable **trail log file validation** for AWS CloudTrail trails.

Here you can read more about [AWS CloudTrail](https://docs.aws.amazon.com/es_es/awscloudtrail/latest/userguide/cloudtrail-user-guide.html).<br><br>
