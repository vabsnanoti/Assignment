# Assignment
Case Studay for Cloud Migration 
This particular example being 8 major applications that drive their business. Nowadays, it gets carried out by IT departments from 3rd party managed services providers throughout the world.
1. E-commerce application built on a Java J2ee stack
2. Customer information management system to design and deliver campaigns
3. FE Apps - Retail store applications – .Net based application
4. BES Backend systems on Linux + Weblogic + Oracle
5. Middleware application with Mule ESB
6. Mobile app built on Android and IOS – B2C and B2B
7. Big Data and analytics on Azure cloud
8. CRM using Salesforce

As An architect on this project, the expectation is that we will draft the entire cloud migration strategy for this project. & move their entire workload from the existing physical DC to Amazon AWS.

Migration Strategy
- Assessment and Planning
1. Analysis of Inventory: Unpacking all apps, dependencies and existing infra
2. Pre-Cloud Readiness: Assess the cloud readiness of each application.
3. Risk Assessment: Identify and respond to risk.
4. Compliance and Security: ensure compliance with industry regulations and security best practices.

- Infrastructure Design
1. High availability —Use AWS services such as EC2, RDS, and ECS/EKS.
2. Backup and DR: The Last step will be to take care of disaster recovery by maintaining cross-region backups using AWS backup service, also implementing a disaster recovery plan on top of that.
3. Auto-scaling: Use an Application Load Balancer with AWS Auto Scaling.
4. Cost Management – Improve your cost visibility, control, and stability using AWS Cost Explorer & Reserved Instances.

- Migration Phases
1. Proof of Concept (PoC): Start with a PoC for non-critical applications to test the migration strategy.
2. Initial Migration: Migrate at a larger scale.

- Application-Specific Migration Plans
1. E-commerce Application
    - Services: AWS EC2, AWS RDS (for database), Amazon S3 (for static content), and Amazon CloudFront (for CDN).
    - Migration Technique: Rehosting (Lift-and-Shift) followed by optimization.

2. Customer Information Management System
    - Services: AWS EC2, Amazon RDS, AWS Lambda (for campaign execution), and Amazon SES (for email services).
    - Migration Technique: Replatforming to leverage managed services.

3. Retail Store Applications
    - Services: AWS Elastic Beanstalk (for .NET), Amazon RDS.
    - Migration Technique: Replatforming.

4. BES Backend Systems
    - Services: AWS EC2 (for Linux instances), Amazon RDS (for Oracle databases), AWS CloudFormation (for infrastructure as code).
    - Migration Technique: Rehosting with gradual rearchitecting.

5. Middleware Application
    - Services: AWS EC2 (for Mule ESB), Amazon SQS (for messaging).
    - Migration Technique: Rehosting.

6. Mobile Apps
    - Services: AWS Amplify (for front-end hosting), AWS Lambda (for serverless backend), Amazon Cognito (for user authentication).
    - Migration Technique: Rebuild to optimize for cloud-native architecture.

7. Big Data and Analytics
    - Services: AWS Redshift, AWS Glue, Amazon Athena, and Amazon S3.
    - Migration Technique**: Data transfer from Azure to AWS, rearchitecting analytics pipeline.

8. CRM
    - Services: Integrate Salesforce with AWS using Amazon AppFlow.
    - Migration Technique: Integrate without migration.
  
##Security and Compliance
- Identity and Access Management (IAM): Implement least privilege access using AWS IAM.
- Data Encryption: Encrypt data at rest and in transit using AWS KMS.
- Compliance: Ensure compliance with industry standards (e.g., GDPR, HIPAA).

### Cost Management
- Cost Optimization: Use AWS Cost Explorer, Reserved Instances, and Savings Plans.
- Monitoring: Use AWS CloudWatch for monitoring and AWS Budgets for cost tracking.

