---
layout: post
title:      "Weather Observation Station 13"
date:       2021-03-15 02:24:51 +0000
permalink:  weather_observation_station_13
---


In this blog I would like to give a detail breakdown how I solved the **Weather Observation Station 13** Challenge in Hacker Rank using Oracle SQL.

In the challenge, it is requested that you write a query that returns the sum of Northern Latitudes (LAT_N) from a table called** Station** where the values are greater than **38.7880** and less than **137.2345**. The value must be truncated to 4 decimal places.

I reviewed the instructions one more time to make sure I captured the key words of what was being asked. 

I ran **Select  *** to see what the data looked like.  I then added to the query where I only return results between 38.7880 and 137.2345;

`Select * From Station;`

Not only does *between* return all values between the two given but it also returns 38.7880 and 137.2345. 

`Select lat_n From Station Where lat_n between 38.7880 and 137.2345;`

Next, I used an analytic function **Sum** to sum all the lat_n returned by my query.

`Select sum(lat_n) sum_lat_n From Station where lat_n between 38.7880 and 137.2345;`

This returns 36354.8135. Our answer, but there is one last thing it asked for us to do. We need to **truncate** sum to the nearest 4 decimals.

`select trunc(sum(lat_n),4) sum_lat_n from station where lat_n between 38.7880 and 137.2345;`

There is our answer!

![Imgur](https://i.imgur.com/M8UmzS1.png)
![Imgur](https://i.imgur.com/oJ4OsOb.png)


