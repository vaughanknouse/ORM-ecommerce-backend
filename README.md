# ORM: E-Commerce Backend

![License](https://img.shields.io/badge/License-MIT-blue.svg)

## Description
E-commerce platforms are quite prevalent throughout the business and economic environments and understanding the fundamental architecture of e-commerce sites is essential for developers. To address this, this week’s UT Austin Coding Boot Camp challenge involved modifying starter code to build the back end for an E-commerce site using Express.js and Sequelize to interact with a PostgreSQL database. This application was built to provide a back end for an e-commerce website that uses the latest technologies so that a manager can work to ensure that his or her company can compete with other e-commerce internet retail companies.

This E-Commerce application demonstrates a functional API capable of handling CRUD operations for categories, products, and tags. It also manages data in a complex database by incorporating several relational data tables. Additionally, this project includes database configuration, schema creation, data seeding, models for products, categories, tags, and product tags, and API route testing. 


## Table of Contents

- [ORM: E-Commerce Backend](#orm-e-commerce-backend)
  - [Description](#description)
  - [Table of Contents](#table-of-contents)
  - [User Story](#user-story)
  - [Acceptance Criteria](#acceptance-criteria)
  - [Technologies Used](#technologies-used)
  - [Installation](#installation)
  - [Usage](#usage)
    - [Screenshots:](#screenshots)
  - [Tests](#tests)
  - [Links](#links)
  - [Credits](#credits)
  - [License](#license)
  - [Questions](#questions)


## User Story

```md
AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies
```

## Acceptance Criteria

```md
GIVEN a functional Express.js API
WHEN I add my database name, PostgreSQL username, and PostgreSQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the PostgreSQL database
WHEN I open API GET routes in Insomnia Core for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia Core
THEN I am able to successfully create, update, and delete data in my database
```


## Technologies Used 

- Node.js
- Express.js
- PostgreSQL
- Sequelize package
- pg package
- dotenv


## Installation

To install the ORM E-Commerce Background application, follow the following steps:

1. Clone the repository to your local machine: `https://github.com/vaughanknouse/ORM-ecommerce-backend.git`.
2. Ensure that the current version of Node.js is installed.
3. Open the cloned repository in a CLI, such as Visual Studio Code.
4. Navigate to the project directory in your terminal.
5. Initialize a project with `package.json` by typing `npm init -y` in the terminal.
6. Install the necessary dependencies by typing `npm install` in the command line to ensure that the `node-modules` folder is operating on your local device and that a `package-lock.json` file is present.
7. To set up environment variables, create a `.env` file in the root directory and add the following:
   ```
   DB_NAME='ecommerce_db'
   DB_USER='your_postgresql_username'
   DB_PASSWORD='your_postgresql_password'
   ```
     - Note: for `'your_postgresql_username'` enter your PostgreSQL username and for `'your_postgresql_password'` enter your PostgreSQL password.
8. Ensure that PostgreSQL is installed on your computer to initialize the database.
9.  Ensure that Insomnia is installed on your computer for unit testing.


## Usage

To use the ORM E-Commerce Background application, follow the following steps:

1. Open the Postgres Shell by typing the command `psql -U postgres` in the terminal.
2. Enter your user database password.
3. Create the `ecommerce_db` database by typing the command `\i db/schema.sql;` in the terminal.
4. Close out of the Postgres Shell by entering `\q` in the terminal.
5. Seed the database by entering `npm run seed` in the terminal.
6. Once your PostgreSQL database is active, navigate to the project directory and start the application by typing `npm start` in the terminal.
7. For unit testing instructions, navigate to the "Tests" section of the README. 


### Screenshots:

The following screenshot demonstrates the application's functionality and appearance:

**GET route to display all categories:**

![Shows GET route to display all categories.](assets/images/GET-categories-screenshot.png)

**POST route to add a new product:**

![Shows GET route to display all categories.](assets/images/POST-product-screenshot.png)


## Tests

Test the following API routes using Insomnia or a similar API client:

- Categories
  - GET `/api/categories`: Get all categories.
  - GET `/api/categories/:id`: Get a single category by id.
  - POST `/api/categories`: Create a new category.
  - PUT `/api/categories/:id`: Update a category by id.
  - DELETE `/api/categories/:id`: Delete a category by id.

- Products
  - GET `/api/products`: Get all products.
  - GET `/api/products/:id`: Get a single product by id.
  - POST `/api/products`: Create a new product.
  - PUT `/api/products/:id`: Update a product by id.
  - DELETE `/api/products/:id`: Delete a product by id.

- Tags
  - GET `/api/tags`: Get all tags.
  - GET `/api/tags/:id`: Get a single tag by id.
  - POST `/api/tags`: Create a new tag.
  - PUT `/api/tags/:id`: Update a tag by id.
  - DELETE `/api/tags/:id`: Delete a tag by id.


## Links 

GitHub Repository: https://github.com/vaughanknouse/ORM-ecommerce-backend

Walkthrough Video Link: https://drive.google.com/file/d/1Ik5bEE1xRbyZkW1wiF6kQTm_2MhISXGF/view?usp=sharing


## Credits
Used the following starter code and sources as tutorials and guidelines:

Starter code provided by UT Austin Coding Boot Camp at the following repository: https://github.com/coding-boot-camp/bookish-sniffle

npm documentation on dotenv: https://www.npmjs.com/package/dotenv

ChatGPT: https://chatgpt.com/?oai-dm=1

Also utilized the Xpert Learning Assistant for some portions of my code:
https://bootcampspot.instructure.com/courses/5293/external_tools/313


## License

This project is licensed under the MIT license. For more information, please visit [this link](https://opensource.org/licenses/MIT).


## Questions

For any questions or feedback, please contact me via email at vaughanknouse@gmail.com.

Additionally, you can find me on GitHub at [vaughanknouse](https://github.com/vaughanknouse).
