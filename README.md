# Task Management Web App

A personal project showcasing a scalable task management application built with Java, Spring Boot, MySQL, Redis, and Docker, deployed on AWS. Users can create, update, and delete tasks with real-time caching and secure authentication.

## Features
- Create, read, update, and delete tasks via RESTful APIs.
- User authentication with JWT.
- MySQL for persistent storage, Redis for caching task lists.
- Containerized with Docker, deployed on AWS Elastic Beanstalk.
- Basic HTML/JS front-end for task management.

## Tech Stack
- Backend: Java, Spring Boot, Hibernate
- Database: MySQL, Redis
- Deployment: Docker, AWS
- Tools: Maven, Postman, IntelliJ IDEA

## Setup Instructions
1. **Prerequisites**: Java 17, MySQL, Redis, Docker, AWS CLI.
2. Clone the repository: `git clone <your-repo-url>`.
3. Configure MySQL and Redis in `application.properties`.
4. Build the project: `mvn clean install`.
5. Run locally: `mvn spring-boot:run` or use Docker: `docker-compose up`.
6. Deploy to AWS: Configure Elastic Beanstalk and upload the Docker image.

## API Endpoints
- `POST /api/auth/register`: Register a new user.
- `POST /api/auth/login`: Login and get JWT.
- `POST /api/tasks`: Create a task.
- `GET /api/tasks`: List all tasks (cached in Redis).
- `PUT /api/tasks/{id}`: Update a task.
- `DELETE /api/tasks/{id}`: Delete a task.

## License
MIT License
