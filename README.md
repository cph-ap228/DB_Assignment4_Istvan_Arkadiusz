# DBAssignment4

## Excercise 1 - User Privileges

![picture](https://github.com/FarkIst/DBAssignment4/blob/master/img/Exercise1.PNG)

#### User Privileges and Arguments

* Inventory: The Inventory user has to access two tables, therefore Create Read Update and Delete privilege was the obvious choice in my opinion.
* Bookkeeping: For this user SELECT rights are sufficient, since the user does not need to update or create entries.
* HR: The user has CRUD rights, because this user handles employees, salaries, etc. In case of hiring or firing an employee this user needs to be able to create or delete an entry. This user has access to both employees and offices tables.
* Sales: Insert for this user is sufficient in my opinion.
* IT: This user has access to all tables and on top of CRUD he can GRANT permissions as well. 

## Exercise 2 - Logging

#### Users and their Privilegdes log

![picture](https://github.com/FarkIst/DBAssignment4/blob/master/img/UsersAndPrivileges.PNG)

#### The 3 Changes to the Database

![picture](https://github.com/FarkIst/DBAssignment4/blob/master/img/employee%20and%20orders.PNG)

#### Attempting to make a change with wrong privileges

![picture](https://github.com/FarkIst/DBAssignment4/blob/master/img/AccessDenied.PNG)

## Exercise 3 - Backup and Recovery

Backup file included in repository. 
A local backup has been created. 

For creating this backup I have used MYSQL Workbench. It is quite simple procedure, we have to select the *Management* tab, and click *Data Export*. This prompts us with export information of what we would like to include in the backup document. 

For importing the data you can use mysql < dump.sql, or simply import sql from Workbench.
