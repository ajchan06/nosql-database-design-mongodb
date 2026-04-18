# SQL Data Analysis & Schema Extension – Music Database System

## Overview
This project demonstrates relational database design, schema extension, and advanced SQL querying using a music database.

It extends an existing dataset by introducing a new entity (`MusicVideo`) and performs real-world data analysis using joins, aggregations, and Common Table Expressions (CTEs).

The project focuses on how structured data systems can be expanded and queried to generate meaningful insights.

---

## Key Features
- Extended an existing relational schema using foreign key constraints
- Designed a new entity (`MusicVideo`) using generalization
- Inserted and validated relational data with integrity checks
- Performed advanced SQL queries (JOIN, GROUP BY, CTEs)
- Analyzed customer behavior and music trends

---

## Database Extension

### MusicVideo Table
A new table was created to represent tracks that have associated music videos.

- Each MusicVideo maps directly to a Track
- Enforced using a foreign key relationship
- Cascade delete ensures referential integrity

Schema:
- TrackId (Primary Key, Foreign Key)
- VideoDirector

---

## Data Operations

### Manual Inserts
Inserted multiple music videos with associated directors.

### Dynamic Insert
Added a music video by querying the TrackId dynamically:
- Prevents duplicate entries
- Ensures correctness without hardcoding IDs

---

## Query Analysis

### Pattern Matching
Identified tracks containing accented characters in their names.

### JOIN Queries
Linked tracks with their corresponding music video directors.

### Aggregation (GROUP BY)
Calculated the number of music videos per album.

### Advanced Queries (CTEs)

#### Customer Analysis
Identified customers who purchased tracks longer than the average duration (excluding extreme outliers).

#### Genre Analysis
Filtered tracks that are not part of the top 5 genres based on average duration.

---

## Key Concepts Demonstrated
- Relational schema extension
- Foreign key constraints with cascading behavior
- Data integrity and normalization
- Multi-table JOIN operations
- Aggregation and grouping
- Common Table Expressions (CTEs)
- Subqueries and filtering logic

---

## What I Learned
- How to extend an existing database schema safely
- Writing efficient and readable SQL queries
- Using CTEs to simplify complex logic
- Applying SQL to real-world data analysis problems
- Maintaining data integrity in relational systems

---

## Future Improvements
- Add indexing for performance optimization
- Build a backend API to expose queries
- Integrate a frontend dashboard for visualization
- Extend to NoSQL (MongoDB) for comparison

---

## Tech Stack
- SQLite
- SQL (Joins, Aggregations, CTEs)

---

## Author
Anthony Chan  
Computer Science, Northeastern University
