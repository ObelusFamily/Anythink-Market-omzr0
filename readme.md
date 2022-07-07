# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

1. [Install Docker](https://docs.docker.com/get-docker/).
2. Run `docker-compose up` from the project root. This will take a while.
3. Now you need to migrate the database in the backend container. To do this,
   1. SSH into the backend container: `docker exec -it anythink-backend /bin/bash`
   2. Get into the backend dir: `cd backend`.
   3. Run migrations: `bundle exec rake db:migrate`
4. 
