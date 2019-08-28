---
layout: post
title:      "Rails with Javascript"
date:       2019-08-28 17:30:18 +0000
permalink:  rails_with_javascript
---


This project was fun! I added a comments model to my application so that users can add comments to recipes. Then, using asynchronous javascript, I added to my recipe show page the ability to render the comment form, display all comments for the recipe or to view an individual comment. I also enhanced the original application by adding the ability to dynamically add ingredients to a recipe on creation using a gem called nested_fields_for. I had a delay at the start of the project with getting my comments to properly render json and to post to the api. It was a matter of making sure you fetch the right API and having all routes in routes.rb and controller set up properly. Once I got all of that set up correctly I added links with listeners to the comments index so that a user can click the comment to view its contents. It was a challenge to set up the functions correctly, ensuring all fetching, document queries, and method calls were written and placed as needed. Once all functions were working it became clear to me how creative you can be using asynchronous javascript and APIs...Using data from a backend rails app to render dynamic content...pretty cool!

