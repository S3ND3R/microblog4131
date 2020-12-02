# microblog4131

## Group Member
Warren Weber

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
\_post.html: this view controls how posts are displayed to the user  
404.html: This view displays an error message when a file cannot be found.  
500.html: This view displays when an error has occurred on the server end.  
base.html: The base view for the page that contains the navigation bar that appears
on all the pages.  
edit_profile.html: the view displayed when the user wants to change their profile  
index.html: the view that displays a form for entering new text message posts.
It also displays all the users post and the posts of those they are following.  
login.html: Displays the form for logging in the user  
register.html: Displays the form for registering the user.  
user.html: Displays the user's page that contains their profile, avatar, last seen date,
number they are following and being followed by, and posts.  

## Tables
* User
  * ID - primary key for user
  * username - name of the user
  * email- users email
  * password hash - hash of the users password
  * posts - posts relationship
  * about me - user profile
  * last seen - time last visited
  * following - following relationship
* Posts
  * ID - primary key for Posts
  * body: text of the posts
  * timestamp: time of posts
  * user_id: foreign key connected to user table
* Follower Relationship
  * user id for follower
  * user id for followed

# Reference
https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world
