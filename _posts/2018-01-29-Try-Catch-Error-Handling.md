---
layout: post
title: Try - Catch - Throw error handling
---

Error handling is a common practice among almost all programming languages. They handle errors. Typically - anticipation, detection, and resolution of programming, application, and communications errors. It produces something the user or developer wants more than an ungraceful error.

**try/catch Syntax**
```
try {

  // code...

} catch (err) {

  // this block gets executed when there is an error

}
```




**try** is a statement where the code inside the block is executed. If it doesn’t work or errors, it moves over to catch, whatever is in catch is executed only once the code in the try scope produces an error.

**throw** creates a custom error. Typically when code fails unexpectedly an error is automatically generated. These help in the debugging process. For example, we have the following block of code:

**Example:**
![js ex](https://i.imgur.com/dSm4jl9.png)
Here we have code that errors in the try method.  The error is caught by the throw and produces a custom error messages like the one above!

_Common dev lingo “This code is not working correctly, it just threw/throw an error”._
