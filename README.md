# Json patch and thumbnail generator
Node.JS 
[![Build Status](https://travis-ci.com/Lundii/HackerBay-Interview-Round-1.svg?branch=develop)](https://travis-ci.com/Lundii/HackerBay-Interview-Round-1) [![Coverage Status](https://coveralls.io/repos/github/Lundii/HackerBay-Interview-Round-1/badge.svg)](https://coveralls.io/github/Lundii/HackerBay-Interview-Round-1)


## Pivotal Tracker Story Board
- https://www.pivotaltracker.com/n/projects/2399135

## Test locally
- clone this repository
- run `npm install` to get all necessary packages 
- create a .env file in the root folder and add the following environmental variables
   ```
    PORT=portnumber
    SECRET_KEY="a string used for generating JWT"
   ```
 - use `npm start` to start the application
 - use `npm test` to run test files
 - visit the urls below with the necessary body.

## APIs 

### Login - `POST {host}/api/v1/auth/login` - Login a user

body
```
  username: "string"
  password: "string"
```


### Json patch - `PATCH {host}/api/v1/user/json-patch` - patch a json object

body
```
  docs: "object"
  patch: "array of path operations"
```


### Thumbnail - `POST {host}/api/v1/user/thumbnail` - download and return a thumbnail

body
```
  imageUrl: "string"
```

## Swagger API documentation
- `GET {host}/api/v1/docs` 

## docker iamge 
- `docker pull lundii/hackerbay1:backend`
