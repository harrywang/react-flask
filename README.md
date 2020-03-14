# About
code for tutorial: https://blog.miguelgrinberg.com/post/how-to-create-a-react--flask-project

Basic steps:

- create react starter folder using `create-react-app`
- create flask starter folder (see below)
- edit `package.json`: 1. proxy react server at 3000 to flask server at 5000, 2. add flask command to yarn

## Setup

Install the followings:

Node.js: The JavaScript runtime that you will use to run your frontend project.
Yarn: A package and project manager for Node.js applications.
Python: A recent Python 3 interpreter to run the Flask backend on.

React frontend:

```
$ npx create-react-app react-frontend
$ cd react-frontend
$ yarn start
```
I made this folder the root of this repo.

Note: I ran into this problem: https://github.com/facebook/create-react-app/issues/8086 and solved it by `npm uninstall -g create-react-app`

Flask backend：

```
$ python3 -m venv venv
$ source venv/bin/activate
$ pip install -r requirements.txt
$ flask run
```

- The .flaskenv file, which Flask automatically imports into the environment on startup if it finds the python-dotenv package installed. FLASK_ENV variable enables Flask's debug mode.

## Start

In two different terminals start frontend and backend:

```
$ yarn start
$ yarn start-api
```
