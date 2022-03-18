
The code for this repo is taken from [Spring Boot Database Migrations with Flyway Example | JavaTechie](https://www.youtube.com/watch?v=w12DsiqpxEg) 
to understand and get started using flyway by implementing a simple database migration.


### flyway_schema_history

flyway keeps a separate table <b>flyway_schema_history</b> to track the database changes. It
refers this table to evaluate from which point it needs to start applying the database version changes as deltas like git.

### Setup

Create a database with name <em>sample</em> in mysql on your local.
Update the application.properties with database access credentials 


### Simulation

Run this commit locally and notice that <em>flyway_schema_history</em> table is created in <em>sample</em> database

Also notice the USERS table and SOCIAL_SECURITY table being populated as per
<em>resources/db/migration/V1.1__createTable.sql</em>


### References
 
1. [Spring Boot Database Migrations with Flyway Example | JavaTechie](https://www.youtube.com/watch?v=w12DsiqpxEg)

2. [Flyway website](https://flywaydb.org/)
