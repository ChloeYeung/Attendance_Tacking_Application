# :clock9: OkiPunch
- Functionalities: 

:cloud: Employee side: show employee salary summary, punch out, show employee attendance on calendar, edit employee infomation

***Employee Side Examples***

- Employee Login
<img width="289" alt="emLlogin" src="https://user-images.githubusercontent.com/106992258/195580663-6675d0c8-9fdc-4898-8e4f-5b6ff6671888.png">


- Employee Summary
<img width="300" alt="emSummary_punch" src="https://user-images.githubusercontent.com/106992258/195580623-8dcaa69e-ac24-4273-96c2-4710e0364fe7.png">

- Employee Calendar
<img width="319" alt="emCalendar" src="https://user-images.githubusercontent.com/106992258/195580631-2f7d569a-10fc-4dd1-97b3-7926e83707d7.png">

- Employee Edit info
<img width="284" alt="emEdit" src="https://user-images.githubusercontent.com/106992258/195580687-b184e260-6ed1-414e-a917-c7292534f3ea.png">


:cloud: Company side: show all employee, punch in with redis, show employee calendar record, edit employee attendance, edit employee infomation, create new employee account

***Company Side Examples***

- Company Login
<img width="298" alt="comLogin" src="https://user-images.githubusercontent.com/106992258/195580785-ed7f4b48-1ea0-464f-84e3-0ac43a7c213f.png">


- Company Show all employee
<img width="293" alt="comShowAllEm" src="https://user-images.githubusercontent.com/106992258/195580801-ed10f743-5ade-4b0f-88c3-0b3fe1d0fa3d.png">

- Company Calendar
<img width="300" alt="comcalendar" src="https://user-images.githubusercontent.com/106992258/195580858-1fe3cd82-0316-4aa8-bede-66072ffc1ff4.png">

- Company Edit info
<img width="295" alt="comEdit" src="https://user-images.githubusercontent.com/106992258/195580893-2c489e73-bc14-4326-99d7-d9a055623483.png">

- One time password punch in
<img width="1228" alt="comPunchin" src="https://user-images.githubusercontent.com/106992258/195580910-107d04c3-1549-468e-b899-62af64c5b204.png">


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

note :
- using incognito open company side (http://localhost:8000/company_login)
- using normal bowser open employee side (http://localhost:8000/employee_login)

### Start the App:

`logo site: http://localhost:8000/logo`
`root site: http://localhost:8000 `

### Account:
- :office: Company:  :bust_in_silhouette: ac: com@com  :key: pw: com
- :construction_worker: Employee: :bust_in_silhouette: ac: em@em   :key: pw: em
- (more accounts find on /seeds)
