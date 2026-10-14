# Grocery Store Database

A relational database exercise modelling the core data and relationships of a grocery-store operation.

## Data Model

The schema covers:

- Employee positions and employees
- Customers and transactions
- Product groups and products
- Shopping carts and receipts

Primary keys and foreign-key constraints are defined in the schema to demonstrate relational integrity.

## SQL Scripts

| File | Purpose |
| --- | --- |
| [`01_create_tables.sql`](01_create_tables.sql) | Defines tables, columns and relationships |
| [`02_insert_data.sql`](02_insert_data.sql) | Populates the schema with sample records |
| [`03_updates_and_deletes.sql`](03_updates_and_deletes.sql) | Demonstrates targeted updates and deletes |

## Relationship Overview

```text
Position ──< Employee
                  │
Customer ──< Transaction >── Employee
                  │
Product Group ──< Product ──< Cart
                                  │
Transaction ────────────────< Receipt
```

## Concepts Demonstrated

- Data Definition Language (DDL)
- Data Manipulation Language (DML)
- Primary and foreign keys
- Entity relationships and schema design
- Updating and deleting targeted records

## Run Locally

The scripts use Oracle-style data types and date literals, so use an Oracle-compatible SQL environment.

Run the files in this order:

1. `01_create_tables.sql`
2. `02_insert_data.sql`
3. `03_updates_and_deletes.sql`

Review the update/delete statements before executing them, and use a test schema rather than a database containing important data.

## Project Status

A compact database-design exercise focused on relational modelling, constraints and basic data manipulation.
