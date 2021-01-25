---
layout: post
title:      "Javascript Challenge #5"
date:       2021-01-25 02:56:13 +0000
permalink:  javascript_challenge_5
---


Welcome Back! Tips and Tricks to make us better coders! Let's get to it!

**Today's Topic: How do you empty an Array?**

Seems easy right? When I saw this question the first method I could think of is the following:

**Method 1-**

`array = []`

However, I learned this is recommended only if you are not referencing the original array somewhere else. If this array is referenced somewhere else the original array will remain unchanged. Go check your code quick! I know it makes me want to check mine.

![Imgur](https://i.imgur.com/z8ZwRdL.png)

**Method 2 - **

`array.length = 0;`

This will clear the existing array by setting the length to zero. This method will also update all the reference variable that point to the original array. Pretty cool, right?!

![Imgur](https://i.imgur.com/bqATVu9.png)

**Method 3- **

`array.splice(0, array.length);`

This method empties the array and also update all references to the original array. Splice is just a way to add or remove items in an array. The above code is adding zero items and removing the number of items in the array. This is definitely a tip I will keep in my back pocket!

![Imgur](https://i.imgur.com/Kn2uXCz.png)

Hopefully this will help you like it helped me. I loved every minute of doing this challenge. My one tip to give, is to not just read about a challenge. Try it out yourself. It will stick more and is more fun too.

Til next time...


