# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

I would choose an App Service as there is not much customization needed for the
application. In terms of scalability, as the application is light weight, the scalability options
under App Service is sufficient to host our application. For availability, App Service provides
horizontal scaling to ensure services are running even if one of the nodes is down. App 
Service also supports CI/CD from git, which is suitable as we are developing this code using on github.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

If there is a requirement to customize the application (i.e. security, features) at the OS level, 
we might have to switch to VM as it allows better customization, and if compute requirements increases
with the increase in concurrent users, then switching to VM is better due to its higher scalability
than App Services.