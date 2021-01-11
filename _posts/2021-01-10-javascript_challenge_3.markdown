---
layout: post
title:      "Javascript Challenge 3  "
date:       2021-01-10 21:02:44 -0500
permalink:  javascript_challenge_3
---


What will the code below output to the console and why?

```
var myObject = {

foo: "bar",
func: function() {

		var self = this;

		console.log("outer func:  this.foo = " + this.foo);
		console.log("outer func:  self.foo = " + self.foo);

		(function() {				
				console.log("inner func:  this.foo = " + this.foo);
				console.log("inner func:  self.foo = " + self.foo);						
		} ());
}
};
```

myObject.func()

This challenge at first glace looks intimidating until each later is peeled back. The key word* this* its the object's property, that object itself which is why the first two console logs prints as expected. Then an immediately-invoked function expression (IIFE) is used and this referenced inside is the global Object(Window object). Therefore this.foo means Window.foo which is undefined.

However, self is accessible inside that function which has value equal to that object. This allows console log to print the foo variable sucessfully.

![Imgur](https://i.imgur.com/WzMyHcs.png)

