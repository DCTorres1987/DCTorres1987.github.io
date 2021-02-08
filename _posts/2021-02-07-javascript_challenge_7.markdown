---
layout: post
title:      "JavaScript Challenge #7"
date:       2021-02-08 04:07:43 +0000
permalink:  javascript_challenge_7
---


**Explan equality in JavaScript?**

When comparing values for equality, JavaScript provides three different value-comparison operations.

*Strict Comparison* (===), checks for value equality without allowing coercion. 

![Imgur](https://i.imgur.com/HLOzTAa.png)

Abstract comparison (==), checks for value equality with coercion allowed.

![Imgur](https://i.imgur.com/dYbTfmW.png)

Do not use *Abstract Comparisons* if:

* The value on either side of the comparison can be true or false.
* The value on either side of the comparison can be zero, " ", or an empty array.

**One Example:**

Oh no! True returns when comparing a string and an integer. We only want true when its the same value and data type.

![Imgur](https://i.imgur.com/bQyOkGn.png)

Thats better! 

![Imgur](https://i.imgur.com/4WfT1Ne.png)

That wasn't so bad was it? Let's continue!

We also have another comparison operator called *Object.is*. This method compares two values and determine if they are the same type. How cool is that!

![Imgur](https://i.imgur.com/B33Dw3S.png)

Hope everyone found today's topic interesting. Please be here for my next blog when we review another Javascript challenge! Remember don't just ready about it! Code about it!

Until next time...


