# Celestial Bodies Database 🌌

A PostgreSQL relational database project completed as part of the freeCodeCamp Relational Database curriculum.

## Project Overview

The Celestial Bodies Database is designed to represent astronomical objects and their relationships, including galaxies, stars, planets, moons, and asteroids.

The project demonstrates practical relational database design and SQL skills through table creation, data modeling, constraints, and relationships.

## Database Structure

The database consists of five tables:

| Table      | Description                                                                    |
| ---------- | ------------------------------------------------------------------------------ |
| `galaxy`   | Stores galaxy information, including name, type, age, and whether it has life. |
| `star`     | Stores star information and its relationship with galaxies.                    |
| `planet`   | Stores planet information and its relationship with stars.                     |
| `moon`     | Stores moon information and its relationship with planets.                     |
| `asteroid` | Stores asteroid information, discovery year, and description.                  |

## Entity Relationships

* Each star can reference a galaxy through `galaxy_id`.
* Each planet can reference a star through `star_id`.
* Each moon can reference a planet through `planet_id`.
* Each table has a primary key.
* Unique constraints prevent duplicate names within each table.

## Technologies Used

* PostgreSQL
* SQL

## SQL Concepts Applied

* Database and table creation
* Primary Keys and Foreign Keys
* One-to-Many Relationships
* UNIQUE Constraints
* Sequences and Auto-increment IDs
* Data Types and Boolean Values
* Inserting and managing relational data

## Project Structure

```text
celestial-bodies-database/
│
├── universe.sql
└── README.md
```

## How to Run

1. Install PostgreSQL.
2. Open the SQL script using `psql` or a compatible PostgreSQL client.
3. Execute `universe.sql` to create and populate the database.

**Note:** The script includes `DROP DATABASE universe`, so make sure you do not have an existing database with that name containing data you need to keep.

## Learning Outcomes

* Gained practical experience with PostgreSQL.
* Improved understanding of relational database design.
* Applied primary and foreign key constraints.
* Practiced modeling relationships between multiple entities.

---

**Course:** freeCodeCamp – Relational Database
**Status:** Completed
