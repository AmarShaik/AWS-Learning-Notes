# Amazon Web Services (AWS) – Introduction and Fundamentals

# 1. What Is AWS?

**AWS stands for Amazon Web Services.**

AWS is a cloud computing platform provided by Amazon. It offers computing resources and services over the internet so that individuals, developers, startups, and large organizations can build, deploy, manage, and scale applications without purchasing and maintaining all the physical infrastructure themselves.

In simple words:

> AWS allows you to use computing resources such as servers, storage, databases, networking, and AI services over the internet instead of managing all the physical hardware yourself.

AWS provides services for:

- Computing
- Storage
- Databases
- Networking
- Security
- Artificial Intelligence
- Machine Learning
- Analytics
- Application development
- Application deployment
- Monitoring
- Containers
- Serverless computing

### Simple Example

Suppose you want to build a website.

Normally, you might need:

- A physical server
- RAM and CPU
- Storage
- A database
- Networking equipment
- Security configuration
- Maintenance

But using AWS, you can use:

- **Amazon EC2** – To run your application on a virtual server.
- **Amazon S3** – To store files and images.
- **Amazon RDS** – To use a managed relational database.
- **Amazon VPC** – To create a logically isolated network.
- **AWS IAM** – To manage users and permissions.
- **Amazon CloudWatch** – To monitor your resources.

You can build and run your application using these services without purchasing your own physical data center infrastructure.

---

# 2. Who Owns AWS?

AWS is owned and operated by **Amazon**.

Amazon is the parent company, and Amazon Web Services is its cloud computing business.

### Simple Relationship

```text
Amazon
   |
   v
Amazon Web Services (AWS)
   |
   +-------------------+
   |         |         |
   v         v         v
  EC2       S3        RDS
   |         |         |
   v         v         v
Compute   Storage   Database
```

---

# 3. When Was AWS Started?

AWS was launched in **2006**.

It was introduced to provide computing infrastructure and technology services over the internet.

The idea was to allow organizations and developers to access computing resources without having to build and maintain their own large-scale physical infrastructure.

Over time, AWS expanded into many areas, including:

- Computing
- Storage
- Databases
- Networking
- Security
- Analytics
- AI and Machine Learning
- Serverless computing
- Containers
- Internet of Things

Today, AWS is one of the major cloud computing platforms used around the world.

---

# 4. Why Was AWS Created?

Imagine a company wants to launch an application.

Before cloud computing became widely available, the company generally needed to:

1. Purchase physical servers.
2. Purchase storage devices.
3. Set up networking equipment.
4. Install operating systems.
5. Configure the infrastructure.
6. Maintain hardware.
7. Handle hardware failures.
8. Upgrade infrastructure when necessary.

This required money, time, and technical resources.

AWS provides another approach.

Instead of purchasing all the infrastructure, the company can use AWS services.

```text
Traditional Approach
        |
        v
Purchase Physical Hardware
        |
        v
Install and Configure
        |
        v
Maintain Infrastructure
        |
        v
Run Application
```

```text
AWS Approach
        |
        v
Create AWS Account
        |
        v
Choose Required Services
        |
        v
Configure Resources
        |
        v
Run Application
```

### Main Reasons for Using AWS

1. Reduced upfront infrastructure investment.
2. Faster deployment.
3. Flexible resource allocation.
4. Scalability.
5. Global infrastructure.
6. Large variety of cloud services.
7. Usage-based pricing options.
8. Managed infrastructure services.
9. Security and monitoring capabilities.
10. Support for different types of applications and workloads.

---

# 5. What Can We Do With AWS?

AWS is not limited to hosting websites.

You can use AWS for many different purposes.

| Requirement | AWS Service | Purpose |
|---|---|---|
| Run a virtual server | EC2 | Compute |
| Store files and images | S3 | Object storage |
| Store relational data | RDS | Database |
| Manage users and permissions | IAM | Identity and access |
| Create a private network | VPC | Networking |
| Distribute incoming traffic | Elastic Load Balancing | Load balancing |
| Monitor applications | CloudWatch | Monitoring |
| Run code without managing servers | Lambda | Serverless computing |
| Deliver content globally | CloudFront | Content delivery |
| Manage containers | ECS / EKS | Container orchestration |
| Create NoSQL databases | DynamoDB | Database |
| Manage DNS | Route 53 | Domain name services |
| Build AI applications | Bedrock | Generative AI |
| Build machine learning workflows | SageMaker | Machine learning |

These are only some of the AWS services. We will study them individually later.

---

# 6. What Are AWS Services?

An **AWS Service** is a particular cloud capability provided by AWS to solve a specific requirement.

For example:

Suppose you need a server.

You use EC2.

Suppose you need storage.

You use S3.

Suppose you need a relational database.

You use RDS.

Suppose you need to control access.

You use IAM.

### Simple Diagram

```text
                  AWS
                   |
       +-----------+-----------+
       |           |           |
       v           v           v
     EC2           S3          RDS
       |           |           |
       v           v           v
    Compute     Storage     Database
```

Each service has its own purpose.

**Important:** AWS is the overall cloud platform. EC2, S3, RDS, IAM, and other products are individual AWS services.

---

# 7. Main Categories of AWS Services

AWS services can be grouped according to what they do.

## 7.1 Compute Services

Compute services provide processing power to run applications, programs, and workloads.

Important services:

- Amazon EC2
- AWS Lambda
- AWS Elastic Beanstalk
- Amazon ECS
- Amazon EKS
- AWS Fargate

Examples:

| Service | Purpose |
|---|---|
| EC2 | Virtual servers |
| Lambda | Run code without managing traditional servers |
| Elastic Beanstalk | Deploy and manage applications |
| ECS | Manage containers |
| EKS | Managed Kubernetes |
| Fargate | Run containers without managing the underlying server infrastructure |

## 7.2 Storage Services

Storage services allow you to store and retrieve data.

Important services:

- Amazon S3
- Amazon EBS
- Amazon EFS
- Amazon S3 Glacier storage classes

Examples:

