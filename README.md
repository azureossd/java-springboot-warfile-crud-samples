# SpringBootWarfileDatabaseExamples

Spring Boot .WAR file based CRUD applications using different database providers that are deployed and tested on Azure.

Below is a list of accessible endpoints for CRUD operations.

#### `mysql` Usage
Create an [Azure Database for MySQL](https://docs.microsoft.com/en-us/azure/mysql/) instance and set the following environment variables in the `application.yml` file to the below:
 - `${MYSQL_HOST}`: The host name of your MySQL server
 - `${MYSQL_DATABASE_NAME}`: The name of your MySQL database. The `mysql` example uses 'springbootwarfiletasks'. Refer to the `mysql/database` folder.
 - `${MYSQL_USER}`: The MySQL username
 - `${MYSQL_PASSWORD}`: Your MySQL password


- Routes:
   - `/` - Root path
   - `/api/mysql/task/find` - `GET` request to retrieve all todos
   - `/api/mysql/task/find/{id}` - `GET` request to retrieve a todo by ID
   - `/api/mysql/task/delete/{id}` - `DELETE` request to remove a todo by ID
   - `/api/mysql/task/update/{id}` - `PUT` request to update a todo by ID
   - `/api/mysql/task/add` - `POST` request to add a new todo

#### `postgres` Usage

Create an [Azure Database for PostgreSQL](https://docs.microsoft.com/en-us/azure/postgresql/overview) instance and set the following environment variables in the `application.yml` file to the below:
 - `${POSTGRES_HOST}`: The host name of your Postgres server
 - `${POSTGRES_DATABASE_NAME}`: The name of your Postgres database. The `postgres` example uses 'springbootwarfiletasks'. Refer to the `postgres/database` folder.
 - `${POSTGRES_USER}`: The Postgres username
 - `${POSTGRESL_PASSWORD}`: Your Postgres password

- Routes
   - `/` - Root path
   - `/api/postgres/task/find` - `GET` request to retrieve all todos
   - `/api/postgres/task/find/{id}` - `GET` request to retrieve a todo by ID
   - `/api/postgres/task/delete/{id}` - `DELETE` request to remove a todo by ID
   - `/api/postgres/task/update/{id}` - `PUT` request to update a todo by ID
   - `/api/postgres/task/add` - `POST` request to add a new todo
