Subjects / parts of the exams:

Compute 

**third-party database**  (use EC2) 
Customer data comes in all shapes, sizes, and systems. 
The data that companies collect directly is first-party data. 
Other data comes from partners or is purchased, what we call second-party and third-party data.
Third-party data is collected by another entity that is entirely separate from your relationship with your audience

**automatic failover** failover is a backup computer taking over saving a file if the main computer suddenly breaks down.

**Data-pipeline**
AWS Data Pipeline is a web service that you can use to automate the movement and transformation of data.

**Amazon Lightsail**
- Amazon LightSail provides developers compute, storage, and networking capacity and capabilities to deploy and manage websites, web applications, and databases in the cloud.
- LightSail provides preconfigured virtual private servers (instances) that include everything required to deploy and application or create a database.
- Deploying a server on LightSail is extremely easy and does not require knowledge of how to configure VPCs, security groups, network ACLs etc.
- Managed MySQL database


**AWS Lambda**
- AWS Lambda is a serverless compute service that runs your code in response to events and automatically manages the underlying compute resources for you. 
- Lambda is a compute service that lets you run code without provisioning or managing servers. 
capacity provisioning and automatic scaling, code monitoring and logging.
- Lambda functions scale out rather than up running multiple invocations of the function in parallel

**The Scale-Out**
- Computing on AWS solution helps customers deploy and operate a multiuser environment for computationally intensive workflows, such as computer-aided engineering (CAE). 

**AWS CodeDeploy** 
AWS CodeDeploy is a fully managed deployment service that automates software deployments to a variety of compute services such as Amazon EC2, AWS Lambda, and your on-premises servers. 

**Deployment in general**
Software deployment refers to the process of making the application work on a target device, whether it be a test server, production environment or a user's computer or mobile device.

**Benefits EC2 provide over using non-cloud servers**
- Inexpensive
- Elastic webscale computing
- Trade fixed expense for variable expense 
- Benefit from massive economies of scale
- Stop guessing 
- Increase speed and agility
- Stop spending money running and maintaining data centers
- Go global in minutes
It provides you with complete control of your computing resources and lets you run on Amazon's proven computing environment.
- Amazon EC2 reduces the time required to obtain and boot new server instances to minutes, allowing you to quickly scale capacity, both up and down, as your computing requirements change.
Note:
- Amazon EC2 does NOT!!! provide any control of the hypervisor or underlying hardware infrastructure.

**snapshots**
- You can take snapshots of EC2 instances which creates a point-in-time copy of the instance. Snapshots are stored on S3
- If you make periodic snapshots of a volume, the snapshots are incremental, which means that only the blocks on the device that have changed after your last snapshot are saved in the new snapshot. (incremental = toenemend)

**Tagging resources**
- Tagging your AWS resources lets you assign custom metadata to instances, images, and other resources. 
- AWS Cost Explorer and detailed billing reports support the ability to break down AWS costs by tag.
- AWS allows customers to assign metadata to their AWS resources in the form of tags. Each tag is a simple label consisting of a customer-defined key and an optional value that can make it easier to manage, search for, and filter resources.
- For example, you can categorize resources by owner, purpose, or environment, which helps you organize them and assign cost accountability.
- A resource is an entity that you can work with.
- An entity is a single object extracted from the source data.
- Extraction: Data is taken from one or more sources or systems. (web pages, emails, text documents, PDFs, scanned text, mainframe reports, or spool files)

**Bootstrapping**
- the execution of automated actions to services such as EC2 and RDS. This is typically in the form of scripts that run when the instances are launched.
- In computing, a bootstrap loader is the first piece of code that runs when a machine starts, and is responsible for loading the rest of the operating system.

**Userdata** "bootstrap" 
- eerste stukje code userdata om bijvoorbeeld je webserver op te starten. User is de gebruiker van EC2 niet perse een persoon/account/employee. 

**Containerization**
Containers are packaged software that runs in a Docker image. Services such as Amazon ECS and Fargate can run Docker containers.

**DOCKER** 
- Docker container: A Docker container is an instantiated (running) Docker image.
- Docker image: a read-only template that contains a set of instructions for creating a container that can run on the Docker platform.
- The Amazon Linux container image is built from the same software components that are included in the Amazon Linux AMI.
- Amazon Linux 2 AMI run's Docker Images

**ECR** 
- Amazon Elastic Container Registry (ECR), an image registry for storing and quickly retrieving Docker images.
- Amazon Elastic Container Registry (ECR) is a fully-managed Docker container registry that makes it easy for developers to store, manage, and deploy Docker container images.


**ECS**
- Amazon Elastic Container Service (ECS) is a highly scalable, high performance container management 
- service that supports Docker containers and allows you to easily run applications on a managed cluster of Amazon EC2 instances.


**Multiple applications running on EC2** 
- If you have multiple EC2 instances that are part of an application, you should deploy them into separate availability zones (AZs).
- Each AZ has redundant power and is also fed from a different grid.
- AZs also have low-latency network links which is often advantageous for most applications
- Regions ---> AZ  avai.zone
- only 1 VPC needed
- Grid is "rooster" schedule
- redundant power is "overloedig" 

**elastic web-scale**  (is in EC2)
Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers.