| Service | Purpose |
|---|---|
| S3 | Object storage |
| EBS | Block storage for EC2 |
| EFS | Managed shared file storage |
| S3 Glacier storage classes | Long-term archival storage options |

## 7.3 Database Services

Database services allow you to store, organize, manage, and retrieve application data.

Important services:

- Amazon RDS
- Amazon DynamoDB
- Amazon Aurora
- Amazon Redshift
- Amazon ElastiCache

Examples:

| Service | Purpose |
|---|---|
| RDS | Managed relational databases |
| DynamoDB | Managed NoSQL database |
| Aurora | Relational database compatible with MySQL and PostgreSQL |
| Redshift | Data warehouse |
| ElastiCache | Managed in-memory caching |

## 7.4 Networking Services

Networking services help connect AWS resources and control network communication.

Important services:

- Amazon VPC
- Elastic Load Balancing
- Amazon Route 53
- AWS Direct Connect
- AWS Site-to-Site VPN

Examples:

| Service | Purpose |
|---|---|
| VPC | Logically isolated virtual network |
| Load Balancer | Distributes incoming traffic |
| Route 53 | DNS and domain routing |
| Direct Connect | Dedicated network connection to AWS |
| Site-to-Site VPN | Encrypted connection between networks |

## 7.5 Security and Identity Services

These services help protect resources and manage access.

Important services:

- AWS IAM
- AWS KMS
- AWS Secrets Manager
- AWS Certificate Manager
- Amazon GuardDuty
- AWS WAF
- AWS Shield

Examples:

| Service | Purpose |
|---|---|
| IAM | Users, roles, and permissions |
| KMS | Manage encryption keys |
| Secrets Manager | Store and manage secrets |
| Certificate Manager | Manage certificates |
| GuardDuty | Threat detection |
| WAF | Web application firewall |
| Shield | DDoS protection |

## 7.6 Monitoring and Management Services

These services help monitor resources and manage cloud environments.

Important services:

- Amazon CloudWatch
- AWS CloudTrail
- AWS Config
- AWS Systems Manager
- AWS CloudFormation

Examples:

| Service | Purpose |
|---|---|
| CloudWatch | Metrics, logs, and alarms |
| CloudTrail | Records AWS account activity |
| Config | Tracks resource configurations |
| Systems Manager | Manage AWS resources |
| CloudFormation | Infrastructure as Code |

## 7.7 AI and Machine Learning Services

AWS also provides services for artificial intelligence and machine learning.

Important services:

- Amazon Bedrock
- Amazon SageMaker AI
- Amazon Rekognition
- Amazon Textract
- Amazon Transcribe
- Amazon Polly
- Amazon Comprehend

Examples:

| Service | Purpose |
|---|---|
| Bedrock | Build generative AI applications using foundation models |
| SageMaker AI | Build, train, and deploy machine learning models |
| Rekognition | Image and video analysis |
| Textract | Extract text and information from documents |
| Transcribe | Speech-to-text |
| Polly | Text-to-speech |
| Comprehend | Natural language processing |

---

# 8. AWS and Cloud Computing

Now let's connect AWS with what we learned in the previous topic.

Cloud Computing is the delivery of computing resources and services over a network, usually the internet.

AWS is one of the platforms that provides those cloud services.

### Relationship

```text
Cloud Computing
       |
       v
Cloud Service Providers
       |
       +-------------------+
       |         |         |
       v         v         v
      AWS      Azure      GCP
       |
       v
AWS Services
       |
       +---------+---------+
       |         |         |
       v         v         v
      EC2       S3        RDS
```

### Important Difference

| Cloud Computing | AWS |
|---|---|
| A computing model | A cloud platform |
| Describes how computing services are delivered | Provides actual cloud services |
| Can be implemented by different providers | One particular provider |
| Includes concepts such as IaaS, PaaS, and SaaS | Provides services that fit different service models |

Remember:

**Cloud Computing = Concept**

**AWS = Platform that provides cloud computing services**

---

# 9. AWS and Cloud Service Models

In Cloud Computing, we studied:

1. IaaS
2. PaaS
3. SaaS
4. FaaS
5. CaaS
6. DBaaS
7. STaaS

AWS provides services that fit into these conceptual categories.

| Service Model | AWS Example | Explanation |
|---|---|---|
| IaaS | EC2 | Virtual computing infrastructure |
| PaaS | Elastic Beanstalk | Application deployment platform |
| FaaS | Lambda | Run individual functions |
| CaaS | ECS / EKS | Container management |
| DBaaS | RDS | Managed relational database |
| STaaS | S3 | Object storage service |

These are conceptual classifications. AWS does not necessarily use every XaaS term as an official product category.

### Important Point

AWS is not itself just IaaS or PaaS.

AWS provides a broad collection of services that can fit into different cloud service models.

---

# 10. AWS Global Infrastructure

This is one of the most important AWS fundamentals.

AWS operates physical infrastructure in different geographical locations around the world.

This infrastructure allows AWS customers to deploy applications closer to their users and design systems for availability and fault tolerance.

The main infrastructure concepts are:

1. Regions
2. Availability Zones
3. Data Centers
4. Edge Locations
5. Local Zones
6. Wavelength Zones

Let's understand each one.

---

# 11. What Is an AWS Region?

An **AWS Region** is a separate geographical area where AWS has infrastructure.

AWS operates multiple Regions around the world.

Examples include:

- Asia Pacific (Mumbai)
- Asia Pacific (Hyderabad)
- Asia Pacific (Singapore)
- US East (N. Virginia)
- Europe (Frankfurt)

A Region contains multiple Availability Zones.

### Example

```text
                  AWS
                   |
       +-----------+-----------+
       |           |           |
       v           v           v
    Mumbai      Singapore   Frankfurt
    Region       Region      Region
```

Each Region is designed to be isolated from other Regions.

### Why Do We Need Regions?

Suppose your application is mainly used by people in India.

You might choose an AWS Region in India to place your resources closer to those users.

This can help reduce network latency, depending on the application and network conditions.

Other reasons include:

- Data residency requirements
- Legal and compliance requirements
- Disaster recovery
- Availability
- Geographic distribution
- Application performance

### Important Points

