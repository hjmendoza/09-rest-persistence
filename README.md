![cf](https://i.imgur.com/7v5ASc8.png) Lab 09: Vanilla REST API w/ Persistence - Haley Mendoza

[![Build Status](https://travis-ci.com/hjmendoza/09-rest-persistence.svg?branch=master)](https://travis-ci.com/hjmendoza/09-rest-persistence)

TRAVIS: https://travis-ci.com/hjmendoza/09-rest-persistence
HEROKU: https://haley-09-rest-persistence.herokuapp.com/
PR: https://github.com/hjmendoza/09-rest-persistence/pull/1


#### Feature Tasks
* created an HTTP server using the native NodeJS `http` module
* created a custom parser module that:
  * uses promises to parse the JSON body of `POST` and `PUT` requests
  * uses the NodeJS `url` and `querystring` modules to parse the request url
* created a router constructor that allows you to register custom routes for `GET`, `POST`, `PUT`, and `DELETE` requests
* created a data model constructor that creates a _simple resource_ (e.g. notes) with at least 3 properties
* created a data model storage interface that can store data through different storage mechanisms.
  * created storage modules for in-memory and file-system storage

## Server Endpoints
### `/api/vi/simple-resource-name
* `POST` request
 * pass data as stringifed JSON in the body of a **POST** request to create a new resource
* `GET` request
 * pass `?id=<uuid>` as a query string parameter to retrieve a specific resource (as JSON)
* `DELETE` request
 * pass `?id=<uuid>` in the query string to **DELETE** a specific resource
 * this should return a 204 status code with no content in the body

## To Start Application
Clone down code
Install node dependencies
Create a .env file and define `PORT` and `storage`
Run app from terminal using `npm start`. View app at `http://localhost:<PORT>`
Test restful routes by quering at localhost:<PORT>/api/v1/notes or through httpie or postman