**auto scaling EC2**
- Auto Scaling automates the process of adding (scaling up) OR removing (scaling down) EC2 instances based on the traffic demand for your application.
- Amazon EC2 Auto Scaling is configured within the EC2 console and can launch instances within a VPC across multiple AZs.

**Reserved Instance RI**
Reserved Instances (RI) provide a significant discount (up to 72%) compared to On-Demand pricing and provide a capacity reservation when used in a specific Availability Zone
- “Reserve capacity” is also a correct answer.
- “Reduced cost"
- significant discounts for fixed term contracts?

- Scheduled RI: These are available to launch within the time windows you reserve.
- Convertible RI: These provide a discount (up to 54% off On-Demand) and the capability to change the attributes of the RI as long as the exchange results in the creation of Reserved Instances of equal or greater value.
- Standard RIs: These provide the most significant discount (up to 75% off On-Demand) and are best suited for steady-state usage 

**Resource group**
Resource Group AWS
A resource group is a collection of AWS resources in the same AWS Region that match tag-based criteria provided in a search query. 
- A resource group is a collection of resources that share one or more tags or portions of tags. 
- To create a resource group, you simply identify the tags that contain the items that members of the group should have in common.
- Resource Groups and a Tag Editor. Resource Groups allow you to easily create, maintain, and view a collection of resources that share common tags.
- Regions and resources can be combined onto a TAG'

**Reserved Instances** 
Pricing options 
- discount (up to 75%) compared to On-Demand pricing 
- All upfront
- Partial upfront
- No upfront
Dit betreft reserved RI !!!!

**scheduled RI**
With RIs, you can choose the type that best fits your applications needs.
- Standard RIs: These provide the most significant discount (up to 75% off On-Demand) and are best suited for steady-state usage.
- Convertible RIs:
 These provide a discount (up to 54% off On-Demand) Convertible RIs are best suited for steady-state usage.
- Scheduled RIs: 
These are available to launch within the time windows you reserve. This option allows you to match your capacity reservation to a predictable recurring schedule that only requires a fraction of a day, a week, or a month.

**Elastic Beanstalk**
- AWS Elastic Beanstalk can be used to quickly deploy and manage applications in the AWS Cloud. 
- Developers upload applications and Elastic Beanstalk handles the deployment details of:
capacity provisioning, load balancing, auto-scaling, and application health monitoring. 
Considered a Platform as a Service (PaaS) solution. Supports Java, .NET, PHP, Node.js, Python, Ruby, Go, and Docker web applications.

**Lambda**
- AWS Lambda lets you run code as functions without provisioning or managing servers. 
- With serverless computing, your application still runs on servers, but all the server management is done by AWS.
- Lambda-based applications (also referred to as serverless applications) are composed of functions triggered by events.

**Amazon Cognito**
- Amazon Cognito lets you add user sign-up, sign-in, and access control to your web and mobile apps quickly and easily.

**Amazon Linux 2 AMI**
Is billed per second, with a minimum of 60 seconds.

**auto scaling ec2**
- Amazon EC2 Auto Scaling launches and terminates instances as demand changes
- This helps with resiliency and high availability as it can also be set to ensure a minimum number of instances are always available.
- Stop guessing about capacity

**Spot Instances**
- In your launch template, you can optionally request Spot Instances with no end date or duration. 
- Amazon EC2 Spot Instances are spare capacity available at steep discounts compared to the EC2 On-Demand price. 

**On Demand** 
- With On-Demand instances you pay for hours used with no commitment. 
- There are no upfront costs so you have maximum flexibility.

**Instance store volumes**
- Instance-store is over 5x faster than EBS-SSD for uncached reads


**EBS**
- EBS-backed means the root volume is an EBS volume and storage is persistent. (aanhoudend)
- Instance store-backed means the root volume is an instance store volume and storage is not persistent. - Both EBS and Instance store volumes are block-based storage devices.

**app-facing services**
- AWS Lambda and Amazon API Gateway are both app-facing components of the AWS Serverless infrastructure

**Elastic Beanstalk** 
- Can be used to quickly deploy and manage applications in the AWS Cloud.
- Developers upload applications and Elastic Beanstalk handles the deployment details of capacity       provisioning, load balancing, auto-scaling, and application health monitoring.

**Amazon CloudWatch**
Logs to monitor, store, and access your log files from Amazon Elastic Compute Cloud (Amazon EC2) instances, AWS CloudTrail, Route 53, and other sources

Relational Database
- A relational database, or relational database management system (RDMS), stores information in tables. Often, these tables have shared information between them, causing a relationship to form between tables. This is where a relational database gets its name from.
- Zoeken op bijv: trackname, artist, color, size is relational database. 

Non-relational
Enceclopedy, zoeken op 1 woord is sneller! 

Type databases: 
talen: SQL
Engine: MariaDB, Microsoft SQLserver, Mysql, Oracle, PostgreSQL 

Data-wharehouse questions: Redshift

SUpport Plans goed bestuderen 
what is the minimal level that gives you 24/7 support
Answer: Basic   ;)   strikvraag

All movements of users are saved in: cloudtrail
Serverless Containers: Fargate

vraag 38




**Macie Machine Learning** 
AI that analyses your S3 for sensitive data (personal information, credit card numbers etc)
**GuardDuty** 
Intelligent treath detection service. It can detect account compromise, instance compromise, and malicious activity


