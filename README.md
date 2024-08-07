# Assignment
Case Studay for Cloud Migration 
The example  has 8 major applications that power their business. It is today managed and supported by  IT departments from 3rd party managed services providers across the world.
1. E-commerce application built on a Java J2ee stack
2. Customer information management system to design and deliver campaigns
3. FE Apps - Retail store applications – .Net based application
4. BES Backend systems on Linux + Weblogic + Oracle
5. Middleware application with Mule ESB
6. Mobile app built on Android and IOS – B2C and B2B
7. Big Data and analytics on Azure cloud
8. CRM using Salesforce

As An architect on this project, the expectation is that we will draft the entire cloud migration strategy for this project. & move their entire workload from the existing physical DC to Amazon AWS.

**Migration Strategy
1. ##Assessment and Planning
    - Inventory Analysis**: Detailed assessment of all applications, dependencies, and current infrastructure.
    - Cloud Readiness**: Evaluate each application's cloud readiness.
    - Risk Assessment**: Identify potential risks and mitigation strategies.
    - Compliance and Security**: Ensure adherence to industry regulations and security best practices.

2. ##Infrastructure Design
    - High Availability**: Use AWS services like EC2, RDS, and ECS/EKS to ensure high availability.
    - Disaster Recovery**: Implement cross-region backups and disaster recovery plans using AWS Backup and AWS Disaster Recovery.
    - Scalability**: Use AWS Auto Scaling and Elastic Load Balancing for dynamic scaling.
    - Cost Management**: Use AWS Cost Explorer and Reserved Instances for cost optimization.

3. ##Migration Phases
    - Proof of Concept (PoC)**: Begin with a PoC for non-critical applications to validate migration strategies.
    - Pilot Migration**: Migrate a small set of critical applications.
    - Full Migration**: Execute a phased migration for all remaining applications.

### Application-Specific Migration Plans
1. #E-commerce Application**
    - Services**: AWS EC2, AWS RDS (for database), Amazon S3 (for static content), and Amazon CloudFront (for CDN).
    - Migration Technique**: Rehosting (Lift-and-Shift) followed by optimization.

2. #Customer Information Management System**
    - Services**: AWS EC2, Amazon RDS, AWS Lambda (for campaign execution), and Amazon SES (for email services).
    - Migration Technique**: Replatforming to leverage managed services.

3. #Retail Store Applications**
    - Services**: AWS Elastic Beanstalk (for .NET), Amazon RDS.
    - Migration Technique**: Replatforming.

4. #BES Backend Systems**
    - Services**: AWS EC2 (for Linux instances), Amazon RDS (for Oracle databases), AWS CloudFormation (for infrastructure as code).
    - Migration Technique**: Rehosting with gradual rearchitecting.

5. #Middleware Application**
    - Services**: AWS EC2 (for Mule ESB), Amazon SQS (for messaging).
    - Migration Technique**: Rehosting.

6. #Mobile Apps**
    - Services**: AWS Amplify (for front-end hosting), AWS Lambda (for serverless backend), Amazon Cognito (for user authentication).
    - Migration Technique**: Rebuild to optimize for cloud-native architecture.

7. #Big Data and Analytics**
    - Services**: AWS Redshift, AWS Glue, Amazon Athena, and Amazon S3.
    - Migration Technique**: Data transfer from Azure to AWS, rearchitecting analytics pipeline.

8. #CRM
    - Services**: Integrate Salesforce with AWS using Amazon AppFlow.
    - Migration Technique**: Integrate without migration.
  
### Security and Compliance
- Identity and Access Management (IAM)**: Implement least privilege access using AWS IAM.
- Data Encryption**: Encrypt data at rest and in transit using AWS KMS.
- Compliance**: Ensure compliance with industry standards (e.g., GDPR, HIPAA).

### Cost Management
- Cost Optimization**: Use AWS Cost Explorer, Reserved Instances, and Savings Plans.
- Monitoring**: Use AWS CloudWatch for monitoring and AWS Budgets for cost tracking.

