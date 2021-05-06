# Class 10 Summary :

### JavaScript Call Stack :

* Call Stack : it is synchronous, excutes the function one at the time used for calling the function.

* when calles function the interpreter add this function in call stack, when another function called by this function also added into call stack and excute when the calls reached. When the function finished the interpreter take it out call stack .

* LIFO : (last in, first out) used to manage function calling. The last function enter call stack, it will be the first to be out.

* Example of call stack :

![call stack](https://i.ytimg.com/vi/2ZH_1d8TYVg/maxresdefault.jpg)

![call stack2](https://miro.medium.com/max/638/1*CCHexfHNCNo-f8aw3rbRew.jpeg)

* Stack overflow : caused when there is a function calls itself .

**************************************************************************

### JavaScript Error Message:

* Reference errors : if you want to use variable you doesn't declare yet.also (letand const).

* syntax errors : when you make somthing wrong in syntax or in the source code of program .

* Range errors : when trying to pass value as an argument to function that not allow a range that includes the value.

* Type errors : when use or access the types (boolean, number, string,...) are incompatible. (access undefined types).

* Breakpoint : stopping or pausing place in the program during the execution. we can get it by putting a debugger statement in the breakpoint which we want in the code.

* Debugger : detect and remove the existing errors in the software code which cause crash or unexpected behaviour.

*******************************************************

* Sources:

[source1](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

[source2](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)