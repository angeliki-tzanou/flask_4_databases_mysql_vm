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

<img width="1000" alt="Screenshot 2023-10-11 at 11 39 26 PM" src="https://github.com/angeliki-tzanou/flask_4_databases_mysql_vm/assets/141374140/5c033a63-8c14-46a0-932d-1dbc1cc839b8">
    
***Similar steps and the same information were imported within the GCP platform to create a VM on there as well***

Below is the screenshot of the GCP VM deployed:

<img width="1000" alt="Screenshot 2023-10-11 at 11 36 51 PM" src="https://github.com/angeliki-tzanou/flask_4_databases_mysql_vm/assets/141374140/2a2b9c81-0bd6-4f02-a282-06fa222743b8">
