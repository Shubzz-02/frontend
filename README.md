# Nodejs login-register
A simple Login/Register application developed in Nodejs using Express and deployed on Azure Web App service, using GitHub Actions.
Click Here[https://frontendappavail.azurewebsites.net/home] to access website and here[] for Github Action[.github/workflows/docker-hub.yml] file

### Installing dependencies:
Enter this command it will install all the dependencies at once:

```
npm install
```
Or you can install them individually:

```
npm install express express-session mysql pug-cli bcrypt util.promisify
```

Sometimes you get errors and access denied add sudo to the command

```
sudo npm install express express-session mysql pug-cli bcrypt util.promisify
```

### Start the application

```
npm start
```
or
```
node app
```
### Database

For this application the database  name is 'www', it contains only one table 'users'

Go to core/pool.js enter your database username and password, you can use you own database name just make sure it's the same in the pool.js file so you can connect to database.

### Setting up the database

You can use PhpMyAdmin just import the database.sql file includes in the project directory

Use those queries:

```
CREATE DATABASE www;
```
```
USE www;
```
```
CREATE TABLE users (id int AUTO_INCREMENT, username varchar(20), fullname varchar(20), password varchar(128), PRIMARY KEY (id));
```

if you correcty setting up the database you shouldn't get any errors.
