# [ThECS, AWS Support Plans, Trusted Advisor]

Learn about the Support plans and there diffirences, What is Elastic Container Service, Trusted Advisory, AWS config and Cloud Trail. 

## Exercise study: 

**ECS**
Amazon Elastic Container Service:
Run highly secure, reliable, and scalable containers

-  Launch thousands of containers across the cloud using your preferred continuous integration and delivery (CI/CD) and automation tools.
- Optimize your time with AWS Fargate serverless compute for containers, which eliminates the need to configure and manage control plane, nodes, and instances.
- Save up to 50 percent on compute costs with autonomous provisioning, auto-scaling, and pay-as-you-go pricing.
- Integrate seamlessly with AWS management and governance solutions, standardized for
compliance with virtually every regulatory agency around the globe.

Deploy in a hybrid environment:
- Build container-based applications on-premises or in the cloud with Amazon ECS Anywhere and enjoy consistent tooling, management, workload scheduling, and monitoring across environments.

Support batch processing: 
- Plan, schedule, and execute batch computing workloads across the full range of AWS services, including Amazon Elastic Compute Cloud (EC2), Fargate, and Amazon EC2 Spot Instances.

Scale web applications:
- Automatically scale and run web applications in multiple Availability Zones with the performance, scale, reliability, and availability of AWS.

![ECS](../00_includes/ECS.png)

**AWS Support Plans**

Why a support plan? 
- Move faster with AWS
- Automate management of your environment
- Focus on what matters
- Manage and mitigate risks
- Highly-trained engineers, large network of subject-matter experts
- Engineers empowered to help you achieve your goals

Types of Support: 

**Developer Support**

We recommend AWS Developer Support if you are testing or doing early development on AWS and want the ability to get technical support during business hours as well as general architectural guidance as you build and test.

Includes: 

- Enhanced technical support
Business hours email access to Cloud Support engineers. You can have one primary contact that can open an unlimited amount of cases. Response times for general guidance is less than 24 business hours* and system impaired is less than 12 business hours*.

- Architectural support
General guidance on how to use AWS products, features, and services together. AWS Solutions Architects leverage the AWS Well-Architected framework when providing recommendations.

- Customer service and communities
24x7 access to customer service, documentation, whitepapers, and support forums.


**Business support**

We recommend AWS Business Support if you are running production workloads on AWS and want 24x7 access to technical support from engineers, access to Health API, and contextual architectural guidance for your use-cases.

Includes: 
- Enhanced technical support
24x7 access to Cloud Support Engineers via phone, chat, and email. You can have an unlimited number of contacts that can open an unlimited amount of cases. Response times for general guidance is less than 24 hours, system impaired is less than 12 hours, production system impaired is less than 4 hours, and production system down is less than an hour.

- Third-party software support
Guidance, configuration, and troubleshooting of AWS interoperability with many common operating systems, platforms, and application stack components.

- Customer service and communities
24x7 access to customer service, documentation, whitepapers, and support forums.


**Enterprise On-Ramp**

We recommend Enterprise On-Ramp if you have production/business critical workloads in AWS and want 24x7 access to technical support from engineers, access to Health API, consultative architectural guidance, and a pool of Technical Account Managers (TAMs) to coordinate access to AWS subject matter experts.

Includes:
- Enhanced technical support
24x7 access to Cloud Support Engineers via phone, chat, and email. You can have an unlimited number of contacts that can open an unlimited amount of cases. Response times for general guidance is less than 24 hours, system impaired is less than 12 hours, production system impaired is less than 4 hours, production system down is less than an hour, and business critical system down is less than 30 minutes

- Billing and account management
AWS billing and account experts specialize in working with enterprise accounts. They will quickly and efficiently assist you with your billing and account inquiries, and work with you to implement billing and account best practices so that you can focus on what matters: running your business.

- Third-party software support
Guidance, configuration, and troubleshooting of AWS interoperability with many common operating systems, platforms, and application stack components.

- A pool of Technical Account Managers
A pool of Technical Account Managers helps you onboard, provides advocacy and guidance to help plan and build solutions using best practices, coordinates access to subject matter experts, assists with case management, and presents insights and recommendations on your AWS spend, workload optimization, and event management, which proactively keeps your AWS environment healthy.

