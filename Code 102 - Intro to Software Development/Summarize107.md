# Functions
Generally speaking, a **function**  is a "subprogram" that can be called by code external (or internal in the case of recursion) to the function. Like the program itself,
a function is composed of a sequence of statements called the function body,Values can be passed to a function, and the function will return a value.

In JavaScript, **functions** are first-class objects, because they can have properties and methods just like any other object. What distinguishes them from other objects is that functions can be called.
In brief, they are Function objects.
For more examples and explanations, see also the JavaScript guide about functions.
[MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions)

----

## Description
Every function in JavaScript is a **Function** object. See Function for information on properties and methods of Function objects.

To return a value other than the default, a **function** must have a return statement that specifies the value to return.
A **function** without a return statement will return a default value. In the case of a constructor called with the new keyword, the default value is the value of its this parameter. 
For all other functions, the default return value is undefined.

The parameters of a function call are the function's arguments. Arguments are passed to functions by value. 
If the function changes the value of an argument, this change is not reflected globally or in the calling function. 
However, object references are values, too, and they are special: if the function changes the referred object's properties, that change is visible outside the function

----

## The function declaration (function statement)
There is a special syntax for declaring functions (see function statement for details):

function name([param[, param[, ... param]]]) {
   statements
}

----

**name:** The function name.

**param:** The name of an argument to be passed to the function.

**statements:** The statements comprising the body of the function.

The **function** expression (function expression)
A function expression is similar to and has the same syntax as a function declaration (see function expression for details). A function expression may be a part of a larger expression. One can define "named" function expressions (where the name of the expression might be used in the call stack for example) or "anonymous" function expressions. Function expressions are not hoisted onto the beginning of the scope, therefore they cannot be used before they appear in the code.

function [name]([param[, param[, ... param]]]) {
   statements
}

