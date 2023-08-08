This project is an API built using **Java, Java Spring, Flyway Migrations, PostgresSQL as the database, and Spring Security and JWT for authentication control.**

The API was developed during my studies about Spring Security to demonstrate how to configure Authentication and Authorization in Spring application using Spring Security.
You can follow a tutorial where I learned from by taking a look at this YouTube channel: https://www.youtube.com/@kipperdev 

## Installation

1. Clone the repository:

```bash
git clone <https://github.com/CodeThales/standard.spring.security.api.token-authentication.git>
```

1. Install dependencies with Maven
2. Install [PostgresSQL](https://www.postgresql.org/)

## Usage

1. Start the application with Maven
2. The API will be accessible at [http://localhost:8080](http://localhost:8080/)

## API Endpoints

The API provides the following endpoints:

```markdown
GET /product - Retrieve a list of all products. (all authenticated users)

POST /product - Register a new product (ADMIN access required).

POST /auth/login - Login into the App

POST /auth/register - Register a new user into the App

```

## Authentication

The API uses Spring Security for authentication control. The following roles are available:

```
USER -> Standard user role for logged-in users.
ADMIN -> Admin role for managing partners (registering new partners).

```

To access protected endpoints as an ADMIN user, provide the appropriate authentication credentials in the request header.

## Database

The project utilizes [PostgresSQL](https://www.postgresql.org/) as the database. The necessary database migrations are managed using Flyway.