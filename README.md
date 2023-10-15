# Docker Compose Nodejs and Postgres example

## Run the System
We can easily run the whole with only a single command:
```bash
docker compose up
```

Docker will pull the Postgres and Node.js images (if our machine does not have it before).

The services can be run on the background with command:
```bash
docker compose up -d
```

## Stop the System
Stopping all the running containers is also simple with a single command:
```bash
docker compose down
```

If you need to stop and remove all containers, networks, and all images used by any service in <em>docker-compose.yml</em> file, use the command:
```bash
docker compose down --rmi all
```

For more detail, please visit:
> [Docker Compose Node.js and Postgres example](https://www.bezkoder.com/docker-compose-nodejs-postgres/)

Related Posts:
> [Node.js, Express & PostgreSQL: CRUD Rest Api example](https://www.bezkoder.com/node-express-sequelize-postgresql/)

> [Node.js Express Pagination with PostgreSQL example](https://www.bezkoder.com/node-js-pagination-postgresql/)

> [Import CSV data into PostgreSQL using Node.js](https://www.bezkoder.com/node-js-csv-postgresql/)

> [Export PostgreSQL data to CSV file using Node.js](https://www.bezkoder.com/node-js-export-postgresql-csv-file/)

> [Node.js JWT Authentication & Authorization with PostgreSQL example](https://www.bezkoder.com/node-js-jwt-authentication-postgresql/)

Associations:
> [Sequelize Associations: One-to-Many Relationship example](https://bezkoder.com/sequelize-associate-one-to-many/)

> [Sequelize Associations: Many-to-Many Relationship example](https://bezkoder.com/sequelize-associate-many-to-many/)
