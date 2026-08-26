# SARASAVI Config Server

The **SARASAVI Config Server** provides centralized, externalized configuration management for all microservices in the SARASAVI Bookshop platform.

## Port
- Default: `8888`

## Features
- Spring Cloud Config Server native repository
- Centralized profiles for all microservices:
  - `application.yml` (shared)
  - `book-inventory-service.yml`
  - `sales-order-service.yml`
  - `media-service.yml`
  - `api-gateway.yml`
- Environment variable overrides without code modification
- Actuator health check endpoint: `/actuator/health`

## How to Run
```bash
mvn clean spring-boot:run
```

## Verify Health
```bash
curl http://localhost:8888/actuator/health
```
