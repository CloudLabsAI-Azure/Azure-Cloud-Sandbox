# Azure Cloud Sandbox



## About the Sandbox Environment

### **Sandbox Environment Resource Details**

| **Resources** | **Value / Scope** | **SKU** | **Remarks** |
| --- | --- | --- | --- |
| **Azure Storage Account (Blob Storage)** | 1. Allow create & delete buckets.<br>2. Allow upload and delete objects.<br>3. Allowed Features: Enable bucket versioning, Enable event notifications.<br>4. Storage Size: Minimum 1 GB. | **Allowed All SKUs** | Full control for storage-related operations within defined limits. |
| **Azure SQL Database** | 1. Allow create, update, and delete database instance.<br>2. Database Engine: **MS SQL Server**.<br>3. Instance Size: As per standard configuration.<br>4. Storage: 20 GB.<br>5. Availability Zone: Single AZ.<br>6. Allowed Regions: Standard regions only. | **Allowed all except** `Hyperscale`, `BusinessCritical`, `Premium` | Limited to standard SQL SKUs for cost and performance optimization. |
| **Virtual Machine (VM)** | 1. Allow launch and terminate instances.<br>2. Instance Type: Free-tier eligible.<br>3. Volume: 30 GB (General Purpose SSD). | **Allowed SKUs:**<br>`Standard_D2s_v3`, `Standard_B2s`, `Standard_B2ms`, `Standard_DS2_v2`, `Standard_D2as_v4`, `Standard_D4s_v3`, `Standard_B4ms`, `Standard_DS3_v2`, `Standard_D4as_v4`, `Standard_B1s`, `Standard_B1ls` | Only listed SKUs are permitted. All others restricted. |
| **Identity and Access Management (IAM)** | 1. IAM User Creation: Limited to Read-Only.<br>2. IAM Role Creation: Limited to defined services.<br>3. Read Access to IAM Console.<br>4. Create RBAC roles and policies. | N/A | Access limited to predefined roles and scopes. |
| **Virtual Network (VNet)** | 1. Allow Create, Update, and Delete VNet and associated resources.<br>2. Allow creation of Default VNet and Subnets.<br>3. Allow configuration of Inter-Region Peering. | N/A | Full network configuration within defined subscription scope. |
| **App Service** | 1. Create App Service for full-stack .NET applications.<br>2. Connect to SQL Server Database.<br>3. Deploy .NET App with App Insights enabled.<br>4. Environment setup via both CLI and Portal. | **All SKUs Allowed** | Full deployment and monitoring permissions. |
| **Azure Monitor** | 1. Allow creation of 1 Dashboard and 1 Alert.<br>2. Monitor App Service, Database, and VM instances. | Allowed | Limited monitoring resources to observe deployed services. |
| **Key Vault** | Create and remove key pairs. | **Allowed All SKUs** | Key management supported for encryption and secrets. |
| **Azure Functions** | Create, edit, and delete multiple Azure Functions with public endpoints and triggers. | **Allowed All SKUs** | Serverless compute allowed for development purposes. |
| **Azure DevOps Organizations** | Access to Azure Boards for project planning. | Allowed | DevOps project tracking and board setup permitted. |
| **Azure Entra ID User** | Pre-created Entra ID user account | NA |You will receive one Entra ID user account for authentication and access management. |
| **Azure Subscription Permissions** | Reader role privilege over Azure Subscription | NA |You will get Reader role access on the Azure Subscription. |
|**VM Idle Start/Stop**|The virtual machine is set up with a custom feature called Idle start/stop. This custom package will check the virtual machine's idleness every 2 hours/120 minutes. | NA | If the virtual machine is left idle for over 2 hours, a pop-up window will appear, prompting you to respond. If you do not act within 15 minutes, the virtual machine will shut down automatically.This feature is enabled for virtual machines to optimize Azure costs.|
| **Azure Credit** | 20 USD | NA | A consumption limit of 20 USD is applied to manage Azure spending. |
| **Credit Alerts** | Credit Alerts are set on consumption of 50%, 75%, 90%, 95%, and 100% of total Azure credits. | NA |Check your registered email inbox for credit alert notifications to manage your Azure usage effectively. |
| **Sandbox Duration** | 7 Days / 168 Hours or until Azure Consumption Credits are exhausted | NA |The sandbox environment will be automatically deleted after 10 days or when credits are fully utilized, whichever occurs first. |


## Notes:
* The Azure credit consumption includes all the resources which you will be deploying while using the sandbox environment for your use case. 
* You will have **Reader** privilege access on Azure Subscription, you can freely explore the features of required services and are recommended to use it only for learning purposes. 
* As each sandbox environment has a fixed budget/cap of $20 USD, Sandbox as they can consume the Azure credit leading to the automatic deallocation of the Sandbox as soon as the credit limit is reached.  

## Cost Monitoring:
To monitor and analyse your Azure credit spend, you can navigate to the Azure Subscription page by following the steps mentioned below.
+ From the Azure portal home page, search for **Subscriptions (1)** using the search bar and select the same from the suggestions.
  
  ![](media/subscription-01.jpg)
  
+ Select the Cost Analysis tab from the Cost Management pane. You can access a comprehensive breakdown of your Azure spending, offering a granular view of costs associated with various services, and resources. To get the accurate consumed cost by you, select the **Calendar (2)** from **Cost analysis (1)**  then **Custom date Range (3)**.

   ![](media/costanlysis.png)

+ Now, select the custom dates.
    + **Start Date: (1)** The date when you redeemed voucher and launch the Sandbox environment.
    + **End Date: (2)** Current or future date. If you select the future date, you can also get the forecasted cost based on the current resources you deployed.
    + You can see the **ACTUAL COST (USD) (4)** and the **FORECAST: CHART VIEW ON (5)** cost.

   ![](media/costanylysis-02.png)

## Best Practices:
+ **Resources usage:** Please stop the virtual machines, WebApps, Azure Kubernetes service, Azure Container Instance and other resources when not in use to minimize the Azure spend.
+ **Azure Cost Analysis:** Maintain a practice of regularly checking the Cost Analysis report for the assigned Azure subscription to ensure the sustainability of the environment over an extended period.
+ **Alert notifications:** Make sure to check your registered email's inbox for any alert-related emails. Alerts give you can head start to keep your Azure spending in control and to plan out the remaining credits in the best way possible.

## Common Troubleshooting

Here are few common issues and fix which you might encounter while performing the lab.

- VM Remote connection issue: RDP: [Known Functionality Issues | CloudLabs Documentation](https://docs.cloudlabs.ai/Learner/Troubleshooting/RDP/)

- Copy Paste Issue: [Copy Paste | CloudLabs Documentation](https://docs.cloudlabs.ai/Learner/Troubleshooting/CopyPaste/)

## CloudLabs Support Contacts:
You can reach out to the support team in case you face any difficulty in using the sandbox environment, any permission, or Azure consumption-related queries.

* Sandbox user Email Support:  cloudlabs-support@spektrasystems.com
* Sandbox user Live Chat Support: https://cloudlabs.ai/ms-support