- A Region is a geographical area.
- Different Regions are separate from one another.
- Not every AWS service is available in every Region.
- Resources are often created within a selected Region.
- Some resources and services are global rather than Region-specific.

---

# 12. AWS Region Names and Codes

AWS Regions have human-readable names and Region codes.

Examples:

| Region Name | Region Code |
|---|---|
| US East (N. Virginia) | us-east-1 |
| US West (Oregon) | us-west-2 |
| Asia Pacific (Mumbai) | ap-south-1 |
| Asia Pacific (Singapore) | ap-southeast-1 |
| Asia Pacific (Hyderabad) | ap-south-2 |
| Europe (Frankfurt) | eu-central-1 |

### Important

A Region code is used in AWS tools, configuration, and APIs.

For example:

```text
ap-south-1
```

This represents the AWS Mumbai Region.

---

# 13. What Is an Availability Zone (AZ)?

An **Availability Zone** is an isolated location within an AWS Region.

An Availability Zone consists of one or more data centers with independent infrastructure such as power, networking, and connectivity.

Each Region contains multiple Availability Zones.

### Example

```text
              AWS Mumbai Region
                      |
          +-----------+-----------+
          |           |           |
          v           v           v
         AZ 1        AZ 2        AZ 3
          |           |           |
          v           v           v
       Data       Data        Data
       Center     Center      Center
```

### Why Do We Need Availability Zones?

Imagine your application is running in only one Availability Zone.

If that Availability Zone experiences a failure, your application may become unavailable.

To reduce this risk, you can deploy your application across multiple Availability Zones.

```text
               AWS Region
                    |
          +---------+---------+
          |                   |
          v                   v
         AZ 1                AZ 2
          |                   |
          v                   v
       Server 1             Server 2
          |                   |
          +---------+---------+
                    |
                    v
                Application
```

If one Availability Zone experiences a problem, the application may continue operating through resources in another Availability Zone, provided the architecture supports failover.

### Important Points

- AZ means Availability Zone.
- An AZ exists inside a Region.
- AZs are designed to be isolated from one another.
- Multiple AZs help improve availability and fault tolerance.
- Deploying across multiple AZs does not automatically configure failover; the application architecture must support it.

---

# 14. Difference Between Region and Availability Zone

| Region | Availability Zone |
|---|---|
| Geographical area | Isolated location within a Region |
| Contains multiple AZs | Contains one or more data centers |
| Larger geographical boundary | Smaller infrastructure location |
| Example: Mumbai | An AZ inside Mumbai |
| Used for geographical deployment | Used for availability and fault tolerance |

### Easy Way to Remember

```text
Region = City / Geographic Area

Availability Zone = Separate Infrastructure Location
                     within that Region
```

A Region contains multiple Availability Zones.

---

# 15. What Is a Data Center?

A **Data Center** is a physical facility containing computing infrastructure.

It can include:

- Physical servers
- Storage systems
- Networking devices
- Power systems
- Cooling systems
- Physical security systems

AWS uses data centers to operate its cloud infrastructure.

### Relationship

```text
AWS Region
     |
     v
Availability Zones
     |
     v
Data Centers
     |
     v
Physical Servers
```

### Important Difference

A data center is a physical facility.

An Availability Zone is an isolated infrastructure location that consists of one or more data centers.

---

# 16. What Are Edge Locations?

An **Edge Location** is a location in AWS's global network used to deliver content and services closer to end users.

Edge locations are especially important for services such as Amazon CloudFront.

### Why Do We Need Them?

Suppose your website is hosted in Mumbai, but a user accesses it from the United States.

Without content delivery optimization, the user may need to retrieve content from the origin server far away.

With a CDN such as CloudFront, eligible content can be cached at edge locations closer to the user.

```text
              Origin Server
                   |
                   v
              AWS Network
                   |
          +--------+--------+
          |                 |
          v                 v
      Edge Location     Edge Location
          |                 |
          v                 v
       User A             User B
```

This can reduce latency and improve content delivery performance.

### Important

Edge locations are not the same as Availability Zones.

- Availability Zones are part of a Region.
- Edge locations are part of AWS's global edge network.

---

# 17. What Are Local Zones?

**AWS Local Zones** extend selected AWS services closer to major population, industrial, and IT centers.

They are designed for applications that need low latency to users in a particular metropolitan area.

### Example

Suppose your application requires very low latency for users in a city.

A Local Zone can help place supported compute and storage resources closer to those users.

### Remember

```text
Region
  |
  v
Availability Zones

Local Zone
  |
  v
AWS Infrastructure Closer to Users
```

Local Zones are not the same as Availability Zones.

---

# 18. What Are Wavelength Zones?

**AWS Wavelength** brings selected AWS services closer to users by deploying infrastructure within telecommunications providers' 5G networks.

It is designed for applications that need very low latency for 5G devices and users.

Examples of potential use cases:

- Real-time gaming
- Connected vehicles
- Industrial applications
- Real-time video processing

### Simple Idea

```text
5G Device
    |
    v
Telecommunications Network
    |
    v
AWS Wavelength
    |
    v
Application
```

---

# 19. Global Infrastructure Summary

| Concept | Meaning |
|---|---|
| Region | Separate geographical area |
| Availability Zone | Isolated location within a Region |
| Data Center | Physical facility containing infrastructure |
| Edge Location | Location used to deliver content closer to users |
| Local Zone | AWS infrastructure closer to metropolitan users |
| Wavelength Zone | AWS infrastructure within 5G telecommunications networks |

### Complete Structure

```text
                    AWS
                     |
                     v
                  Region
                     |
          +----------+----------+
          |          |          |
          v          v          v
         AZ 1       AZ 2       AZ 3
          |          |          |
          v          v          v
      Data       Data       Data
      Centers    Centers    Centers


          AWS Global Edge Network
                     |
                     v
              Edge Locations


              Other Extensions
                     |
             +-------+-------+
             |               |
             v               v
         Local Zones    Wavelength Zones
```

---

# 20. What Is an AWS Account?

An **AWS Account** is the basic account boundary through which you access and manage AWS resources.

When you sign up for AWS, you create an AWS account.

