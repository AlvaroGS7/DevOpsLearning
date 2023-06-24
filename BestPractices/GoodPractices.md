## DevOps Best Practices
**This is just a best practice compilation made by Álvaro González. Some of the most important ones could be missing but I've tried to have most of them.
![enter image description here](https://w7.pngwing.com/pngs/401/951/png-transparent-devops-software-developer-agile-software-development-software-testing-puppet-icon-devops-logo-text-logo-engineering.png)

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

## Azure Cloud
![enter image description here](https://www.evozon.com/wp-content/uploads/2017/05/Azure-Banner.png)
 - Your code should create **all the items within a resource.**
 - The goal of your code should be that you can **compile and run without any prerequisites**.
 - **CI/CD**
	 - Set up CI pipelines to **automatically build and test** your code whenever changes are pushed to the repository.
	 - Implement CD pipelines to **automate the deployment process.**
 - Store **build artifacts**, such as compiled binaries or deployment packages, in a centralized repository.
 - Use **separate environments** for development, testing (QA), staging, and production.
 - Ensure **consistent and reproducible infrastructure deployments.** You can do this using Azure Resource Manager templates, Az CLI or Az Poweshell.
 - Incorporate **security and compliance practices** into your pipeline.
 - Use **role-based access controls and secrets management** to protect sensitive information.
 - Implement **monitoring and logging solutions** to gain visibility into your applications and infrastructure. Here you can use Azure Monitor or Application Insights.
 - Regularly **review and improve** your pipelines and processes.


