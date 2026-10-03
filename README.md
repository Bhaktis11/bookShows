# BookShows

A Spring Boot backend for a seat reservation system designed to prevent double-selling of seats during concurrent reservations.

## Tech Stack

- Java 17
- Spring Boot 4.1.1
- PostgreSQL 18
- Docker
- Maven
- Spring Data JPA
- Spring Boot Actuator

## Prerequisites

- Java 17
- Docker Desktop
- Maven (or use the included Maven Wrapper)

## Run Locally

### 1. Start PostgreSQL

```bash
docker volume create postgres_data
docker run -d --name my-postgres -e POSTGRES_DB=myappdb -e POSTGRES_USER=myappuser -e POSTGRES_PASSWORD=<your-password> -p 5432:5432 -v postgres_data:/var/lib/postgresql postgres:18

### 2. Set environment variables

```text
DB_USERNAME=myappuser
DB_PASSWORD=<your-password>