### Overview of EC2
<details>
<summary>Elastic Compute Cloud (EC2)</summary>
EC2 is a web service that provides resizable compute capacity in the cloud, allowing for easy scalability and flexibility. It enables running applications without the need to invest in hardware upfront and allows scaling capacity up or down as needed.
</details>
<details>
<summary>Key Concepts</summary>
Instances: Virtual servers running applications.

AMI (Amazon Machine Image): A template that includes the software configuration (OS, application server, applications) required to launch an instance.

Instance Types: Various configurations of CPU, memory, storage, and networking capacity.

Regions and Availability Zones: Data centers located in different geographical areas to ensure low latency and high availability.
</details>
<details>
<summary>Instance Types</summary>
General Purpose: Balanced resources for diverse workloads (e.g., T3, M5).
Compute Optimized: High-performance processors for compute-intensive tasks (e.g., C5, C6g).
Memory Optimized: For memory-intensive applications (e.g., R5, X1).
Storage Optimized: High, sequential read/write access to large data sets (e.g., I3, D2).
Accelerated Computing: Using hardware accelerators or co-processors (e.g., P3, G4).
</details>
<details>
<summary>Purchasing Options</summary>
On-Demand Instances: Pay by the second, no long-term commitments, suitable for short-term, unpredictable workloads.
Reserved Instances: Significant discount (up to 75%) for committing to a 1 or 3-year term.
Spot Instances: Up to 90% discount for using unused EC2 capacity, can be interrupted.
Dedicated Hosts: Physical servers dedicated for your use, can help reduce costs by using existing server-bound software licenses.
Savings Plans: Flexible pricing model offering significant savings over On-Demand instances in exchange for a commitment to a consistent amount of usage (measured in $/hour) for a 1 or 3-year term.
</details>
<details>
<summary>Networking</summary>
VPC (Virtual Private Cloud): Isolated network to launch AWS resources.

Security Groups: Virtual firewall to control inbound and outbound traffic to instances.

Elastic IPs: Static IPv4 addresses designed for dynamic cloud computing.
</details>
<details>
<summary>Storage</summary>
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
<summary>Security and Management</summary>
IAM (Identity and Access Management): Manage access to AWS resources securely.

EC2 Key Pairs: Secure login information for your instances.

EC2 Auto Scaling: Automatically adjusts the number of instances to handle the load.

CloudWatch: Monitoring service for AWS resources and applications.

Elastic Load Balancing (ELB): Distributes incoming application traffic across multiple targets.
</details>
<details>
<summary>Best Practices</summary>
Right-sizing: Choose the correct instance type and size based on workload requirements to optimize performance and cost.
Security: Implement least privilege access, regularly update and patch instances, and use security groups and network ACLs effectively.
Automation: Use Auto Scaling, Elastic Beanstalk, and AWS Lambda for automated 
</details>
<details>
<summary></summary>
Monitoring and Logging: Use CloudWatch for monitoring and AWS CloudTrail for logging API activity.
Cost Management: Use AWS Cost Explorer, Trusted Advisor, and Budget to monitor and optimize costs.
</details>
<details>
<summary>Additional Services Integration</summary>

RDS (Relational Database Service): Managed relational database service integrating with EC2.

Lambda: Serverless compute service that triggers code based on events.

Elastic Beanstalk: PaaS that makes it easy to deploy and manage applications.

EKS (Elastic Kubernetes Service): Managed Kubernetes service running on EC2.
</details>