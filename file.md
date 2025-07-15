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

# (Continue similarly for remaining questions)
