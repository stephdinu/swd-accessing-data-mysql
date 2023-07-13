# My Spring App Bound to a MySQL Database
This is a demonstration of a Spring application connected to a MySQL Database (as opposed to the default in-memory, embedded database H2). The application uses Spring Data JPA to access the database.

How to test the application:
1. After forking the repository and establishing a clean build, please run the following command to add a new user to the database: curl http://localhost:8080/demo/add -d name=First -d email=someemail@someemailprovider.com . The reply should be 'Saved'.
2. Run the following command to show all users: curl http://localhost:8080/demo/all . The reply will give an .xml response of all the users in the database.
