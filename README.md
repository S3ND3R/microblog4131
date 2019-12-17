# microblog4131

## Group Member
Warren Weber

## Project Type
I completed a C project

## Live link to microblog tutorial project
https://flask-microblog4131.herokuapp.com/

## Git code repository
https://github.com/S3ND3R/microblog4131

## Controllers
login: handles logging a user into the Microblog application by accessing the
user table.  
index: Controls the home page view. The index accesses the post and user table
allowing users to post a new message and see messages that have been posted.  
register: accesses the User table to allow users to register.  
user: accesses the user table to select about me message, last seen time stamp,
and following. It handles displaying avatars.  
edit_profile: Handles altering the about me values in the database  
follow: Handles altering the following relationship in the database to add a new
follower given that they exist and are not the current user.  
unfollow: Handles altering the following relationship in the database to remove
a follower given that they exist and are not the current user.  
explore: Access the Posts table to display all posts that have been entered.  

## Views


## Tables

# Reference
https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world
