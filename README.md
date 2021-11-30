# Simple Node with Express Server with REST https://teams.microsoft.com/l/meetup-join/19%3ameeting_ZTI2MzJhOTktMjU0NS00YzBkLThkYzQtNzMzNzEzZWY3YzE3%40thread.v2/0?context=%7b%22Tid%22%3a%2293f33571-550f-43cf-b09f-cd331338d086%22%2c%22Oid%22%3a%22fad9cfd8-29c0-4c3e-9ccf-b8fb8656f561%22%7d


[![Build Status](https://travis-ci.org/rwieruch/node-express-server-rest-api.svg?branch=master)](https://travis-ci.org/rwieruch/node-express-server-rest-api) [![Slack](https://slack-the-road-to-learn-react.wieruch.com/badge.svg)](https://slack-the-road-to-learn-react.wieruch.com/) [![Greenkeeper badge](https://badges.greenkeeper.io/rwieruch/node-express-server-rest-api.svg)](https://greenkeeper.io/)

An easy way to get started with a Express server offering a REST API with Node.js. [Read more about it.](https://www.robinwieruch.de/node-express-server-rest-api)

## Features

- Express
- REST API

## Requirements

- [node & npm](https://nodejs.org/en/)
- [git]

## Installation
- `cd node-express-server-rest-api`
- `npm install`
- `npm start`
- optional: include _.env_ in your _.gitignore_

### GET Routes

- visit http://localhost:3000
  - /messages
  - /messages/1
  - /users
  - /users/1

### Beyond GET Routes

#### CURL

- Create a message with:
  - `curl -X POST -H "Content-Type:application/json" http://localhost:3000/messages -d '{"text":"Hi again, World"}'`
- Delete a message with:
  - `curl -X DELETE -H "Content-Type:application/json" http://localhost:3000/messages/1`

#### Postman

- Install [Postman](https://www.getpostman.com/apps) to interact with REST API
- Create a message with:
  - URL: http://localhost:3000/messages
  - Method: POST
  - Body: raw + JSON (application/json)
  - Body Content: `{ "text": "Hi again, World" }`
- Delete a message with:
  - URL: http://localhost:3000/messages/1
  - Method: DELETE
