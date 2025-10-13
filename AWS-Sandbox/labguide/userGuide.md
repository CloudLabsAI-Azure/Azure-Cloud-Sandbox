# AWS Cloud Sandbox

## **About the Sandbox Environment**

| **Resources**                | **Value**                                                                                                                                                                                                                                                                                           | **Remarks**                                                                                                                                                                     |
| ---------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Enabled Services**         | Amazon S3, Amazon RDS (MySQL), Amazon EC2, AWS Identity and Access Management (IAM), Amazon VPC, Amazon DynamoDB, Amazon Elastic Container Registry (ECR), Amazon Elastic Container Service (ECS), Amazon CloudWatch, AWS Key Management Service (KMS), AWS Lambda, AWS CodePipeline, AWS CodeBuild | You will have access to create, modify, and explore the listed AWS services within the defined sandbox limits.                                                                  |
| **AWS IAM User**             | Pre-created IAM user account                                                                                                                                                                                                                                                                        | You will receive one IAM user account for authentication and access to the AWS sandbox environment.                                                                             |
| **AWS Account Permissions**  | Restricted privileges with limited resource creation and administrative access                                                                                                                                                                                                                      | The sandbox environment enforces a predefined permission boundary allowing you to work only with specific services and resource limits. Administrator-level access is disabled. |
| **Region Availability**      | N. Virginia (us-east-1)                                                                                                                                                                                                                                                                             | Most resources and services are available only in the **N. Virginia** region to maintain consistency and compatibility across AWS services.                                     |
| **Resource Limits**          | EC2: Max 2 instances (t2.micro, t3.micro, t3.small, t3.medium, 30 GB gp2/gp3)<br>RDS: 1 instance (MySQL, db.t3.micro, 20 GB)                                                                                                                                                                        | Limits are applied to ensure fair usage and cost optimization across all users in the shared sandbox environment.                                                               |
| **AWS Credits**              | USD 20 equivalent                                                                                                                                                                                                                                                                                   | A credit limit of **USD 20** is applied to control AWS spending within the sandbox environment.                                                                                 |
| **Environment Duration**     | 10 Days / 240 Hours or until AWS Credits are exhausted                                                                                                                                                                                                                                              | The sandbox environment will automatically terminate after **10 days** or once allocated AWS credits are fully utilized, whichever occurs first.                                |
| **Idle Resource Monitoring** | Automated idle monitoring for EC2                                                                                                                                                                                                                                                                   | Idle compute instances (EC2) are automatically stopped after a defined period of inactivity to optimize AWS cost usage.                                                    |                                                                                                                                                                                                                           

### **Best Practices**

- **Resource Usage:**
Ensure to stop or terminate EC2 instances, RDS databases, Lambda functions, and other compute resources when not in use to prevent unnecessary AWS credit consumption. Also, delete unused EBS volumes, snapshots, and Elastic IPs to minimize ongoing costs.

- **AWS Cost Explorer:**
Regularly review your usage and spending through **AWS Cost Explorer** or **Billing Dashboard** to track resource costs and ensure efficient utilization of your sandbox environment over time.

## Common Troubleshooting

Here are few common issues and fix which you might encounter while performing the lab.

- VM Remote connection issue: RDP: [Known Functionality Issues | CloudLabs Documentation](https://docs.cloudlabs.ai/Learner/Troubleshooting/RDP/)

- Copy Paste Issue: [Copy Paste | CloudLabs Documentation](https://docs.cloudlabs.ai/Learner/Troubleshooting/CopyPaste/)

## CloudLabs Support Contacts:
You can reach out to the support team in case you face any difficulty in using the sandbox environment, any permission, or Azure consumption-related queries.

* Sandbox user Email Support:  cloudlabs-support@spektrasystems.com
* Sandbox user Live Chat Support: https://cloudlabs.ai/ms-support
