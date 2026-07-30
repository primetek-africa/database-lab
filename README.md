# PostgreSQL Database Laboratory

A reusable Docker-based laboratory for learning relational databases with
**PostgreSQL** and **pgAdmin 4**. This repository provides a complete
environment for teaching SQL, database design, data modeling, and
database administration throughout the Relational Database course.

Students will use this environment to create multiple databases, design
tables, insert records, execute SQL queries, and progressively learn
more advanced database concepts.

---

# Program Information

**Organization:** PrimeTek Africa - Codecamp Academy

**Program:** Advanced Full-Stack Software Development

**Module:** Programming Foundations

**Instructor:** Cristian Camilo Cortes Ortiz

**Instructor Role:** Systems Engineer & Full-Stack Software Development
Instructor

---

# Course Overview

This laboratory provides a consistent PostgreSQL environment that can be
reused throughout the entire database module. Instead of creating a new
server for every project, students will work with a single PostgreSQL
instance and create multiple databases as they progress through the
course.

Using Docker ensures that every student has the same development
environment regardless of their operating system.

---

# Learning Objectives

By using this laboratory, students will learn how to:

- Install and use Docker for database development.
- Work with PostgreSQL.
- Use pgAdmin 4 for database administration.
- Create databases.
- Create tables.
- Define primary keys.
- Define foreign keys.
- Apply database constraints.
- Insert, update, and delete records.
- Query relational databases using SQL.
- Design normalized database schemas.
- Create relationships between tables.
- Write complex SQL queries.
- Perform aggregate operations.
- Work with joins.
- Create views.
- Create indexes.
- Manage transactions.
- Backup and restore databases.

---

# Technologies

- Docker
- Docker Compose
- PostgreSQL 17
- pgAdmin 4
- SQL

---

# Prerequisites

Before using this project, install:

- Docker Desktop
- Git

Verify the installation:

```bash
docker --version
```

```bash
docker compose version
```

---

# Clone the Repository

```bash
git clone https://github.com/primetek-africa/database-lab
```

```bash
cd database-laboratory
```

---

# Environment Variables

Create a `.env` file in the project root.

Example:

```dotenv
POSTGRES_USER=academy_admin
POSTGRES_PASSWORD=academy123
POSTGRES_DB=academy_lab
POSTGRES_PORT=5432

PGADMIN_DEFAULT_EMAIL=admin@academy.com
PGADMIN_DEFAULT_PASSWORD=academy123
PGADMIN_PORT=5050

TIMEZONE=UTC
```

---

# Start the Containers

```bash
docker compose up -d
```

Verify that both containers are running.

```bash
docker ps
```

Expected containers:

- postgres-lab
- pgadmin4

---

# Access pgAdmin

Open your browser.

```
http://localhost:5050
```

Login credentials:

**Email**

```text
admin@academy.com
```

**Password**

```text
academy123
```

---

# Register PostgreSQL Server

Create a new server.

## General

Name

```text
Local PostgreSQL
```

## Connection

Host

```text
postgres
```

Port

```text
5432
```

Maintenance Database

```text
academy_lab
```

Username

```text
academy_admin
```

Password

```text
academy123
```

Save the server.

---

# Course Projects

Throughout the module, students will create several independent
databases.

Examples include:

- library_db
- electronics_store_db
- school_db
- hospital_db
- hotel_db
- ecommerce_db

Each project introduces new SQL concepts and database design techniques.

---

# Topics Covered

## Database Fundamentals

- Relational databases
- Database Management Systems
- SQL introduction
- PostgreSQL architecture
- pgAdmin

## Database Design

- Tables
- Columns
- Data types
- Constraints
- Keys
- Relationships

## SQL

- CREATE DATABASE
- CREATE TABLE
- ALTER TABLE
- DROP TABLE
- INSERT
- UPDATE
- DELETE
- SELECT

## Querying Data

- WHERE
- ORDER BY
- LIMIT
- LIKE
- BETWEEN
- IN
- AND
- OR

## Aggregate Functions

- COUNT
- SUM
- AVG
- MIN
- MAX

## Relationships

- One-to-One
- One-to-Many
- Many-to-Many

## Advanced SQL

- JOIN
- GROUP BY
- HAVING
- Views
- Indexes
- Transactions

---

# Typical Workflow

1. Create a database.
2. Create tables.
3. Insert records.
4. Query data.
5. Update records.
6. Delete records.
7. Create relationships.
8. Build complete database projects.

---

# Useful Docker Commands

Start containers

```bash
docker compose up -d
```

Stop containers

```bash
docker compose down
```

View running containers

```bash
docker ps
```

View logs

```bash
docker compose logs
```

Restart containers

```bash
docker compose restart
```

Remove containers

```bash
docker compose down -v
```

---

# Useful PostgreSQL Commands

List databases

```sql
\l
```

Connect to a database

```sql
\c database_name
```

List tables

```sql
\dt
```

Describe a table

```sql
\d table_name
```

Exit PostgreSQL

```sql
\q
```

---

# Best Practices

- Create one database for each project.
- Use meaningful table names.
- Define primary keys for every table.
- Use foreign keys to maintain relationships.
- Follow consistent naming conventions.
- Test SQL queries frequently.
- Backup important databases.
- Keep SQL scripts organized.

---

# Learning Outcomes

After completing this module, students will be able to:

- Design relational databases.
- Build normalized database schemas.
- Write SQL queries confidently.
- Retrieve and manipulate data.
- Create relationships between tables.
- Manage PostgreSQL databases.
- Use pgAdmin professionally.
- Integrate PostgreSQL with backend applications.

---

# License

This repository is intended for educational purposes as part of the
**PrimeTek Africa - Codecamp Academy** Advanced Full-Stack Software
Development program.