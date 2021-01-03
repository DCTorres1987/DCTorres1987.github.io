---
layout: post
title:      "Javascript Challenge: Palidrome"
date:       2021-01-03 16:18:05 -0500
permalink:  javascript_challenge_palidrome
---


A common Javascript Interview Question is determining if a string is a Palindrome. A Palidrome is a string that reads the same frontward and backward.  One way to determine if a string is a palidrome is to use the following code:

```
function palindrome(string) {
    let reverseString = string.split("").reverse().join("");
		
		if (string == reverseString)
		    console.log('palindrome');
		else 
		    console.log('not palindrome');
}

palindrome('racecar')
```

The above code is a function called, palindrome. A value is being passed into the function called, *string*. When the function is called, it creates an variable called reverseString. The value that is stored is the reverse of the string inputed. For example, say if the word racecar is the string that is inputed, the split method is called to split each letter in the string into an element in an array.

![Imgur](https://i.imgur.com/SDfIsAu.png)

Then the reverse method is called and it reverse the elements in the array.

![Imgur](https://i.imgur.com/p4moYRe.png)

Lastly, the join method is called and it combines the elements back into a string.

![Imgur](https://i.imgur.com/KMZXn1W.png)

After the variable value has been set, the if then else statement compares the string 'racecar' to the reverseString that was set, *racecar* and if they match it will console.log or print *palindrome* else *not palindrome*.

![Imgur](https://i.imgur.com/7mqpPt3.png)

Palindrome returns because, *racecar*, is the same going forward and backward. Where a string like *cat*, would not return as a palindrome.

![Imgur](https://i.imgur.com/7O48f58.png)

This is the easiest way to solve this challenge if you ever receive it in a coding interview challenge. However, as they say, there is more than one way to skin a cat. Please let me know how you would approach this challenge.
