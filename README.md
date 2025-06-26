First, we are starting the query with START TRANSACTION to wrap all the code inside a transaction. Then, we are checking if tables: movies, albums, and media_library exist. If they exist already, we are dropping them with the DROP statement.

Then, we are creating three tables using CREATE TABLE statements for movies, albums, and media_library. We are adding columns to "media_library" with movies_id and albums_id, later we are making them foreign key with FOREIGH KEY statement that REFERENCES to movies(id) and albums(id).

In order to check out our query, we are inserting some data into the tables we created. Finally, we are finishing up the transaction with the ROLLBACK keyword, later we can use COMMIT to confirm our changes. 