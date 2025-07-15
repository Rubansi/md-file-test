# AWS Certified Cloud Practitioner Advanced Practice Questions

**Total Questions: 250 (expandable)**

---

### Question 1  
A company wants to reduce costs by using reserved EC2 instances but faces challenges managing multiple department accounts with unused reserved capacity in some accounts and insufficient capacity in others.

Which AWS feature enables sharing reserved instances across accounts?

A) AWS Organizations Consolidated Billing  
B) EC2 Instance Savings Plans  
C) Reserved Instance Marketplace  
D) AWS Reserved Instance Sharing

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** A

**Explanation:**  
AWS Organizations with consolidated billing allows sharing Reserved Instances (RIs) across member accounts in the organization, enabling cost optimization when some departments have unused RIs and others require more capacity. This avoids isolated unused RIs and enables flexible resource utilization.

</details>

---

### Question 2  
Which AWS service provides automatic encryption of data at rest for objects stored in S3 without requiring user interaction?

A) AWS Key Management Service (KMS)  
B) Amazon S3 Server-Side Encryption (SSE-S3)  
C) AWS Shield  
D) Amazon Macie

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** B

**Explanation:**  
Amazon S3 offers Server-Side Encryption with S3-managed keys (SSE-S3), which automatically encrypts data at rest without user intervention. While KMS offers more control (SSE-KMS), SSE-S3 is fully managed and transparent.

</details>

---

### Question 3  
A customer wants to distribute incoming HTTP traffic across multiple EC2 instances in one or more Availability Zones with support for advanced request routing (e.g., path-based routing).

Which AWS service should the customer use?

A) Classic Load Balancer  
B) Network Load Balancer  
C) Application Load Balancer  
D) Amazon Route 53

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** C

**Explanation:**  
The Application Load Balancer operates at the application layer (Layer 7) and supports advanced routing features such as host-based or path-based routing. This is suitable for distributing HTTP/HTTPS traffic to multiple EC2 instances.

</details>

---

### Question 4  
Which AWS pricing model provides the most cost savings for applications with predictable, steady-state workloads?

A) On-Demand Instances  
B) Spot Instances  
C) Reserved Instances  
D) Dedicated Hosts

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** C

**Explanation:**  
Reserved Instances provide significant discounts compared to On-Demand pricing and are best suited for predictable, steady-state workloads since customers commit to 1- or 3-year terms for capacity.

</details>

---

### Question 5  
Which AWS feature allows configuring a multi-account setup where each AWS account can have its own security boundaries, but still be centrally managed?

A) AWS IAM  
B) AWS Organizations with Service Control Policies (SCPs)  
C) AWS Control Tower  
D) AWS CloudTrail

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** B

**Explanation:**  
AWS Organizations allows multiple accounts to be managed centrally, and Service Control Policies (SCPs) are applied to accounts or organizational units to enforce permissions and security boundaries while keeping accounts separate.

</details>

---

# AWS Certified Cloud Practitioner Advanced Practice Questions (Batch 2)

---

### Question 6  
A startup runs a web application on EC2 instances behind an Application Load Balancer (ALB). They want to save costs by shutting down instances during off-peak hours but keep the application highly available.

Which AWS feature or strategy best supports this goal?

A) Use Auto Scaling with scheduled scaling policies to reduce instances during off-peak hours  
B) Manually stop EC2 instances every evening and start them in the morning  
C) Use Spot Instances exclusively to save costs  
D) Move the entire workload to a single large EC2 instance

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** A

**Explanation:**  
Auto Scaling with scheduled scaling policies allows automatic adjustment of EC2 capacity based on predefined schedules, reducing instances during off-peak hours to save costs while maintaining availability. Manual stopping risks downtime, and Spot Instances may be interrupted. Moving to a single instance reduces availability.

</details>

---

### Question 7  
A company needs to store sensitive customer data that must be encrypted and comply with regulatory standards. The data should be accessible by multiple AWS services with granular access control.

Which AWS service should be used to manage encryption keys securely?

A) AWS Secrets Manager  
B) AWS Key Management Service (KMS)  
C) AWS Certificate Manager  
D) Amazon Macie

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** B

