---
layout: post
title:      "My First Project"
date:       2020-03-16 23:05:43 +0000
permalink:  my_first_project
---


During the past two weeks the words, "My Project", has instilled so much emotional turmoil it was literally like being on a rollercoaster.  There were so many moments of, "Yes, I'm killing it!", to, "OMG! I don't know what I'm doing. I'm going to fail!", but I never quit.

For my first CLI Project I created a Movie Showtime Search.  It would allow the user to enter a zipcode for their local area and retrieve movie listings.  From there, the user can choose a movie they would like to see and the application will retrieve showtimes for that movie.

I began by searching for a good website where I could get movie showtime API data and with the guidance of my cohort leader I discovered Gracenote Developer Video & Sport.  The website allowed me to pull movie showtime information by zipcode. I immediately requested a key and began reviewing the documentation.

Once a good sample request was found.  I began setting up my project so everything would be ready for me to begin coding, and I would be able to push my code to my repository on github.

After making a big attempt and feeling good about what I coded. I soon discovered that it was not meeting all the requirements of the project and I had to start fresh. I began worrying that I wouldn't make the deadline in time, but I couldn't give up.

My first attempt at coding my project did not have a deeper search besides retrieving movie listing and showtimes by a zipcode, so the easiest way to fix this problem was to have seperate classes. One for Theatre and another for Showtimes.  

I created attr_accessors for each class, initialized them in a method, and created a .all method so that it would hold all the information needed in the appropriate classes.

**Theatre Class:** theatre names

**Showtimes Class:** movie title, genres, description, date time, ticketuri

I coded the Movieshowtimes::API to handle settng variables, so they may be used to create Theatre and Showtimes instances.

I created the following methods so I could code a find or create by name method to ensure duplicate theatre names would not be pushed into the @@all array that I will be using in my CLI file.

**1.  save method**
 def save 
    @@all << self 
  end
	
**2. .create method**
def self.create(theatre)
    theatre = self.new(theatre)
    theatre.save
    theatre
  end
	
**3. .find by name method**
  def self.find_by_name(theatre)
    @@all.detect do |name|
      name.theatre == theatre
    end
  end
	
Once I finished coding what I needed for my Theatre and Showtime class. I began coding my CLI file.  I began writing a series of methods that would allow a user to enter a zip and date of the showing. It would then displayed a logo and retrieve a list of theatres in that area.  

Finally, I was able to code a method for a deeper search.  I created a series of methods that would return movie listings. One of the methods would also allow the user to choose a movie and see showtimes, and the ticketuri for that movie.

Getting to this point, I realized more than half of my project was complete.  I added to my project the option for the user to choose another movie or theatre otherwise the application would complete with the final goodbye method.  

Growing excited, I began testing and fixing any issues that was discovered until everything was finally complete.  I felt so proud of myself. I never thought I would be able to code something like this and get it to work properly. I'm super excited to demo to my cohort and super excited to learn even more.

