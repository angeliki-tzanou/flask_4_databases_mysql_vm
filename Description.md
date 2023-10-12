## MySQL Setup process on Azure and GCP Virtual Machines:
### Azure Setup:
- First, login into your Azure account dashboard
- Then you can search through the Compute Engine, Virtual Machine instances
- When creating a new virtual machine instance can choose the configurations best fit for the situation
  - In this case, the most affordable plan selections were chosen such as the smallest VM size etc.
- A username and password authentication system was also integrated and created
- In the inbound port rules all options were checked which included HTTP, HTTPS, SSH
- Before deploying the VM the option of enabling auto-shutdown is provided in which we can choose the best time for the VM to shutdown based on its utilization (in this case it was set for 11:59pm)
- Lastly, when we are satisfied with the overview of the information that was used to create the VM we can deploy the VM instance
- Deployment could take a couple of minutes to complete.
- Then we can go to resource groups and find our deployed VM instance and search for its characteristics
  - Ex: IP address, activity log/status, the username of the VM to be used for purposes such as connecting in SQLworkbench etc.
  - In this case, before proceeding we ensured that our destination port ranges under the inbound security rule, was set to 3306 to connect openly to our workbench
    
***Similar steps and the same information were imported within the GCP platform to create a VM on there as well***
