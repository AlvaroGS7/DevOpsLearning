## Good Practices Compilation
**This is just a best practice compilation made by Álvaro González. Some of the most important ones could be missing but I have tried to have most of them.
![General DevOps IMG](https://ibagroup.kz/wp-content/uploads/2020/06/banner_1300-357_DevOps.png)
## INDEX
**1.-** [General Good Practices](#general)

**2.-** [Azure Cloud](#azcloud)

**3.-** [Amazon Web Services Cloud](#awscloud)

**4.-** [Google Cloud Platform](#googlecloud)

## General Good Practices
 - Give your resources and objects **descriptive and useful names** so they are easy to **identify** in the 	environment.
 - The DevOps team and devs should **work together to build the original pipeline**.
 -   **DO NOT EXPOSE** (If you do, is always better with secrets and vars, not in plain text):
	 -  Sensitive data
	 - Credentials
	 - Company data
	 - IP's
	 - URL's 
	 - Private files.
 - All code should be under **version control**.
 - [Work on the most important thing first](http://www.theagilemindset.co.uk/the-scrum-philosophy/)
 - Focus on **continuous improvement** of processes in manufacturing, engineering, development, and business management.
 - Developers are responsible for **monitoring and alerting**
 -  **Maintain up-to-date documentation** to ensure proper knowledge sharing and collaboration within your team.
	 - You can use tools like *Google Docs, Google Drive*, or third-party documentation platforms.

## Azure Cloud
![AZ Cloud IMG](https://www.evozon.com/wp-content/uploads/2017/05/Azure-Banner.png)
 - Your code should create **all the items within a resource.**
 - The goal of your code should be that you can **compile and run without any prerequisites**.
 - **CI/CD**
	 - Set up CI pipelines to **automatically build and test** your code whenever changes are pushed to the repository.
	 - Implement CD pipelines to **automate the deployment process.**
 - Store **build artifacts**, such as compiled binaries or deployment packages, in a centralized repository.
 - Use **separate environments** for development, testing (QA), staging, and production.
 - Ensure **consistent and reproducible infrastructure deployments.** 
	 - You can do this using Azure Resource Manager templates, Az CLI or Az Poweshell.
 - Incorporate **security and compliance practices** into your pipeline.
 - Use **role-based access controls and secrets management** to protect sensitive information.
 - Implement **monitoring and logging solutions** to gain visibility into your applications and infrastructure. 
	 - Here you can use Azure Monitor or Application Insights.
 - Regularly **review and improve** your pipelines and processes.

## Amazon Web Services Cloud
![AWS Cloud IMG](https://tudip.com/wp-content/uploads/2019/01/awsBanner.jpg)

 - **Use a configuration management tool** to define and provision your infrastructure resources programmatically.
	 - You can use *AWS CloudFormation or AWS CDK.*
 - Store your infrastructure code and related scripts in a **version control system like Git**.
 - Use **immutable infrastructure**, where resources are treated as disposable entities. 
	 - Tools like *AWS Auto Scaling and AWS Elastic Beanstalk* can help with this approach.
 - **Follow the principle of least privilege**, granting only the necessary permissions to users and services. 
	 - Use *AWS Identity and Access Management (IAM)* roles, security groups, and network ACLs.
 - **Automate repetitive tasks** and processes to increase efficiency and reduce human error. 
	 - Use AWS services like *AWS Lambda, AWS Step Functions, and AWS Systems Manager Automation*.
 - **Implement CI/CD pipelines** to automate the building, testing, and deployment of your applications. 
	 - Services like *AWS CodePipeline, AWS CodeBuild, and AWS CodeDeploy* can help you achieve this.
 - Establish a **monitoring and logging** strategy to gain visibility.
	 - Use *AWS CloudWatch* to monitor metrics, set up alarms and visualize logs. Consider using A*WS CloudTrail* for auditing and *AWS X-Ray* for distributed tracing.
 - Implement **backup and disaster recovery** to protect your data and ensure business continuity. 
	 - Use services like *AWS Backup, AWS S3 for backups, and AWS Glacier* for long-term archiving.
 - **Optimize your resource usage and costs** by rightsizing your infrastructure, utilizing cost-effective instance types, and leveraging services
	 - You can use *AWS Cost Explorer and AWS Budgets* to monitor and control your expenses. You can also use *AWS Reserved Instances* for predictable workloads.

## Google Cloud Platform
![Google Cloud IMG](https://d3iux33l8x59j6.cloudfront.net/imagenes/noticias/google-cloud-banner.jpg)

 - **Define and provision your infrastructure resources programmatically.** This enables repeatability, version control, and easier management of your infrastructure.
	 - You can use utilities like *Google Cloud Deployment Manager or Terraform*.
 - **Implement security measures** . Follow the principle of least privilege.
	 - You can use *Google Cloud Identity and Access Management (IAM)* to manage access controls.
 - **Automate repetitive tasks and processes** to increase efficiency.
	 - Leverage tools like *Google Cloud Functions, Google Cloud Scheduler, and Google Cloud Pub/Sub*.
 - **Implement CI/CD pipelines** to automate the building, testing, and deployment of your applications.
	 - In Google Cloud you have Google Cloud Build, Google Cloud Source Repositories, and Google Cloud Deployment Manager.
 - Embrace **monitoring and logging.**
	 - Use services like *Google Cloud Monitoring, Google Cloud Logging, and Google Cloud Trace.
 - Design your applications for **high availability and fault tolerance**.
	 - Use *Google Cloud Load Balancing, Google Kubernetes Engine (GKE)* for container orchestration, and *Google Cloud Memorystore* for managed Redis.
 - Implement **backup and disaster recovery** mechanisms.
	 - Use services like *Google Cloud Storage* for backups, *Google Cloud SQL*  for managed relational databases with built-in replication and backups, and  *Google Cloud Spanner* for globally distributed relational databases.
 - **Optimize your resource usage and costs** by rightsizing your infrastructure.
	 - Use services like *Google Cloud Billing API and Google Cloud Cost Management* tools.
