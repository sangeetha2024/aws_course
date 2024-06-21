### <h1>Overview of EC2</h1>
<details>
<summary><h3>Elastic Compute Cloud (EC2)<h3></summary>
EC2 is a web service that provides resizable compute capacity in the cloud, allowing for easy scalability and flexibility. It enables running applications without the need to invest in hardware upfront and allows scaling capacity up or down as needed.
</details>
<details>
<summary><h3>Key Concepts</summary>
<b>Instances: Virtual servers running applications.</b>
AMI (Amazon Machine Image): A template that includes the software configuration (OS, application server, applications) required to launch an instance.

Instance Types: Various configurations of CPU, memory, storage, and networking capacity.

Regions and Availability Zones: Data centers located in different geographical areas to ensure low latency and high availability.
</details>
<details>
<summary><h3>Instance Types</summary>
General Purpose: Balanced resources for diverse workloads (e.g., T3, M5).

Compute Optimized: High-performance processors for compute-intensive tasks (e.g., C5, C6g).

Memory Optimized: For memory-intensive applications (e.g., R5, X1).

Storage Optimized: High, sequential read/write access to large data sets (e.g., I3, D2).

Accelerated Computing: Using hardware accelerators or co-processors (e.g., P3, G4).
</details>
<details>
<summary><h3>Purchasing Options</summary>
On-Demand Instances: Pay by the second, no long-term commitments, suitable for short-term, unpredictable workloads.

Reserved Instances: Significant discount (up to 75%) for committing to a 1 or 3-year term.

Spot Instances: Up to 90% discount for using unused EC2 capacity, can be interrupted.

Dedicated Hosts: Physical servers dedicated for your use, can help reduce costs by using existing server-bound software licenses.

Savings Plans: Flexible pricing model offering significant savings over On-Demand instances in exchange for a commitment to a consistent amount of usage (measured in $/hour) for a 1 or 3-year term.

</details>
<details>
<summary><h3>Networking</summary>
VPC (Virtual Private Cloud): Isolated network to launch AWS resources.

Security Groups: Virtual firewall to control inbound and outbound traffic to instances.

Elastic IPs: Static IPv4 addresses designed for dynamic cloud computing.
</details>
<details>
<summary><h3>Storage</summary>
EBS (Elastic Block Store): Block-level storage volumes for use with EC2 instances. Types include:

General Purpose SSD (gp2, gp3)

Provisioned IOPS SSD (io1, io2)

Throughput Optimized HDD (st1)

Cold HDD (sc1)

Instance Store: Temporary block-level storage for instances.

EFS (Elastic File System): Scalable file storage for use with EC2 instances.

S3 (Simple Storage Service): Object storage service providing scalability, data availability, security, and performance.
</details>
<details>
<summary><h3>Security and Management</summary>
IAM (Identity and Access Management): Manage access to AWS resources securely.

EC2 Key Pairs: Secure login information for your instances.

EC2 Auto Scaling: Automatically adjusts the number of instances to handle the load.

CloudWatch: Monitoring service for AWS resources and applications.

Elastic Load Balancing (ELB): Distributes incoming application traffic across multiple targets.
</details>
<details>
<summary><h3>Best Practices</summary>
Right-sizing: Choose the correct instance type and size based on workload requirements to optimize performance and cost.

Security: Implement least privilege access, regularly update and patch instances, and use security groups and network
 ACLs effectively.

Automation: Use Auto Scaling, Elastic Beanstalk, and AWS Lambda for automated 

Monitoring and Logging: Use CloudWatch for monitoring and AWS CloudTrail for logging API activity.

Cost Management: Use AWS Cost Explorer, Trusted Advisor, and Budget to monitor and optimize costs.

</details>
<details>
<summary><h3>Additional Services Integration</summary>

RDS (Relational Database Service): Managed relational database service integrating with EC2.

Lambda: Serverless compute service that triggers code based on events.

Elastic Beanstalk: PaaS that makes it easy to deploy and manage applications.

EKS (Elastic Kubernetes Service): Managed Kubernetes service running on EC2.
</details>

 # EC2 MCQS

## 1. Which of the following is a primary advantage of using AWS Lambda?

- A) Persistent connections
- B) Reduced latency for long-running processes
- C) Automatic scaling and payment based on compute time used
- D) Customizable hardware configurations

<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red; font-weight: bold;">Answer: C) Automatic scaling and payment based on compute time used</p>
</details>

## 2. Which of the following instance types would be most suitable for a web application that requires consistent baseline performance?

- A. T3
- B. M5
- C. C5
- D. R5

<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: A. T3</p>
  <p style="color: black;">Explanation: T3 instances provide a baseline level of CPU performance with the ability to burst when needed, making them suitable for applications with consistent baseline usage like web servers.</p>
</details>


