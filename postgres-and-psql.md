# PostgreSQL

**Postgres** is the database engine and SQL (Structured Query Language) is the language used to interact with the database. SQL is used to manage data in **relational databases**. 

## Psql in the command line

To enter postgres in the command line, enter `psql`

Exit psql: `\q`

List all databases: `\l`

Create a new database: `CREATE DATABASE my-db;`

Connect to the database: `\c my-db`

Once connected to the database, the prompt should look like: `my_db=#`

From this point on, any SQL will run on the connected database. 

Displaying tables in a database: `\dt`

To view the schema of a table: `\d tableName`


## Using Postgres with a project

Make sure to connect to psql and the database starting in the project directory in the terminal, since we will need to run sql files that are within the project directory (ex. seeds).

To run sql files form a project in psql: 
`\i path_to_file/filename.sql`

For example to run the schema against an empty database: 
 `\i server/db/schema.sql`

 Then to run the seeds:
 `\i server/db/seeds.sql`
 