Through this account, you can:

- Launch EC2 instances.
- Create S3 buckets.
- Create databases.
- Configure networks.
- Manage users and permissions.
- Monitor resources.
- View billing information.
- Access AWS services.

### Simple Example

Imagine you create an AWS account.

Inside that account, you create:

```text
                AWS Account
                     |
       +-------------+-------------+
       |             |             |
       v             v             v
      EC2           S3            RDS
       |             |             |
       v             v             v
    Server         Files        Database
```

All these resources belong to your AWS account.

### Important

An AWS account is not the same as an IAM user.

An AWS account is the overall account boundary.

IAM users, roles, and policies help control access to resources within the account.

---

# 21. Root User

When you create an AWS account, AWS provides a **root user** identity.

The root user has complete access to the account and its resources.

It is associated with the email address used to create the AWS account.

### Important Security Practices

- Do not use the root user for everyday activities.
- Enable multi-factor authentication (MFA).
- Do not share root credentials.
- Keep root credentials secure.
- Use appropriately permissioned identities for regular work.

### Simple Relationship

```text
                AWS Account
                     |
                     v
                 Root User
                     |
                     v
             Complete Account Access
```

The root user should be protected carefully.

---

# 22. What Is IAM?

**IAM stands for Identity and Access Management.**

AWS IAM is a service used to manage identities and permissions.

It helps control:

- Who can access AWS?
- What resources can they access?
- What actions can they perform?

### Example

Suppose you have a company with three employees.

```text
                  AWS Account
                       |
                       v
                      IAM
                       |
          +------------+------------+
          |            |            |
          v            v            v
       Employee A  Employee B   Employee C
          |            |            |
          v            v            v
       EC2 Access   S3 Access   Read-Only Access
```

Each employee can receive different permissions.

### Important IAM Concepts

| Concept | Meaning |
|---|---|
| IAM User | Identity for an individual or application that needs long-term credentials |
| IAM Group | Collection of IAM users |
| IAM Role | Identity with permissions that can be assumed |
| IAM Policy | Document defining permissions |
| MFA | Additional authentication factor |

### Important

IAM is a foundational AWS security service.

We will study IAM in detail as a separate topic.

---

# 23. AWS Management Console

The **AWS Management Console** is a web-based interface used to access and manage AWS services.

You can open the console through a web browser.

From the console, you can:

- Create EC2 instances.
- Create S3 buckets.
- Configure databases.
- Manage IAM.
- Create networks.
- View billing.
- Monitor services.

### Simple Example

```text
          Your Web Browser
                 |
                 v
        AWS Management Console
                 |
       +---------+---------+
       |         |         |
       v         v         v
      EC2        S3        RDS
```

It is generally the easiest way for beginners to explore AWS.

---

# 24. AWS CLI

**CLI stands for Command Line Interface.**

AWS CLI allows you to interact with AWS services using commands in a terminal.

Instead of clicking through the AWS Management Console, you can execute commands.

For example:

```powershell
aws --version
```

This checks whether AWS CLI is installed and available.

Another example:

```powershell
aws s3 ls
```

This lists S3 buckets accessible to the configured identity.

### Why Use AWS CLI?

- Automate tasks.
- Manage resources from a terminal.
- Execute repetitive commands.
- Integrate AWS operations into scripts.
- Work with deployment pipelines.

We will learn AWS CLI and its Windows setup later.

---

# 25. AWS SDK

**SDK stands for Software Development Kit.**

AWS SDKs allow developers to interact with AWS services directly from programming languages.

AWS provides SDKs for languages such as:

- Python
- JavaScript
- Java
- .NET
- Go

### Example

Suppose you are developing a Python application.

You want your application to upload an image to an S3 bucket.

You can use the AWS SDK for Python, commonly called **Boto3**, to interact with S3.

```text
Python Application
        |
        v
     Boto3 SDK
        |
        v
      AWS S3
        |
        v
    Store Image
```

### CLI vs SDK vs Console

| Method | Purpose |
|---|---|
| Management Console | Manage AWS using a web interface |
| AWS CLI | Manage AWS using terminal commands |
| AWS SDK | Access AWS services from application code |

---

# 26. What Is an AWS API?

**API stands for Application Programming Interface.**

An API allows different software systems to communicate with each other.

AWS services expose APIs that can be used to create, configure, manage, and access resources.

For example:

A program can send a request to an AWS service to create a resource.

```text
Application
    |
    v
AWS API Request
    |
    v
AWS Service
    |
    v
Perform Requested Action
```

The AWS Console, CLI, and SDK use AWS service APIs behind the scenes.

---

# 27. What Is an AWS Resource?

An **AWS Resource** is an individual entity that you create or manage within an AWS service.

Examples:

- An EC2 instance
- An S3 bucket
- An RDS database
- A VPC
- An IAM user
- A Lambda function

### Example

```text
AWS Account
    |
    +--------------------+
    |                    |
    v                    v
   EC2                  S3
    |                    |
    v                    v
EC2 Instance          S3 Bucket
```

Here:

- EC2 is the service.
- The EC2 instance is a resource.
- S3 is the service.
- The S3 bucket is a resource.

---

# 28. What Is an AWS Workload?

A **Workload** is an application, service, or collection of resources that performs a particular business or technical task.

For example, an online shopping application is a workload.

It may contain:

- Frontend application
- Backend application
- Database
- File storage
- Networking
- Security configuration
- Monitoring

### Example Architecture

```text
             Users
               |
               v
          Web Application
               |
               v
             EC2
               |
       +-------+-------+
       |               |
       v               v
      RDS             S3
   Database       File Storage
```

Together, these resources support the shopping application workload.

---

# 29. What Is an AWS ARN?

**ARN stands for Amazon Resource Name.**

An ARN is a unique identifier used to identify specific AWS resources.

It is commonly used in IAM policies and other AWS configurations.

### Example Format

```text
arn:partition:service:region:account-id:resource
```

For example, an S3 bucket ARN can look like:

```text
arn:aws:s3:::my-example-bucket
```

An EC2 instance ARN can look like:

```text
arn:aws:ec2:ap-south-1:123456789012:instance/i-0123456789abcdef0
```

