Direct Connect: EFS uses direct connect with on-premesis
Macie: Discover & protect youre sensitive data at Scale
Cloudfront: 
Code Commit: Managed source control System
Route 53: DNS server, latency based routing, register DNS in Route 53. 
EBS: Elastic Block Store, data remains when EC2 is terminated
EBS Snapshots: is an incremental backup, Toenemend.  16Tibite, connect via 1 AZ 
EFS: Elastic File System: Linux File system, regional, auto scales, connect via: Regions
Hypervisor: run's EC2
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
AWS Trusted Advisor:PILLARS Cost optimization, Performance, security, Fault Tolerance, Service limits. 






