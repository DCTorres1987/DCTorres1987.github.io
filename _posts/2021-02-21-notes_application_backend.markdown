---
layout: post
title:      "Notes Application Backend"
date:       2021-02-22 02:53:12 +0000
permalink:  notes_application_backend
---


I'm currently working on the Backend of my Notes Applications that will handle my data and passing to the front and what is passing in from the front to the back. I worked on the generating models, model relationships and table migrations using rails generators such as:

`rails g model User name:string password:string;`

**Migration:**
![Imgur](https://i.imgur.com/s9svFiW.png)

**Model:**
![Imgur](https://i.imgur.com/NFa0872.png)

Next I started building out my controllers for Categories, Subjects, Users, and Notes. I tested by starting up the server using `rails s-p 3001`.

![Imgur](https://i.imgur.com/Cmdjy6p.png)

I passed the data to the server as a JSON and was able to confirm everything appears to be working as expected so far. Next I will be starting on my front end to get the data to populate the DOM.

Example of JSON:

![Imgur](https://i.imgur.com/Qq6panG.png)


