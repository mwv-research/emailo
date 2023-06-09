<!-- Before starting to use this template, find and replace occurences of ABC wit your repo name (case sensitive) -->

<div align="center">
  <h1>Emailo</h1>
  <h3>Email Management System: Users can register & send emails to registered users.</a></h3>
</div>

## Contents

-   [Contents](#contents)
-   [Description](#description)
    -   [What's the problem we are trying to solve?](#whats-the-problem-we-are-trying-to-solve)
    -   [How can Emailo help?](#how-can-abc-help)
    -   [The idea](#the-idea)
-   [Project structure](#project-structure)
-   [Project roadmap](#project-roadmap)
-   [Getting started](#getting-started)
    -   [Prerequisites](#prerequisites)
        -   [Softwares needed](#softwares-needed)
        -   [Knowledge needed](#knowledge-needed)
    -   [Installing](#installing)
-   [Future Scope](#future-scope)
-   [Built with](#built-with)
-   [Contributing](#contributing)
-   [Authors](#authors)

## Description

\_ Email Management System: Users can register & send emails to registered users. User registration will be done after verifying their phone number with OTP send to their phone. A unique email will be generated by the system for the user. User can login using that email-id & password. Sending of emails is facilitated between registered users with the system. Email features included are: Sending Mails, Archive & Unarchive their mails, Fetch all mails sent & received by the user.

### What's the problem we are trying to solve?

\_ Many users wonder about the email-id or username they will keep while registering with a new system. 

### How can Emailo help?

\_ The system generates a unique email by itself for the user.

### The idea

\_ The system checks its database & collects the frequency of the duplicate entries of names already present. It then generates a email-id using user's first & last name. Email-id format: "firstname.lastname[count]@mindwebs.com"

## Project structure

The current project structure is as follows:

```
/
  ├── .github/                    scripts and configs for github templating and workflows
  ├── .nyc_output/                istanbul coverage output (generated on running npm run cover:test)
  ├── build/                      JS build of the project (generated on running npm run build)
  ├── coverage/                   istanbul coverage report (generated on running npm run cover:report)
  ├── docs/                       code documentation by typedoc (generated on running npm run docs)
  ├── node_modules/               directory that stores generated code of every node module
  ├── scripts/                    deploy scripts
  ├── src/
      ├── config/                 configurations for modules like db, swagger doc, etc go here
      ├── controllers/            controller functions for every route. controllers make calls to services
      ├── dtos/                   data transfer object definitions for cross function object passing
      ├── middlewares/            middlewares for various routes go here
      ├── models/                 database schema / models go here
      ├── routes/                 routes or endpoint definitions go here, routes make calls to controllers
      ├── services/               files that process and query the database go here
      ├── tests/                  directory for endpoint testing
        ├── fixtures/             for pre-defining data and environments for tests
        ├── integration/          for integration tests using BDD methodology
        ├── utils/                utility functions used for testing go here
      ├── views/                  the frontend of the project in EJS, CSS and js
      ├── utils/                  utility or helper functions go here
      ├── aether-api.ts           entry point to our expres app
  ├── .env.production             environment variables used in the project for prod
  ├── .env.development            environment variables used in the project for dev
  ├── .gitignore                  stores files and directories to be ignored in commits
  ├── .prettierrc                 configuration for prettier to help maintain a common code formatting
  ├── docker-compose.prod.yml     config file to define containers (for prod)
  ├── docker-compose.yml          config file to define containers
  ├── Dockerfile                  Docker commands to create the docker image go here
  ├── package.json                metadata of the project
  ├── package-lock.json           stores version of every package used in the project
  ├── readme.md                   details and instructions about the project go here
  ├── sonar-project.properties    configs for sonarqube, used for code quality analysis
  └── tsconfig.json               typescript configs

```

## Project roadmap

\_

## Getting started

\_ This section is for the development team or anyone wishing to browse the codebase or even contribute to it.

### Prerequisites

#### Softwares needed

-   Node and npm (ls/gallium)
-   Mongo DB and Compass
-   Postman/ ThunderClient

#### Knowledge needed

-   How REST APIs are written in node / ts
-   What authentication an authorization is
-   Microservices architecture and how it is better than Monolithic architecture
-   Service meshing and API Gateways

### Installing

\_ A step by step series of instructions that tell you how to get the project running locally is given below.

-   set the project directory up by cloning and creating .env.production and .env.development files, taking help from .env.example
-   run `npm install` to install all node modules used
-   read the scripts under package.json and use accordingly

## Future Scope

\_ Various Authentication ethods support-
-   Email Password Based JWT Token Authentication

## Built with

**Backend:**

-   [Express](https://expressjs.com/) - a NodeJS framework
-   [Mongo DB](https://www.mongodb.com/) and the [Mongoose](https://mongoosejs.com/) DOM

## Contributing

Please read [contributing.md](https://github.com/mindwebs/.github/contributing.md) for details on our code committing guidelines.

## Authors

<a href="https://mwv.one">
  <img src="https://avatars.githubusercontent.com/u/56452701?s=200&v=4" />
</a>
