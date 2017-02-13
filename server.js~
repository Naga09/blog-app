

var express = require('express');
var blogapp = express();
var cookieParser = require('cookie-parser');
var bodyParser = require('body-parser');
var db_file = "blog.db";

// sqllite middleware
var sqlite3 = require('sqlite3').verbose();
var db = new sqlite3.Database(db_file);

// body-parser middlewares

blogapp.use(bodyParser.json());
blogapp.use(bodyParser.urlencoded({extended: false}));
blogapp.use(cookieParser());


// creating the blog table
db.serialize(function() {
    db.run("CREATE TABLE IF NOT EXISTS blogs (post_id INTEGER, title TEXT, body TEXT)");
});




// Server listening at 8089
blogapp.listen(8089);

console.log("Server is running on port 8089...");



