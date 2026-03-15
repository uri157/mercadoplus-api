```markdown
# MercadoPlus API

Backend API for **MercadoPlus**, a MercadoLibre-style e-commerce platform.

This project was my **first full backend system** built with ASP.NET Core.  
I designed and implemented the API end-to-end, including authentication, catalog management, shopping cart logic, transactions, and email notifications.

The API was successfully consumed by both a **web frontend** and a **mobile client** developed by teammates.

---

## Overview

MercadoPlus provides the backend services for a collaborative academic e-commerce project inspired by Mercado Libre.

Main capabilities include:

- Product catalog with search and filtering
- User registration and authentication
- Shopping cart management
- Purchase / transaction flow
- Reviews and notifications
- Admin catalog management
- Email notifications

The API exposes a **RESTful interface** documented with Swagger and secured with JWT authentication.

---

## Tech Stack

- **C#**
- **.NET 8**
- **ASP.NET Core Web API**
- **Entity Framework Core**
- **SQL Server**
- **ASP.NET Core Identity**
- **JWT Authentication**
- **Swagger / OpenAPI**
- **Mailgun API**

---

## Architecture

The project follows a layered structure separating HTTP concerns from business logic.

```

Controllers   → HTTP endpoints
Services      → business logic
Interfaces    → service contracts
Models        → domain entities
DTOs          → request / response objects
Context       → EF Core database context

```

This structure keeps controllers thin while business logic is handled in services through dependency injection.

---

## Core Features

### Authentication & Accounts

- User registration
- Email confirmation
- JWT-based login
- Role-based authorization

### Catalog

- Product publications
- Categories
- Product states
- Photo management

### Shopping Flow

- Shopping cart
- Transactions
- Payment methods
- Purchase notifications

### Social Features

- Product reviews
- Publication visits tracking

---

## API Documentation

Swagger UI is enabled for exploring and testing the API.

```

/swagger

````

---

## Running Locally

### Prerequisites

- .NET 8 SDK
- SQL Server instance

### Run the API

```bash
dotnet restore
dotnet build
dotnet run
````

Swagger should be available at:

```
/swagger
```

---

## What I Learned

This project helped me understand and apply:

* REST API design
* Dependency Injection
* layered backend architecture
* authentication and authorization with Identity + JWT
* Entity Framework data modeling
* third-party service integration (Mailgun)
* API documentation with Swagger

It was my **first real backend system consumed by external clients**.

---

## Project Context

MercadoPlus was developed as a **team academic project**.

My responsibility was the **backend API**, which I implemented end-to-end.
The web frontend and mobile client were built by teammates and integrated against this API.

---

## Repository Status

This repository is presented as a **legacy portfolio project**, preserved as an example of my early backend work and architectural learning process.

---

## License

Educational/demo project.

```
