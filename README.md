The compose setup used for Aventum development purposes, it uses `nodemon` on the server and dev server on the dashboard for live/hot reloading.

Inside `dashboard` folder create `src` folder and put [Aventum Dashboard](https://github.com/TryAventum/dashboard) source code in it.

Inside `server` folder create `src` folder and put [Aventum Server](https://github.com/TryAventum/server) source code in it.

> The environment variable COMPOSE_CONVERT_WINDOWS_PATHS=1 in `.env` file, it is for Docker For Windows only.

> Use `docker-compose -f docker-compose.postgres.yml up` to use PostgreSQL or use `docker-compose -f docker-compose.mongodb.yml up` to use MongoDB if you want to rebuild add `--build` to the end of the command like `docker-compose -f docker-compose.postgres.yml up --build`, the app will be accessed through http://localhost

> **THE FIRST PAGE TO VISIT AFTER docker-compose up IS COMPLETED IS http://localhost/setup IN ORDER OR SETUP THE SUPER USER!**

> Just replace http://localhost with you url, for example http://mydomain.com
