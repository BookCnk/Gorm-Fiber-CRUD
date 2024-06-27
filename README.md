# Book CRUD API with Fiber and Gorm

This is a simple CRUD API for managing books using the Fiber web framework and Gorm ORM in Go. The API supports creating, reading, updating, and deleting books in a PostgreSQL database.

## Prerequisites

- Go (1.16 or later)
- PostgreSQL
- Docker (optional, for running PostgreSQL in a container)
- Postman (for testing the API)

## Getting Started

### Setting Up PostgreSQL

You can set up PostgreSQL using Docker or install it directly on your machine.

#### Using Docker

```bash
docker run --name mydatabase -e POSTGRES_USER=myuser -e POSTGRES_PASSWORD=mypassword -e POSTGRES_DB=mydatabase -p 5432:5432 -d postgres
```
## Example API endpoints

### create a new book

- **method:** `POST`
- **url:** `http://localhost:3000/books`
- **body:** (select raw and JSON)

```json
{
    "name": "The Go Programming Language",
    "author": "Alan Donovan",
    "description": "A comprehensive guide to Go programming."
}
```
