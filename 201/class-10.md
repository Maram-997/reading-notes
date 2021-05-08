# Read: 10 - Error Handling & Debugging
#### ORDER OF EXECUTION
To find the source of an error, it helps to know how scripts are processed.The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run:
![img](/images/debugging.png)
This script above creates a greeting message, then writes it to an alert box (see right-hand page). In order to create that greeting, two functions are used:(greetUser () and getName ()).
#### EXECUTION CONTEXTS
The JavaScript interpreter uses the concept of execution contexts.There is one global execution context; plus, each function creates a new execution context. They correspond to variable scope.
**EXECUTION CONTEXT**
Every statement in a script lives in one of three
execution contexts:
* GLOBAL CONTEXT : Code that is in the script, but not in a function.There is only one global context in any page.
* FUNCTION CONTEXT : Code that is being run within a function.Each function has its own function context.
* EVAL CONTEXT (NOT SHOWN) : Text is executed like code in an internal function called eval ().
**VARIABLE SCOPE**
* VARIABLE SCOPE : If a vane of code atriable is declared outside a function, it can be used anywhere because it has global scope.
* FUNCTION-LEVEL SCOPE : When a variable is declared within a function,it can only be used within that function.
#### THE STACK
The javascript interpreter processess one line of code at a time,when a statement needs data from another function, it stack the new function on top of the current task.
#### EXECUTION CONTEXT & HOISTING
Each time a script enters a new execution context, there are two phases of activity:
1. prepare : 
* The new scope is created
* Variables, functions, and arguments are created
* The value of the this keyword is determined
2. execute : 
* Now it can assign values to variables
* Reference functions and run their code
* Execute statements
#### UNDERSTANDING SCOPE
In the interpreter, each execution context has its own variables object.It holds the variables, functions, and parameters available within it.Each execution context can also access its parent's variables object.
Functions in JavaScript are said to have lexical scope.
They are linked to the object they were defined within.
So, for each execution context, the scope is the current execution context's variables object, plus the variables object for each parent execution context.
Imagine that each function is a nesting doll.
The children can ask the parents for information in their variables. But the parents cannot get variables from their children. Each child will get the same answer from the same parent.
#### UNDERSTANDING ERRORS
If a JavaScript statement generates an error, then it throws an exception.At that point, the interpreter stops and looks for exception-handl ing code.
If you are anticipating that something in your code may cause an error, you can use a set of statements to handle the error,This is important because if the error is not handled, the script will just stop processing and the user will not know why. So exception-handling code should inform users when there is a problem.
Whenever the interpreter comes across an error, it will look for error-handling code. In the diagram below, the code has the same structure as the code you saw in the diagrams at the start of the chapter. The statement at step 1 uses the function in step 2, which in turn uses the function in step 3. Imagine that there has been an error at step 3.
#### ERROR OBJECTS
Error objects can help you find where your mistakes are and browsers have tools to help you read them.
![img](/images/error.png)
#### ERROR OBJECTS CONTI NUED
![img](/images/error2.png)
![img](/images/error3.png)
#### HOW TO DEAL WITH ERRORS
1. DEBUG THE SCRIPT TO FIX ERRORS
2. HANDLE ERRORS GRACEFULLY
#### A DEBUGGING WORKFLOW
**WHERE IS THE PROBLEM?**
1. Look at the error message, it tells you:
* The relevant script that caused the problem.
* The line number where it became a problem for the interpreter. 
* The type of error (although the underlying cause of the error may be different).
2. Check how far the script is running.
3. Use breakpoints where things are going wrong.
**WHAT EXACTLY IS THE PROBLEM?**
1. When you have set breakpoints, you can see if the variables around them have the values you would expect them to. If not, look earlier in the script.
2. Break down I break out parts of the code to test smaller pieces of the functionality.
* Write values of variables into the console.
* Calrfunctions from the console to check if they are returning what you would expect them to.
* Check if objects exist and have the methods I properties that you think they do.
3. Check the number of parameters for a function, or the number of items in an array.
#### LOGGING DATA TO THE CONSOLE
This example shows several uses of the console.log() method.
1. The first line is used to indicate the script is running.
2. Next an event handler waits for the user leaving a text input,and logs the value that they entered into that form field.
When the user submits the form,four values are displayed:
3. That the user clicked submit
4. The value in the width input
5. The value in the height input
6. The value of the area variable
#### GROUPING MESSAGES
1. If you want to write a set of related data to the console, you can use the console. group () method to group the messages together. You can then expand and contract the results.
2. When you have finished writing out the results for the group, to indicate the end of the group the console .groupEnd () method is used.
#### WRITING TABULAR DATA
In browsers that support it, the console.table() method lets you output a table showing:
* objects
* arrays that contain other objects or arrays
#### WRITING ON A CONDITION
Using the console.assert() method, you can test if a condition is met, and write to the console only if the expression evaluates to false.
#### BREAKPOINTS
You can pause the execution of a script on any line using breakpoints. Then you can check the values stored in variables at that point in time.
#### STEPPING THROUGH CODE
If you set multiple breakpoints, you can step through them one-by-one to see where values change and a problem might occur.
#### CONDITIONAL BREAKPOINTS
You can indicate that a breakpoint should be triggered only if a condition that you specify is met. The condition can use existing variables.
#### DEBUGGER KEYWORD
You can create a breakpoint in your code using just the debugger keyword. When the developer tools are open, this will automatically create a breakpoint.
You can also place the debugger keyword within a conditional statement so that it only triggers the breakpoint if the condition is met. This is demonstrated in the code below.
#### HANDLING EXCEPTIONS
If you know your code might fail, use try, catch, and finally.
Each one is given its own code block.
1. TRY : 
First, you specify the code that you think might throw an exception within the try block.
2. CATCH :
If the try code block throws an exception, catch steps in with an alternative set of code.
3. FINALLLY :
The contents of the finally code block will run either way - whether the try block succeeded or failed.
#### COMMON ERRORS
![img](/images/common.png)
