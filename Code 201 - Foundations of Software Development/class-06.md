# Class 06 Summary

### Problems Domain:
    Understanding Problem domain is the hardest part of programming

#### Hardest things in writing code:
1. Learning new technology
2. Naming things
3. Testing our code
4. Debugging
5. Fixing bugs

To make Programming easy we should understand the problem domain
***********************************************************************************************
### Object In JavaScript:
#### What is object?
     a set of variables and functions to create a model of something from the real world.
 
 * Properties are variables in an object , and Functios become Methods.
 * Properties and Methods have name and value . the name called a key.
* An object cannot have two keys with the same name.
* Property value can be string, number, Boolean, array or another object.but the value of method is always a function.

* Example:
 var person = {
  firstName: "John",
  lastName: "Doe",
  age: 50,
  eyeColor: "blue"
};

* We use dot notation to access object properties and methods.
example: let name=person.firstName;
or name = person['firstname'];


#### Document Object Model(DOM):
Making The HTML Model and With the HTML DOM,JavaScript can access and change all the elements of an HTML document.

* The DOM tree is a model of a web page.it consists of 4 types of nodes:
1. The document node.
2. Element nodes.
3. Attribute nodes.
4. Text Nodes

![Img1](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/08/Js-Dom-Tree.png)

* DOM Queries: methods to find elements in the DOM tree .

* Storing elements in variables = storing the location of the elements in DOM tree.
  Example :
  var itemOne = getElementById('one');

DOM queries  return one element, or  return a Nodelist,
which is a collection of nodes.

* Methods return a single element node:
1. getElementById('id')
2. querySelector('css selector')

* Methods return nodeList:
1. getElementByClassName('class')
2. getElementByTagName('tagname')
3. querySelectorAll('css selector')

* If we have a nodeList we can loop through each node and do statement to each.

Example:
var myNodelist = document.querySelectorAll("p");
var i;
for (i = 0; i < myNodelist.length; i++) {
  myNodelist[i].style.color = "red";
}






