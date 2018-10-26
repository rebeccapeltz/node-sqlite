# sequelize-sqlite-express-vue

A silly toy contacts management application that I used in my [StackAbuse](stackabuse.com) blog article [Using Sequelize.js and SQLite in an Express.js App](http://stackabuse.com/using-sequelize-js-and-sqlite-in-an-express-js-app/) demonstrating how to use Vue.js, Node.js, Express.js and sequelize.js in combination with a SQLite database.

## Usage

1) Clone repo

```sh
git clone https://github.com/amcquistan/sequelize-sqlite-express-vue.git
```

2) install dependencies (Built with Node.js version 8.10)

```sh
cd sequelize-sqlite-express-vue/
npm install
```

3) run migrations and seeders

```sh
node_modules/.bin/sequelize db:migrate
node_modules/.bin/sequelize db:seed:all
```

4) start express server

```sh
npm start
```

<!-- https://stackabuse.com/using-sequelize-js-and-sqlite-in-an-express-js-app/ -->

npm install --save express body-parser sequelize sequelize-cli sqlite3 nodemon

### generate a model
node_modules/.bin/sequelize model:generate --name Contact --attributes firstName:string,lastName:string,phone:string,email:string

### add table to sqllite
node_modules/.bin/sequelize db:migrate

### run sqlite3 from the command line
sqlite3 database.sqlite3 ??

### create dummy data
node_modules/.bin/sequelize seed:generate --name seed-contact

### run migrations and populate database with seed data
node_modules/.bin/sequelize db:seed:all

### npm start

### node with sql lite
https://stackabuse.com/a-sqlite-tutorial-with-node-js/