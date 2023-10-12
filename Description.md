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


### Then going into Google Shell followed the commands below:
1. First ensure that our UBUNTU server is up to date by using the command ```sudo apt-get update``` to update it
2. ```sudo apt install mysql-server mysql-client``` in order to install MYSQL into google shell
3. In order to log into the SQL account used ```sudo mysql```
4. At this point, created a new user by using the command ```CREATE USER 'ang2'@'%' IDENTIFIED BY ‘yourPassword’;```

<img width="934" alt="Screenshot 2023-10-11 at 11 52 45 PM" src="https://github.com/angeliki-tzanou/flask_4_databases_mysql_vm/assets/141374140/67e8d881-35e0-429d-9a2d-18e9a65b611b">

- Ensured in google shell that access was granted to the new user and then proceeded:
<img width="1000" alt="successful login1" src="https://github.com/angeliki-tzanou/flask_4_databases_mysql_vm/assets/141374140/0a032884-b120-4e9a-9d05-a7c859ae84c0">

<img width="1000" alt="successful login" src="https://github.com/angeliki-tzanou/flask_4_databases_mysql_vm/assets/141374140/12104304-6e2b-4347-8327-2f1331bc2f76">


5. After successfully linking with my SQL workbench I went ahead and created a database:

<img width="1190" alt="db creation" src="https://github.com/angeliki-tzanou/flask_4_databases_mysql_vm/assets/141374140/6ca68f9b-2a43-4e99-a797-b6edb90aebf8">

6. Then inside that database that I created went ahead and created the two tables:

<img width="1186" alt="table content" src="https://github.com/angeliki-tzanou/flask_4_databases_mysql_vm/assets/141374140/d0e5bd23-3139-4ee4-b948-9f13fa957027">

## ERRORS encountered:
- 



