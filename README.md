# todo-api

A RESTful Todo API on Spring Boot with in-memory storage. My first REST API —
built to learn HTTP, controllers, and JSON serialization.

## Endpoints

| Method | Endpoint                    | Description       |
|--------|-----------------------------|-------------------|
| GET    | `/api/todo`                 | Get all todos     |
| POST   | `/api/todo`                 | Create a todo     |
| GET    | `/api/todo/{id}`            | Get todo by ID    |
| PATCH  | `/api/todo/{id}/complete`   | Mark as completed |
| DELETE | `/api/todo/{id}`            | Delete todo by ID |

## Run

Requires Java 17+.

```bash
./mvnw spring-boot:run
```

Example:

```bash
curl -X POST http://localhost:8080/api/todo \
  -H "Content-Type: application/json" \
  -d '{"title":"Write a test"}'
```

## Stack

Java 17 · Spring Boot 3 · Maven

## License

See [LICENSE](LICENSE).
