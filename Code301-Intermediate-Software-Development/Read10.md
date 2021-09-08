# The JavaScript Call Stack - What It Is and Why It's Necessary

##What is a ‘call’?

 is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call)

## How many ‘calls’ can happen at once?

JavaScript can do one single thing at a time because it has only one call stack

## What does LIFO mean?

When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.







## Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

![](https://media.geeksforgeeks.org/wp-content/uploads/20201213102457/global.png)

thirdFunction();

# What causes a Stack Overflow?

A StackOverflowError is a runtime error in java. It is thrown when the amount of call stack memory allocated by JVM is exceeded. A common case of a StackOverflowError being thrown, is when call stack exceeds due to excessive deep or infinite recursion. In the above case, it can be avoided by doing programmatic changes.

# What is a ‘refrence error’?

The TypeError object represents an error when an operation could not be performed, typically (but not exclusively) when a value is not of the expected type. A TypeError may be thrown when: an operand or argument passed to a function is incompatible with the type expected by that operator or function; or.

# What is a ‘syntax error’?

It is thrown when the JavaScript engine encounters tokens or token order that does not conform to the syntax of the language when parsing code.

# What is a ‘range error’?

Description. A RangeError is thrown when trying to pass a value as an argument to a function that does not allow a range that includes the value. This can be encountered when: passing a value that is not one of the allowed string values to String.

# What is a ‘tyep error’?

# when a value is not of the expected type. A TypeError may be thrown when: an operand or argument passed to a function is incompatible with the type expected by that operator or function; or.

# What is a breakpoint?

At each breakpoint, JavaScript will stop executing, and let you examine JavaScript values. After examining values, you can resume the execution of code (typically with a play button).

# What does the word ‘debugger’ do in your code?

The debugger statement stops the execution of JavaScript, and calls (if available) the debugging function. Using the debugger statement has the same function as setting a breakpoint in the code. Normally, you activate debugging in your browser with the F12 key, and select “Console” in the debugger menu.
