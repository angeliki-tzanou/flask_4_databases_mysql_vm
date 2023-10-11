## MySQL Setup process on Azure and GCP Virtual Machines:
### Azure Setup:
- First, login into your Azure account dashboard
- Then you can search through the Compute Engine, Virtual Machine instances
- When creating a new virtual machine instance can choose the configurations best fit for the situation
  - In this case, the most affordable plan selections were chosen such as the smallest VM size etc.
- A username and password authentication system was also integrated and created
- In the inbound port rules all options were checked which included HTTP, HTTPS, SSH
- Before deploying the VM the option of enabling auto-shutdown is provided in which we can choose the best time for the VM to shutdown based on its utilization (in this case it was set for 11:59pm)
- Lastly, when we are satisfied with the overview of the information that was used to create the VM we ca de[ploy the VM instance
- Deployment could take a couple of minutes to complete.