### Why Are ARNs Needed?

ARNs help AWS identify resources precisely.

For example, an IAM policy can specify which S3 bucket or EC2 resource an identity is allowed to access.

---

# 30. What Is an AWS Service Quota?

An **AWS Service Quota** is a limit on how much of a particular AWS service or resource you can use.

For example, an account may have a limit on the number of EC2 instances it can run in a particular Region.

Other quotas can apply to:

- Storage
- API requests
- Networking resources
- Database resources
- Concurrent executions

Some quotas can be increased by submitting a quota-increase request.

### Important

Service quotas help manage resource usage and protect the cloud environment.

---

# 31. AWS Shared Responsibility Model

This is one of the most important AWS concepts, especially for security.

The **Shared Responsibility Model** means that security responsibilities are shared between AWS and the customer.

AWS is responsible for security **of the cloud**.

The customer is responsible for security **in the cloud**.

The exact division depends on the AWS service being used.

---

## 31.1 AWS Responsibility: Security of the Cloud

AWS is responsible for protecting the underlying cloud infrastructure.

This includes:

- Physical data centers
- Physical servers
- Physical networking
- Hardware
- Infrastructure facilities
- Underlying virtualization infrastructure

### Example

You use an EC2 instance.

AWS manages the physical server on which the EC2 instance runs.

You do not need to enter the AWS data center to maintain the physical server.

---

## 31.2 Customer Responsibility: Security in the Cloud

Customers are responsible for securing the resources and configurations they use.

Depending on the service, this can include:

- Customer data
- User permissions
- Application security
- Operating system updates
- Network configuration
- Encryption settings
- Access policies
- Security group configuration

### Example

Suppose you create an EC2 instance.

AWS manages the underlying physical infrastructure.

You are responsible for managing the guest operating system, installing updates, securing your application, and configuring the appropriate access controls.

---

## Shared Responsibility Diagram

```text
             AWS CLOUD SECURITY
                    |
          +---------+---------+
          |                   |
          v                   v
       AWS                   Customer
          |                   |
          v                   v
   Security OF Cloud    Security IN Cloud
          |                   |
          v                   v
   Physical Hardware     Customer Data
   Data Centers          Applications
   Infrastructure        OS Configuration
   Physical Security     Access Permissions
                         Security Settings
```

### Important: Responsibilities Depend on the Service

For example:

**EC2:**

The customer has more responsibility because they manage the guest operating system and applications.

**S3:**

AWS manages the underlying infrastructure, while the customer manages data, access permissions, and relevant security settings.

### Easy Way to Remember

```text
AWS       = Security OF the Cloud

Customer  = Security IN the Cloud
```

---

# 32. AWS Pricing Basics

AWS provides different pricing models depending on the service.

Many services offer usage-based pricing.

This means that you may pay according to the resources you consume.

However, AWS does not use one single pricing model for every service.

### Common Pricing Models

## 32.1 On-Demand

You pay for resources according to the time or usage specified by the service's pricing model.

You generally do not need a long-term commitment.

## 32.2 Savings Plans

Savings Plans offer discounted rates in exchange for committing to a specified amount of eligible usage over a period of time.

## 32.3 Reserved Instances

Some AWS services offer reservation-based pricing options for eligible resources.

The exact commitment and discount conditions depend on the service and offering.

## 32.4 Spot Instances

EC2 Spot Instances use spare AWS compute capacity at discounted prices.

However, AWS can interrupt Spot Instances when it needs the capacity back.

They are suitable for workloads that can tolerate interruptions.

### Pricing Comparison

| Pricing Model | Basic Idea |
|---|---|
| On-Demand | Pay according to usage |
| Savings Plans | Commit to eligible usage for discounted rates |
| Reserved Instances | Reservation-based pricing for eligible services |
| Spot Instances | Use spare EC2 capacity at discounted rates, with interruption risk |

---

# 33. AWS Free Tier

AWS provides Free Tier offers for eligible services and accounts.

These offers can help beginners explore AWS without paying the normal price for every eligible usage amount.

However, **Free Tier does not mean everything in AWS is free**.

Important things to remember:

- Free offers have eligibility conditions.
- Some offers have usage limits.
- Some services are not included.
- Exceeding included usage can create charges.
- Certain resources may continue generating costs even when you are not actively using them.

Always check the current pricing and Free Tier details before creating resources.

### Important Safety Practices for Beginners

1. Understand the pricing before launching resources.
2. Set up billing alerts or AWS Budgets.
3. Monitor your AWS usage.
4. Stop or delete resources when they are no longer needed.
5. Check storage, snapshots, IP addresses, and other resources that may continue generating charges.
6. Never assume that an inactive resource is automatically free.

---

# 34. What Is AWS Billing?

AWS Billing helps you understand and manage the costs associated with using AWS.

You can use AWS billing tools to:

- View charges.
- Track usage.
- Understand service costs.
- Monitor spending.
- Review invoices.
- Set budgets and alerts.

### Example

Suppose you use:

```text
EC2       = Compute Cost
S3        = Storage Cost
RDS       = Database Cost
```

Your AWS bill can include charges from these services.

The final cost depends on usage, configuration, Region, pricing options, and applicable charges.

---

# 35. What Is AWS Budgets?

**AWS Budgets** allows you to create budgets to monitor your AWS costs and usage.

For example, suppose you want to keep your monthly AWS spending within a certain amount.

You can create a budget and configure alerts when actual or forecasted spending reaches specified thresholds.

### Example

```text
Monthly Budget = $10

Usage Reaches 80%
       |
       v
Receive Alert

Usage Reaches 100%
       |
       v
Receive Alert
```

The alerts help you monitor spending.

**Important:** A budget alert does not automatically stop all AWS resources or guarantee that you cannot exceed your budget.

---

# 36. What Is AWS Organizations?

**AWS Organizations** is a service that helps centrally manage multiple AWS accounts.

For example, a large company may have separate AWS accounts for:

- Development
- Testing
- Production
- Finance
- Research

Instead of managing every account completely independently, the organization can use AWS Organizations to manage them centrally.

