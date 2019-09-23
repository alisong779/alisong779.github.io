---
layout: post
title:      "React/Redux Final Project"
date:       2019-09-23 17:43:05 +0000
permalink:  react_redux_final_project
---


Ive submitted my final project for Flatiron School - React/Redux with a Rails API. I can say without a doubt that this journey has been one of many lows but much greater highs. The excitement I feel when completing a project or seeing something come to life or finding and resolving an error makes every low moment irrelevant. I can say with all honesty that I wondered many times along the way if I could do this. Was a coding bootcamp the right choice  for me? Though there were days I thought about giving up and walking away, I just stuck with it. I just kept showing up, learning what I could at my own pace, putting the time in and stayed focused. Its hard! No doubt about that. As I come to the end of this journey I realize the confidence Ive gained. I realize how much Ive learned and the awesome things I have the ability to create now! I feel a great sense of accomplishment and am proud of myself for sticking with it. This is one of the hardest things Ive ever done, yet has come with such great reward even before landing a job. Get up, show up, put the time in, stay focused and stick with it! Its worth the pain :D

On React/Redux:
The most important thing I learned while creating my React/Redux project is that when using associated models (a goal has_many task, a task belongs_to a goal) make sure you set up your reducers properly. If you’re going to update an associated objects state, the parents state needs to be updated as well. It took a while to figure that out. When I would add or remove tasks they weren’t rendering on the page. This was due to the fact that I had my reducers separated and the states did not know about each-other. I’ll post a link to a good article on the subject below. This was a challenging yet fun project! Good luck to all!

https://redux.js.org/recipes/structuring-reducers/immutable-update-patterns