### 3. What feature of AWS EC2 allows users to temporarily increase CPU capacity beyond the baseline for burstable workloads?
A) Auto Scaling
B) Reserved Instances
C) Spot Instances
D) Burstable Performance Instances
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: D) Burstable Performance Instances</p>
</details>

### 4. Which AWS service provides the ability to predictably control and manage costs for EC2 instances?
A) AWS Lambda
B) AWS Budgets
C) AWS Cost Explorer
D) AWS CloudFormation
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: B) AWS Budgets</p>
</details>


### 5. For applications that require the lowest cost per compute ratio, which EC2 purchasing option is most suitable?
A) On-Demand Instances
B) Reserved Instances
C) Spot Instances
D) Dedicated Hosts
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: C) Spot Instances</p>
</details>


### 6. Which of the following storage options is NOT directly associated with EC2 instances?
A) Amazon EBS
B) Amazon S3
C) Instance Store
D) Amazon EFS
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: B) Amazon S3</p>
</details>

#### 7. Which EC2 instance type is designed for applications that require high-performance computing using dedicated hardware?
A) T3
B) M5
C) C5
D) F1
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: D) F1</p>
</details>

### 8. What is the primary difference between On-Demand Instances and Reserved Instances?
A) On-Demand Instances offer lower costs.
B) Reserved Instances require no upfront payment.
C) On-Demand Instances provide flexibility without long-term commitments.
D) Reserved Instances guarantee availability during peak times.
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: C) On-Demand Instances provide flexibility without long-term commitments.</p>
</details>

9. Which EC2 instance type is optimized for applications that require a balance of compute, memory, and network resources?
A) M5
B) C5
C) R5
D) X1
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: A) M5</p>
</details>

### 10. Which of the following is a benefit of using Amazon EBS (Elastic Block Store) with EC2 instances?
A) High-performance, flash-based storage
B) Cost-effective, long-term storage
C) Near-zero latency access for all workloads
D) Unlimited storage capacity
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: A) High-performance, flash-based storage</p>
</details>

11. Which feature of EC2 allows users to save costs by leveraging unused EC2 capacity?
A) Reserved Instances
B) On-Demand Instances
C) Spot Instances
D) Dedicated Hosts
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: C) Spot Instances</p>
</details>

12. Which of the following is true about Amazon EC2 Auto Scaling?
A) It helps reduce network latency for EC2 instances.
B) It automatically adjusts the number of EC2 instances in a fleet based on demand.
C) It provides dedicated physical servers for EC2 instances.
D) It offers guaranteed access to EC2 instances during peak times.
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: B) It automatically adjusts the number of EC2 instances in a fleet based on demand.</p>
</details>

13. Which EC2 instance type is suitable for memory-intensive applications, databases, and distributed memory caches?
A) T3
B) M5
C) R5
D) X1
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: C) R5</p>
</details>

14. What is an Availability Zone in the context of Amazon EC2?
A) A geographic location with multiple isolated data centers for high availability.
B) A software-defined network overlay for EC2 instances.
C) A type of EC2 instance with enhanced networking capabilities.
D) A data storage option for EC2 instances.
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: A) A geographic location with multiple isolated data centers for high availability.</p>
</details>

15. Which AWS service can be used to automate the deployment, scaling, and management of EC2 instances?
A) AWS Lambda
B) AWS CloudFormation
C) AWS Step Functions
D) AWS Elastic Beanstalk
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: B) AWS CloudFormation</p>
</details>

16. Which EC2 instance purchasing option provides the highest level of cost savings for predictable workloads with steady state usage?
A) On-Demand Instances
B) Reserved Instances
C) Spot Instances
D) Dedicated Hosts
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: B) Reserved Instances</p>
</details>

17. What is an EC2 instance profile used for?
A) To specify the AWS region where an EC2 instance should be launched.
B) To define the hardware configuration (CPU, memory, etc.) of an EC2 instance.
C) To define the networking configuration (VPC settings, subnets, security groups) of an EC2 instance.
D) To grant permissions to an EC2 instance to access AWS resources.
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: D) To grant permissions to an EC2 instance to access AWS resources.</p>
</details>

18. Which of the following is NOT a type of Amazon Machine Image (AMI) used with EC2 instances?
A) Public AMI
B) Custom AMI
C) Shared AMI
D) Private AMI
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: C) Shared AMI</p>
</details>

19. What is an Elastic IP address in the context of Amazon EC2?
A) A static IPv4 address designed for dynamic cloud computing.
B) An IP address that automatically scales with EC2 instance size.
C) An IP address used for internal communication between EC2 instances.
D) An IP address reserved for high-performance EC2 instances.
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: A) A static IPv4 address designed for dynamic cloud computing.</p>
</details>

20. Which EC2 instance type is optimized for compute-intensive applications requiring high performance from processors?
A) T3
B) M5
C) C5
D) P3
<details>
  <summary>Click to reveal answer</summary>
  <p id="answer" style="color: red;">Answer: D) P3</p>
</details>