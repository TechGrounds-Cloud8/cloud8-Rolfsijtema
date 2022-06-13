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

**AWS Lambda**
AWS Lambda is a serverless compute service that runs your code in response to events and automatically manages the underlying compute resources for you. Lambda is a compute service that lets you run code without provisioning or managing servers. 
capacity provisioning and automatic scaling, code monitoring and logging.

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

**Containerization**
Containers are packaged software that runs in a Docker image. Services such as Amazon ECS and Fargate can run Docker containers.

**DOCKER** 
- Docker container: A Docker container is an instantiated (running) Docker image.
- Docker image: a read-only template that contains a set of instructions for creating a container that can run on the Docker platform.
- The Amazon Linux container image is built from the same software components that are included in the Amazon Linux AMI.
- Amazon Linux 2 AMI run's Docker Images

**ECR** Amazon Elastic Container Registry (ECR), an image registry for storing and quickly retrieving Docker images.

















**Macie Machine Learning** 
AI that analyses your S3 for sensitive data (personal information, credit card numbers etc)
**GuardDuty** 
Intelligent treath detection service. It can detect account compromise, instance compromise, and malicious activity


