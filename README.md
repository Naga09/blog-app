blog-app Rest API
===========

### install npm and node 
` https://nodejs.org/en/download/ `



### get the blog-app api repo

 git clone git@github.com:Naga09/blog-app.git

 cd blog-app/

###To install the packages

npm install

### To start the server

node server.js.



### To post a blog

```
curl -H "Content-Type: application/json" -X POST -d '{"title":"i am the title of the blog","body":"i am the body of the blog"}' http://localhost:8089/blog

```

### to get all the blogs

```
curl -i "localhost:8089/blogs"

```
