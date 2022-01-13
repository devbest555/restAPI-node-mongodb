# REST API Development with Node.js, Express, and MongoDB

**NodeJs** using **MongoDB** as database

## Features

- Basic Authentication (Register/Login with hashed password)
- Account confirmation with 4 (Changeable) digit OTP.
- Email helper ready just import and use.
- JWT Tokens, make requests with a token after login with `Authorization` header with value `Bearer yourToken` where `yourToken` will be returned in Login response.
- Pre-defined response structures with proper status codes.
- Included CORS.
- **Book** example with **CRUD** operations.
- Validations added.
- Included API collection for Postman.
- Light-weight project.
- Test cases with [Mocha](https://mochajs.org/) and [Chai](https://www.chaijs.com/).
- Code coverage with [Istanbuljs (nyc)](https://istanbul.js.org/).
- Included CI (Continuous Integration) with [Travis CI](https://travis-ci.org).
- Linting with [Eslint](https://eslint.org/).

## Software Requirements

- Node.js **8+**
- MongoDB **3.6+** (Recommended **4+**)

### Setting up environments

1.  find `.env.example` on root directory of project.
2.  Create a new file by copying and pasting the file and then renaming it to just `.env`
    ```bash
    cp .env.example .env
    ```
3.  The file `.env` is already ignored, so you never commit your credentials.
4.  Change the values of the file to your environment. Helpful comments added to `.env.example` file to understand the constants.

### Running API server locally

```bash
npm run dev
```

**Note:** `YOUR_DB_CONNECTION_STRING` will be your MongoDB connection string.

### Creating new models

If you need to add more models to the project just create a new file in `/models/` and use them in the controllers.

### Creating new routes

If you need to add more routes to the project just create a new file in `/routes/` and add it in `/routes/api.js` it will be loaded dynamically.

### Creating new controllers

create a new file in `/controllers/` and use them in the routes.

## Tests

### Running Test Cases

```bash
npm test
```
