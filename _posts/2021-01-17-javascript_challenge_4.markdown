---
layout: post
title:      "Javascript Challenge 4"
date:       2021-01-18 00:28:45 +0000
permalink:  javascript_challenge_4
---


Will the below functions return the same thing?

```
function test1()
{
   return {
	     Danielle: 'hello'
	 }
};

function test2()
{
   return
	 {
	    Danielle: 'hello'
		};
}
```

When looking at the above code. It really stomped me at first. What is the difference between these two?  I came to an understanding that they probably produced different results, otherwise why would it be a challenge.  The only difference I saw was that the *return* in test2 is on its own line while the return in test1 wasn't. Here is what happened when I ran the above functions:

![Imgur](https://i.imgur.com/VjXfidi.png)
![Imgur](https://i.imgur.com/A8fbHWC.png)

The second function returns undefined!  

Surprised? I was!  

The reason this is occuring is because semcolons are optional in JavaScript, however excluding them is considered bad form. As a result, when the line containing the *return* statement, with nothing else on the line, is encounted in the second function, a semicolon is automatically inserted immediately after the return statement.

No error is thrown as the remainder of the code is valid, but ignored. It's unused code.

Makes you think doesn't it? About how you've written all your previous code...

Stay tune for the next challenge...
