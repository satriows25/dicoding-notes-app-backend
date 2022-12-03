# Notes App Back-End

> Proyek latihan kelas [Belajar Fundamental Aplikasi Back-End](https://www.dicoding.com/academies/271) di [Dicoding Indonesia](https://www.dicoding.com).

## Mengonfigurasi Environment
- File `.env` (development):
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
```
- File `.prod.env` (production):
```
# server configuration
HOST=0.0.0.0
PORT=5000
```

## Menjalankan di local

```bash
$ git clone https://github.com/satriows25/dicoding-notes-app-backend.git
$ cd dicoding-notes-app-backend
$ npm install
$ npm run start-dev
```

## Postman Collection dan Environment untuk Notes API

- **Collection**: /postman/Notes API Test.postman_collection.json
- **Environment**: /postman/Notes API Test.postman_environment.json
