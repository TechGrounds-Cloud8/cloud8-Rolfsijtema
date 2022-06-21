Direct Connect: EFS uses direct connect with on-premesis
Macie: Discover & protect youre sensitive data at Scale
Cloudfront:  web service that speeds up distribution of your static and dynamic web content, such as . html, . css, . js, and image files, to your users.
Code Commit: Managed source control System
Route 53: DNS server, latency based routing, register DNS in Route 53. 
EBS: Elastic Block Store, data remains when EC2 is terminated
EBS Snapshots: is an incremental backup, Toenemend.  16Tibite, connect via 1 AZ 
EFS: Elastic File System: Linux File system, regional, auto scales, connect via: Regions
Hypervisor: part that make everything virtual, runs ECS or appl
S3: Amazon Simple Storage Service  1bucket= 5TB max  99.99999999% durability
Lifecycle Policies: moves data automaticly to deeper storage classes when used less...
Object Keys: are unique identifiers of the data placed in the s3 buckets
RDS:infrastructure: run data in the cloud. failover, auto-patching Redundancy, backups. 
is available on six database engines, which optimize for memory, performance, or input/output (I/O). Supported database engines include:
Aurora, PostgreSQL, MySQL, MariaDB, Oracle Database,Microsoft SQL Server
Aurora: is enterprise-class relational database DATAbase Engine!!!  It is up to five times faster than standard MySQL,three times faster than standard PostgreSQL  1/10 of the price of commercial databases, data replication, 15 read replica. continiue's backups to S3
Relational data: "sql" Single items have: productname, size, price,...
Non-relational: simple flexibal schema, 
Dynamo DB: SERVERLESS! non relational database, NoSql, NOT for complex data,create tables, Purpose build, milliseconds, fully managed, highly scalable.
Is a key-value database, you can add or remove attributes from items in the table at any time. Additionally, not every item in the table has to have the same attributes. 
Redshift: data wharehousing as a service, 10x faster in big data, single API call. helps you to understand relationships and trends across your data.
DMS:  Database Migration Service, source database stays functional during migration, source & target database dont have to be from the same type. 
Schema diversion tool!  devops test datab/migration. consolidation.
MongoDB: Document DB for catalogs, content. 
Neptune: Graph Database, social networking,  fraud detection
Blockchain: 
QL-DB: Supply Chain, banking financial records. entry' can never be deleted. 
ElastiCache: service that adds caching layers on top of your databases to help improve the read times of common requests. It supports:  Redis and Memcached.
DAX: is an in-memory cache for DynamoDB. 
It helps improve response times from single-digit milliseconds to microseconds.
Shared Responsibility: Customers IN the cloud, Amazon OF the cloud. ;)
Customer: Security: Customer Data, platform, applications, ID/acces management, OS networking/firewall.
AWS: Security of the cloud, Hypervisor, network, physical parts, storage, compute, regions, AZ, edge Loc. database. 
MFA: multi factor IDentifycation
IAM Idenity Acces Managemend, ROOT-user can acces all" IAM: default no acces at all! all users need to be adjusted to accesses,  "least priveledges principle"  works with Policies. You can make Policy's for group users. CREATE ID to Roles: temp acces to appl.  so todat you make coffee, tomorrow you do cash registry, each day is diffirent role with it's diffirent permissions. 
An IAM policy:  is a document that allows or denies permissions to AWS services and resources.
AWS Orginizations:creates a ROOT from where you do:  Centralized managemend of multiple accounts, consolidated billing/bulk discounts, grouping accounts, service & API actions acces control. 
SCP: Service Control Policies.
Organizational units: group accounts into organizational units (OU's)make it easier to manage accounts with similar business or security requirements. When you apply a policy to an OU, all the accounts in the OU automatically inherit the permissions specified in the policy.  
Artifact: a service that provides on-demand access to AWS security and compliance reports and select online agreements.  AWS Artifact Agreements and AWS Artifact Reports.
Health Insurance Portability and Accountability Act (HIPAA).
Customer Compliance Center: contains resources to help you learn more about AWS compliance. An auditing security checklist, An overview of AWS risk and compliance, AWS answers to key compliance questions.
DDoS: DA denial-of-service (DoS) attack is a deliberate attempt to make a website or application unavailable to users. SlOWLORIS ATTACK, HTTP-ATTACK, UPD-FLOOD.

Security Groups: help to prevent DDoS. by selective traffic settings
Elastic Load Balancers also help, they handle traffic
WAF: Web Application Firewall, lets you monitor network requests that come into your web applications. 

AWS Shield Standard: auto protect without any costs. 
AWS Shield Advanced; level of protection, is a paid service that provides detailed attack diagnostics and the ability to detect and mitigate sophisticated DDoS attacks. 

AWS KMS: Key Management Service: You can use AWS KMS to create, manage, and use cryptographic keys. You can also control the use of keys across a wide range of services and in your applications.

Amazon Inspector: Amazon Inspector is an automated vulnerability management service that continually scans AWS workloads for software vulnerabilities and unintended network exposure.

Amazon GuardDuty: is a service that provides intelligent threat detection for your AWS infrastructure and resources. It identifies threats by continuously monitoring the network activity and account behavior within your AWS environment.

Cloudwatch: is a web service that enables you to monitor and manage various metrics and configure alarm actions based on data from those metrics. 
CloudWatch alarms: perform actions if the value of your metric has gone above or below a predefined threshold. Get a note when alarms triggered

The CloudWatch dashboard: single location that can show all metrics of all ur applications. 

Cloudtrail: records API calls for your account. The recorded information includes the identity of the API caller, the time of the API call, the source IP address of the API caller, and more. Events are typically updated in CloudTrail within 15 minutes after an API call.
CloudTrail Insights: helps AWS users identify and respond to unusual activity associated with write API calls by continuously analyzing CloudTrail management events.

AWS Trusted Advisor: is a web service that inspects your AWS environment and provides real-time recommendations in accordance with AWS best practices.5-PILLARS Cost optimization, Performance, security, Fault Tolerance, Service limits. 
Lambda: 
App-facing: Lambda & API gateway
Free Tier: Always free or 12months free, trails  (s3 is free for 12months max 5gb)
The AWS Pricing: Calculator lets you explore AWS services and create an estimate for the cost of your use cases on AWS. You can organize your AWS estimates by groups that you define. A group can reflect how your company is organized, such as providing estimates by cost center.When you have created an estimate, you can save it and generate a link to share it with others.
Billing & cost management Dashboard: to pay your AWS bill, monitor your usage, and analyze and control your costs.
Cost & Usage reports: via the dashboard you can make reports
Consolidated billing: this feature of AWS Organizations enables you to receive a single bill for all AWS accounts in your organization, it's a free service. By consolidating, you can easily track the combined costs of all the linked accounts in your organization. The default maximum number of accounts allowed for an organization is 4, but you can contact AWS Support to increase your quota, if needed.On your monthly bill, you can review itemized charges incurred by each account. still one bill but detailed by each account. share bulk discount pricing, Savings Plans, and Reserved Instances.
AWS Budgets: you can create budgets to plan your service usage, service costs, and instance reservations, also get a notification when budget is passed. By email. 
AWS Cost explorer: is a tool that enables you to visualize, understand, and manage your AWS costs and usage over time. Make reports and save them, You can apply custom filters and groups to analyze your data, up untill the hourly level. 
BASIC SUpport: 24/7 customer service, Doc. whitepapers, AWS health-dashboard
Developer Support: basic supp. + emailsupport. Best practice guidance, Client-side diagnostic tools

Business support: basic+developer supp. + phone, infra event management. All AWS Trusted Advisor checks,Limited support for third-party software, such as common operating systems and application stack components, All AWS Trusted Advisor checks. all AWS Trusted Advisor checks!!!

Enterprices level: basic+dev+business + 15min SLA + TAM technical Account Manager. Application architecture guidance,Infrastructure event management,

S3: HTTP code 
200: Succesfull uploads
300: re-direction
400: Client error
500: server Error. 

TAM: specialized/monitoring technical account managers.  

The Well-Architected framework has pillars and these pillars are Operational 

- Excellence
- Security
- Reliability
- Performance Efficiency
- Cost Optimization

AWS Marketplace: is a curated digital catalog that makes it easy for customers to find, buy, deploy, and manage third-party software and services that customers need to build solutions and run their businesses
AWS CAF: Cloud Adoption Framework: Looking at what is needed to Migrate there is made a CAF-Action-Plan that helps to guide your orginization for the cloud. 
6-Core perspectives: Business, People, Governance, Platform, Security, Operations.
Re-hosting: lift-and-shift: can save up to 30% on costs. involves moving applications without changes
Re-platforming: lift, tinker, and shift,involves making a few cloud optimizations to realize a tangible benefit.
Re-factoring/re-architecting: involves reimagining how an application is architected and developed by using cloud-native features.
Re-purchasing: involves moving from a traditional license to a software-as-a-service model 
Re-taining: consists of keeping applications that are critical for the business in the source environment. 
Re-tiring: is the process of removing applications that are no longer needed.
Snow-Family: is a collection of physical devices that help to physically transport data up to: exabytes into the cloud. 
AWS SnowCone: is a small, rugged, and secure edge computing and data transfer device. It got 2 CPUs, 4 GB of memory, and 8 TB of usable storage.
AWS Snowball-Edge: Storage: 80 TB of hard disk drive (HDD) capacity for block volumes and Amazon S3 compatible object storage, and 1 TB of SATA solid state drive (SSD) for block volumes. Compute: 40 vCPUs, and 80 GiB of memory to support Amazon EC2 sbe1 instances (equivalent to C5).
AWS: Snow-Mobile: is an exabyte-scale data transfer service used to move large amounts of data to AWS.You can transfer up to 100 petabytes of data per Snowmobile, a 45-foot long ruggedized shipping container, pulled by a semi trailer truck.
VMware Cloud: lift ur own VMware directly onto AWS via VMware-cloud
Amazon Sage-Maker: build, deploy, machine learning at scale, custom models. 
Amazon A2I: Augumented EI. 
Amazon LEX: the heart of Alexa, interactive chatbots (ready to go)
Amazon Textract: Extracting text and data from documents. 
AWS Deepracer: Experiment with machinelearning. Internet of things
AWS Groundstation: have your own satellite? Ground Station and only pay for the satellite time you actually need?
AWS Training and Certification offers training classes on many of these technologies already, and every month, AWS seems to release something even better for us to talk about. Innovate with AWS Services

When examining how to use AWS services, it is important to focus on the desired outcomes. You are properly equipped to drive innovation in the cloud if you can clearly articulate the following conditions: 

The current state
The desired state
The problems you are trying to solve

Consider some of the paths you might explore in the future as you continue on your cloud journey. 

Advantages of cloud computing

- Trade upfront expense for variable expense.
Upfront expenses include data centers, physical servers, and other resources that you would need to invest in before using computing resources. 

- Benefit from massive economies of scale.
By using cloud computing, you can achieve a lower variable cost than you can get on your own. Because usage from hundreds of thousands of customers aggregates in the cloud, providers such as AWS can achieve higher economies of scale. Economies of scale translate into lower pay-as-you-go prices.

- Stop guessing capacity.
With cloud computing, you don’t have to predict how much infrastructure capacity you will need before deploying an application

- Increase speed and agility.
The flexibility of cloud computing makes it easier for you to develop and deploy applications.

- Stop spending money running and maintaining data centers.
Cloud computing in data centers often requires you to spend more money and time managing infrastructure and servers

- Go global in minutes.
The AWS Cloud global footprint enables you to quickly deploy applications to customers around the world, while providing them with low latency

Dedecated Host: An Amazon EC2 Dedicated Host is a physical server fully dedicated for your use.flexibility and cost effectiveness of using your own licenses.

**DIGITAL CLOUD**

AWS Config: 
IAM: is global!
Cost Management: show the overall cost of EC2 
Budgets: setup budgets and get notes when exeded
Billing preferences: compare departments
Look at cost per application, number of requests, read data
VPC: virtual private cloud,  in a VPC deploy ur resources
Elasticy: system is ready to receive lots of sudden data. 
Legacy IT, is the old model of IT compare to AWS/cloud computing
Elastisearch: Elasticsearch is a distributed search and analytics engine built on Apache Lucene.
Private cloud: VMware Microsoft, RedHat, openstack
Public cloud: AWS, Azure, google cloud
Hybrid cloud: combination of on premises and privatecloud. 
Multicloud: 2 or more public clouds at the same time. 
IaaS: Install ur application on it, heaving a room in a hotel. 
Paas: all you manage is the data and codes  Elastic Beanstalk
SaaS: software as service: all you need to do is create an account, and use the software as a service. 
In a private model you have to manage everything urself. 
Scaling out: vertical: more Virtual Machines
Scaling UP: same EC2 but more CPU more memory, faster VMachines
Database Scaling out: spread the Dataload
fault tolerance: built in redundancy, more CPU's more HD's make sure everything keeps on running
EC2: OS of EC2 are AMI machine images (you can choose serveral services)
EBS is storage on the EC2 (elastic block storage)
Storage types: 
Block storage: (EBS) virtual HD in the cloud, internal or network attached. 
File storage: (corporate dir) Mount filesystem to ur OS using networkshare 
Object storage: container, massive scalable, low cost, uses REST API, reacts on Codes. ideal for automating 
DynamoDB: non relational DB, very fast
SQL, mySQL, postSQL, Graph Database sees realations between databases. 
RDS can carry, manage, patch, update OS, resize a database but also replicate a database to diffirent AZ's helps with disaster discovery.
Serverless Lambda: upload code to lambda and run it. No server to manage, pay only when code runs, scales automatically. can be low cost. 
Redshift: data wharehouse, ideal for analytics
EMR elastic Map Reduce, Rekognition of details, celebs, smile, mountinbike. 
High available due to AUto Scaling,  when instance failes it creates automatically new instances. Cloudwatch helps monitoring this. 
Benefits: scale on actual load, auto recovery when EC2 fail's. auto direct users to healty EC2's. 
Automation: efficientie: 
Elastic beanstalk: developers can upload a code that includes everything from building EC2, startup nodeJS, It has presets for example: high availability, that will auto include Autoscale and ELBalancing.  PaaS. 
Cloudformation: make template files with codes of a infrastructures, build as a code. Easy to copy ur setup to another region. 

6 Advantages of Cloud Computing:
1 Trade capital Expense for Variable expense capex - opex
2 Benefit from massive economy's of scale
3 Stop guessing capacity (utilization,ongebruikt)
4 Increase speed and Agility (agile is speed to react to change)
5 Stop spending money on maintaining datacenter, put money in devops
6 Go Global in minutes, 24regions, deploy code straith away. 

Usecases
Cloud Bursting: burst temp, into a cloud
Cloud backup/archive
Streaming Data & analytics, easy to setup services to collect and analize data. 
Serverless workflows are easy to build and run as Lambda Functions
Audio and video streaming: Data from S3 buckets cache data to edge locations 

