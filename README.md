# api-to-database-quotes-example
This integration takes a set of Quotes from a Mock REST API and inserts them into a SQL Server Database table. This project can be repurposed for any data type beyond just Quotes. Be sure to clear the database table of Quotes before moving the data.

This project requires creating a mock API to pass the data from. This is the site I use to create mock API endpoints: https://mockapi.io/projects

I've included a database SQL schema in the "dbSQLSchema" folder in src/main/resources which should allow you to easily create the MySQL database table required for this use case

This project includes notable "extras" including a For Each loop to process records independently and "Upsert" logic that checks if a matching record already exists before inserting / updating the DB
