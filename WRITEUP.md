### Analyze, choose, and justify the appropriate resource option for deploying the app.

- App service: Only be responsible for developing part of the project and deploying code. It is useful for teams with less members and less experience hardware. Azure service is simple, quick, and easy for deploying web apps.

- Virtual machine: It provides on-premises hardware, we have no need to take care of the physical security of the machine or manage them. We have responsibilities for creating middleware, enviroments, and dependencies for our apps to run. VM is more expensive than Azure App Service to run.

For this current state of this app, I can use app services to make use of the advantages of this. If the app has scope to expand in the future, I prefer Azure VMs. VMs are more secure than Azure App Service. There are also some limitations in support of programming languages in Azure App Service.

### Assess app changes that would change your decision.

- If the app need to scale up in the future.
- The app is storing a huge user's data.
- The app performance is much more important.

Demonstrations are in images_evident folder.
The code has been changed to adapt to “Sign in with Microsoft”.

Live website: http://20.205.113.241/
App service: http://myappservicename.azurewebsites.net/
