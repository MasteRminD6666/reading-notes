# For And While Loops:

----
# For Loop
## for ([initialization]; [condition]; [final-expression]){
##   statement}

---

**Initialization:**  This expression may optionally declare new variables with var or let keywords. Variables declared with var are not local to the loop, i.e. they are in the same scope the for loop is in. Variables declared with let are local to the statement.
An expression (including assignment expressions) or variable declaration evaluated once before the loop begins. Typically used to initialize a counter variable.
The result of this expression is discarded.

**Condition:** An expression to be evaluated before each loop iteration. If this expression evaluates to true, statement is executed. This conditional test is optional. 
If omitted, the condition always evaluates to true. If the expression evaluates to false, execution skips to the first expression following the for construct.

**Final-expression:** An expression to be evaluated at the end of each loop iteration. This occurs before the next evaluation of condition. Generally used to update or increment the counter variable.
statement

**A statement** that is executed as long as the condition evaluates to true. To execute multiple statements within the loop, use a block statement ({ ... }) to group those statements. 
To execute no statement within the loop, use an empty statement (;).

[MDN:Refrence](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for)
----

# While Loop

**while (condition)
  statement**
  


**Condition:** An expression evaluated before each pass through the loop. If this condition evaluates to true, statement is executed. When condition evaluates to false, execution continues with the statement after the while loop.


**Statement:** An optional statement that is executed as long as the condition evaluates to true. To execute multiple statements within the loop, use a block statement ({ ... }) to group those statements.

**Note:** Use the break statement to stop a loop before condition evaluates to true.

[MDN:Refrence](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/while)
