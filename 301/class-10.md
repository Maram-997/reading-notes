# Read : Class 10 -  In memory storage
#### **What is a ‘call’**
 With the call() method, you can write a method that can be used on different objects.

#### **How many ‘calls’ can happen at once**
 Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

#### **What does LIFO mean** 
Last In, First Out,it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

#### Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
![img](../imgs301/call-stack.png)

#### **What causes a Stack Overflow** 
A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

## Types of error messages:
1. Reference errors
2. Syntax errors
3. Range errors
4. Type errors

> There are also warnings, for instance telling you about a deprecated method, which can be found more frequently in firefox developer tools.

## QUES
**What is a ‘refrence error’?**
In JavaScript a reference error is mainly thrown when a code is attempting to reference a variable that does not exist, but there are many ways we can write our code that may trigger this reference error to be thrown.
**What is a ‘syntax error’?**
An exception caused by the incorrect use of a pre-defined syntax. Syntax errors are detected while compiling or parsing source code. For example, if you leave off a closing brace ( } ) when defining a JavaScript function, you trigger a syntax error.
**What is a ‘range error’?**
A RangeError is thrown when trying to pass a value as an argument to a function that does not allow a range that includes the value. This can be encountered when: passing a value that is not one of the allowed string values to String.
**What is a ‘type error’?**
The TypeError object represents an error when an operation could not be performed, typically (but not exclusively) when a value is not of the expected type.
A TypeError may be thrown when:
1. an operand or argument passed to a function is incompatible with the type expected by that operator or function; or
2. when attempting to modify a value that cannot be changed; or
3. when attempting to use a value in an inappropriate way.
**What is a breakpoint?**
In the debugger window, you can set breakpoints in the JavaScript code.
At each breakpoint, JavaScript will stop executing, and let you examine JavaScript values.
After examining values, you can resume the execution of code (typically with a play button).
**What does the word ‘debugger’ do in your code?**
The debugger keyword stops the execution of JavaScript, and calls (if available) the debugging function.
This has the same function as setting a breakpoint in the debugger.
If no debugging is available, the debugger statement has no effect.
With the debugger turned on, this code will stop executing before it executes the third line.