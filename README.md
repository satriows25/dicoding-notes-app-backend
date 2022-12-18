# Notes App Back-End

Proyek latihan kelas [Belajar Fundamental Aplikasi Back-End](https://www.dicoding.com/academies/271) di [Dicoding Indonesia](https://www.dicoding.com).

## Mengonfigurasi Environment

File `.env` (development):

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

## Menjalankan di local

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
