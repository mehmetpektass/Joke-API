# Joke API 🃏

## Description

Joke API is a simple RESTful API built using Express.js that allows users to perform CRUD operations on a collection of jokes. The API provides endpoints to retrieve random jokes, get specific jokes by ID, filter jokes by type, add new jokes, update existing jokes, and delete jokes. It also includes authentication for deleting all jokes using a master key.

## Installation and Using

1. Clone this repository to your local machine:
2. Navigate to the project directory.
3. Install dependencies by running:


```bash
import express from "express";
import bodyParser from "body-parser";
import masterKey from "./masterkey.js";
...

1. Use your preferred API testing tool (e.g., Postman, Insomnia) to interact with the endpoints.
2. Ensure to include appropriate request bodies and parameters as mentioned in the documentation.
3. You need a Master Key to delete all the data that is the last operation, the Master Key in my project is stored in the masterkey.js file, and this key is stored so that all the data is not deleted.
```

```bash
cd /path/to/your/project

npm install express body-parser

node index.js

```

## Endpoints
1. GET /random: Retrieves a random joke from the collection.
2.  GET /jokes/:id: Retrieves a specific joke by its ID.
3. GET /filter?type=[jokeType]: Retrieves jokes filtered by the specified joke type.
4. POST /jokes: Adds a new joke to the collection.
5. PUT /jokes/:id: Updates an existing joke by its ID.
6. PATCH /jokes/:id: Partially updates an existing joke by its ID.
7. DELETE /jokes/:id: Deletes a specific joke by its ID.
8. DELETE /all?key=[masterKey]: Deletes all jokes from the collection (requires a master key for authentication).

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.🚀
