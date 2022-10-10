# :clock9: OkiPunch
- Functionalities: 
- 
:cloud: Employee side: show employee salary summary, punch out, show employee attendance on calendar, edit employee infomation

***some of the examples***

<img width="312" alt="emSummary" src="https://user-images.githubusercontent.com/106992258/194916597-226b0aa7-2e75-43b1-ad11-3ee60162c113.png">

<img width="343" alt="calendar" src="https://user-images.githubusercontent.com/106992258/194916605-5640cdb9-5105-48cb-b645-edec0f9825b8.png">


:cloud: Company side: show all employee, punch in with redis, show employee calendar record, edit employee attendance, edit employee infomation, create new employee account

***some of the examples***

<img width="348" alt="showWorker" src="https://user-images.githubusercontent.com/106992258/194916632-9be6e577-b195-42b6-a81d-1bdd98e56c75.png">

<img width="325" alt="punchIn" src="https://user-images.githubusercontent.com/106992258/194916694-0dd9796e-a83a-442e-8fdf-6387dd6c6d1a.png">

<img width="338" alt="addNewWorker" src="https://user-images.githubusercontent.com/106992258/194916722-d452f60b-4802-4fb2-b4c3-ec743b0c9881.png">


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

** note **
** using incognito open company side (http://localhost:8000/company_login) **
** using normal bowser open employee side (http://localhost:8000/employee_login) **

### Start the App:

`logo site: http://localhost:8000/logo`
`root site: http://localhost:8000 `

### Account:
- :office: Company:  :bust_in_silhouette: ac: com@com  :key: pw: com
- :construction_worker: Employee: :bust_in_silhouette: ac: em@em   :key: pw: em
- *** more accounts find on /seeds ***