**Explanation:**  
AWS KMS provides centralized control over encryption keys, enabling secure key storage, management, and access policies integrated with many AWS services. Secrets Manager manages secrets but not encryption keys, Certificate Manager focuses on SSL/TLS certificates, and Macie provides data discovery and classification.

</details>

---

### Question 8  
A retail company wants to implement a multi-region disaster recovery strategy for their database workloads with minimal downtime.

Which AWS feature or service combination allows the most effective failover between regions?

A) Amazon RDS Multi-AZ Deployment  
B) Amazon RDS Read Replicas within the same region  
C) Amazon RDS Cross-Region Read Replicas with manual promotion  
D) Backups to Amazon S3 without replication

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** C

**Explanation:**  
Amazon RDS Cross-Region Read Replicas provide asynchronous replication to a different AWS region. They can be promoted to standalone databases to enable failover during disaster recovery with minimal downtime. Multi-AZ is limited to one region; same-region replicas do not protect against regional failures. S3 backups help with recovery but involve longer downtime.

</details>

---

### Question 9  
A large enterprise wants to monitor API calls made across multiple AWS accounts in their organization for security and compliance auditing.

Which service allows centralized collection and analysis of this data?

A) AWS Config  
B) AWS CloudTrail with organization trails  
C) Amazon GuardDuty  
D) Amazon Inspector

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** B

**Explanation:**  
AWS CloudTrail organization trails enable centralized logging of API calls across all member accounts in an AWS Organization, supporting comprehensive auditing and security analysis. AWS Config tracks resource configurations, GuardDuty detects threats, and Inspector assesses security vulnerabilities.

</details>

---

### Question 10  
A DevOps team wants to automate deployment pipelines for their containerized applications running on Amazon ECS. They require continuous integration and continuous delivery (CI/CD) with automated testing.

Which AWS managed service provides the best end-to-end solution?

A) AWS CodePipeline  
B) AWS CodeDeploy  
C) AWS CodeBuild  
D) Amazon ECR

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** A

**Explanation:**  
AWS CodePipeline is a fully managed CI/CD service that automates the build, test, and deployment phases. It integrates with CodeBuild for builds/tests and CodeDeploy for deployments. CodeBuild is focused on the build step alone, CodeDeploy on deployment, and ECR is a container registry, not a pipeline.

</details>

---

### Question 11  
A media company streams video content globally and desires low latency for users in Asia, Europe, and the Americas. Their videos are stored in an S3 bucket in the US East (N. Virginia) region.

Which AWS service can help achieve low latency content delivery globally?

A) Amazon CloudFront  
B) AWS Global Accelerator  
C) VPC peering between regions  
D) AWS Direct Connect

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** A

**Explanation:**  
Amazon CloudFront is a global content delivery network (CDN) that caches copies of content at edge locations worldwide, lowering latency for global users. AWS Global Accelerator optimizes global traffic routing but is more suited for TCP/UDP apps. VPC peering and Direct Connect are network connectivity tools, not CDNs.

</details>

---

### Question 12  
A finance company requires that access to critical workloads be restricted based on the source IP address for audit and compliance.

Which AWS service and feature combination allows enforcing this control using identity and access management?

A) AWS IAM policies with IP address conditions  
B) Network ACLs in the VPC  
C) Security groups with IP address filters  
D) AWS WAF rules on the application firewall

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** A

**Explanation:**  
IAM policies support condition elements, including source IP addresses (e.g., aws:SourceIp), enabling fine-grained access control to AWS API actions based on requester IP addresses. Network ACLs and security groups control traffic at the network level but do not manage AWS API permissions. AWS WAF is for web application firewall control.

</details>

---

### Question 13  
A healthcare organization wants to ensure their data stored in AWS complies with HIPAA regulations and only authenticated users can access it.

Which AWS service provides compliance features and secure user access management?

A) Amazon Cognito  
B) AWS Artifact  
C) AWS IAM combined with encrypted Amazon S3 buckets  
D) Amazon Macie

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** C