### Example

```text
             AWS Organization
                    |
          +---------+---------+
          |         |         |
          v         v         v
       Account 1 Account 2 Account 3
          |         |         |
          v         v         v
         Dev       Test      Production
```

This helps with account management, governance, and consolidated billing.

---

# 37. What Is an AWS IAM Role?

We introduced IAM earlier.

Now let's understand one important IAM concept: the role.

An **IAM Role** is an identity with permissions that can be assumed by a trusted user, application, or AWS service.

For example:

Suppose an EC2 application needs to access an S3 bucket.

Instead of storing long-term access keys inside the application, you can attach an appropriate IAM role to the EC2 instance.

```text
EC2 Instance
     |
     v
IAM Role
     |
     v
Permission to Access S3
     |
     v
S3 Bucket
```

This is a common way to grant AWS resources permission to communicate with other AWS services.

---

# 38. What Is High Availability in AWS?

**High Availability (HA)** means designing an application so that it remains accessible even when some infrastructure components fail.

AWS provides infrastructure across multiple Availability Zones, which can help create highly available architectures.

### Example

Suppose your application runs on one EC2 instance in one Availability Zone.

If that instance or Availability Zone fails, your application may stop working.

A more resilient design can use multiple EC2 instances across multiple Availability Zones.

```text
                 Users
                   |
                   v
             Load Balancer
                   |
          +--------+--------+
          |                 |
          v                 v
         EC2               EC2
        AZ 1              AZ 2
          |                 |
          +--------+--------+
                   |
                   v
               Database
```

A properly designed architecture can route traffic to healthy resources when another resource fails.

### Important

High availability requires proper application architecture and configuration.

Simply creating an EC2 instance in AWS does not automatically make an application highly available.

---

# 39. What Is Fault Tolerance?

**Fault Tolerance** means the ability of a system to continue operating even when certain components fail.

For example:

Suppose your application uses two servers.

If one server fails, another server can continue handling the workload.

```text
           Application
                |
       +--------+--------+
       |                 |
       v                 v
    Server 1          Server 2
       |                 |
       v                 v
    Working             Working
```

If Server 1 fails:

```text
           Application
                |
       +--------+--------+
       |                 |
       v                 v
    Server 1          Server 2
    FAILED             ACTIVE
                          |
                          v
                   Handles Traffic
```

High availability and fault tolerance are related, but they are not exactly the same.

- High availability focuses on minimizing downtime.
- Fault tolerance focuses on continuing operation despite failures.

---

# 40. What Is Disaster Recovery?

**Disaster Recovery (DR)** is the process of restoring applications, systems, and data after a major failure or disaster.

Examples:

- Data center failure
- Accidental data deletion
- Cyberattack
- Regional outage
- Major infrastructure failure

AWS offers services and capabilities that help organizations create disaster recovery strategies.

These can include:

- Backups
- Data replication
- Multiple Regions
- Recovery procedures
- Automated infrastructure deployment

### Simple Example

```text
Primary Region
      |
      v
Application Running
      |
      v
Major Failure
      |
      v
Recovery Strategy
      |
      v
Backup / Secondary Environment
      |
      v
Restore Application
```

### Important Difference

| High Availability | Disaster Recovery |
|---|---|
| Focuses on minimizing downtime | Focuses on recovery after major disruption |
| Often uses multiple AZs | May use backups or another Region |
| Designed for component failures | Designed for larger incidents |
| Keeps services available | Restores services after disruption |

---

# 41. What Is Scalability in AWS?

Scalability means increasing or decreasing computing resources according to workload requirements.

AWS supports different scaling approaches.

## Vertical Scaling

Increase the resources of an existing EC2 instance.

```text
Before:
Small EC2 Instance

       |
       v

After:
Larger EC2 Instance
```

## Horizontal Scaling

Add more EC2 instances.

```text
Before:
EC2 Instance 1

       |
       v

After:
EC2 Instance 1
EC2 Instance 2
EC2 Instance 3
```

AWS provides services such as EC2 Auto Scaling to help automatically adjust the number of EC2 instances according to configured conditions.

---

# 42. What Is Elasticity in AWS?

Elasticity means dynamically adjusting resources according to changing demand.

For example:

Suppose your website normally receives 100 users.

During a sale, it receives 10,000 users.

You may need additional computing capacity.

After the sale, traffic decreases and you may reduce the resources.

```text
Normal Traffic
      |
      v
2 EC2 Instances
      |
      v
Traffic Increases
      |
      v
5 EC2 Instances
      |
      v
Traffic Decreases
      |
      v
2 EC2 Instances
```

AWS Auto Scaling can help automate this process when configured correctly.

### Remember

Scalability = Ability to handle more workload.

Elasticity = Ability to adjust resources dynamically according to demand.

---

# 43. What Is a Load Balancer?

A **Load Balancer** distributes incoming traffic across multiple targets, such as EC2 instances.

Suppose 1,000 users access your application.

Instead of sending all requests to one server, a load balancer can distribute requests across multiple healthy servers.

```text
             1,000 Users
                  |
                  v
             Load Balancer
                  |
         +--------+--------+
         |        |        |
         v        v        v
       EC2 1    EC2 2    EC2 3
```

Benefits:

- Distributes incoming traffic.
- Helps avoid overloading one server.
- Supports highly available architectures.
- Can route traffic to healthy targets.

AWS provides Elastic Load Balancing for this purpose.

---

# 44. What Is Serverless Computing?

Serverless computing allows developers to run code without directly managing traditional server infrastructure.

**Important:** Serverless does not mean that servers do not exist.

Servers still exist, but the cloud provider manages the underlying infrastructure.

### AWS Example: Lambda

Suppose you want to execute a function when a user uploads an image.

You can configure an AWS Lambda function to run when an S3 upload event occurs.

```text
User Uploads Image
        |
        v
      S3 Bucket
        |
        v
   Trigger Event
        |
        v
   AWS Lambda
        |
        v
  Process Image
```

You focus on writing the function rather than managing a traditional server for it.

---

# 45. What Is AWS Infrastructure as Code (IaC)?

