---
layout: post
title:      "Javascript Interview Question #1"
date:       2020-12-27 00:19:43 +0000
permalink:  javascript_interview_question_1
---

As a Full Stack Software Engineer, I feel it is important we know how to solve basic interview question to prove our skills. Here is what I reviewed today.


What is a potential pitfall with using typeof bar === "object" to determine if bar is an object? How can this pitfall be avoided?


Although the above is a reliable way of checking if bar is an object, *null* is also considered an object.  The following code will, log *true* (not false) to the console:

```
var bar = null;
console.log(typeof bar === 'object'); // logs true!
```

This problem can be avoided by also checking if bar is null:

`console.log((bar !== null) && (typeof bar === 'object')); //logs false`

The above solution will return *false* if bar is a function. In situations where you want to also return *true* for functions you can change the code to be:

`console.log((bar !== null) && ((typeof bar === 'object') || (typeof bar === 'function')));`

The above solution will return *true* if bar is an array (e.g., if var bar = []; ). In situations where you want to return * false* for arrays, you can change the above solution to be:

console.log((bar !== null) && (typeof bar === "object") && (toString.call(bar) !== "[object Array]"));

However, there's one other alternative that returns *false* for nulls, arrays, and functions, but *true* for objects:

`console.log((bar !== null) && (bar.constructor === Object));`






