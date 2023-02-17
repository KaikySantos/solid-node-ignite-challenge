![cover-node js](https://user-images.githubusercontent.com/56506919/219757505-28223f79-45ea-4f62-be3d-ca0f0b3da48b.png)

## 🖥️ Challenge 02: Introduction to SOLID

User listing and registration application. Developed using some SOLID concepts!

<br />

## 🚀 Technologies

This project was developed with the following technologies:

- [Typescript](https://www.typescriptlang.org/)
- [Express](https://expressjs.com/)
- [Nodemon](https://nodemon.io/)
- [Uuid](https://www.npmjs.com/package/uuid)
- [Jest](https://jestjs.io/)
- [Supertest](https://www.npmjs.com/package/supertest)

<br />

## 🛣️ Application routes

<table>
  <tr>
    <th>Method</th>
    <th>Path</th>
    <th></th>
  </tr>
  <tr>
    <td>POST</td>
    <td>/users</td>
    <td>
      Register a new user
    </td>
  </tr>
  <tr>
    <td>PATCH</td>
    <td>/users/:user_id/admin</td>
    <td>
      Turn a user into an admin
    </td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/users/:user_id</td>
    <td>
      User specific information
    </td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/users</td>
    <td>
      List of all users
    </td>
  </tr>
</table>

<br />

## 🧪 Tests

- Model
  - Should be able to create an user with all props
- Repository
  - Should be able to create new users
  - Should be able to list all users
  - Should be able to find user by ID
  - Should be able to find user by e-mail address
  - Should be able to turn an user as admin
- UseCases
  - Should be able to create new users
  - Should not be able to create new users when email is already taken
  - Should be able to turn an user as admin
  - Should not be able to turn a non existing user as admin
  - Should be able to get user profile by ID
  - Should not be able to show profile of a non existing user
  - Should be able to list all users
  - Should not be able to a non admin user get list of all users
  - Should not be able to a non existing user get list of all users

- Routes
  - [POST] /users
    - Should be able to create new users
    - Should not be able to create new users when email is already taken
  - [PATCH] /users/:user_id/admin
    - Should be able to turn an user as admin
    - Should not be able to turn a non existing user as admin
  - [GET] /users/:user_id
    - Should be able to get user profile by ID
    - Should not be able to show profile of a non existing user
  - [GET] /users
    - Should be able to list all users
    - Should not be able to a non admin user get list of all users
    - Should not be able to a non existing user get list of all users

<br />

## ℹ️ How To Use
```bash
# Clone the repository
$ git clone https://github.com/kaikySantos/solid-node-ignite-challenge.git

# Go into the directory
$ cd solid-node-ignite-challenge

# Install dependencies
$ npm i

# Run the application
$ npm run dev

# Run the tests
$ npm run test
```

<br />

---

Made with ♥ by Kaiky 👋🏻
