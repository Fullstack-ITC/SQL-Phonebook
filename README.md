# Task: Phonebook API with Express.js and SQL Database

## Objective
Create a simple phonebook API using Express.js that performs CRUD (Create, Read, Update, Delete) operations on phone numbers. This time, the data should be stored in an SQL database.

## Prerequisites
Basic knowledge of SQL and relational databases. If students have not completed the previous task involving the local file system, they can still proceed with this one, as it stands alone in its context.

## Specifications

### Setup
- Initialize a new Node.js project (or use the existing one if you've completed the previous task).
- Install Express.js using npm (if not already installed).
- Setup a basic Express.js server.
- Choose an SQL database (e.g., MySQL, PostgreSQL, SQLite) and set it up. Install the necessary npm packages to integrate it with your Express app.

### Database Schema
- Create a table named 'phonebook' with columns: 'id', 'name', and 'phoneNumber'.
- The 'id' column should be an auto-increment primary key.

### API Endpoints
- `GET /phonebook`: Retrieve all phone numbers from the database.
- `POST /phonebook`: Add a new phone number and name to the database. The body should contain fields named 'name' and 'phoneNumber'.
- `PUT /phonebook/:id`: Update an existing phone number and/or name in the database using the provided 'id'.
- `DELETE /phonebook/:id`: Delete a specific phone number and name from the database using the provided 'id'.

### Error Handling
- Handle scenarios where a phone number might not exist in the database for update or delete operations.
- Provide meaningful error messages to the client, including potential database errors.

### Testing
- Use tools like Postman or any REST client to test each of the endpoints.
- Ensure that each operation (fetch, save, update, delete) works as expected with the SQL database.
