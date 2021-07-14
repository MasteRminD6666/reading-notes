Error Handling & Debuggin
-----

Because JavaScript is a loosely and weakly typed language, it has always been its weakness in error debugging. If the script makes a mistake, the error message given to us is often a clueless hint; the good news is that due to the continuous upgrade of the browser, JavaScript The debugging ability is getting better and better.


## 1.try...catch debugging

``try{
   window.dddd();
}catch(e){
   alert(e);
}``
------

This non-existent method, if there is an error, directly print it out in catch, e and js have two attributes of name and message, you can directly print out the name and information of e.name or e.message;

## error type

There are many kinds of errors that may occur when executing code. Each error has a corresponding error type, ECMA-262

Defined7Types of errors:
----
* ``Error``

* ``EvalError``

* ``RangeError``

* ``ReferenceError``

* ``SyntaxError``

* ``TypeError``

* ``URIError``

Among them, Error is the base type (the parent type of the other six types), and other types inherit from it. Error types are rare and are generally thrown by browsers. This base type is mainly used by developers to throw custom errors
Common error types
Because JavaScript is a loosely typed language, many errors occur during runtime. Generally speaking, needPay attention to 3 kinds of errors:
* ``Type conversion error;``

* ``The data type is wrong;``

*  ``Communication error;``

These three errors generally occur in a specific mode or without adequately checking the value. In the early days of JavaScript, browsers did not provide debugging tools for JavaScript, so developers came up with a set of their own debugging methods, such as alert(). This method can print whether you have obtained the corresponding value you suspect, or
Put it somewhere in the program to see if it can be executed, and know that the previous code is correct.


## Try and catch Example 

![try](https://image.slidesharecdn.com/015debuggingtechniques-190503093158/95/javascript-chapter-15-debugging-techniques-5-638.jpg?cb=1556876159)

