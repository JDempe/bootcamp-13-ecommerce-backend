# CBC Week 13 Challenge: E-Commerce Backend
## Description

This is the thirteenth week's challenge assignment for the UCB Coding Bootcamp program.  The assignment is to build the back end for an e-commerce site.  The application uses Express.js for the server and MySQL for the database.  The database is seeded using Sequelize.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Final Product](#final-product)
- [Credits](#credits)
- [License](#license)
- [How to Contribute](#how-to-contribute)



## Prerequisites

To run the application locally, you will need to install [Node.js](https://nodejs.org/en/).

## Final Product

The final product is available at https://github.com/JDempe/bootcamp-13-ecommerce-backend.

### Usage Instructions

#### Running the Application Locally

To run the application locally, follow the following steps.

1. Clone the repository to your local machine.
2. At the command line, run `npm install` to install the dependencies.
3. Create a `.env` file in the root directory of the project.  Add the following to the file, replacing the values with your MySQL credentials.
   DB_NAME='ecommerce_db'
   DB_USER='root'
   DB_PASSWORD='<your password>'
4. Create the MySQL Schema using the `schema.sql` file in the `db` directory. You can do this using MySQL Workbench or the command line.  If using the command line, run `mysql -u root -p` and enter your password.  Then run `source db/schema.sql` to create the database.  then type `quit` to exit MySQL.
5. Run `npm run seed` to seed the database.
6. Run `npm start` to start the server.

Below is a example video showing this process:

https://github.com/JDempe/bootcamp-13-ecommerce-backend/assets/123279032/e4214c62-3e09-4845-af6c-f6d6a6381e61

### User Interface

The application does not have a user interface.  It is tested using Postman.  The routes are also available in the `routes` directory.  They are as follows:

- `GET /api/categories` returns all categories.
- `GET /api/categories/:id` returns a single category by id.
- `POST /api/categories` creates a new category.
- `PUT /api/categories/:id` updates a category by id.
- `DELETE /api/categories/:id` deletes a category by id.

- `GET /api/products` returns all products.
- `GET /api/products/:id` returns a single product by id.
- `POST /api/products` creates a new product.
- `PUT /api/products/:id` updates a product by id.
- `DELETE /api/products/:id` deletes a product by id.

- `GET /api/tags` returns all tags.
- `GET /api/tags/:id` returns a single tag by id.
- `POST /api/tags` creates a new tag.
- `PUT /api/tags/:id` updates a tag by id.
- `DELETE /api/tags/:id` deletes a tag by id.

Here is an example of the routes in Postman:

https://github.com/JDempe/bootcamp-13-ecommerce-backend/assets/123279032/e66248c1-38b6-4455-8d91-8c5c3f9106cc

## Credits

### Resources

The below resources contributed to the project.

- UC Berkeley Extension provided the starter code for the project.  The helper functions, classes, middleware and routes were provided, as well as the frontend pages.

- [Node.js](https://nodejs.org/en/) is a JavaScript runtime built on Chrome's V8 JavaScript engine.  The file system module is used to read and write files.

- [Express](https://expressjs.com/) is a Node.js web application framework.  It is used to serve the static files for the application.

- [MySQL](https://www.mysql.com/) is an open-source relational database management system.  It is used to store the data for the application.

- [Sequelize](https://sequelize.org/) is a promise-based Node.js ORM for Postgres, MySQL, MariaDB, SQLite and Microsoft SQL Server.  It is used to interact with the MySQL database.

- [dotenv](https://www.npmjs.com/package/dotenv) is a zero-dependency module that loads environment variables from a .env file into process.env.  It is used to store the MySQL credentials.

- [Postman](https://www.postman.com/) is a collaboration platform for API development.  It is used to test the API routes.

### Collaborators

On this project, there was no peer review or collaboration.

## License

Refer to the LICENSE in the repository.

## How to Contribute

Contribute at https://github.com/JDempe/bootcamp-13-ecommerce-backend.
