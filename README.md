# Notes App Back-End

The Notes App Back-End is a practice project for the [Belajar Fundamental Aplikasi Back-End](https://www.dicoding.com/academies/271) class in [Dicoding Indonesia](https://www.dicoding.com/). It is a RESTful API back-end application with several important features, including:

1. PostgreSQL Database: The application uses PostgreSQL as a database to store user notes data.

2. JWT-based Authentication and Authorization: The application has an authentication and authorization system that uses JSON Web Tokens (JWT) to secure access to notes data.

3. RabbitMQ Message Broker: The application uses RabbitMQ as a message broker to export notes.

4. Storage: The application provides a feature to store image files related to notes.

5. Redis-based Caching: The application uses Redis as a cache to improve performance by storing frequently accessed notes data in cache.

With these features, the application can help users manage and store their notes more effectively and securely. Users can easily access and manipulate their notes data through the available API, as well as obtain faster performance through the use of Redis as a cache.

## Configuring the Environment

`.env` file (development):

```
# server configuration
HOST=localhost
PORT=5000

# node-postgres configuration
PGUSER=
PGHOST=localhost
PGPASSWORD=
PGDATABASE=notesapp
PGPORT=5432

# JWT Token
ACCESS_TOKEN_KEY=
REFRESH_TOKEN_KEY=
ACCESS_TOKEN_AGE=1800

# Message broker
RABBITMQ_SERVER=amqp://localhost

# aws-sdk
AWS_ACCESS_KEY_ID=
AWS_SECRET_ACCESS_KEY=
AWS_BUCKET_NAME=

# Redis
REDIS_SERVER=localhost
```

## Running Locally

```bash
$ git clone https://github.com/satriows25/dicoding-notes-app-backend.git
$ cd dicoding-notes-app-backend
$ npm install
$ npm run migrate up
$ npm run start-dev
```

## [Postman Collection dan Environment untuk Notes API](https://github.com/satriows25/dicoding-notes-app-backend/tree/main/postman)

- **Collection**: `/postman/Notes API Test.postman_collection.json`
- **Environment**: `/postman/Notes API Test.postman_environment.json`
