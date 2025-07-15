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



