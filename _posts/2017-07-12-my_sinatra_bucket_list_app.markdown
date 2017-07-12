---
layout: post
title:  "My Sinatra Bucket List App"
date:   2017-07-12 11:47:23 -0400
---

Today marks the day that I have finally finished my Sinatra Portfolio project. There have been a lot of things going on in my life (school, moving across states, etc.) and I am so happy to have gotten to this milestone. 

I would love to say that I am a creative goddess and my mind is just churning out different/wonderful project ideas -- but let me be honest with you, although the instructions for this project were simple and to the point, it took me a *long* time to come up with a project idea. I did not want my project to be too similar to the example project ideas that were suggested in the instructions (I figure, there must be tons of those projects out there by now). So, I spent a lot of time deciding on what I could do, ultimately choosing to make a bucket list app.

# Summary

My project allows a user to add life goals to thier bucket list. Once a life goal is added, the user can view the full bucket list, view the details of that specific goal, edit the goal, and delete the goal. 

Users can also mark a goal complete when editing the goal and add a reflection. Once a goal is complete, it will be moved to the "Completed" section of their bucket list.

# The Process 

Coming up with the idea is always the hardest part for a project for me (and most stressful, as the whole project centers around this one idea). So once I decided on my idea, I was extremely excited to start working on my project. I really enjoy the MVC framework and it seems to make a lot of sense to me. I'd like to think of myself as a somewhat organized person, and this is a great way to keep everything uniform and organized in your app. 

Before I started my project, I planned out what kind of models I needed, views I wanted, and the basic structure of my project. I used the Corneal Gem to set up the skeleton structure, then I went through and added basic database migrations, models, views, and controller actions in order to get a working base. 

I am not sure if this was the *best* idea, but my project has two models: the User model (used for user accounts) and the LifeGoal model (used for a user's life goals). I started off my project by getting a basic LifeGoal model, views, and controller working. Once that was working properly, I went in and added the User model, views, and controller to get that working. Next, I started connecting them together so that a life goal is associated with a user, and only a user can view, list, edit, and delete their own life goals. I thought this would be a great way to make progress on my application (and it did work!), but I do wonder if it would be best if I had started with my users model/view/controller funtionality first and then added in the life goals. All in all, I guess this is just a food-for-thought kind of thing, and something to think about for my next project!

After I got a basic application working, with the user and their life goals working and communicating together properly, I went in with the details, added links throughout the application, validations to the models, flash messages, refactored my code, and fixed some of the details (such as navigation link positioning). 

Lastly, I added the "Completed" feature to my project. While working on my project, I thought it would be nice if users could mark a life goal as completed and have the opportunity to add a reflection to this goal as a way to jornal thier experience and save their list of life goals if they wanted instead of only having the option to delete them once completed. So I added two more columns to the life_goals database table: completed and reflection. This next part took lots of testing, but I ended up using radios to mark if a goal is completed or not. Then I edited the full bucket list to display the in progress goals at the top of the page and the completed goals at the bottom of the page. 

After this, I added my README and made some final touches!

# Something to Come Back to 

This is more of a note-to-self, but something that I think I should come back to in the future:
* flash messages!!  (I used flash messages in my project and had to do a lot of testing and a bit of debugging with them. If I have more time, I think reviewing further capabilities of flash messages would be great!)
