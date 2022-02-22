### Analyze, choose, and justify the appropriate resource option for deploying the app.

| Aspects       | Azure VM                  | Azure App Service         |
| :------------: |:---------------:          | :----------------------:|
| Pricing       | More expensive.           | Cheaper. For e.g. Basic Tier; |
|               | A1 v2: 1 Cores,           | 1 B1 (1 Core(s), |
|               | 2 GB RAM,                 | 1.75 GB RAM, |
|               | 10 GB Temporary           | 10 GB Storage) x 730 Hours; |
|               | storage, $0.065/hour      | Windows OS |
|               | On average: Monthly: $47.45 | On average: Monthly: $32.12 |
|               | Offer Pay-as-you-go and reserved (with discount) | Don't offer Pay-as-you-Go |
| Scalability   | Scale limit: Platform image: 1000 nodes per scale set, Custom image: 600 nodes per scale set. | Scale limit: 30 instances, 100 with App Service Environment. 14GB of memory and 4 vCPU cores per instance max. Vertical scaling, without having to redeploy.|
| Availability  | 95% of Connectivity is the least      | 99.95% of Available is the least. No SLA is provided for Apps under either the Free or Shared tiers |
| Workflow      | Infrastructure-as-a-Service  | Platform-as-a-Service   |
|               | Focus on applications, data, runtime, middleware, OS| Focus on application and Data   |

- App service: Only be responsible for developing part of the project and deploying code. It is useful for teams with less members and less experience hardware. Azure service is simple, quick, and easy for deploying web apps. App Service have constraints about scalability comparing to Azure VM.

- Virtual machine: It provides on-premises hardware, we have no need to take care of the physical security of the machine or manage them. We have responsibilities for creating middleware, enviroments, and dependencies for our apps to run. VM is more expensive than Azure App Service to run, and also takes more time consuming of developers than App Sercice.

--> For this current state of this app, I can use app services to make use of the advantages of this. If the app has scope to expand in the future, I prefer Azure VMs. VMs are more secure than Azure App Service. There are also some limitations in support of programming languages in Azure App Service.

### Assess app changes that would change your decision.

- If the app need to scale up in the future.
- The app is storing a huge user's data.
- The app performance is much more important.

Demonstrations are in images_evident folder.
The code has been changed to adapt to “Sign in with Microsoft”.

Live website: http://20.205.113.241/
App service: http://myappservicename.azurewebsites.net/
