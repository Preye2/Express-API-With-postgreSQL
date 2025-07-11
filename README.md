# PostgreSQL Express API

A simple Express.js API that connects to PostgreSQL and performs CRUD operations.

## Setup

1. Install PostgreSQL and Node.js
2. Create a database named `mini_project`
3. Run the table creation SQL (provided in app.js comments)
4. Clone this repository
5. Install dependencies: `npm install`
6. Create a `.env` file with your database credentials
7. Start the server: `node app.js`

## API Endpoints

- `GET /users` - Get all users
- `GET /users/:id` - Get a specific user
- `POST /users` - Create a new user
- `PUT /users/:id` - Update a user
- `DELETE /users/:id` - Delete a user

## Testing

---

![database connection in my VSC](https://github.com/Preye2/Express-API-With-postgreSQL/blob/main/images%2Fdatabase-is-connected.jpg)
https://github.com/Preye2/Express-API-With-postgreSQL/blob/main/images%2Fdatabase-is-connected.jpg?raw=true

___


![Postgres DB connection](https://github.com/Preye2/Express-API-With-postgreSQL/blob/main/images%2Fpostgres-db.jpg)
https://github.com/Preye2/Express-API-With-postgreSQL/blob/main/images%2Fpostgres-db.jpg?raw=true

---

![GET API Implementation](https://github.com/Preye2/Express-API-With-postgreSQL/blob/main/images%2Fget-api.jpg)
https://github.com/Preye2/Express-API-With-postgreSQL/blob/main/images%2Fget-api.jpg?raw=true

---

![GET All](https://github.com/Preye2/Express-API-With-postgreSQL/blob/main/images%2Fget-all-api.jpg)
https://github.com/Preye2/Express-API-With-postgreSQL/blob/main/images%2Fget-all-api.jpg?raw=true

---

![Get by ID](https://github.com/Preye2/Express-API-With-postgreSQL/blob/main/images%2Fget-user-id.jpg)
https://github.com/Preye2/Express-API-With-postgreSQL/blob/main/images%2Fget-user-id.jpg?raw=true

---

![POST API](https://github.com/Preye2/Express-API-With-postgreSQL/blob/main/images%2Fpost-api.jpg)
https://github.com/Preye2/Express-API-With-postgreSQL/blob/main/images%2Fpost-api.jpg?raw=true

---

![PUT by ID](https://github.com/Preye2/Express-API-With-postgreSQL/blob/main/images%2Fput-user-id.jpg)
https://github.com/Preye2/Express-API-With-postgreSQL/blob/main/images%2Fput-user-id.jpg?raw=true

---

![Delete by ID](https://github.com/Preye2/Express-API-With-postgreSQL/blob/main/images%2Fdelete-user-id.jpg)
https://github.com/Preye2/Express-API-With-postgreSQL/blob/main/images%2Fdelete-user-id.jpg?raw=true

---

You can test the API using Postman or curl:

```bash
# Create a user
curl -X POST -H "Content-Type: application/json" -d '{"name":"John Doe","email":"john@example.com"}' http://localhost:3000/users

# Get all users
curl http://localhost:3000/users

# Get a specific user
curl http://localhost:3000/users/1

# Update a user
curl -X PUT -H "Content-Type: application/json" -d '{"name":"John Updated","email":"john.updated@example.com"}' http://localhost:3000/users/1

# Delete a user
curl -X DELETE http://localhost:3000/users/1
