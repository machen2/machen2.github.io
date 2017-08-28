---
layout: post
title:  "Crafty: My Rails Final Project!"
date:   2017-08-25 19:40:28 -0400
---


I have always been interested in arts and crafts since I was a kid, so when it came time to think of an app I could create for my Rails Portfolio project, I was set on making a crafting app. "Crafty" is an app in which users can create, manage, and keep a record of any crafts they have created. In addition, user can also view each other's crafts (but only edit thier own) in case they would like to try making art using someone else's instructions! 

When a user creates a craft, they are able to add information such as: title, brief description, set a difficulty level, add a picture, add instructions for how to make that craft, and add different tags associated with that craft. 

Users can view by crafts, tags, "my crafts", and most popular tags. They can also view crafts made by a specific user if they decide to click on the link to the author's name on any specific craft show page. 

## the process
For my Rails Project, although I had an idea of what kind of app I wanted to create, it did take me a while to get started. I took a few days planning out what models I needed to have, drawing diagrams on how I should set up my database, and deciding what features I wanted my final project to have in the end. Once I had a basic outline of features and structure I wanted for my app, I decided to jump right into my project. I first set up my database, then my models, and then added in some basic validations and associations I wanted those models to have. 

When completing my last project (my Sinatra Project), I first created a basic, workable app and then incorporated a small authentication system for signing up, loggin in/out, and limiting what a user can access. Although it worked for me to create my basic app and then add in the authentication system last, I told myself that it might be a bit easier to try starting off my Rails Project with the authentication system first, and this is what I ended up doing for my project.

I used my own authentication system with a registrations and a sessions controller for this project instead of using a gem like Devise. Although Devise is very handy and might have saved me some coding and debugging time, I wanted extra practice at creating my own workable authentication system. In the end, I am glad I chose this route for my project, because I feel I was able to review a lot about how authentication systems are created. It also allowed me to practice problem solving while debugging my code (which I believe is always a great thing for me to practice!).

After I had an authentication system up and running, I began working on the rest of my app, starting with the Craft model first and then working into the Tag model and finally the User model. This consisted of setting up the correct routes, adding the views, setting up the controller actions, and working my code into partials. I also added flash messages throughout my process in order to make sure my users would be getting correct alerts when data was not input correctly or they were trying to access a page they were not authorized to and they were getting success messages when a craft was successfully created or edited. 

After I got my app base working, I refactored my code and added in some new features (such as the ability to add in photos to one's crafts). When I am working on a project, I like to list all of the features I would like it to have, but a handful of them I leave on a "To Do Later" list. I see these as "extra" features that would not take anything away from my project passing the specs, but would only make it better. For example, having pictures in my app was not required in the specs for this project, but I knew they would look nice, so I added them to my to do list to be implemented at a time when the rest of my app was finished and working. 

Adding some Bootstrap to my project was also on my list of things to do later that were not needed for the assessment, but would help to organize and make my app look better overall. I have only used bootstrap last year when I began my full stack web dev journey. This program had some labs that used bootstrap. However, since then, I have not continued working with Bootstrap in any way (especially not with one of my own projects!), so I spent one day reviewing and doing research. I watched a few different YouTube videos and read a handful of different articles about Bootstrap. In the end, I was able to add a little bit of Bootstrap's features to my app, mainly a navigation bar and basic responsiveness. I really love how even with the few elements of Bootstrap I added, my app looks much better. I can only imagine how great it would look if I was more fluent in using Bootstrap. This is something that I hope to improve on in the future and learn more about!

## takeaway
Athough I learned so much during this project from practicing custom authentication logic, using nested forms, implementing a custom attribute writer, adding in validations and flash messages, using a tiny bit of Bootstrap, etc., I think my greatest takeaway is that I really learned how to be more calm when it comes to running into bugs and problems in my code. When I first started my coding journey, I would get very frustrated at bugs in my code. I would get frustrated at the time it takes to fix a problem or the time I "wasted" because of a small syntax error in my program that I "should have" avoided and done correctly the first time. 

Now, I noticed that I have become much more relaxed when I run into errors in my code. I realize that bugs happen to everyone, no matter how big or tiny they are! I know a few different ways I can debug my apps, and how to approach errors and problems I am facing. I am much more relaxed now and find errors as something that is part of the programming process and a "puzzle to solve" and learn from. They have become fun challenges for me to work on my problem solving skills and hopefully help me become a better programmer. 

## to do
In the future, I would really love to also add the ability for users to comment on the show pages for different crafts. It would also be cool for users to "like" different crafts they are interested in or "bookmark" them to remember later. Adding in some more Bootstrap or front end design to my project when I become more fluent is also something on my list of to do's. 

