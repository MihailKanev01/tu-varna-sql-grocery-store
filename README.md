# Grocery Store Database

A relational SQL database exercise modelling the core data of a grocery-store operation.

## Overview

The database models:

- employee positions
- employees
- customers
- transactions
- product groups
- products
- shopping carts
- receipts

Primary keys and foreign-key constraints are defined directly in the schema.

## What is demonstrated

### DDL

[`01_create_tables.sql`](01_create_tables.sql) creates the relational schema and defines:

- primary keys
- foreign keys
- column types
- relationships between entities

### DML

[`02_insert_data.sql`](02_insert_data.sql) populates the database with sample positions, employees, customers, transactions, products, carts and receipts.

[`03_updates_and_deletes.sql`](03_updates_and_deletes.sql) demonstrates:

- UPDATE statements
- DELETE statements
- targeted record changes

## Data model

```text
Position ──< Employee
                  │
Customer ──< Transaction >── Employee
                  │
Product Group ──< Product ──< Cart
                                  │
Transaction ────────────────< Receipt
```

## File structure

```text
01_create_tables.sql
02_insert_data.sql
03_updates_and_deletes.sql
```

## How to use it

Run the scripts in order:

1. Create the tables with `01_create_tables.sql`.
2. Insert sample data with `02_insert_data.sql`.
3. Apply the update/delete examples from `03_updates_and_deletes.sql`.

The SQL syntax includes Oracle-style data types and date literals, so an Oracle-compatible SQL environment is the appropriate target.

## Project status

A compact database-design and SQL exercise focused on relational modelling, constraints and basic data manipulation.

## License

See [LICENSE](LICENSE).