- Access to subject matter experts
Cloud Support Engineers, Solutions Architects, and product teams are available to provide guidance and help as needed. The AWS Trust & Safety team assists you when your AWS resources are used to engage in abusive behaviors, such as spam, port scanning, denial-of-service (DoS) attacks, or malware


**Enterprice**
We recommend Enterprise Support for 24x7 technical support from high-quality engineers, tools and technology to automatically manage health of your environment, consultative architectural guidance, and a designated Technical Account Manager (TAM) to coordinate access to proactive / preventative programs and AWS subject matter experts.

- Enhanced technical support
24x7 access to Cloud Support Engineers via phone, chat, and email. You can have an unlimited number of contacts that can open an unlimited amount of cases. Response times for general guidance is less than 24 hours, system impaired is less than 12 hours, production system impaired is less than 4 hours, production system down is less than an hour, and business critical system down is less than 15 minutes.

- Billing and account management
AWS billing and account experts specialize in working with enterprise accounts. They will quickly and efficiently assist you with your billing and account inquiries, and work with you to implement billing and account best practices so that you can focus on what matters: running your business.

- Third-party software support
Guidance, configuration, and troubleshooting of AWS interoperability with many common operating systems, platforms, and application stack components.

- Technical account management
Designated point of contact
A Technical Account Manager (TAM) is your designated technical point of contact who helps you onboard, provides advocacy and guidance to help plan and build solutions using best practices, coordinates access to subject matter experts, assists with case management, presents insights and recommendations on your AWS spend, workload optimization, and event management, and proactively keeps your AWS environment healthy.

- Access to subject matter experts
Cloud Support Engineers, Solutions Architects, Technical Account Managers, and product teams are available to provide guidance and help as needed. The AWS Trust & Safety team assists you when your AWS resources are used to engage in abusive behaviors, such as spam, port scanning, denial-of-service (DoS) attacks, or malware.

[importantsheet](https://aws.amazon.com/premiumsupport/plans/)

**Trusted Advisor**

AWS Trusted Advisor provides recommendations that help you follow AWS best practices.

 Trusted Advisor evaluates your account by using checks. These checks identify ways to optimize your AWS infrastructure, improve security and performance, reduce costs, and monitor service quotas. You can then follow the check recommendations to optimize your services and resources.

It depends on the Support-type you choose what options are included.

- AWS Basic Support and AWS Developer Support customers can access core security checks and all checks for service quotas.

- AWS Business Support and AWS Enterprise Support customers can access all checks, including cost optimization, security, fault tolerance, performance, and service quotas. For a complete list of checks and descriptions, see the Trusted Advisor Best Practices.

![trustedadvisor](../00_includes/Trusted%20Advisor.png)

- Cost optimization
Trusted Advisor can help you save cost with actionable recommendations by analyzing usage, configuration and spend. Examples include identifying idle RDS DB instances, underutilized EBS volumes, unassociated Elastic IP addresses, and excessive timeouts in Lambda functions.

- Performance
Trusted Advisor can help improve the performance of your services with actionable recommendations by analyzing usage and configuration. Examples include analyzing EBS throughput and latency, compute usage of EC2 instances, and configurations on CloudFront.

- Security
Trusted Advisor can help improve the security of your AWS environment by suggesting foundational security best practices curated by security experts. Examples include identifying RDS security group access risk, exposed access keys, and unnecessary S3 bucket permissions.

- Fault tolerance
Trusted Advisor can help improve the reliability of your services. Examples include examining Auto scaling EC2 groups, deleted health checks on Route 53, disabled Availability Zones, and disabled RDS backups.

- Service quotas/limits
Service quotas are the maximum number of resources that you can create in an AWS account.  AWS implements quotas to provide highly available and reliable service to all customers, and protects you from unintentional spend. Trusted Advisor will notify you once you reach more than 80% of a service quota. You can then follow recommendations to delete resources or request a quota increase.

**AWS Config**


**AWS Cloud Trail**

### Sources

[ECS](https://aws.amazon.com/ecs/)

[supportplans](https://aws.amazon.com/premiumsupport/)

[trustedAdvisor](https://aws.amazon.com/premiumsupport/technology/trusted-advisor/)

### Overcome challanges
[Give a short description of your challanges you encountered, and how you solved them.]

### Results
[Describe here the result of the exercise. An image can speak more than a thousand words, include one when this wisdom applies.]
