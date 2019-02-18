# How to make a Rails API

## Create the Rails API 
```
$ rails new my-rails-api --api --database=postgresql
$ cd my-rails-api
```
## Create the schema
```
$ rake db:migrate
```
## Create the Post model and controller
```
$ rails g scaffold Post title:string body:text
```
## Create the database
```
$ rake db:setup
```

The API is now ready to go, so let's run the server:
```
$ rails s
```

We can now build a frontend (and/or mobile app) which can interact with our API. Or for now we can just use something like Postman app which gives us frontend functionality immediately, so we can test our API.

## How to send and receive requests using Postman

In Postman (other products are available):

Use this address: http://localhost:3000/posts/

## How to POST a message

Choose 'POST' from the dropdown on the left of the browser address box. In the body of the POST request (the big empty box I feel is the best way to describe it), type
```
{"post": {"title": "mr postman", "body":"hello world!"}}
```
Be sure to click 'raw' and JSON (application/json) from the dropdown and click 'SEND'. It should look something like this:

![POST request screenshot](https://github.com/jdm79/rails-api/blob/master/public/post-request.png)

## How to GET all posts

Choose 'GET' from the dropdown on the left of the browser address box. Use this address: http://localhost:3000/posts/ (same as for the POST request). All posts in the database will be displayed. It should look something like this:

![GET request screenshot](https://github.com/jdm79/rails-api/blob/master/public/get-request.png)




# README (to be filled in later)

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...




