---
layout: post
title:      "Javascript..."
date:       2020-09-04 11:13:56 -0400
permalink:  javascript
---


Javascript is top down one of the hardest section of the program that I've been through. It is not for the faint of heart, but I will grab my sword and my shield and prepare myself to slay this dragon. Going through the lessons, seemed like traveling through a fog at times. I was able to push through, but wasn't always clear of the path. I learn concepts such as hoisting, ES6 syntax sugar, rest, and spread. I really enjoyed one of the labs, Andy's Toy Chest, but as I grew closer to project week. Fear set in.

What would my project be? Did I learn enough to put something together?  Would I fail?  Failure and Fear are the two friends that always show up at the end of every module. Despite my feelings I pushed forward. I came up with an idea to do a pokemon team generator. It would allow a user ('trainer') to create their on pokemon team and add pokemon to their team. I gathered what resources I could and began to type out my code. At first everything was messy and far from DRY (meaning Don't Repeat Yourself). I only cared about getting my website to work. I worked on  a form that would allow a user to create a new team or add to an existing team. The user could open and close the form whenever needed. I worked on my AJAX calls of get, post, and delete. 

My 2nd pass, through all my code was about refactoring. How could I make it better? What could I do to make things more efficient and DRY? What code could be moved to other classes? Several times I broke my website and rewrote it better. Until the error.. Error 500 SQL Busy Database is Locked. This error occured when fetch post iterated through a selected random pokemon array. Apparantely ForEach and Fetch Post don't agree due to asynchronous nature of how fetch works. Fetch while still processing will continue on excuting code even if it hasn't finished and because forEach runs in seconds it causes Fetch to throw an error that its busy (think dial tone) and as a result a pokemon doesn't get created. I did absolutely everything I could think of to get around this error, googled to I couldn't google no more, and nothing resolved it. What if it happened during my assessment would I fail. 

Sometimes we have to let go of something in order to continue forward. Crying wasn't going to fix this issue so the only thing I could do was find a work around. Pass one pokemon and fetch post one at a time without using ForEach. After extensive testing the issue has not occured. I added a few more things to style my project and double checked the requirements. Now its time to schedule my assessment. I'm ready with a shield and sword..will I win?
