Hack Reactor "Coding Terms"
================================
###The difference between writing a function and invoking a function

Functions are reusable units of code. You can write a function once and invoke it several times. Functions are two types, either they do something or they return a value or both. 


Functions break a program into logical chunks and implement a piece of functionality. First we start off with declaring a function with the keyword function.
The implementation of a function is in a block, anything inside this block will be executed when the function is called.
Invoking functions is like calling the function, when you invoke a function you ask the function to perform specific tasks that the function is designed to carry out.  

###Passing functions as arguments to other functions

Imagine you have a function that executes 3 steps. We are not sure what our function should do on the second step. We can provide the second step as a function argument. Meaning that when we invoke our function, we pass in another function that can be used in the second step of our function. This enables us to pass different functions as parameters and reuse the code that is shared in our function. 

For example: 
~~~
// Returns a sum of parameters
var add = function (a, b) { 
	return a+b;
}

var multiply = function (a,b) {
	return a * b; 
}
var calculateAndPrint = function (perform, a, b) {
	var result = perform(a,b);	
	console.log(result);
}

calculateAndPrint(add, 3, 5);
calculateAndPrint(multiply, 3, 5);

~~~


According to JavaScriptissexy.com, “Because functions are first-class objects, we can pass a function as an argument in another function and later execute that passed-in function or even return it to be executed later. This is the essence of using callback functions in JavaScript.” 

In further reading “A callback function is a function that is passed as an argument of another function and it is invoked after some kind of event. The name “call back” can be attributed to the nature of the function, since once its parent function completes, the function that got passed as an argument gets called. In other words, the parent function “calls-back and executes the function passed as an argument.”
As you can already imagine, callbacks are extremely useful. They allow for you to call a function within a function.


### Iterating through an array or an object using a for 
Iteration is when you go through each element of a collection of objects. 



You can use the for loop structure to iterate over an array. 
In terms of iterating an array object you would iterate through 
~~~
for (var property in obj) {
			// Do something 
}
~~~








###Using if statements to let your code make decisions

You can program an If statement by using the following code that illustrates its
syntax:
~~~
If (Expression) Then
  Program statements
End If
~~~
An If statement consists of an expression that determines whether a program
statement or statements execute. An expression can be the comparison of two values.
To compare values you may use any of the following operators:

`>,<,>=,=<,===`

By placing variables on both sides of the operator we can create true and false statements.

Example: 

(Use if statements to let your code execute depending on conditions)

Reading in a file there are separate file extensions (comma separate and tab separated values). The program parses the incoming file extension, However the program parses the file differently depending on the extension. 

Ex. 
~~~
var filename = “…”
var fileExention = '',
    file;

// Check whether the extension is a comma separated value format
if (fileExtension === '.csv') {
    parseCSV(file);
} else if (fileExtension === '.xml') {
    parseXML(file);
} else {
    // Unsupported format that you can't parse
    throw Exception ()
}

functionparsefileName(fileName) {

   var fileExtension = fileName.match(//),
    file;

// Check whether the extension is a comma separated value format
  if (fileExtension === '.csv') {
    parseCSV(file);
  } else if (fileExtension === '.xml') {
    parseXML(file);
  } else {
    // Unsupported format that you can't parse
     throw "Unsupported file format";
  }
 }
}
~~~




