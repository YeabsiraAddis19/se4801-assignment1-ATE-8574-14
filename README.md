# ShopWave Starter (Spring Boot)

ShopWave Starter is a Maven-based Spring Boot 3.x application that demonstrates a simple product domain with a layered architecture (entities, repositories, services, and REST controllers). It uses Spring Data JPA with an in-memory H2 database for development and includes basic validation and error handling suitable for coursework and rapid prototyping.

## Author

- Name: `Yeabsira Addis`
- Student number: `ATE/8574/14`

## Tech stack

- Java 21
- Spring Boot 3.2.x
- Spring Web, Spring Data JPA, Actuator
- H2 Database
- Lombok
- JUnit 5 + Mockito + Spring Boot Test

## How to build

From the project root:

```bash
mvn clean package
```

## How to run

From the project root:

```bash
mvn spring-boot:run
```

The app starts on port `8080`.

## How to run tests

```bash
mvn test
```

You can also run a single test class:

```bash
mvn -Dtest=ProductServiceTest test
```

## API quick test (examples)

- `POST /api/products`
- `GET /api/products`
- `GET /api/products/{id}`
- `GET /api/products/search?keyword=laptop&maxPrice=2000`
- `PATCH /api/products/{id}/stock` with body `{"delta": -2}`

## AI assistance disclosure

During development, an AI model from a current version of Anthropic’s Claude family was used to assist with debugging, code support, and implementation guidance. All generated output was reviewed and adapted to meet the project requirements.