**Infrastructure as Code (IaC)** means defining and managing infrastructure using code or configuration files instead of manually creating everything through a graphical interface.

For example, you can define:

- EC2 instances
- S3 buckets
- VPCs
- Security groups
- Databases

AWS provides **AWS CloudFormation** for infrastructure provisioning using templates.

Terraform is another popular Infrastructure as Code tool, but it is developed by HashiCorp, not AWS.

### Example

```text
Infrastructure Template
          |
          v
    CloudFormation
          |
          v
       AWS Cloud
          |
     +----+----+
     |    |    |
     v    v    v
    EC2   S3   VPC
```

---

# 46. What Is AWS Monitoring?

Monitoring means observing the performance, health, and behavior of cloud resources and applications.

AWS provides **Amazon CloudWatch** for monitoring.

You can use it to:

- Collect metrics.
- Store and view logs.
- Create alarms.
- Monitor resource performance.
- Track application behavior.

### Example

Suppose your EC2 instance is using too much CPU.

CloudWatch can monitor CPU utilization and trigger an alarm when a configured threshold is reached.

```text
EC2 Instance
      |
      v
CloudWatch
      |
      v
Monitor CPU Usage
      |
      v
Threshold Reached
      |
      v
Generate Alarm
```

---

# 47. What Is AWS CloudTrail?

**AWS CloudTrail** records account activity and API events.

It helps answer questions such as:

- Who performed an action?
- What action was performed?
- When did it happen?
- Which resource was affected?

### Example

Suppose someone deletes an S3 bucket.

CloudTrail can help you investigate the API activity associated with that action, subject to the event type and logging configuration.

### CloudWatch vs CloudTrail

| CloudWatch | CloudTrail |
|---|---|
| Monitoring and observability | Account activity and API auditing |
| Metrics, logs, alarms | Records API events |
| Helps monitor resource health | Helps investigate who did what |

---

# 48. How Does a Typical Application Work on AWS?

Let's imagine you want to deploy a full-stack web application.

Your application has:

- Frontend
- Backend
- Database
- Images and documents
- Users

You could use AWS services like these:

```text
                  Users
                    |
                    v
                CloudFront
                    |
                    v
              Frontend / Web
                    |
                    v
              Load Balancer
                    |
                    v
                  EC2
                    |
             +------+------+
             |             |
             v             v
            RDS           S3
         Database      File Storage
```

You might also use:

```text
IAM        -> Access management
VPC        -> Network isolation
CloudWatch -> Monitoring
CloudTrail -> Activity tracking
```

This is an example architecture. Actual architectures depend on application requirements.

---

# 49. AWS vs Microsoft Azure vs Google Cloud

AWS is not the only cloud provider.

Other major cloud platforms include:

1. Amazon Web Services (AWS)
2. Microsoft Azure
3. Google Cloud Platform (GCP)

| Category | AWS | Azure | Google Cloud |
|---|---|---|---|
| Compute | EC2 | Azure Virtual Machines | Compute Engine |
| Object Storage | S3 | Blob Storage | Cloud Storage |
| Relational Database | RDS | Azure SQL Database | Cloud SQL |
| Serverless | Lambda | Azure Functions | Cloud Run Functions |
| Identity | IAM | Microsoft Entra ID / Azure RBAC | Cloud IAM |
| Kubernetes | EKS | AKS | GKE |

All three provide cloud computing services, but their service names, features, pricing, and architecture differ.

---

# 50. AWS Terminology You Must Know

Here are some important terms you will frequently encounter while learning AWS.

| Term | Meaning |
|---|---|
| AWS | Amazon Web Services |
| Cloud | Delivery of computing resources over a network |
| Region | Geographical AWS infrastructure area |
| AZ | Availability Zone |
| Data Center | Physical facility containing computing infrastructure |
| Edge Location | Location used to deliver content closer to users |
| Instance | A running virtual server, such as an EC2 instance |
| Resource | An individual AWS entity that you create or manage |
| Workload | Application or collection of resources performing a task |
| IAM | Identity and Access Management |
| ARN | Amazon Resource Name |
| CLI | Command Line Interface |
| SDK | Software Development Kit |
| API | Application Programming Interface |
| MFA | Multi-Factor Authentication |
| VPC | Virtual Private Cloud |
| HA | High Availability |
| DR | Disaster Recovery |
| IaC | Infrastructure as Code |
| CDN | Content Delivery Network |
| DNS | Domain Name System |
| IaaS | Infrastructure as a Service |
| PaaS | Platform as a Service |
| SaaS | Software as a Service |
| FaaS | Function as a Service |
| TCO | Total Cost of Ownership |

---

# 51. Important AWS Concepts: Quick Revision

| Concept | Simple Explanation |
|---|---|
| AWS | Amazon's cloud computing platform |
| AWS Service | A cloud capability offered by AWS |
| AWS Account | Account boundary for managing AWS resources |
| Root User | Original identity with complete account access |
| IAM | Manages identities and permissions |
| Region | Geographic area containing AWS infrastructure |
| Availability Zone | Isolated location within a Region |
| Data Center | Physical facility containing servers and infrastructure |
| Edge Location | Helps deliver content closer to users |
| Resource | An individual AWS entity |
| Workload | Application or collection of resources |
| ARN | Unique AWS resource identifier |
| Shared Responsibility | Security responsibilities divided between AWS and customer |
| AWS Console | Web-based AWS management interface |
| AWS CLI | Command-line access to AWS |
| AWS SDK | Programmatic access to AWS from code |
| AWS Billing | Tracks AWS charges |
| AWS Budgets | Monitors configured spending and usage budgets |
| CloudWatch | Monitoring and observability |
| CloudTrail | Records account activity and API events |
| CloudFormation | Infrastructure as Code |
| EC2 | Virtual computing |
| S3 | Object storage |
| RDS | Managed relational database |
| VPC | Logically isolated virtual network |
| Lambda | Serverless functions |

---

# 52. AWS Learning Roadmap

Now that we understand what AWS is and its fundamentals, we can start learning individual AWS services.

Here is the learning sequence.

## Phase 1: AWS Fundamentals

