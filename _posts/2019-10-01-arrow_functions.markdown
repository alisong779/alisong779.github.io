---
layout: post
title:      "Arrow Functions "
date:       2019-10-01 04:18:19 +0000
permalink:  arrow_functions
---


Why use Arrow Functions

A javascript function is a block of code that performs a task or calculates a value. A function is executed when its invoked. It can be invoked by an event (button click etc), self invoked or invoked within JS code. The function computes a return value and that value is returned to the “caller” who invoked it. When using the this keyword with functions there are some interesting facts that can be pretty confusing.


In regular functions, ES5 and earlier, the value of this is determined by the context in which the function is executed which is called runtime binding. It can vary each time a function is called. If a function is defined as a method of an object, this refers to the object itself. If the function is a regular function and not part of an object, this references the global object of window or global (except in strict mode - which is beyond the scope of this blog). 
The this keyword looses binding when assigned as a function (or method) reference. 
To control the value of this we can explicitly assign the value using .call, .apply or .bind method workarounds to bind the value of this.

In other words, the this keyword represents the object that called the function but can be explicitly assigned a value:

self = this 	//closure


bind.this
 

Javascript ES6 introduced the arrow function. Arrow functions eliminate the need to use the function and return keywords (return is implicit in arrow functions) and the use of curly brackets for single statement functions. Arrow functions allow for shorter syntax and simplified scope.
Arrow functions do not bind this. Since they do not bind this that means the value of this is searched for in the call stack. Therefore using an arrow function as a method on an object will not work, as the value of this will return as undefined. They also cannot be used in constructors when creating an object. Arrow functions bind this lexically, meaning to maintain its value from original context. They reduce the confusion around the this keyword by allowing you to retain the scope of the “caller” inside function. So you don’t need to create an explicit value of this using self = this or bind. At the same time arrow functions this value can’t be changed so if you need a new value for this you need a new function or function expression.

Heres an example of previous function types:

const word = function( ) {
	return “My word function”
}

ES6 arrow functions can be simplified down to one line of code:

const word = ( ) => “My word function”

If using parameters they can be passed inside the parentheses (w/o parentheses for one parameter):

const word = (val1, val2) => someAction(val, val2)

OR

const word = val => “My word function” + val



Use function expressions when you need a dynamic this and arrow functions for lexical this. Also, use function (regular functions) in the global scope, class for object constructors and arrow functions elsewhere. 
