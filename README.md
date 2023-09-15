# <h1 align = "center"> User Management </h1>

"User Management," is a robust Spring Boot application designed for managing user data efficiently. It provides a set of RESTful API endpoints that allow you to perform various operations on user records, such as adding, retrieving, updating, and deleting user information. 

- **Framework:** Spring Boot

### Controller

2. **Add Users:** `POST /users`
3. **Get All Users:** `GET /users`
4. **Get User by ID:** `GET /user/{userID}`
5. **Update User Phone Number:** `PUT /user/{userID}/number/{phoneNumber}`
6. **Update User Address:** `PUT /user/{userID}/address/{email}`
7. **Delete User by ID:** `DELETE /user/{userID}`

## Services

The Services layer implements the core business logic, data processing, and interaction with the data repository. Key responsibilities include:

- Validating input data.
- Performing CRUD operations on user data.
- Handling data transformations and interactions with external systems (if applicable).

## Repository

The Repository layer manages data access to the underlying database. It handles database operations such as Create, Read, Update, and Delete (CRUD) for user data. Additionally, it may include data mapping and conversion between Java objects and database entities.

## Database Design

The project's database design includes tables for user management, with fields such as:

- `userId` (User ID)
- `userName` (User Name)
- `type` (User Type)
- `userEmail` (Email Address)
- `userContactNo` (Phone Number)
- `dob` (Date of Birth)
- Timestamps for record creation and modification

### User Class

The `User` class defines the structure for user data and includes the following fields:

- `userId` (User ID): An integer that serves as a unique identifier for each user.
- `userName` (User Name): A string representing the user's full name.
- `type` (User Type): An enumeration specifying the user type, including ADMIN, INTERNAL, and EXTERNAL.
- `userEmail` (Email Address): A string containing the user's email address.
- `userContactNo` (Phone Number): A string representing the user's phone number (e.g., 911234567890).
- `dob` (Date of Birth): A date field indicating the user's date of birth.
- Timestamps for record creation and modification.

### Type Enum

The `Type` enum enumerates the possible user types:

- `ADMIN`: Represents an administrator user.
- `INTERNAL`: Represents an internal user.
- `EXTERNAL`: Represents an external user.

## License
This project is licensed under the [MIT License](LICENSE).



