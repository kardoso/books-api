
<h1 align="center">
  <img alt="Express" title="Express" src="https://expressjs.com/images/express-facebook-share.png" width="200px" />
</h1>
<h3 align="center">
  This is a small API of books. Implementing almost all REST Verbs, contains Unit and Integration testing with mocha and uses Hypermedia for self documenting API.
</h3>

<p align="center">
  <a href="#bulb-what-was-used">What was used</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#blue_book-importing-data">Importing data</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#checkered_flag-installation">Installation</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#wrench-tests">Tests</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#incoming_envelope-routes">Routes</a>
</p>

## :bulb: What was used

- [Node](https://nodejs.org/)
- [Npm](https://www.npmjs.com/) - Package Manager
- [ESList](https://eslint.org/) - Find code problems and fix syntax
- [Nodemon](https://nodemon.io/) - (Dev dependencie) Monitor file changes
- [Express](https://expressjs.com/) - Server framework
- [MongoDB](https://www.mongodb.com/) - Database
- [Mongoose](https://mongoosejs.com/) - Database Object modeling
- [Mocha](https://mochajs.org/) - Testing
- [Sinon](https://sinonjs.org/) - Testing
- [Should](https://www.npmjs.com/package/should) - Testing
- [Supertest](https://www.npmjs.com/package/supertest) - Integration testing

## :blue_book: Importing data
Import Book data into your mongoDB database.

Make sure MongoDB is running with the command `mongod` then run `mongo bookAPI < booksJson.js` from the command line.

## :checkered_flag: Installation
First of all, make sure that you have Node.js installed on your machine. Choose a package manager (NPM or Yarn)

Now, to install the dependencies

```
    npm install
```

To start the application
```
    npm start
```

## :wrench: Tests
This project has unit and integration tests.

Run tests with `npm test`

## :incoming_envelope: Routes

| Paths                    | HTTP Method | Description                                     |
| ------------------------ | ----------- | ----------------------------------------------- |
| /api/books               | GET         | Show All books                                  |
| /api/books               | POST        | Create a new book                               |
| /api/books?genre=Fantasy | GET         | Filter books of a genre, "Fantasy" in this case |
| /api/books/:id           | GET         | Get book with id                                |
| /api/books/:id           | PUT         | Edit all informations of a book                 |
| /api/books/:id           | PATCH       | Edit book                                       |
| /api/books/:id           | DELETE      | Delete book                                     |
