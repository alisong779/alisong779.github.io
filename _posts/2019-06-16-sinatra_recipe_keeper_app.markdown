---
layout: post
title:      "Sinatra Recipe Keeper App"
date:       2019-06-17 00:50:34 +0000
permalink:  sinatra_recipe_keeper_app
---


My second portfolio project was a Recipe Keeper App built using the MVC (Model, View Controller) paradigm to create a Sinatra Framework. The MVC paradigm allows for seperation of concerns by grouping files according to their jobs and defining how they willl interact with each other. This project also uses ActiveRecord for database support, database mapping and creating association between Models. 

My Recipe Keeper App allows for the creation of user accounts. A user can signup, login and logout. I enabled the use of Sessions which creates a hash used to store user data on the server. The session secret is also set which is an encryption key used to create the session_id. The session id is set and unique to the users session. I used the Bcrypt gem to ensure that passwords are encrypted. Including the has_secure_password in the User model and password_digest in the users table stores the salted password in the database.

Once a user creates an account or logs in they can access the CRUD actions - Create, Read, Update or Delete/Destroy. The user can Create recipes, Edit recipes, Delete recipes and View recipes. The application ensures that a user can only CRUD their own recipes. 

I enjoyed working with Sinatra and ActiveRecord on this project. Organizing the routes, views and controllers properly can get a little tricky so it was important to draw things out on paper first. I also took some time to learn and include a little CSS so that my application didnt look too plain. Its quite an accomplishment to build an actual web application from scratch after only two months in this program. Sinatra and ActiveRecord simplify some really complicated operations and its nice to know whats going on behind the scenes! Im excited about continuing this journey and hopping into Rails!

