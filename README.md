# OkiPunch

### Install Node Packages

`npm install express-flash express passport bcrypt express-session express-handlebars knex dotenv express-session passport-local path pg redis`

### setup for DB connect

- 3 variables in .env
  `DB_NAME, DB_USERNAME, DB_PASSWORD`

- set up dummy data, run:
  `knex migrate:latest`
  `knex seed:run`

### setup for Redis connect

- change direction to your current redis version
  `cd redis-7.0.4`
- start the server
  `redis-server --daemonize yes`
- open the cli to interact with the server
  `redis-cli`

### Use two browser for company admin side and employee admin side separately

**_note_**
**_ using incognito open company side (http://localhost:8000/company_login) _**
**_ using normal bowser open employee side (http://localhost:8000/employee_login) _**

### Start the App:

`logo site: http://localhost:8000/logo`
`root site: http://localhost:8000 `
