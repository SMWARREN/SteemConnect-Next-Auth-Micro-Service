# NextAuth Example

## About NextAuth Example

This is an example of how to use the [NextAuth](https://www.npmjs.com/package/next-auth) module with [Sequelizejs](http://docs.sequelizejs.com/) and [SteemConnect](https://github.com/steemit/steemconnect)

## Getting Started

You can run this project like any other Next.js project but First update the environment variables by creating a file in this directory called **.env**. Follow the instructions below. Also create a new mysql database, with a username and password and also grant privileges to that user Sequelize will Handle the rest..

To run it locally, just use:

    nmp run dev

To run it it production mode, use:

    npm build
    npm start

## Using NextAuth

NextAuth is included in this project here:

* index.js

## Pages

This example includes the following pages:

* pages/index.js
* pages/auth/index.js
* pages/auth/error.js
* pages/auth/check-email.js
* pages/auth/callback.js

## Configuration

It also includes the following configuration files:

* next-auth.config.js
* next-auth.functions.js
* next-auth.providers.js

An example **.env** file is provided in **.env.example** which you can copy over to use for simple configuration:

```
DB_USER=
DB_PASS=
DB_NAME=
STEEMCONNECT_authorizationURL= https://steemconnect.com/oauth2/authorize
STEEMCONNECT_tokenURL= https://steemconnect.com/oauth2/token
STEEMCONNECT_clientID=  
STEEMCONNECT_clientSecret=  
STEEMCONNECT_callbackURL= http://localhost:3000/auth/oauth/oauth2/callback
SERVER_URL= http://localhost:3000
PORT=3000
DB_HOST=
DB_PORT=
FACEBOOK_ID=
FACEBOOK_SECRET=
GOOGLE_ID=
GOOGLE_SECRET=
TWITTER_KEY=
TWITTER_SECRET=
EMAIL_FROM=username@gmail.com
EMAIL_SERVER=smtp.gmail.com
EMAIL_PORT=465
EMAIL_USERNAME=username@gmail.com
EMAIL_PASSWORD=
```

If you don't specify oAuth or SMTP email details you will not be able to log in.
