# Project on: SQL, JDBC and Hibernate

#### Task: 
we have a MySQL relational database with a schema (country-city, language by country). And there is a frequent query of the city, which slows down. We came up with a solution - to put all the data that are frequently queried into Redis (in memory storage of the key-value type).

#### The used software:
IDEA Ultimate,
Workbench,
Docker,
Redis.

#### Our plan of action:

- Configure the docker 
- Run the MySQL server as a docker container.
- Deploy the dump.
- Create a project in Idea, add maven dependencies.
- Make a domain layer.
- Write a method to get all data from MySQL.
- Write a method of data transformation (in Redis we will write only those data which are often requested).
- Run the Redis server as a docker container.
- Write the data into Redis.
- Optional: install redis-insight, look at the data stored in Redis.
- Write a method to retrieve data from Redis.
- Write a method to get data from MySQL.
- Compare the speed of getting the same data from MySQL and Redis.

___List of running containers___

![](https://github.com/GrSvitlana/db_project/blob/main/img/docker%20ps.png?raw=true)

***Database connection in IDEA***

![](https://github.com/GrSvitlana/db_project/blob/main/img/mysql.png?raw=true)

___Displaying keys and their values in Redis___

![](https://github.com/GrSvitlana/db_project/blob/main/img/redis.png?raw=true)

___Test results___

![](https://github.com/GrSvitlana/db_project/blob/main/img/test.png?raw=true)