**Explanation:**  
AWS IAM provides secure authentication and authorization that controls which users can access data, combined with encrypted S3 buckets, which protect data at rest to meet HIPAA requirements. AWS Artifact provides compliance documentation but doesn't enforce security. Amazon Cognito manages user sign-up/sign-in but is mostly for frontend apps. Macie helps discover sensitive data but does not enforce access.

</details>

---

### Question 14  
A company uses Lambda functions to process uploaded files in an S3 bucket. They notice that files above 6 MB are sometimes failing to trigger the Lambda.

What is the cause, and how can it be fixed?

A) S3 event notification size limit exceeded; use Amazon SQS as an event source for Lambda for large files  
B) Lambda function timeout set too low; increase timeout setting  
C) Lambda payload size is limited; use Amazon S3 event notifications with Amazon SNS to invoke Lambda indirectly  
D) File size exceeds Lambda deployment package size limit

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** C

**Explanation:**  
Lambda has a payload size limit for direct invocation (~6 MB via S3 event). Large files cause invocation failures. Using Amazon SNS or SQS as an intermediary for S3 event notifications allows Lambda to process large payloads because Lambda can retrieve the file directly from S3, bypassing the size limit.

</details>

---

### Question 15  
An analytics team wants to run interactive queries on datasets stored in Amazon S3 using SQL without managing any infrastructure.

Which AWS service should they use?

A) Amazon Athena  
B) Amazon Redshift  
C) Amazon EMR  
D) AWS Glue

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** A

**Explanation:**  
Amazon Athena is a serverless interactive query service that allows running standard SQL queries directly against data stored in Amazon S3 without managing servers. Redshift is a data warehouse requiring cluster management, EMR is for big data processing with Hadoop/Spark, and Glue is for ETL.

</details>

---

# AWS Certified Cloud Practitioner Advanced Practice Questions (Batch 3)

---

### Question 16  
A company runs a web app on AWS Lambda and wants to track and troubleshoot function errors in near real-time.

Which AWS service provides detailed logs and error metrics to achieve this?

A) AWS CloudTrail  
B) Amazon CloudWatch Logs and CloudWatch Alarms  
C) AWS Config  
D) AWS X-Ray only

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** B

**Explanation:**  
Amazon CloudWatch Logs collects and stores Lambda function logs, while CloudWatch Alarms can notify when error thresholds are exceeded. CloudTrail tracks API calls but not detailed function logs. AWS X-Ray helps with detailed tracing but CloudWatch is the primary tool for logs and metrics.

</details>

---

### Question 17  
An online retailer wants to deploy a multi-tier web application with separation between web, application, and database layers. They also want logical isolation within the AWS environment.

Which AWS service allows them to create isolated networks for each tier while controlling network traffic?

A) Virtual Private Cloud (VPC) with subnets and security groups  
B) AWS IAM roles  
C) AWS Lambda  
D) AWS CloudFront

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** A

**Explanation:**  
Amazon VPC allows creating isolated networks using subnets and routing, while security groups control inbound/outbound traffic at the instance level. IAM roles manage permissions, Lambda is for serverless compute, and CloudFront is a CDN.

</details>

---

### Question 18  
A startup needs to quickly host a static website with high availability and low latency globally with minimal operational overhead.

Which AWS solution should they choose?

A) Amazon EC2 with load balancer  
B) Amazon S3 with CloudFront distribution  
C) AWS Elastic Beanstalk  
D) AWS Lambda with API Gateway

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** B

**Explanation:**  
Hosting static websites in Amazon S3 combined with CloudFront CDN provides high availability, low latency delivery worldwide, and requires minimal management. EC2 and Elastic Beanstalk are more suited for dynamic sites. Lambda/API Gateway is used for serverless APIs.

</details>

---

### Question 19  
A company implements AWS IAM roles to grant EC2 instances permission to access an S3 bucket securely.

Which of the following is the most secure practice?

A) Embed AWS access keys directly in the EC2 instance code  
B) Assign an IAM role with the required S3 permissions to the EC2 instance profile  
C) Use root user credentials to configure access on EC2  
D) Store credentials in environment variables on the EC2 instance

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** B

