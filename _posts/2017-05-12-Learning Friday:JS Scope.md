---
layout: post
title: Learning Friday&#58; JS Scope - Global, Function, and Block 
---

Hey there! Here are some notes I took after reading Kyle Simpson's YDKJS and watching his "Advanced Front-end Masters" on Scope. Let me know if theres anything I can improve with this article via the links below. There's always room to improve!

# What is Scope?
According to W3Schools, scope is the set of variables you have access to.

There are 3 types of Scopes in JS:
- Global Scope
- Function Scope
- Block Scope

## Global Scope
This is whatever's not in function or block. These variables are accessible from wherever.

## Function Scope
Variables declared within a function are considered to be in the Function Scope. This is the most common type of scope you'll run into. Whenever there is a variable declared within a function it is also accessible by the nested function. For example:

```
function holdsTheHi(){
  var greeting = "hello";
  helloBob();
  function helloBob(){
    console.log(greeting, "Bob"); // greeting is within holdsTheHi's function scope
  }
}
holdsTheHi(); // "hi Bob"
console.log(greeting);            // greeting is not defined
```

## Block Scope
In old school vanilla JS these are not so common. Block Scopes are used within things like for-loops, if-loops, and try/catch's. For example:
```
for (var i=0; i<10; i++) { // i declared within for block
	console.log( i );
}
```
### let
However as of ES6, you're able to use **let** instead of **var** to declare variables. In short, this keeps the variable accessible within the two parens {..} of a block scope. That's it. For example:
```
var foo = true;

if (foo) {
	{ // <-- explicit block
		let bar = 2;
		bar = 3;
		console.log( bar );
	}
  console.log(bar); // ReferenceError
}

console.log( bar ); // ReferenceError
```
We explicitly define a block here that only logs the **bar** within the block scope. If we use a **var** instead of **let** to declare **bar**, all 3 of these would be outputted.
