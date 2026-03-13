# n8n with PostgreSQL

Starts n8n with PostgreSQL as database.

## Start

To start n8n with PostgreSQL simply start docker-compose by executing the following
command in the current folder.

**IMPORTANT:** But before you do that change the default users and passwords in the `.env` file!

```bash
docker-compose up -d
```

To stop it execute:

```bash
docker-compose stop
```

## Configuration

The default name of the database, user and password for PostgreSQL can be changed in the `.env` file in the current directory.

## Environment Variables

- `POSTGRES_USER`: The superuser for PostgreSQL.
- `POSTGRES_PASSWORD`: The password for the superuser.
- `POSTGRES_DB`: The name of the database.
- `POSTGRES_NON_ROOT_USER`: The limited user for n8n.
- `POSTGRES_NON_ROOT_PASSWORD`: The password for the limited user.
- `N8N_RUNNERS_MODE`: Set to `internal` for simple local setups.
