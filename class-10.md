# Class 10 Summary:

## Error Handling & Debugging:

#### Order Of Excution:
* To find the source of an error, it helps to know how scripts are processed. some tasks
cannot complete until another statement or function has been run.
* JavaScript interpreter uses the concept of execution cntexts. ther is one execution context and each function creates a new execution context.

#### The Stack:
* JavaScript process one line of code at a time. when statement need data from a function it stack the new function on the top of the task.

#### Tow phases of activity when enter a new execution context:
1. Prepare (new scope created, variable and functions created, the value of this keyword determined).
2. Execute (assign values to variables,run functions code,Execute Statements).
* The error when generated it throws an exception.interpreter stops & looks for exception handling code.

#### Error Objects:
* can help to find where the mistakes are and there are tools in browsers help to read them.

#### Error Bojects:
* Syntax Error: incorrect use of the language rules.
* Reference Error:variable that is not declared or is out of scope.
* Type Error:value in unexpected data type.
* Range Error:Number outside of range.

#### Debugging Workflow:
eliminating potential causes of an error.
###### Workflow Techniques :
1. Where is the Problem?
2. What Exactly is the Problem?

##### Script Errors:
1. Go back to basics
2. missed extra characters.
3. Data type Issues.

##### If we know that we may get an error, we can handle it gracefully using the (try, catch, finally) statements.

**Thank You**

**Sukina AbuHammad**