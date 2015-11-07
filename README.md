# AngularJS Best-Practice App Package

---

### Table of Contents
* [What is this?](#what-is-this)
* [Features](#features)
* [Requirements](#requirements)
* [Installation](#installation)
* [Run Application and start development Server](#run-application-and-start-development-server)
* [Run Tests](#run-tests)
* [Run UI Tests](#run-ui-tests)
* [Build Application for Deployment](#build-application-for-deployment)
* [Why bower AND npm?](#why-bower-and-npm)
* [Bugs / Feature request](#bugs--feature-request)

---

## What is this?
This small AngularJS application contains some simple examples explaining the components of angular.
It tries to use the best-practice design pattern for everything and is inspired by following projects:
- [johnpapa/angular-styleguide](https://github.com/johnpapa/angular-styleguide)
- [angular/angular-seed](https://github.com/angular/angular-seed)
- [paislee/healthy-gulp-angular](https://github.com/paislee/healthy-gulp-angular)
- [Gregor Woiwode](https://github.com/GregOnNet)

## Features
Beside the AngularJS demonstrations this package even contain a complete setup.
Usable as template for future projects.
Containing:
- dependency loading and startup with [npm](http://npmjs.com) and [bower](http://bower.io)
- better IDE support with `jshint` by `.jshintrc` file
- included simple development web-server with [node.js](http://nodejs.org) and [express](http://expressjs.com)
- testing angular with [jasmin](https://jasmine.github.io) and [karma](https://karma-runner.github.io)
- ui testing with [jasmin](https://jasmine.github.io) and [protractor](https://angular.github.io/protractor)
- deployment build with [gulp](http://gulpjs.com)

## Requirements
You need [node.js](http://nodejs.org) with [npm](http://npmjs.com) on your machine.
For some automatically npm builds you will even need a version of [python](http://www.python.org) installed, but this is not necessary to run the app itself.

## Installation
This app will install all required dependencies automatically. 
Just start the commands below in the root folder where you stored the package.
``SH
$ npm install
``

## Run Application and start development Server
To run this app in your browser just start everything whit the comment below in the applications root folder.
It will update everything an start a simple web server on ``http://localhost:1337/``
``SH
$ npm start
``

## Run Tests
All unit tests are performed with [jasmin](https://jasmine.github.io) and [karma](https://karma-runner.github.io).
Predefined are dependencies for `PhantomJS`, `Firefox` and `Chrome`.
You might define the environment variables `FIREFOX_BIN` and `CHROME_BIN` to locate your browsers correctly.

Run command below to execute all unit test:
``SH
$ npm test
``

## Run UI Tests
All end-to-end tests are performed with [jasmin](https://jasmine.github.io) and [protractor](https://angular.github.io/protractor).
Make sure your development web-server and `webdriver-manager` is running.
You will need three open shells. 
**Start Web-Server:**
``SH
$ npm start
``
**Start Webdriver-Manager:**
``SH
$ npm run start-webdriver
``
**Execute e2e tests:**
``SH
$ npm run protractor
``

## Build Application for Deployment
// ToDo

## Why bower AND npm?
It is possible to do everything by `package.json` over `npn`.
But the idea is to split the dependencies in development and browser/client files.
So `npm` contains everything for development, and `bower` defines the dependencies available to the user in browser.

## Bugs / Feature request
Please [report](http://github.com/eisbehr-/angular-best-practice/issues) bugs and feel free to [ask](http://github.com/eisbehr-/angular-best-practice/issues) for new features directly on GitHub.
