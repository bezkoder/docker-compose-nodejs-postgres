# Docker Compose Nodejs and Postgres example

## How to run

### Run the System
We can easily run the whole with only a single command:
```bash
docker compose up
```

Docker will pull the Postgres and Node.js images (if our machine does not have it before).

The services can be run on the background with command:
```bash
docker compose up -d
```

### Stop the System
Stopping all the running containers is also simple with a single command:
```bash
docker compose down
```

If you need to stop and remove all containers, networks, and all images used by any service in <em>docker-compose.yml</em> file, use the command:
```bash
docker compose down --rmi all
```

## Developing locally
If you want to only run the postgres container run:
```bash
docker compose up postgresdb -d
```

Then you can run the application using [nodemon](https://www.npmjs.com/package/nodemon). This allows you to devop in the application and it will automatically restart when you save a file.

To add the config for the applciation, create a `.env` file inside the `bezkoder-app` folder with the following contents:

```ini
DB_HOST=localhost
DB_USER=postgres
DB_PASSWORD=123456
DB_NAME=bezkoder_db
DB_PORT=5433

NODE_DOCKER_PORT=8080
```

Note this has the same keys as the `.env.sample` file and the same values as the `.env` file from the root of the repo.

To run the application, first navigate to the application folder where `package.json` resides. e.g.

```bash
cd bezkoder-app
```

Then download the dependencies and run the application locally (provided [nodeJS](https://nodejs.org/en/download) is installed):

```bash
npm install
npm run dev
```

## Additional resources

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
