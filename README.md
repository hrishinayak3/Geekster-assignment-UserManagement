# User Managemnent

"User Management," is a robust Spring Boot application designed for managing user data efficiently. It provides a set of RESTful API endpoints that allow you to perform various operations on user records, such as adding, retrieving, updating, and deleting user information.

Data Flow
Controller
The Controller layer is responsible for handling incoming HTTP requests and delegating them to the appropriate services. It defines API endpoints for the following operations:

Add User: POST /user
Add Users: POST /users
Get All Users: GET /users
Get User by ID: GET /user/{userID}
Update User Phone Number: PUT /user/{userID}/number/{phoneNumber}
Update User Address: PUT /user/{userID}/address/{email}
Delete User by ID: DELETE /user/{userID}



