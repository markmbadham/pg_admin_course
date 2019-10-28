# The Basics

## PostgreSQL exams

EnterpriseDB has Postgresql exams

[Exams](https://www.enterprisedb.com/training/postgres-certification)

- The associate exam must be taken first
- [Free Training Preparation for Associate Exam](https://www.enterprisedb.com/training/free-postgres-training)

## Why PostgreSQL?

- Open Source
- Flexible
- Powerful
- enterprise-class relational database management system
- application platform
- faster than or matches that of many other databases
- large set of data types including JSON
- can create custom data types
- a data type is created for each table
- support for non-relational data via extensions
    - ltree: graphs
    - hstore: key-value pair
- 20 years old
- platform independent
- new major release every year
- Can write stored procedures and functions in many languages
    + pgSQL / SQL
    + Tcl
    + Python
    + Perl
    + C
	+ C++
	+ R
	+ Java
	+ PHP
	+ Ruby
	+ Scheme

[Features](http://www.postgresql.org/about/featurematrix/)

[Limits](https://www.postgresql.org/docs/12/limits.html)

--

## Why Not PostgreSQL?

- Commercial support
- Transaction rates
- not suitable for installation on small devices
- security could be overkill for small applications
- not available on many shared-hosting environments

--

## Where to Get PostgreSQL

Can either be compiled from source or installed from binary packages. Easiest and recommended way is to install from latest, stable binary packages.

  [https://www.postgresql.org/download](https://www.postgresql.org/download)


  ```sh
  sudo yum install postgresql-server postgresql-contrib
  sudo postgresql-setup initdb
  sudo systemctl start postgresql
  ```
--

## Administration Tools
### psql

 - Useful with- command-line interface
- included in all distributions
- more detail: pg 276
- can import and export CSV files
- can generate HTML output
- powerful tool for expert users ssh

-- 

### Other shell commands

```sh
# man -k postgres | grep -v ':'
clusterdb (1)        - cluster a PostgreSQL database
createdb (1)         - create a new PostgreSQL database
createlang (1)       - define a new PostgreSQL procedural language
createuser (1)       - define a new PostgreSQL user account
dropdb (1)           - remove a PostgreSQL database
droplang (1)         - remove a PostgreSQL procedural language
dropuser (1)         - remove a PostgreSQL user account
initdb (1)           - create a new PostgreSQL database cluster
oid2name (1)         - resolve OIDs and file nodes in a PostgreSQL data directory
pg_archivecleanup (1) - clean up PostgreSQL WAL archive files
pg_basebackup (1)    - take a base backup of a PostgreSQL cluster
pg_controldata (1)   - display control information of a PostgreSQL database cluster
pg_createcluster (8) - create a new PostgreSQL cluster
pg_ctl (1)           - start, stop, or restart a PostgreSQL server
pg_ctlcluster (8)    - start/stop/restart/reload a PostgreSQL cluster
pg_dropcluster (8)   - completely delete a PostgreSQL cluster
pg_dump (1)          - extract a PostgreSQL database into a script file or other archive file
pg_dumpall (1)       - extract a PostgreSQL database cluster into a script file
pg_isready (1)       - check the connection status of a PostgreSQL server
pg_lsclusters (1)    - show information about all PostgreSQL clusters
pg_receivexlog (1)   - streams transaction logs from a PostgreSQL cluster
pg_resetxlog (1)     - reset the write-ahead log and other control information of a PostgreSQL database cluster
pg_restore (1)       - restore a PostgreSQL database from an archive file created by pg_dump
pg_standby (1)       - supports the creation of a PostgreSQL warm standby server
pg_test_fsync (1)    - determine fastest wal_sync_method for PostgreSQL
pg_updatedicts (8)   - build PostgreSQL dictionaries from myspell/hunspell ones
pg_upgrade (1)       - upgrade a PostgreSQL server instance
pg_upgradecluster (8) - upgrade an existing PostgreSQL cluster to a new major version.
pg_virtualenv (1)    - Create a throw-away PostgreSQL environment for running regression tests
pg_wrapper (1)       - wrapper for PostgreSQL client commands
pg_xlogdump (1)      - Display a human-readable rendering of the write-ahead log of a PostgreSQL database cluster
pgbench (1)          - run a benchmark test on PostgreSQL
pgsql_table (5)      - Postfix PostgreSQL client configuration
postgres (1)         - PostgreSQL database server
postgresql-common (7) - wrapper for PostgreSQL client commands
postgresqlrc (5)     - Per-user PostgreSQL cluster configuration
postmaster (1)       - PostgreSQL database server
psql (1)             - PostgreSQL interactive terminal
reindexdb (1)        - reindex a PostgreSQL database
user_clusters (5)    - File linking users to PostgreSQL clusters
vacuumdb (1)         - garbage-collect and analyze a PostgreSQL database
vacuumlo (1)         - remove orphaned large objects from a PostgreSQL database
```

`man` is a commandline tool for getting help on a shell command.  For any of the above command you can use man to get more information.  For example:

`man postgres`

 --

### pgAdmin
 - https://www.pgadmin.org/
 - Genral GUI admin tool
 - graphical client
- platform independent
- installs a web server and works through a web-browser
- user-friendly but can't do everything the command-line client can
- creation, maintenance and use of database objects
- manage users
- manage permissions
- ad-hoc maintenance including VACUUM, ANALYZE, REINDEX and CLUSTER
- import and export of data
- backup and restore
- query tool
- can install optional pgAgent on the server for job scheduling

[Free e-book](https://www.syncfusion.com/ebooks/postgres) guide to PostgreSQL admin using pgAdmin.


### phpPgAdmin
 - http://phppgadmin.sourceforge.net/doku.php
 - Web based admin tool
 - Often supplied by hosting companies

--

### Adminer
 - https://www.adminer.org/
 - Works with MySQL, MariaDB, PostgreSQL, SQLite, MS SQL, Oracle, SimpleDB, Elasticsearch, MongoDB

--

### DBeaver
 - https://dbeaver.io
 - https://github.com/dbeaver/dbeaver/wiki

--

## PostgreSQL Database Objects
 - Schemas
 - Tables
 - Views
 - Functions
 - Sequence

--

## What’s New in Latest Versions of PostgreSQL?
### Why Upgrade?
 - Features
 - Bugs
 - End of Life

https://www.postgresql.org/support/versioning/

--

### Features Introduced in PostgreSQL 12

[Release Notes](https://www.postgresql.org/docs/10/release-12.html)

### Features Introduced in PostgreSQL 11

[Release Notes](https://www.postgresql.org/docs/10/release-11.html)

### Features Introduced in PostgreSQL 10

[Release Notes](https://www.postgresql.org/docs/10/release-10.html)

### Features Introduced in PostgreSQL 9.6

[Release Notes](https://www.postgresql.org/docs/9.6/release-9-6.html)

### Features Introduced in PostgreSQL 9.5

[Wiki](https://wiki.postgresql.org/wiki/What%27s_new_in_PostgreSQL_9.4)

### Features Introduced in PostgreSQL 9.4

[Wiki](https://wiki.postgresql.org/wiki/What%27s_new_in_PostgreSQL_9.4)

--

## Database Drivers

- ODBC
- JDBC - JAVA
- .NET
- Python
- PHP
- Perl
And many more

--

## Where to Get Help

 - [Postgres Community](https://www.postgresql.org/list/pgsql-general/)
 - Commercial Support
   - [EnterpriseDB](https://www.enterprisedb.com/)
   - [Cybertec](https://www.cybertec-postgresql.com/)

## Notable PostgreSQL Forks

 - Redshift, Amazon
 - EnterpriseDB
 - [Wiki](https://wiki.postgresql.org/wiki/PostgreSQL_derived_databases)

--

# Database Administration
## Configuration Files

CENTOS: /var/lib/pgsql/data
 - postgresql.conf - Main Configuration file
 - pg_hba.conf - Host Based Authentication
 - pg_ident.conf - User Maps
  
~/
 - .pgpass - Stored password for auto login
 - .psql_history - previous psql commands for user
 - .psqlrc - local configuration for the psql client software.

--

### Making Configurations Take Effect

Most changes require a reload, i.e. just reread config files.
Some changes e.g. bind to different interface require restart.

Reload
- `pgctl reload`
- `SELECT pg_reload_conf();`
- `systemctl resload postgresql-10` - Recommended on CENTOS

Restart
 - `systemctl restart postgresql-10` - Recommended on CENTOS

### The postgresql.conf File

This is the main configuration file for the PostgreSQL Server.

On CENTOS you can edit the file using VI or Nano as follows:

`vim /var/lib/pgsql/11/data/postgresql.conf`

or 

`nano /var/lib/pgsql/11/data/postgresql.conf`

The file contains name and key value pairs like:

- `listen_address = 'localhost'`
  
Tuning params include:
 - max_connections = 100
 - shared_buffers = 2GB
 - effective_cache_size = 6GB
 - maintenance_work_mem = 512MB
 - checkpoint_completion_target = 0.9
 - wal_buffers = 16MB
 - default_statistics_target = 100
 - random_page_cost = 1.1
 - effective_io_concurrency = 200
 - work_mem = 5242kB
 - min_wal_size = 1GB
 - max_wal_size = 2GB
 - max_worker_processes = 4
 - max_parallel_workers_per_gather = 2
 - max_parallel_workers = 4
 
Good staring values for these params can be obtained from:
[pgTune](https://pgtune.leopard.in.ua)

 --

### The pg_hba.conf File

Controls who can connect to each database and from where.
Consists of rows with the following fields.

`TYPE  DATABASE USER ADDRESS METHOD`

--

TYPE:
 - local - using the unix socket
 - host - connection over TCP/IP socket ssl optional
 - hostssl, hostnossl -  ssl not optional
  

DATABASE
 - "all" 
 - "sameuser"
 - "samerole"
 - "replication" 
 - database name
 - comma-separated list 

-- 

USER

 - "all"
 - a user name
 - a group name prefixed with "+" 
 - comma-separated list

file name prefixed with "@" to include names from a separate file.

--

METHOD
 - "trust"
 - "reject"
 - "md5"
 - "password"
 - "scram-sha-256"
 - "gss"
 - "sspi"
 - "ident"
 - "peer"
 - "pam"
 - "ldap"
 - "radius"
 - "cert".

--

## Managing Connections

 - view activity
    - `pg_stat_activity;`
- `pg_<terminate|cancel>_backend`

- Config Parameters
    - deadlock_timeout
    - statement_timeout
    - lock_timeout
    - idle_in_transaction_session_timeout

--

## Check for Queries Being Blocked

 - New features to pg_stat_activities

## Roles

 - Role based access control.
    - user is a role that can login
    - group is role with members
    - a role may be both

### Creating Login Roles

- CREATE ROLE
    - LOGIN - is a user i.e. can login
    - PASSWORD - followed by password
    - CREATDB - user can create databases.
- CREATE USER - same 
- `man createuser` shell command

### Creating Group Roles

- CREATE ROLE/GROUP
- GRANT group_role TO user_role
- SET ROLE

## Database Creation

- CREATE DATABASE
- createdb shell command

## Template Databases

 - default template1
 - CREATE DATABASE db_name TEMPLATE my_template

## Using Schemas

- `CREATE SCHEMA schema_name`
- `show search_path`
- `SET search_path schema_name`



## Privileges
### Types of Privileges

GRANT `ALL` includes:
- SELECT
- INSERT 
- UPDATE
- ALTER
- DELETE
- TRUNCATE
- EXECUTE

TO:
- role

ON:
 - DATABASE (does not necessarily include tables in db)
 - TABLE 
 - TABLES in SCHEMA
 - columns

WITH GRANT OPTION:
- allows user to give permissions to others

CREATE privilege is given using CREATE or ALTER
DROP privilege resides the the OWNER of the database.




## Extensions
### Installing Extensions

```sh
sudo yum install postgesql11-contrib
```

Using pg_stat_statements extensios
[Article](https://www.cybertec-postgresql.com/en/3-ways-to-detect-slow-queries-in-postgresql/) 

### Common Extensions
## Backup and Restore
### Selective Backup Using pg_dump
 
Can create either a plain text SQL dump or a custom format backup:

 - `pg_dump database_name` "SQL dump"
 - `pg_dump -Fc database_name` Custom format
 - `pg_dump -Fd` use directory i.e. mutiple files.

### Creating a porable SQL dump file

 We can compress the output of an SQL dump using `pg_dump` and an external file:

 ```sh
$  sudo -u postgres pg_dump northwind > northwind_dump.sql
$  sudo -u postgres pg_dump northwind | gzip > northwind_dump.sql.gz
$  sudo -u postgres pg_dump northwind | bzip2 > northwind_dump.sql.bz2
$  sudo -u postgres pg_dump northwind | compress > northwind_dump.sql.Z
$ ls -sh  northwind_dump.sql*
208K northwind_dump.sql   36K northwind_dump.sql.bz2   48K northwind_dump.sql.gz   48K northwind_dump.sql.gz.bz2   76K northwind_dump.sql.Z

 ```
 ### Using the "Custom format"

Sing file backup

 ```sh
$  sudo -u postgres pg_dump -Fc northwind -f northwind.backup
```

Multi file backup (1 file per table)

```sh
$  sudo -u postgres pg_dump -Fd northwind -f backup/
```

Viewing the output
```sh
$ ls -l northwind.backup backup/
-rw-rw-r--. 1 student student 55523 Oct 25 10:25 northwind.backup

backup/:
total 76
-rw-rw-r--. 1 student student   250 Oct 25 10:28 3756.dat.gz
-rw-rw-r--. 1 student student  5328 Oct 25 10:28 3757.dat.gz
-rw-rw-r--. 1 student student  1312 Oct 25 10:28 3758.dat.gz
-rw-rw-r--. 1 student student 11219 Oct 25 10:28 3759.dat.gz
-rw-rw-r--. 1 student student 20227 Oct 25 10:28 3760.dat.gz
-rw-rw-r--. 1 student student  2011 Oct 25 10:28 3761.dat.gz
-rw-rw-r--. 1 student student   103 Oct 25 10:28 3762.dat.gz
-rw-rw-r--. 1 student student  2102 Oct 25 10:28 3763.dat.gz
-rw-rw-r--. 1 student student    25 Oct 25 10:28 3764.dat.gz
-rw-rw-r--. 1 student student 12251 Oct 25 10:28 toc.dat

 ```

### Systemwide Backup Using pg_dumpall

see `man pg_dumpall`
- SQL dump format
- includes database creation commands


### Restoring Data from SQL dump

Typically a `pg_dump` packup is restored into an empty data base:

```sh
createdb -U admin restore;
psql -U admin restore < northwind_dump.sql
```
or
```sh
zcat northwind_dump.sql.gz | psql -U admin restore 
```

or
```sh
bzcat northwind_dump.sql.bz2 | psql -U admin restore 
```


### Restoring Data from custom format backup

Restore usine the `pg_restore` command

```sh
sudo -u postgres pg_restore -d northwind /tmp/northwind.backup
```


## Managing Disk Storage with Tablespaces

Table spaces are alternate disk locations where tables or entire databases may be stored

### Creating Tablespaces

```sh
postgres=# \h create tablespace
Command:     CREATE TABLESPACE
Description: define a new tablespace
Syntax:
CREATE TABLESPACE tablespace_name
    [ OWNER { new_owner | CURRENT_USER | SESSION_USER } ]
    LOCATION 'directory'
    [ WITH ( tablespace_option = value [, ... ] ) ]
```

### Moving Objects Among Tablespaces

```sh
ALTER DATABASE name SET TABLESPACE new_tablespace

ALTER TABLE ... name ...  SET TABLESPACE new_tablespace
```


## Verboten Practices

- Don’t Delete PostgreSQL Core System Files and Binaries
- Don’t Grant Full OS Administrative Privileges to the Postgres System Account (postgres)
- Don’t Set shared_buffers Too High
- Don’t Try to Start PostgreSQL on a Port Already in Use

# psql
## Environment Variables
## Interactive versus Noninteractive psql
## psql Customizations
### Custom Prompts
### Timing Executions
### Autocommit Commands
### Shortcuts
### Retrieving Prior Commands
## psql Gems
### Executing Shell Commands
### Watching Statements
### Retrieving Details of Database Objects
### Crosstabs
### Dynamic SQL Execution
## Importing and Exporting Data
### psql Import
### psql Export
### Copying from or to Program
## Basic Reporting


# Using pgAdmin
## Getting Started
### Overview of Features
### Connecting to a PostgreSQL Server
### Navigating pgAdmin
## pgAdmin Features
### Autogenerating Queries from Table Definitions
### Accessing psql from pgAdmin3
### Editing postgresql.conf and pg_hba.conf from pgAdmin3
### Creating Database Assets and Setting Privileges
### Import and Export
### Backup and Restore
## pgScript
## Graphical Explain
## Job Scheduling with pgAgent
### Installing pgAgent
### Scheduling Jobs
### Helpful pgAgent Queries


# Data Types

## Numerics

### Serials
PostgreSQL - SERIAL - Generate IDs (Identity, Auto-increment) SERIAL data type allows you to automatically generate unique integer numbers (IDs, identity, auto-increment, sequence) for a column.

### Generate Series Function

```sh
SELECT * 
FROM generate_series(1, 5);
 generate_series
-----------------
               1
               2
               3
               4
               5
```


## Textuals
### String Functions
### Splitting Strings into Arrays, Tables, or Substrings
### Regular Expressions and Pattern Matching
## Temporals
### Time Zones: What They Are and Are Not
### Datetime Operators and Functions
## Arrays
### Array Constructors
### Unnesting Arrays to Rows
### Array Slicing and Splicing
### Referencing Elements in an Array
### Array Containment Checks
## Range Types
### Discrete Versus Continuous Ranges
### Built-in Range Types
### Defining Ranges
### Defining Tables with Ranges
### Range Operators
## JSON
### Inserting JSON Data
### Querying JSON
### Outputting JSON
### Binary JSON: jsonb
### Editing JSONB data
## XML
### Inserting XML Data
### Querying XML Data
## Full Text Search
### FTS Configurations
### TSVectors
### TSQueries
### Using Full Text Search
### Ranking Results
### Full Text Stripping
### Full Text Support for JSON and JSONB
## Custom and Composite Data Types
### All Tables Are Custom Data Types
### Building Custom Data Types
### Composites and NULLs
### Building Operators and Functions for Custom Types

# Tables, Constraints, and Indexes
## Tables
### Basic Table Creation
### Inherited Tables
### Partitioned Tables
### Unlogged Tables
### TYPE OF
## Constraints
### Foreign Key Constraints
### Unique Constraints
### Check Constraints
### Exclusion Constraints
## Indexes
### PostgreSQL Stock Indexes
### Operator Classes
### Functional Indexes
### Partial Indexes
### Multicolumn Indexes

# SQL: The PostgreSQL Way

see [Tutorial Intro to PostgreSQL](https://www.postgresql.org/docs/10/tutorial.html)

## Views
### Using Triggers to Update Views

Using rules:
```sh
CREATE [ OR REPLACE ] RULE name AS ON event
    TO table [ WHERE condition ]
    DO [ ALSO | INSTEAD ] { NOTHING | command | ( command ; command ... ) }
```

### Materialized Views
## Handy Constructions
### DISTINCT ON
### LIMIT and OFFSET
### Shorthand Casting
### Multirow Insert
### ILIKE for Case-Insensitive Search
### ANY Array Search
### Set-Returning Functions in SELECT
### Restricting DELETE, UPDATE, and SELECT from Inherited Tables
### DELETE USING
### Returning Affected Records to the User
### UPSERTs: INSERT ON CONFLICT UPDATE
### Composite Types in Queries
### Dollar Quoting
### DO
### FILTER Clause for Aggregates
### Percentiles and Mode
## Window Functions
### PARTITION BY
### ORDER BY
## Common Table Expressions
### Basic CTEs
### Writable CTEs
### Recursive CTE
## Lateral Joins
## WITH ORDINALITY
## GROUPING SETS, CUBE, ROLLUP
# Writing Functions
## Anatomy of PostgreSQL Functions
### Function Basics
### Triggers and Trigger Functions
### Aggregates
### Trusted and Untrusted Languages
## Writing Functions with SQL
### Basic SQL Function
### Writing SQL Aggregate Functions
### Writing PL/pgSQL Functions
## Basic PL/pgSQL Function
### Writing Trigger Functions in PL/pgSQL
## Writing PL/Python Functions
### Basic Python Function
## Writing PL/V8, PL/CoffeeScript, and PL/LiveScript Functions
### Basic Functions
### Writing Aggregate Functions with PL/V8
### Writing Window Functions in PL/V8

# Query Performance Tuning
## EXPLAIN
### EXPLAIN Options
### Sample Runs and Output
### Graphical Outputs
## Gathering Statistics on Statements
## Writing Better Queries
### Overusing Subqueries in SELECT
### Avoid SELECT `*`
### Make Good Use of CASE
### Using FILTER Instead of CASE
## Parallelized Queries
### What Does a Parallel Query Plan Look Like?
### Parallel Scans
### Parallel Joins
## Guiding the Query Planner
### Strategy Settings
### How Useful Is Your Index?
### Table Statistics
### Random Page Cost and Quality of Drives
## Caching
# Replication and External Data
## Replication Overview
 - transaction plug slony, pg_pool
 - log shipping copy wall file to the remote machine
 - 1 streaming replication
 - logical replication

## Replication Jargon
## Evolution of PostgreSQL Replication
## Third-Party Replication Options
## Setting Up Full Server Replication
## Configuring the Master
## Configuring the Slaves for Full Server Cluster Replication
## Initiating the Streaming Replication Process
## Replicating Only Some Tables or Databases with Logical Replication
## Foreign Data Wrappers
## Querying Flat Files
## Querying Flat Files as Jagged Arrays
## Querying Other PostgreSQL Servers
## Querying Other Tabular Formats with ogr_fdw
## Querying Nonconventional Data Sources

# Appendices
## A. Installing PostgreSQL
- Windows and Desktop Linux
- CentOS, Fedora, Red Hat, Scientific Linux
- Debian, Ubuntu
- FreeBSD
- macOS

-- 

## B. PostgreSQL Packaged Command-Line Tools
Database Backup Using pg_dump
Server Backup: pg_dumpall
Database Restore: pg_restore
psql Interactive Commands
psql Noninteractive Commands