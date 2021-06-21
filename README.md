## Table of Contents
1. [General Info](#general-info)
2. [Screenshot](#screenshot)
3. [Built With](#built-with)
4. [Usage](#usage)
5. [Deployment](#deployment)

## General Info
#### `#MERN compactLinks`
> *MERN compactLink app was created using MERN stack technologies.
> The state management functionality of this app was built with advanced level of using [React Hooks](https://reactjs.org/docs/hooks-intro.html). 
The app was created to compact links for a specific user to make them more organised and easy to use.* 

## Screenshot


## Built With
* [React](https://reactjs.org/docs/getting-started.html) - a popular JS frontend library for building composable and highly reusable component-based UIs for SPA.
* [MongoDB](https://www.mongodb.com) - a cross-platform document-oriented database. 
* [Node.js](https://nodejs.org/en/about/) - a back-end JavaScript runtime environment that runs on the V8 engine for a fast execution of JavaScript code outside a web browser.
* [Express.js](https://expressjs.com/) - a back end web application framework for Node.js.
* [Heroku](https://www.heroku.com/) - a fully managed container-based cloud platform used to deploy and run you back-end applications.
* [Materialize](https://materializecss.com/) - A modern responsive front-end framework based on Material Design for mobile and desktop React web applications.

## Usage
* To clone and run this application, you need **npm/node** installed, **MongoDB** account for managing database, **Heroku** account for **Node.js** and **React** backend and frontend deployments.
* Add your own strings for the DB **mongoUri** and **jwtSecret** to the **'config'** file. From your command line:

````sh
# Install dependencies for server
npm install

# Install dependencies for client
npm run client

# Run the client & server concurrently
npm run dev

# Run the Express server only
npm run server

# Run the React client only
npm run client

# Server runs on http://localhost:5000 and client on http://localhost:3000
````

## Deployment
Inside app 'server' create a new file called **'.gitignore'** and add in there unnecessary for uploading **node_modules/**
Add 1 more file called **'Procfile'** and in there type: **web: npm run start** to make app to start as soon as it's deployed.

##### #Heroku
````sh
# Login in Heroku account and 'Create new app'

# Download and Install Heroku CLI

# From app 'server' terminal login into Heroku CLI
heroku login
heroku git:remote -a <your app name>

# Continue process from 'server' terminal
git add .
git commit -m "init"
git push heroku master
