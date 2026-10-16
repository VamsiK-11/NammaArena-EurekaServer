# NammaArena - Eureka Server

Service Discovery Server for the NammaArena microservices architecture, built with Spring Cloud Netflix Eureka.

## Tech Stack
- Java 17
- Spring Boot 3.2.0
- Spring Cloud Netflix Eureka Server

## Port
`8761`

## Getting Started

### Prerequisites
- Java 17
- Maven 3.9+

### Run Locally
```bash
mvn clean package -DskipTests
java -jar target/*.jar
```

### Run with Docker
```bash
docker build -t nammaarena-eureka-server .
docker run -p 8761:8761 nammaarena-eureka-server
```

## Eureka Dashboard
Once running, access the Eureka dashboard at:
```
http://localhost:8761
```

## Registered Services
The following services register with this Eureka Server:
- `auth-service` — port 8081
- `turf-service` — port 8082
- `booking-service` — port 8083
- `payment-service` — port 8084
- `api-gateway` — port 8080

## Part of NammaArena Microservices
| Service | Repository |
|---|---|
| Eureka Server | [NammaArena-EurekaServer](https://github.com/VamsiK-11/NammaArena-EurekaServer) |
| API Gateway | [NammaArena-APIGateway](https://github.com/VamsiK-11/NammaArena-APIGateway) |
| Auth Service | [NammaArena-AuthService](https://github.com/VamsiK-11/NammaArena-AuthService) |
| Turf Service | [NammaArena-TurfService](https://github.com/VamsiK-11/NammaArena-TurfService) |
| Booking Service | [NammaArena-BookingService](https://github.com/VamsiK-11/NammaArena-BookingService) |
| Payment Service | [NammaArena-PaymentService](https://github.com/VamsiK-11/NammaArena-PaymentService) |
