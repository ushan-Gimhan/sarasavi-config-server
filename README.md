# SARASAVI Config Server

**Author**: S.K.M Ushan Gimhan  
**Student ID**: 241711098  
**Slack Handle**: Ushan Gimhan  
**Module**: ITS 2130 — Enterprise Cloud Architecture  
**GCP Project ID**: `project-af908f5b-1cbf-40dc-9a7`

## Project Description
Centralized Spring Cloud Config Server for the SARASAVI Enterprise Bookshop Management System. Serves externalized configuration to all microservices using the native filesystem profile (`classpath:/config-repo`).

## Technology Stack
- Java 25
- Spring Boot 3.5.3
- Spring Cloud Config Server 2025.0.1
- Spring Boot Actuator

## Port
`8888`

## Setup / Getting Started

### Prerequisites
- Java 25+
- Maven 3.9+

### Build
```bash
mvn clean package -DskipTests
```

### Run
```bash
java -jar target/config-server-1.0.0.jar
```

### Environment Variables
| Variable | Default | Description |
|----------|---------|-------------|
| `PORT` | `8888` | Server port |

### Health Check
```
GET http://localhost:8888/actuator/health
```
