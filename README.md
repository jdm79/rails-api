# README

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


## How to make a Rails API

```
$ rails new my-rails-api --api --database=postgresql
$ cd my-rails-api
$ rake db:migrate
$ rails g scaffold Post title:string body:text
$ rake db:setup
$ rails s
```

Then in Postman (other products are available):

address: http://localhost:3000/posts/

In the body of the POST request (the big empty box I feel is the best way to describe it), type

{"post": {"title": "mr postman", "body":"hello world!"}}

Be sure to click 'raw' and JSON (application/json) from the dropdown.

![POST request screenshot](https://github.com/jdm79/rails-api/blob/master/public/post-request.png)


![GET request screenshot](https://github.com/jdm79/rails-api/blob/master/public/get-request.png)


