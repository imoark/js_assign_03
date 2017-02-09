#CLOSURE EXPLANATION

Explaining Closure in a simple way, think of a property (building, house, real estate, mall). The function is a private property that is secluded. Making an inner function to that parent function will create a public area in the property. Another way of saying this is that the JavaScript parent function variables are private/hidden and only accessible through the JavaScript inner function variables which are public/accessible from outside the function.

By creating an inner function that is connected to the parent function, it creates a shortcut, and we can call that a Closure.

The point of using Closure is that we can make a private (local) variable that is safe and will not be interrupted with the global variable that we are gonna set in the future. JavaScript adopts lexical scoping, which means that functions are executed using the variable scope that was in effect when they were defined, not the variable scope that is in effect when they are being called. Meaning, it sets the scope (range of functionality) of a variable so that it may only be called (referenced) from within the block of code in which it is defined (inside of the function only).

##Closure example:

``` js

function sayHello(name) {
  var text = 'Hello ' + name;
  var say = logConsole() { 
  	console.log(text);
  }
  say(); // 
}
sayHello('Joe');

// It will output Hello Joe

```

[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures#Closure]

Youtube - 9.3: JavaScript Closure - p5.js Tutorial - [https://www.youtube.com/watch?v=-jysK0nlz7A]

Reliable JavaScript : How to Code Safely in the World's Most Dangerous Language, Spencer, Lawrence, Richards, Seth - Wrox 2015
