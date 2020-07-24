---
layout: post
title:      "Rails, Failure, and Success"
date:       2020-07-24 20:58:27 +0000
permalink:  rails_failure_and_success
---


I was nervous, but slightly confident that I would wow the instructor during my project review. I mean, come on! I put a lot of blood, sweat, and tears into this project. I made sure I covered all the requirements..wait what?  Did I have a nested form that would create a child record that relates back to the parent controller?  I thought allowing an user to select an attraction from a dropdown on the ticket new form was enough. 

My internal thoughts began to race and a slight chill filled my body. How could I forget this one requirement. I'm going to fail. How could I be so stupid? Why didn't I doublecheck? Can this be salvaged during live code? I was out of time, but my project reviewer gave my rails project high praise and encouragement. Its only this one requirement I need to go back and add. Don't beat yourself up. You almost have this. Get it to work and schedule another review. 

So I got to work. Its a bummer admitting that I failed but we all make mistakes. Its how we get back up again that really matters. 

I tried to accomplish the ask using a nested attribute but could not get it to work. Getting frustated I met with my cohort lead to ask for advice. Turns out I was overthinking the solution. I already had my form working to where a user could create a new attraction using **form_for**. Upon clicking submit it passes into my ticket controller create method. I would only need to create an **if then else statement** to determine if an attraction was chosen from the dropdown or was a newly created one.

I noticed that when a new attraction is created it doesn't have an attraction id, as it haven't been saved to the table yet. So if **params["ticket"]["attraction_id"].empty?** not **nil?** because **nil?** counts " " as being populated, then grab the last zoo created and save to an instance. Then find or create a new attraction record based on **params["ticket"]["attraction"]["name"],** associate it to the zoo, create a new ticket record, and associate it to the newly created attraction.

I tested my change and it worked!!  I did a demo for my cohort lead and I was ready for my review.  That day came quickly, today was the day, I was nervous. Thoughts of failing again in my head but I was ready. I showed off my new form and code and it was an success. Yayyy! I did it, but it wasn't over. Now it was time for the live coding. I needed to create a search engine that would work on the Users index page. It would allow me to return users by username and my reviewer would offer guidance when needed. In my mind, who is my worst enemy and my best friend, doubt crept in. How am I going to do this? Will I fail at this too? However, Google is a wonderful thing. There was a page that walked me through everything I needed to do step by step with a few alterations to work for my purpose. 

Success!! Hearing congratulations for passing my rails project was a fantastic ending to a long week. I did it! If at first you don't succeed, try, try, again. Sometimes we need to fail in order to come back stronger, work harder, to learn. Now on to Javascript...
