# 5. Core Services

## 5.1 Compute
- **EC2 (Elastic Compute Cloud)**: Virtual servers in the cloud with various instance types optimized for different workloads. Pricing options include:
  - On-Demand
  - Reserved
  - Spot
  - Savings Plans
- **Lambda**: Serverless function execution with event-driven compute service for code without provisioning servers. It offers pay-per-millisecond pricing and automatic scaling.
- **ECS (Elastic Container Service)**: Container orchestration with EC2 or Fargate hosting options.
- **EKS (Elastic Kubernetes Service)**: Managed Kubernetes service with EC2 or Fargate hosting options.
- **Fargate**: Serverless compute for containers, eliminating the need to provision and manage servers.
- **Elastic Beanstalk**: PaaS for web applications with automated deployment and scaling.
- **Lightsail**: Simplified VPS service with low, predictable monthly pricing.

## 5.2 Storage
- **S3 (Simple Storage Service)**: Object storage service with unlimited scalability and various storage classes optimized for different access patterns. Examples include:
  - **S3 Standard**: For frequent access with the highest availability (99.99%).
  - **S3 Intelligent-Tiering**: For unknown or changing access patterns.
  - **S3 Standard-IA**: For infrequent access with multiple AZ redundancy.
  - **S3 One Zone-IA**: For infrequent access with single AZ (99.5% availability).
  - **S3 Glacier**: For archive storage with retrieval times from minutes to hours.
  - **S3 Glacier Deep Archive**: For the lowest cost with retrieval time of hours.
- **EBS (Elastic Block Store)**: Persistent block storage for EC2 with volume types optimized for different workloads.
- **EFS (Elastic File System)**: Fully managed NFS file system with elastic capacity and shared access from multiple EC2 instances.
- **Glacier**: Archive storage service with extremely low-cost storage for data archiving.
- **Storage Gateway**: Hybrid cloud storage service with:
  - File Gateway
  - Volume Gateway
  - Tape Gateway
- **Snowball/Snowball Edge**: Physical data transfer devices for large data migrations, disaster recovery, and datacenter decommission.

## 5.3 Databases
- **RDS (Relational Database Service)**: Managed relational database service with support for:
  - MySQL
  - PostgreSQL
  - MariaDB
  - Oracle
  - SQL Server
- **DynamoDB**: Managed NoSQL database service with single-digit millisecond latency at any scale.
- **Aurora**: MySQL and PostgreSQL-compatible relational database with high throughput and storage autoscaling.
- **Redshift**: Data warehousing service optimized for analytics with petabyte-scale capacity.
- **ElastiCache**: In-memory caching service compatible with:
  - Redis
  - Memcached
- **DocumentDB**: MongoDB-compatible document database.
- **Neptune**: Graph database service optimized for complex connected data.
- **Keyspaces**: Apache Cassandra-compatible database.
- **Timestream**: Time series database for IoT and operational metrics.
- **QLDB (Quantum Ledger Database)**: Immutable transaction log with cryptographically verifiable transaction history.

## 5.4 Networking
- **VPC (Virtual Private Cloud)**: Isolated network environment with:
  - Subnets
  - Route tables
  - Internet gateways
  - NAT gateways
  - Security groups -> default deny
  - NACLs -> default allow
  - VPC peering
  - VPC endpoints
- **Route 53**: Scalable Domain Name System (DNS) service with:
  - Domain registration
  - DNS routing
  - Health checking
  - Routing policies
- **CloudFront**: Global content delivery network (CDN) with edge locations worldwide for content caching.
- **API Gateway**: Create, publish, and manage APIs with:
  - RESTful APIs
  - WebSocket APIs
- **Direct Connect**: Dedicated network connection to AWS with consistent network performance and reduced bandwidth costs.
- **ELB (Elastic Load Balancing)**: Distributes incoming traffic with:
  - ALB (Application Load Balancer)
  - NLB (Network Load Balancer)
  - GLB (Gateway Load Balancer)
  - Classic Load Balancer

## 5.5 Management and Governance
- **CloudWatch**: Monitoring and observability service with:
  - Metrics
  - Logs
  - Events
  - Alarms
  - Dashboards
- **CloudTrail**: Track user activity and API usage with governance, compliance, and audit capability.
- **Config**: Resource inventory, configuration history, and change notifications with automated compliance checking.
- **Trusted Advisor**: Real-time guidance to provision resources with:
  - Cost optimization
  - Performance
  - Security
  - Fault tolerance
  - Service limits checks
- **Systems Manager**: Operations management service with:
  - Automation
  - Run command
  - Session manager
  - Patch manager
  - Parameter store
- **Organizations**: Account management and consolidation with centralized management of multiple AWS accounts.
- **Control Tower**: Set up and govern a secure, multi-account environment with:
  - Landing zone
  - Guardrails
  - Account factory
- **License Manager**: Manage software licenses across AWS and on-premises.
