# JavaScript Debugging

## Order of Execution

**ORDER OF EXECUTION**: To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run.

The JavaScript interpreter uses the concept of execution contexts. Every statement in a script lives in one of three execution contexts:

1. **GLOBAL CONTEXT**: Code that is in the script, but not in a function. There is only one global context in any page.
2. **FUNCTION CONTEXT**: Code that is being run within a function. Each function has its own function context.
3. **EVAL CONTEXT**: Text is executed like code in an internal function called `eval()`.(NOT SHOWN)

**Global** and **Function** contexts correspond with the notion of scope, and as we learned, there are two different types of scope:

1. **GLOBAL SCOPE**: If a variable is declared outside a function, it can be used anywhere because it has global scope. If you do not use the var keyword when creating a variable, it is placed in global scope.
2. **FUNCTION-LEVEL SCOPE**: When a variable is declared within a function, it can only be used within that function. This is because it has function-level scope.

## Exception-Handling Code

**Exception-Handling Code**: If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter **stops** and looks for exception-handling code. Using a set of statements, you can handle the error, incase if the error is not handled, the script will just **stop processing** and the user will not know why. So exception-handling code should inform users when there is a problem.

When an exception is thrown, the interpreter stops and checks the current execution context for exception-handling code, and it is keep going through the stack looking for error-handling code until it gets to the global context. If there is still no error handler, the script stops running and the Error object is created.

There are two things you can do with the errors:

1. **Debug the Script to Fix Errors**: Track down the source of the error, and fix it.
2. **Handle Errors Gracefully**: Handle errors gracefully using try, catch, throw, and finally statements.