# The Basics
## Why PostgreSQL?
## Why Not PostgreSQL?
## Where to Get PostgreSQL
## Administration Tools
### psql
### pgAdmin
### phpPgAdmin
### Adminer
### DBeaver

## PostgreSQL Database Objects
## What’s New in Latest Versions of PostgreSQL?
### Why Upgrade?
### Features Introduced in PostgreSQL 10
### Features Introduced in PostgreSQL 9.6
### Features Introduced in PostgreSQL 9.5
### Features Introduced in PostgreSQL 9.4
## Database Drivers
## Where to Get Help
## Notable PostgreSQL Forks

# Database Administration
## Configuration Files
### Making Configurations Take Effect
### The postgresql.conf File
### The pg_hba.conf File
## Managing Connections
## Check for Queries Being Blocked
## Roles
### Creating Login Roles
### Creating Group Roles
## Database Creation
## Template Databases
Using Schemas
Privileges
Types of Privileges
Getting Started
GRANT
Default Privileges
Privilege Idiosyncrasies
Extensions
Installing Extensions
Common Extensions
Backup and Restore
Selective Backup Using pg_dump
Systemwide Backup Using pg_dumpall
Restoring Data
Managing Disk Storage with Tablespaces
Creating Tablespaces
Moving Objects Among Tablespaces
Verboten Practices
Don’t Delete PostgreSQL Core System Files and Binaries
Don’t Grant Full OS Administrative Privileges to the Postgres System Account (postgres)
Don’t Set shared_buffers Too High
Don’t Try to Start PostgreSQL on a Port Already in Use
3. psql
Environment Variables
Interactive versus Noninteractive psql
psql Customizations
Custom Prompts
Timing Executions
Autocommit Commands
Shortcuts
Retrieving Prior Commands
psql Gems
Executing Shell Commands
Watching Statements
Retrieving Details of Database Objects
Crosstabs
Dynamic SQL Execution
Importing and Exporting Data
psql Import
psql Export
Copying from or to Program
Basic Reporting
4. Using pgAdmin
Getting Started
Overview of Features
Connecting to a PostgreSQL Server
Navigating pgAdmin
pgAdmin Features
Autogenerating Queries from Table Definitions
Accessing psql from pgAdmin3
Editing postgresql.conf and pg_hba.conf from pgAdmin3
Creating Database Assets and Setting Privileges
Import and Export
Backup and Restore
pgScript
Graphical Explain
Job Scheduling with pgAgent
Installing pgAgent
Scheduling Jobs
Helpful pgAgent Queries
5. Data Types
Numerics
Serials
Generate Series Function
Textuals
String Functions
Splitting Strings into Arrays, Tables, or Substrings
Regular Expressions and Pattern Matching
Temporals
Time Zones: What They Are and Are Not
Datetime Operators and Functions
Arrays
Array Constructors
Unnesting Arrays to Rows
Array Slicing and Splicing
Referencing Elements in an Array
Array Containment Checks
Range Types
Discrete Versus Continuous Ranges
Built-in Range Types
Defining Ranges
Defining Tables with Ranges
Range Operators
JSON
Inserting JSON Data
Querying JSON
Outputting JSON
Binary JSON: jsonb
Editing JSONB data
XML
Inserting XML Data
Querying XML Data
Full Text Search
FTS Configurations
TSVectors
TSQueries
Using Full Text Search
Ranking Results
Full Text Stripping
Full Text Support for JSON and JSONB
Custom and Composite Data Types
All Tables Are Custom Data Types
Building Custom Data Types
Composites and NULLs
Building Operators and Functions for Custom Types
6. Tables, Constraints, and Indexes
Tables
Basic Table Creation
Inherited Tables
Partitioned Tables
Unlogged Tables
TYPE OF
Constraints
Foreign Key Constraints
Unique Constraints
Check Constraints
Exclusion Constraints
Indexes
PostgreSQL Stock Indexes
Operator Classes
Functional Indexes
Partial Indexes
Multicolumn Indexes
7. SQL: The PostgreSQL Way
Views
Single Table Views
Using Triggers to Update Views
Materialized Views
Handy Constructions
DISTINCT ON
LIMIT and OFFSET
Shorthand Casting
Multirow Insert
ILIKE for Case-Insensitive Search
ANY Array Search
Set-Returning Functions in SELECT
Restricting DELETE, UPDATE, and SELECT from Inherited Tables
DELETE USING
Returning Affected Records to the User
UPSERTs: INSERT ON CONFLICT UPDATE
Composite Types in Queries
Dollar Quoting
DO
FILTER Clause for Aggregates
Percentiles and Mode
Window Functions
PARTITION BY
ORDER BY
Common Table Expressions
Basic CTEs
Writable CTEs
Recursive CTE
Lateral Joins
WITH ORDINALITY
GROUPING SETS, CUBE, ROLLUP
8. Writing Functions
Anatomy of PostgreSQL Functions
Function Basics
Triggers and Trigger Functions
Aggregates
Trusted and Untrusted Languages
Writing Functions with SQL
Basic SQL Function
Writing SQL Aggregate Functions
Writing PL/pgSQL Functions
Basic PL/pgSQL Function
Writing Trigger Functions in PL/pgSQL
Writing PL/Python Functions
Basic Python Function
Writing PL/V8, PL/CoffeeScript, and PL/LiveScript Functions
Basic Functions
Writing Aggregate Functions with PL/V8
Writing Window Functions in PL/V8
9. Query Performance Tuning
EXPLAIN
EXPLAIN Options
Sample Runs and Output
Graphical Outputs
Gathering Statistics on Statements
Writing Better Queries
Overusing Subqueries in SELECT
Avoid SELECT *
Make Good Use of CASE
Using FILTER Instead of CASE
Parallelized Queries
What Does a Parallel Query Plan Look Like?
Parallel Scans
Parallel Joins
Guiding the Query Planner
Strategy Settings
How Useful Is Your Index?
Table Statistics
Random Page Cost and Quality of Drives
Caching
10. Replication and External Data
Replication Overview
Replication Jargon
Evolution of PostgreSQL Replication
Third-Party Replication Options
Setting Up Full Server Replication
Configuring the Master
Configuring the Slaves for Full Server Cluster Replication
Initiating the Streaming Replication Process
Replicating Only Some Tables or Databases with Logical Replication
Foreign Data Wrappers
Querying Flat Files
Querying Flat Files as Jagged Arrays
Querying Other PostgreSQL Servers
Querying Other Tabular Formats with ogr_fdw
Querying Nonconventional Data Sources
A. Installing PostgreSQL
Windows and Desktop Linux
CentOS, Fedora, Red Hat, Scientific Linux
Debian, Ubuntu
FreeBSD
macOS
B. PostgreSQL Packaged Command-Line Tools
Database Backup Using pg_dump
Server Backup: pg_dumpall
Database Restore: pg_restore
psql Interactive Commands
psql Noninteractive Commands