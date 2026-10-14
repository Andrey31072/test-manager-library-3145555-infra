# SDD Implementation Notes

This repository owns only containers, network, volumes, and the empty PostgreSQL engine.
It intentionally contains no `CREATE TABLE` statements and no category seed SQL.
The Laravel API migration owns all DDL and fixed categories.

Run:

```bash
docker compose up --build
```

Then, in another terminal:

```bash
docker compose exec api php artisan migrate --force
```

The API is exposed on `http://localhost:8000/api/v1`.
The React app is exposed on `http://localhost:5173`.