**Explanation:**  
Assigning an IAM role to the EC2 instance is the most secure method because credentials are managed by AWS automatically and rotated. Embedding credentials or storing root access keys is not secure and violates AWS best practices.

</details>

---

### Question 20  
An organization is concerned about data durability for critical backups stored in Amazon S3. They want to ensure data remains intact even after accidental deletion or corruption.

Which S3 feature provides protection against accidental or malicious data deletion?

A) Versioning and MFA Delete  
B) Server-Side Encryption  
C) Lifecycle Policies  
D) Object Lock in Governance mode

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** A

**Explanation:**  
Enabling S3 Versioning allows retention of object versions, while MFA Delete adds an extra layer requiring multi-factor authentication for delete operations, protecting against accidental/malicious deletes. Server-side encryption protects data confidentiality, lifecycle policies manage storage class transitions, and object lock enforces retention, but Versioning + MFA Delete is key here.

</details>

---

### Question 21  
A company wants to automate cost optimization by identifying underutilized EC2 instances and receive recommendations on instance rightsizing.

Which AWS service covers this requirement?

A) AWS Trusted Advisor  
B) AWS Cost Explorer  
C) AWS Config  
D) AWS CloudWatch

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** A

**Explanation:**  
AWS Trusted Advisor provides best-practice recommendations, including identifying underutilized EC2 instances and offering cost optimization tips. Cost Explorer tracks and analyzes spending but does not give rightsizing recommendations. Config monitors compliance, CloudWatch monitors performance.

</details>

---

### Question 22  
A company wants to migrate an on-premises MySQL database to AWS with minimal downtime and continuous replication.

Which AWS service should they use?

A) AWS Database Migration Service (DMS) with CDC enabled  
B) Amazon RDS snapshot restore  
C) AWS DataSync  
D) AWS Snowball

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** A

**Explanation:**  
AWS DMS supports continuous data replication using change data capture (CDC), enabling minimal downtime database migration. Snapshot restore implies downtime. DataSync is for file transfer. Snowball is for bulk physical data transfer.

</details>

---

### Question 23  
A company hosts APIs on Amazon API Gateway integrated with Lambdas. They want to protect the APIs from common web exploits and bot traffic.

Which AWS service should be used to address this?

A) AWS Shield Advanced  
B) AWS WAF (Web Application Firewall)  
C) Amazon Inspector  
D) AWS CloudTrail

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** B

**Explanation:**  
AWS WAF provides customizable rules to filter and block malicious web requests and bot traffic. Shield Advanced protects against DDoS attacks broadly. Inspector is for vulnerability assessments. CloudTrail logs API activity.

</details>

---

### Question 24  
A healthcare provider needs to ensure all their AWS data at rest meets regulatory requirements to encrypt data using customer-controlled keys.

Which AWS feature allows full control over encryption keys?

A) AWS KMS Customer Managed Keys (CMKs)  
B) Amazon S3 Server-Side Encryption (SSE-S3)  
C) AWS Secrets Manager  
D) AWS Certificate Manager

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** A

**Explanation:**  
Customer Managed Keys in AWS KMS provide customers full control over key creation, usage permissions, rotation policies, and lifecycle, enabling compliance needs. SSE-S3 uses AWS-managed keys and offers less control. Secrets Manager manages secrets; Certificate Manager manages certificates.

</details>

---

### Question 25  
A company wants to continuously monitor their AWS environment for unexpected changes to resource configurations and evaluate compliance with rules.

Which AWS service should they implement?

A) AWS CloudTrail  
B) AWS Config  
C) AWS CloudWatch Events  
D) AWS Trusted Advisor

<details>
<summary>Show Answer & Explanation</summary>

**Correct Answer:** B

**Explanation:**  
AWS Config continuously monitors resource configurations, records changes, evaluates compliance with pre-defined rules, and provides audit trails. CloudTrail logs API calls, CloudWatch Events enable event-driven actions, Trusted Advisor provides best practice checks.

</details>

---

# (More question batches can be generated on your request)


