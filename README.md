### TaskList

## Assumptions:
1)	A Person can create tasks, check the progress of the tasks and create or update notes for himself.
2)	A Manager is a Person who can also create new Users, delete existing Users, assign created tasks to the Users and give feedback to the Users. 
3)	A User is a Person who can also add the created tasks to a task list specific to himself, view the task list and view the feedbacks given to him.
4)	Every task has a status. The status can be either “PENDING” or “PROCESSING” or “FINISHED”. 
5)	Every task has a priority assigned to itself during its creation, where the priority varies on a scale of 1 to 5, 1 being the lowest and 5 being the highest. 
6)	A rank has been calculated and assigned to each task. The rank is determined by using the priority and the estimated time interval. 
7)	A task can be set as recurring upon its creation and for simplicity the recurring interval is a fixed 7 days interval. 
8)	Every task has to be created with a priority, estimated time and a recurring value.
9)	Once a task is completed, it is put into the finshedTask list of a User.
10)	To keep things simple, at any moment there can be only one Manager, implemented as a singleton class, and all the managerial stuffs are done by himself.  He has access to the task list of every other user.
11)	Only Manager can give feedbacks and Users can receive feedbacks.


## Class Diagram
![class diagram](https://user-images.githubusercontent.com/40374399/41570069-6c45a4c2-732a-11e8-8179-a7741f6ee3e3.JPG)


## Instruction for Program Execution:
Assuming Java, Maven, Git and MongoDB are setup on device: 
1)	Go to the root directory where there is pom.xml for the file.
2)	Execute command mvn clean install
3)	Execute command mvn spring-boot:run


## Future Enhancements:    
1)	Logins can be added for Managers and Users.
2)	Privileges can be managed through logins. 
3)	A managerial group can be created instead of having a single Manager. 
4)	Managers can also receive feedbacks.
5)	The recurring tasks can be made more flexible instead of having a fixed recurrence interval.
6)	More details can be added to a Task.
7)	More UML diagrams can be added.
8)	More test cases can be added. 
