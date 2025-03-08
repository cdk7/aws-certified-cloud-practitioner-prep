# 7. Cloud Architecture

## 7.1 High Availability Design
- **Multi-AZ deployments**: Replicate across availability zones with:
  - Active-passive or active-active configurations
  - Automated failover for RDS, ElastiCache, etc.
- **Load balancing**: Distribute traffic across multiple targets with:
  - Health checks
  - Auto-scaling groups
- **Auto-recovery**: Automatically recover from instance or hardware failure with:
  - EC2 auto recovery
  - RDS multi-AZ failover

## 7.2 Fault Tolerance
- **Redundant components**: Eliminate single points of failure with:
  - Multiple instances across AZs
  - Multiple network paths
- **Data replication**: Keep multiple synchronized copies of data with:
  - Synchronous (RDS Multi-AZ)
  - Asynchronous (RDS Read Replicas)
- **Failure detection and recovery**: Identify and address failures with:
  - Health checks
  - Automated recovery
  - Graceful degradation

## 7.3 Disaster Recovery
- **RPO (Recovery Point Objective)**: Maximum acceptable data loss.
- **RTO (Recovery Time Objective)**: Maximum acceptable downtime.
- **Strategies**:
  - **Backup and restore**: Lowest cost, highest RPO/RTO with regular backups to S3.
  - **Pilot light**: Core systems running minimally, scaling up when needed.
  - **Warm standby**: Scaled-down but fully functional copy, ready to serve traffic.
  - **Multi-site**: Full production capacity in multiple regions with active-active deployment.

## 7.4 Scalability and Elasticity
- **Horizontal scaling**: Add more instances to increase capacity, distributing load and risk.
- **Vertical scaling**: Increase resources of existing instances, limited by instance size and may require downtime.
- **Auto Scaling**: Automatic adjustment of capacity with:
  - Target tracking
  - Step scaling
  - Scheduled scaling
  - Predictive scaling
- **Load Balancing**: Traffic distribution across multiple targets, improving availability and fault tolerance.

## 7.5 Serverless Architecture
- **No infrastructure management**: Focus on code, not servers, with:
  - Managed runtime environment
  - Automatic scaling
- **Function as a service**: Lambda and Step Functions for event-driven execution with pay-per-use pricing.
- **Event-driven design**: React to events with:
  - SQS
  - SNS
  - EventBridge
  - For event handling and decoupled components
- **Benefits**:
  - Reduced operational complexity
  - Pay-per-use pricing model
  - Automatic scaling to zero
  - Built-in high availability
