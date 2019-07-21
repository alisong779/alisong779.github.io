---
layout: post
title:      "Rails Project Week"
date:       2019-07-21 23:28:20 +0000
permalink:  rails_project_week
---


I will forever refer to my Rails project week as hell week. I started my week enthusiastic and excited which quickly turned to confused and frustrated while finally ending with a somewhat great sense of accomplishment. My greatest challenge this week was getting my nested attributes set up correctly (accepts nested attributes vs attribute= methods vs strong params and nested strong params)...it was a challenge to say the least. Using a join table that required a user submittable attribute required setting up the nested attributes very carefully. Now that its said and done, it makes sense and I can understand clearly how these work together. 
Another challenge I faced was getting my forms working properly with deeply nested attributes using fields_for. I tried using gems such as cocoon, simple forms and nested_forms_for to allow my user to dynamically add and remove fields for ingredients and directions. This ultimatly did not work the way I wanted it to and after watching 100 videos, reading blogs/post etc I realized it was something I had to leave behind...for now at least. Im hoping once we learn Javascript this will be something I can easily do within my application. I was able to at least allow the user to dynamically add direction steps so I'll settle for that at this point. 
I learned quite a bit during hell week which is something that makes it truly worth the pain. A few of the areas I feel more informed on include using scope methods, join tables with has_many, through, and using nested resources. I used scopes to easily query the database for a list of the most recent recipes and sort them by title on my index page. 
There is much to take away from this week and although I stumbled through the week a bit I learned so much. 
