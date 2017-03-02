# Mongodb profiler queries
This is a set of queries useful to get a quick understanding of the output of the MongoDB profiler. You just have to use the queries given in the source file in order to dig into the MongoDB profiler data.

## MongoDB profiler
This tool, provided with MongoDB, is used to log all queries that are considered as *slow*. By default, a slow query is a query with an execution time greater than 100ms. The logs are stored in the `system.profile` collection.
To enable the profiler on one of your database, connect on your mongodb instance thanks to the `mongo` utility and run `db.setProfilingLevel(1)`. More info [here](https://docs.mongodb.com/manual/tutorial/manage-the-database-profiler/).

## Queries
The queries provided on the Javascript source file allow you to get a quick overview of the profiler output :
- Print the slowest and fastest queries ;
- Get information on operations (amount of insert, queries, etc) ;
- Find the queries that may need an index ;
- Get information about the waiting lock time ;
- Get detailled database size on disk.

Feel free to use it ;-)