



## Good Practices Compilation
*This is just a best practice compilation made by **Álvaro González**. Some of the most important ones could be missing but I've tried to have most of them.*

![General DevOps IMG](https://ibagroup.kz/wp-content/uploads/2020/06/banner_1300-357_DevOps.png)
## INDEX
**1.-** [General Good Practices](#general-good-practices)

**2.-** [Cloud](#Cloud)

 - **2.1 -** [Azure Cloud](#azure-cloud)
 - **2.2 -** [Amazon Web Services Cloud](#amazon-web-services)
 - **2.3 -** [Google Cloud Platform](#google-cloud-platform)

**3.-** [Software](#Software)
 - **3.1 -** [Ansible](#ansible)
 - **3.2 -** [Docker](#docker)
 - **3.3 -** [Kubernetes](#kubernetes)
 - **3.4 -** [Helm](#helm)
 - **3.5 -** [Prometheus](#prometheus)
 - **3.6 -** [Grafana](#grafana)

**4.-** [Scripts](#Scripts)

 - **4.1 -** [Python](#Python)
 - **4.2 -** [Shell](#Shell)
 - **4.3 -** [YAML](#YAML)

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
 - Official Documentation Link: https://learn.microsoft.com/en-us/azure/?product=popular

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
 - Follow the official documentation. You can find it here: https://docs.aws.amazon.com

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
 - **Use the official documentation.** Here's the official link: https://cloud.google.com/docs?hl=es

# Software 

## Ansible
![Ansible IMG](https://files.readme.io/4179edf-Cloudsmith-Integrations-Banner-Ansible.png)

 - **Organize your Ansible project using a logical directory structure.** Group related files together, such as playbooks, roles, inventory, and variables, to make it easier to navigate and maintain. Ansible official best practices page says that the structure should look like this:
![enter image description here](https://i.imgur.com/hx7RnJU.png)
 - **Use roles to organize and reuse your Ansible code.** Roles provide a modular approach to defining tasks, handlers, variables, and templates.
 - **Maintain separate inventory files and variable files.** This separation helps to keep the inventory and variables clean and easily manageable.
 - **Protect sensitive information** like passwords, API keys, and certificates using Ansible Vault.
 - **Design your playbooks so they can be executed multiple times** without causing unintended changes.
 - **Include error handling and recovery mechanisms** in your playbooks. Utilize appropriate Ansible error handling modules like `failed_when`and `ignore_errors`
 - **Use existing roles from Ansible Galaxy whenever possible** to avoid reinventing the wheel.
 - **Develop a testing strategy for your Ansible playbooks.** Use Ansible's built-in testing framework, such as `ansible-test`, to validate your playbooks against different scenarios and environments.
 - **Maintain clear and comprehensive documentation for your playbooks**, including their purpose, usage instructions, variable definitions, and any specific requirements.
 - It is suggested that you define groups based on purpose of the **host** (roles) and also **geography** or datacenter location (if applicable)
 - **Using the "state" parameter.** The `state` parameter is optional to a lot of modules. Whether `state=present` or `state=absent`, it’s always best to leave that parameter in your playbooks to make it clear.
 - Use official documentation. You can find it here: https://docs.ansible.com

## Docker
![Docker IMG](https://francofernando.com/assets/img/blog/frameworks/docker/docker.png)

 - Whenever possible, **use official Docker images from trusted sources** like Docker Hub or official repositories (And if you don't, use your own images).
 - Try to **keep your Docker images as small as possible**. Remove unnecessary files, dependencies, and temporary build artifacts to reduce image size.
 - Create a `.dockerignore` file in your project directory to **exclude unnecessary files and directories**.
 - **Follow the principle of "one process per container."** Each container should have a single responsibility or process. This promotes modularity, simplicity, and easier troubleshooting.
 - **Use container orchestration platforms** like *Docker Swarm or Kubernetes* to manage and scale your containerized applications.
 - **Keep your Docker images secure** by regularly updating them with the latest security patches. Here you can use *Docker Security Scanning* to scan you image.
 - **Follow Dockerfile best practices:**
	-   Use a minimal base image.
	-   Leverage caching effectively by ordering your commands intelligently.
	-   Combine related commands using a single `RUN` statement to reduce the number of image layers.
	-   Avoid installing unnecessary packages or tools.
	-   Clean up temporary files and dependencies after each step.
	-   Use explicit version tags for base images and dependencies.
 - **Store persistent data outside of containers** by using *Docker volumes or bind mounts.*
 - **Include only the necessary dependencies** in your container.
 - **Implement monitoring and logging** solutions for your Docker containers.
 - Use official documentation and user shared images:
	 - Documentation (Docker Docs): https://docs.docker.com
	 - Docker Hub: https://hub.docker.com
 ## Kubernetes
 ![enter image description here](https://codefresh.io/wp-content/uploads/2017/02/Intro-to-Kubernetes-blog-b-2.png)
 
 - **Always use namespaces** to logically group and isolate resources.
 - **Set resource requests and limits for your containers.** Resource requests ensure that Kubernetes schedules containers appropriately, while limits prevent containers from monopolizing resources.
 - Use **Deployments** for stateless applications and **StatefulSets** for stateful applications.
 - Use **ConfigMaps** to store configuration data and **Secrets** to manage sensitive information such as credentials, API keys, or certificates. 
 - **Avoid hardcoding configuration values and sensitive data.**
 - **Apply labels** to your resources and **use selectors** to group and query them.
 - **Define readiness and liveness** probes for your containers.
 - **Implement Horizontal Pod Autoscaling** to automatically scale the number of replicas based on CPU or custom metrics.
 - **Use RBAC** to define access controls and permissions.
 - **Implement monitoring and observability solutions** to gain insights into your Kubernetes cluster.
	 - Here, you can use tools like Prometheus and Grafana (i'll give best practices for them later).
 - **Keep your Kubernetes cluster up to date** by regularly applying updates and patches.
 - **Follow the official documentation**, here's the link: https://kubernetes.io/docs/home/
## Helm
![Helm IMG](https://www.adictosaltrabajo.com/wp-content/uploads/2020/05/Captura-de-pantalla-2020-05-08-a-las-14.24.42.png)
 - **Organize your charts** using a logical directory structure. Split your templates, values, and helper files into separate directories for better maintainability. The directory structure should look like this:
![enter image description here](https://i.imgur.com/NIiTTyx.png)
 - **Use subcharts for reusable components.**
 - **Chart names must be lower case letters and numbers.** Words _may_ be separated with dashes (-).
 - **Specify dependencies** in your `requirements.yaml` file to ensure that all necessary components are installed.
 - **Use separate values files for different environments** (such as development, staging, and production) to manage configuration values.
 - **Make your charts configurable** by defining parameters in the `values.yaml` file.
 - **Use Helm's built-in linting feature** (`helm lint`) to check for syntax errors and best practices.
 - **Include comprehensive documentation in your charts.** You can do this using comments, separate files or external tools.
 - **Assign versions to your charts** and follow semantic versioning conventions.
 - **Use official documentation and user shared charts**:
	 - Documentation: https://helm.sh/docs/
	 - Artifact Hub: https://artifacthub.io

## Prometheus
![Prometheus IMG](https://www.cncf.io/wp-content/uploads/2020/08/prometheusBanner-1.png)

 - **Follow a consistent and descriptive naming convention** for metrics.
 - **Avoid instrumenting unnecessary or excessive metrics.**
 - **Use labels** to add better filtering in your metrics.
 - Monitor **infrastructure-level metrics** (CPU, memory, disk usage) and **application-specific metrics** (request latency, error rates, business-specific metrics).
 - **Avoid setting overly sensitive alerts** that can lead to alert fatigue.
 - **Use Grafana, a popular data visualization tool**, to create informative and visually appealing dashboards *(Grafana's best practices explained in the next section)*.
 - **Deploy Prometheus in a highly available way** to ensure resilience and reliability. For example, you can use replica sets, load balancing, and redundant storage.
 - **Monitor the health and performance** of your Prometheus servers using metrics exposed by Prometheus itself.
 - **Track failures and total requests**, not failures and successes.
 - You can find the official documentation here: https://prometheus.io/docs/introduction/overview/
## Grafana
![Grafana IMG](https://pandorafms.com/blog/wp-content/uploads/2019/02/que-es-grafana-1.png)
 - Before creating dashboards, **define the purpose, audience, and specific metrics** you want to display.
 - Give your dashboards, panels, and variables **descriptive names**.
 - **Minimize the number of queries executed per panel.**
 - **Utilize variables in your dashboards** to make them more dynamic and adaptable.
 - **Utilize Grafana's templating feature** to create reusable dashboard templates.
 - Establish and follow **consistent visual styles** across your dashboards.
 - **Use annotations**, since they provide contextual information within your dashboards.
 - **Set up Grafana's alerting feature** to monitor your metrics and trigger notifications when predefined conditions are met.
 - **Implement appropriate access controls and authentication mechanisms**.
 - **Regularly back up** your Grafana dashboards and their associated configuration files.
 - **Monitor the health and performance** of your Grafana instance itself.
 - **Use Grafana community's resources**, including official documentation, forums, and dashboards shared by other users. You can find them here:
	 - User dashboards: https://grafana.com/grafana/dashboards/
	 - Grafana documentation: https://grafana.com/docs/grafana/latest/
	 - Forums: https://community.grafana.com

## Terraform
![Terraform IMG](https://www.turbogeek.co.uk/wp-content/uploads/2018/11/hashicorp-terraform-banner.png)

 - **Use Terraform modules** to encapsulate reusable pieces of infrastructure configuration.
 - **Make your modules flexible by using variables and outputs.**
 - **Configure a backend to store Terraform state files remotely.** 
	 - Backends like *Amazon S3, Azure Blob Storage, or HashiCorp Terraform Cloud* provide secure storage and collaboration features.
 - **Always run** `terraform plan` before applying changes to your infrastructure.
 - **Integrate Terraform into your CI/CD pipeline.**
 - **Assign meaningful tags to your resources** for better organization, cost allocation, and resource management.
 - **Keep your Terraform provider versions up to date.**
 - Follow a good terraform structure(Environments are your terraform Deployments and all the modules in a separate folder). Your terraform folder should look like this:
![enter image description here](https://www.stenic.io/blog/images/terraform-project-structure.png)
 - You can look for the **terraform documentation** [here](https://developer.hashicorp.com/terraform/docs).
 

# Scripts
## Python
![Python IMG](https://michaelwashburnjr.com/hubfs/Imported_Blog_Media/python.jpg)

 - **Stick to the guidelines outlined in PEP 8** (Python Enhancement Proposal 8), which provides recommendations for code formatting, naming conventions, and code organization.
 - **Choose descriptive names** for variables, functions, classes, and modules.
 - Use `snake_case` or `CamelCase`.
 - **Include docstrings and comments** in your functions, classes, and modules to document their purpose.
 - **Break your code into modular and reusable functions or classes.**
 - **Use try-except blocks** to catch and handle exceptions.
 - Use **built-in language features and libraries** for optimal performance.
 - **Follow DRY** (Don't Repeat Yourself) Principle. You can get more info about this [here](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself).
 - **Use virtual environments** (e.g., virtualenv, venv) to create isolated environments for your Python projects.
 - You can find the **official python doc** here: https://docs.python.org/3/

## Shell
![Linux IMG](https://adminscriptbank.files.wordpress.com/2016/09/banner_linux.png)
 - **Start your script with a shebang line** (e.g., #!/bin/bash) to specify the shell interpreter to use.
 - **When referencing variables, double quote them** (e.g., "$variable").
 - **Escape special characters** (e.g., $, `, ") when required to avoid unexpected behavior.
 - **Use comments** to explain the purpose and logic of your code.
 - **Validate and sanitize user input** to ensure it meets the required criteria.
 - **Break down your script into smaller functions** to encapsulate reusable code.
 - **Break your script into multiple files** or modules to improve readability and maintainability.
 - You can find a good b**ash documentation** here: https://devdocs.io/bash/

## YAML
![YAML IMG](https://ucarecdn.com/58b00b7f-42ac-4a85-8e5b-b30dcb015a8e/-/crop/1024x380/0,306/-/preview/)
 - Use **two spaces for each level of indentation** (never use tabs).
 - **Use a consistent format for lists and dictionaries.** For lists, use a hyphen followed by a space ("- item") for each element. For dictionaries, use key-value pairs with a colon and a space ("key: value").
 - **Use the flow style** (using square brackets [ ] for lists and curly braces { } for dictionaries) for simple structures when possible.
 - **If a line becomes too long, break it** into multiple lines to enhance readability.
 - **Use anchors (&) and aliases (*) to reuse** and reference common data structures or values within your YAML file.
 - **Avoid excessive nesting of data structures.**