- What is AWS?
- AWS Global Infrastructure
- Regions and Availability Zones
- AWS Accounts
- Root User
- IAM Fundamentals
- Shared Responsibility Model
- AWS Pricing
- AWS Management Console
- AWS CLI Basics

## Phase 2: Compute Services

- What is Compute?
- Amazon EC2
- EC2 Instance Types
- AMIs
- Key Pairs
- Security Groups
- EBS
- EC2 Pricing
- Elastic Load Balancing
- Auto Scaling
- AWS Lambda
- Elastic Beanstalk

## Phase 3: Storage Services

- Storage Fundamentals
- Amazon S3
- S3 Buckets
- S3 Objects
- Storage Classes
- Bucket Policies
- Versioning
- Lifecycle Rules
- EBS
- EFS
- Backup and Archival

## Phase 4: Networking

- Networking Fundamentals
- Amazon VPC
- CIDR
- Subnets
- Public and Private Subnets
- Route Tables
- Internet Gateway
- NAT Gateway
- Security Groups
- Network ACLs
- Elastic IP
- Route 53
- CloudFront
- VPN
- Direct Connect

## Phase 5: Database Services

- Database Fundamentals
- Amazon RDS
- RDS Engines
- Multi-AZ
- Read Replicas
- DynamoDB
- Aurora
- ElastiCache
- Redshift

## Phase 6: Security

- IAM Users
- IAM Groups
- IAM Roles
- IAM Policies
- MFA
- KMS
- Secrets Manager
- GuardDuty
- WAF
- Shield
- Security Best Practices

## Phase 7: Monitoring and Management

- CloudWatch
- CloudTrail
- AWS Config
- Systems Manager
- AWS Budgets
- AWS Organizations
- CloudFormation

## Phase 8: Advanced AWS

- Containers
- Docker
- ECS
- EKS
- Fargate
- Serverless Architecture
- Event-Driven Architecture
- SQS
- SNS
- EventBridge
- Step Functions
- CI/CD
- Infrastructure as Code
- Terraform
- AWS DevOps

## Phase 9: AI and Machine Learning on AWS

- Amazon Bedrock
- SageMaker AI
- Rekognition
- Textract
- Transcribe
- Polly
- Comprehend
- AI Application Deployment

## Phase 10: Practical Projects

- Host a Static Website using S3
- Deploy a Web Application using EC2
- Build a VPC Architecture
- Host a Full-Stack Application
- Build a Serverless Application
- Create a Backup and Recovery System
- Build a Monitoring Dashboard
- Deploy an AI Application on AWS

---

# 53. Doubts & Clarifications

This section will contain questions that arise during our AWS learning journey.

Whenever we discuss a doubt in a later session, we can add the question and its clarified answer here.

## Doubt 1: Is AWS the Same as Cloud Computing?

**No.**

Cloud Computing is the concept of delivering computing services over a network.

AWS is a platform that provides those services.

Other cloud platforms include Azure and Google Cloud.

## Doubt 2: Does AWS Own Physical Servers?

**Yes.**

AWS operates physical infrastructure in data centers around the world.

Customers access cloud services built on that infrastructure.

## Doubt 3: Is EC2 AWS or Cloud Computing?

EC2 is an AWS service.

It provides virtual computing capacity and is commonly classified as IaaS.

## Doubt 4: Is AWS Just for Hosting Websites?

**No.**

AWS can be used for:

- Web applications
- Mobile application backends
- Databases
- File storage
- Data analytics
- AI and machine learning
- Machine learning model deployment
- Serverless applications
- Enterprise systems
- Backup and disaster recovery

## Doubt 5: Is a Region the Same as an Availability Zone?

**No.**

A Region is a geographical area.

An Availability Zone is an isolated location within that Region.

One Region contains multiple Availability Zones.

## Doubt 6: Does AWS Automatically Make My Application Highly Available?

**No.**

AWS provides infrastructure and services that help build highly available applications.

But you must design and configure your architecture appropriately.

## Doubt 7: Is AWS Free?

**Not completely.**

AWS has Free Tier offers for eligible services and accounts, but many services and usage levels can incur charges.

Always check pricing before creating resources.

## Doubt 8: Is Serverless Computing Really Without Servers?

**No.**

Servers still exist.

The difference is that AWS manages the underlying server infrastructure for you.

## Doubt 9: Is IAM a Separate AWS Account?

**No.**

IAM is a service within AWS used to manage identities and permissions.

## Doubt 10: Are AWS Console, CLI, and SDK Different AWS Services?

They are different ways to interact with AWS.

- Console: Web interface.
- CLI: Terminal commands.
- SDK: Programming language libraries.

They are not interchangeable names for the same thing.

---

# 54. Final Summary

Let's understand the complete AWS picture.

```text
                    AMAZON
                       |
                       v
             AMAZON WEB SERVICES
                       |
                       v
                CLOUD PLATFORM
                       |
       +---------------+---------------+
       |               |               |
       v               v               v
    COMPUTE          STORAGE        DATABASE
       |               |               |
       v               v               v
      EC2              S3              RDS
       |               |               |
       +---------------+---------------+
                       |
                       v
                AWS GLOBAL INFRA
                       |
             +---------+---------+
             |                   |
             v                   v
           REGIONS        EDGE LOCATIONS
             |
             v
     AVAILABILITY ZONES
             |
             v
        DATA CENTERS
             |
             v
       PHYSICAL HARDWARE
```

### Remember These 10 Things

1. AWS stands for Amazon Web Services.
2. AWS is a cloud computing platform provided by Amazon.
3. AWS was launched in 2006.
4. AWS provides compute, storage, database, networking, security, AI, and many other services.
5. EC2 is used for virtual computing.
6. S3 is used for object storage.
7. RDS is used for managed relational databases.
8. A Region is a geographical area, while an Availability Zone is an isolated location within that Region.
9. IAM manages identities and permissions.
10. AWS and its customers share security responsibilities.

**The most important thing:** Don't try to memorize every AWS service right now. First understand what AWS is, how its infrastructure works, how accounts and permissions work, and how you interact with AWS. Then we will study each service deeply with examples and practical exercises.