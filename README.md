# Typist
Typing web-game - race against your friends! Play now: https://typist-app.herokuapp.com

# Build / Development Setup
## Server .env
A .env file is not required to run this project in development. The project is setup to have fallbacks in the case where a .env is not present. For instance, if variables such as a MongoDB connection string are not present, the app will fire up a memory mongo server (a local mongodb installation is not required). However, a .env file can be added at the root of the ```server``` directory should you wish to specify particular vairables when running the project in development. Variables used are:

```
NODE_ENV=<development | production | test>
PORT=<http port to start the server on>
DB_STRING_production=<production mongodb conn string>
DB_STRING_test=<test mongodb conn string>
DB_STRING_development=<development mongodb conn string>
```

## Project Startup
``` bash
# server
cd server

# install dependencies
npm install

# install nodemon globally
npm install nodemon -g

# start with hot reload at localhost:3000
npm run dev

# client
cd client

# install dependencies
npm install

# install vue-cli
npm install -g @vue/cli

# start with hot reload at localhost:8080
npm run serve
```

# Test Setup
## Local Unit Tests
There are unit & integration tests for both server and client directories. As above, if no test MongoDB string is provided - an in-memory mongodb will be started and used.

``` bash
# server
cd server

# install dependencies
npm install

# run unit tests
npm run test:unit

# run integration tests
npm run test:integration

# client
cd client

# install dependencies
npm install

# run unit tests
npm run test
```

## Azure Pipeline
The Microsoft Azure CI Pipeline for this project can be found at: https://dev.azure.com/tobybessant/Typist/_build
