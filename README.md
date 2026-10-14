# Manager Library Infrastructure

This repository starts the database engine, Laravel API, and React application with Docker Compose.

Copy `.env.example` to `.env`, then run `docker compose up --build`.

The database must start empty. This repository must not contain DDL, product tables, or business seed SQL; Laravel migrations in the API own the complete `library` schema.
