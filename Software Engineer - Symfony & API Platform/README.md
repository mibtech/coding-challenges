# Coding Challenge: API Platform (Symfony)

## Objective

Build a RESTful API using the Symfony framework and API Platform. The API will manage a simple library system, allowing users to perform CRUD operations on books and authors. Additionally, the application should be containerized using Docker.

## Requirements

1. **Entities**:
   - **Book**:
     - `id` (integer, auto-increment)
     - `title` (string, not nullable)
     - `description` (text, nullable)
     - `publicationDate` (date, nullable)
     - `author` (relation ManyToOne to Author, not nullable)
     - `categories` (relation ManyToMany to Category)

   - **Author**:
     - `id` (integer, auto-increment)
     - `name` (string, not nullable)
     - `birthDate` (date, nullable)
     - `biography` (text, nullable)
  - **Category**:
     - `id` (integer, auto-increment)
     - `name` (string, not nullable)

2. **API Endpoints**:
   - CRUD operations for both `Book`, `Author` and `Category`.
   - Filter books by publication date.
   - Filter authors by name.

3. **Docker**:
   - You can use the Symfony Docker-based installer provided by Dunglas:
     - [Symfony Docker](https://github.com/dunglas/symfony-docker)

     Follow the instructions provided in the repository for setting up Symfony with Docker.

   - Ensure a separate container for the database (PostgreSQL or MySQL) is used.

4. **Integration Testing**:
   - Write integration tests for the API endpoints.
   - Ensure the tests cover the following scenarios:
     - Creating a new book and author.
     - Retrieving a book and author by ID.
     - Updating a book and author.
     - Deleting a book and author.
     - Filtering books by publication date.
     - Filtering authors by name.

5. **CI/CD**:
   - Implement a basic CI/CD pipeline to automate testing and deployment.

6. **Code Standards and Best Practices**:
   - Follow PSR-1, PSR-2, and PSR-4 standards.
   - Ensure code readability and maintainability.

## Submission

- Once you're done with the test, let us know by sharing the repository link by email to **a.elfannir@mibtech.ma**.

## Questions?

If you have any questions, just be clear and wrap an email to a.elfannir@mibtech.ma, and we will help you as much as we can. 
