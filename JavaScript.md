# JAVASCRIPT CONCEPTS & QUESTIONS

### :scroll: <span style="color: aqua">What is AJAX?</span>
AJAX stands for Asynchronous JavaScript and XML. It isn't a programming language but rather a method through which we are able to make HTTP requests. AJAX uses a combination of:  
* A browser built-in XMLHttpRequest object (to request data from a web server)  
* JavaScript and HTML DOM (to display or use the data)  

AJAX allows web pages to be updated asynchronously by exchanging data with a web server behind the scenes. Meaning that it is possible to update parts of a web page, without reloading the whole page.

### :scroll: <span style="color: aqua">Tell me about when you may need to use AJAX?</span>
When I want some change to occur within a page in real time without reloading the entire page itself. Chat Bot interaction or Captcha validation / reloading are excellent examples where users would need to interact with something on a page and not have the page reload entirely.

### :scroll: <span style="color: aqua">What does callback mean in JS?</span>
JS functions are executed in the sequence they're called, not in the sequence they're defined. A ***callback*** is a function passed as an argument to another function. For instance, a callback function may take an input and display some data on a page. Passing it to a function that performs some calculation and then passing the result to the callback function will then display that calculation. This is a fairly simplified example, callbacks are best seen in asynchronous functions where 1 function has to wait for another function (i.e. waiting for a file to load).

### :scroll: <span style="color: aqua">What is JavaScript?</span>
JavaScript is a client-side and server-side scripting language inserted into HTML pages and is understood by web browsers. JavaScript is also an Object-based Programming language

### :scroll: <span style="color: aqua">Enumerate the differences between Java and JavaScript?</span>
Java is a complete programming language. In contrast, JavaScript is a coded program that can be introduced to HTML pages. These two languages are not at all inter-dependent and are designed for different intent. Java is an object-oriented programming (OOP) or structured programming languages like C++ or C, whereas JavaScript is a client-side scripting language.
### :scroll: <span style="color: aqua">What are JavaScript Data Types?</span>
Following are the JavaScript Data types:
* Primitive Values:    
    * Number
    * String
    * Boolean
    * Null
    * Undefined
    * Symbol
    * BigInt
* Objects

### :scroll: <span style="color: aqua">What is the use of isNaN function?</span>
isNan function checks whether a given value is an illegal number or not. Returns true if the argument is not a number; otherwise, it is false.
### :scroll: <span style="color: aqua">Which is faster between JavaScript and an ASP script?</span>
JavaScript is faster. JavaScript is a client-side language, and thus it does not need the assistance of the webserver to execute. On the other hand, ASP is a server-side language and hence is always slower than JavaScript. Javascript now is also a server-side language (Nodejs).
### :scroll: <span style="color: aqua">What is negative Infinity?</span>
The negative infinity in JavaScript is a constant value which is used to represent a value which is the lowest available. This means that no other number is lesser than this value. Negative infinity results in 0 when divided by any other number. 
### :scroll: <span style="color: aqua">What are undeclared and undefined variables?
</span>
* ***Undeclared variables*** are those that do not exist in a program and are not declared. If the program tries to read the value of an undeclared variable, then a runtime error is encountered.

* ***Undefined variables*** are those that are declared in the program but have not been given any value. If the program tries to read the value of an undefined variable, an undefined value is returned.
### :scroll: <span style="color: aqua">What are global variables? How are these variable declared? </span>
Global variables are available throughout the length of the code (global scope). The let / const keyword is used to declare a local variable or object. If the var/let/const keyword is omitted, a global variable is declared.

Example:
```globalVariable = “Test”;```

The problems faced by using global variables are the clash of variable names of local and global scope. Also, it is difficult to debug and test the code that relies on global variables.
### :scroll: <span style="color: aqua">What is a prompt box?</span>
A prompt box is often used if you want the user to input a value before entering a page. When a prompt box pops up, the user will have to click either "OK" or "Cancel" to proceed after entering an input value. If the user clicks "OK" the box returns the input value.
### :scroll: <span style="color: aqua">What is ‘this’ keyword in JavaScript?</span>
‘This’ keyword refers to the object from where it was called.
### :scroll: <span style="color: aqua">What is the working of timers in JavaScript?</span>
Timers are used to execute a piece of code at a set time or repeat the code in a given interval. This is done by using the functions setTimeout, setInterval, and clearInterval.
The setTimeout(function, delay) function is used to start a timer that calls a particular function after the mentioned delay. The setInterval(function, delay) function repeatedly executes the given function in the mentioned delay and only halts when canceled. The clearInterval(id) function instructs the timer to stop.
Timers are operated within a single thread, and thus events might queue up, waiting to be executed.
### :scroll: <span style="color: aqua">Which symbol is used for comments in Javascript?</span>
Similar to Java:  
// for Single line comments

/* Multi
Line
Comment
*/
### :scroll: <span style="color: aqua">What is the difference between ViewState and SessionState?</span>
- ***‘ViewState’*** is specific to a page in a session.
- ***‘SessionState’*** is specific to user-specific data that can be accessed across all web application pages.

### :scroll: <span style="color: aqua">What is === operator?</span>
=== is called a strict equality operator, it is used for comparison between two variables but this will check strict type, which means it will check datatype and compare two values. It's best to avoid using == (which only compares variables irrespective of datatype).

### :scroll: <span style="color: aqua">Does JavaScript support automatic type conversion?</span>
Yes, JavaScript does support automatic type conversion. It is the common way of type conversion used by JavaScript developers.
### :scroll: <span style="color: aqua">How can the style/class of an element be changed?</span>
It can be done in the following way:  
    document.getElementById("myText"). style. fontSize = "20";  
or  
    document. getElementById ("myText"). className = "anyclass";  

### :scroll: <span style="color: aqua">How to read and write a file using JavaScript?</span>
To my current understanding, its not something you can do client-side, only server-side.

### :scroll: <span style="color: aqua">What are all the looping structures in JavaScript?</span>
Following are looping structures in Javascript:
* For
* While
* Do-while loops

### :scroll: <span style="color: aqua">What is _variable typing_ in Javascript?</span>
It means that JavaScript will figure out what type of data you have and make the necessary adjustments so that you don't have to redefine your different types of data. 

### :scroll: <span style="color: aqua">How can you convert the string of any base to an integer in JavaScript?</span>
The parseInt() function is used to convert numbers between different bases. parseInt() takes the string to be converted as its first parameter. The second parameter is the base of the given string.
To convert 4F (or base 16) to integer, the code used will be – parseInt("4F", 16);

### :scroll: <span style="color: aqua">Difference between “==” and “===”?</span>
“==” checks only for equality in value, whereas “===” is a stricter equality test and returns false if either the value or the type of the two variables are different.
### :scroll: <span style="color: aqua">What would be the result of 3+2+”7″?</span>
Since 3 and 2 are integers, they will be added numerically. And since 7 is a string, its concatenation will be done. So the result would be 57.
### :scroll: <span style="color: aqua">How to detect the operating system on the client machine?</span>
In order to detect the operating system on the client machine, the navigator property.  
- Using ```navigator.userAgent``` returns:
    - "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:97.0) Gecko/20100101 Firefox/97.0"
### :scroll: <span style="color: aqua">What do you mean by NULL in Javascript?</span>
The NULL value is used to represent no value or no object. It implies no object or null string, no valid boolean value, no number, and no array object.
### :scroll: <span style="color: aqua">What is the function of the delete operator?</span>
The delete keyword is used to delete the property as well as its value.
- Example
    - var student= {age:20, batch:"ABC"};
    - Delete student. age;
- If one were wanted to _add_ a property, simple use dot notation with desired variable and set the value:
    - student.gpa = 4.0

### :scroll: <span style="color: aqua">What is an undefined value in JavaScript?</span>
- Undefined value means the
    - Variable used in the code doesn’t exist
    - Variable is not assigned to any value
    - Property does not exist.

### :scroll: <span style="color: aqua">What are all the types of Pop up boxes available in JavaScript?</span>
1. Alert
2. Confirm
3. Prompt

### :scroll: <span style="color: aqua">What is the use of Void (0)?</span>
Void(0) is used to prevent the page from refreshing, and parameter “zero” is passed while calling.  
Void(0) is used to call another method without refreshing the page.
### :scroll: <span style="color: aqua">How can a page be forced to load another page in JavaScript?</span>
The following code has to be inserted to achieve the desired effect:  
```<script language="JavaScript" type="text/javascript" >```
```<!-- location. href="http://newhost/newpath/newfile.html"; //--></script>```

### :scroll: <span style="color: aqua">What is the difference between an alert box and a confirmation box?</span>
An alert box displays only one button, which is the OK button.
But a Confirmation box displays two buttons, namely OK and cancel.
### :scroll: <span style="color: aqua">What are escape characters?</span>
Escape characters (Backslash) is used when working with special characters like single quotes, double quotes, apostrophes, and ampersands. Place backslash before the characters to make it display.
### :scroll: <span style="color: aqua">What are JavaScript Cookies?</span>
Cookies are the small test files stored in a computer, and they get created when the user visits the websites to store information that they need. Examples could be User Name details and shopping cart information from previous visits.
### :scroll: <span style="color: aqua">What a pop() method in JavaScript is?</span>
The pop() method is similar to the shift() method, but the difference is that the Shift method works at the array’s start. The pop() method takes the last element off of the given array and returns it. The array on which it is called is then altered.
### :scroll: <span style="color: aqua">Does JavaScript have concept level scope?</span>
No. JavaScript does not have concept-level scope. The variable declared inside the function has scope inside the function.
### :scroll: <span style="color: aqua">What are the disadvantages of using innerHTML in JavaScript?</span>
If you use innerHTML in JavaScript, the disadvantage is:
- Content is replaced everywhere
- We cannot use it like “appending to innerHTML
- Even if you use +=like “innerHTML = innerHTML + ‘html'” still the old content is replaced by html
- The entire innerHTML content is re-parsed and builds into elements. Therefore, it’s much slower
- The innerHTML does not provide validation, and therefore we can potentially insert valid and broken HTML in the document and break it

### :scroll: <span style="color: aqua">What is break and continue statements?</span>
***Break*** statement exits from the current loop & the ***Continue*** statement continues with next statement of the loop.
### :scroll: <span style="color: aqua">What are the two basic groups of data types in JavaScript?</span>
- Primitive types: numbers, booleans, null, & undefined
- Reference types: objects, arrays, functions

### :scroll: <span style="color: aqua">How can generic objects be created?</span>
Generic objects can be created as:
    - var I = new object();

### :scroll: <span style="color: aqua">What is the use of a type of operator?</span>
‘Typeof’ is an operator used to return a string description of the type of a variable.
### :scroll: <span style="color: aqua">Which keywords are used to handle exceptions?</span>
Try… Catch—finally is used to handle exceptions in the JavaScript  

Try{  
    Code  
}  
Catch(exception){  
    Code to throw an exception.  
}  
Finally{  
    Code runs either it finishes successfully or after catch  
}  

### :scroll: <span style="color: aqua">Which keyword is used to print the text on the screen?</span>
Document. Write (“Welcome”) is used to print the text–Welcome on the screen.

### :scroll: <span style="color: aqua">What is the use of the blur function?</span>
Blur function is used to remove the focus from the specified object.

### :scroll: <span style="color: aqua">What is variable typing?</span>
The type of a variable is determined only when a value is assigned and can change as the variable appears in different contexts. Example:  
- i= 8;
- i="john";

### :scroll: <span style="color: aqua">What are the different types of errors in JavaScript?</span>
There are three types of errors:  
* ***Load time errors***: Errors that come up when loading a web page, like improper syntax errors, are known as Load time errors and generate the errors dynamically.
* ***Runtime errors***: Errors that come due to misuse of the command inside the HTML language.
* ***Logical Errors***: These are the errors that occur due to the bad logic performed on a function with a different operation.

### :scroll: <span style="color: aqua">What is DOM in JavaScript?</span>
JavaScript can access all the elements in a web page using the Document Object Model (DOM). The web browser creates a DOM of the webpage when the page is loaded.
### :scroll: <span style="color: aqua">What is the use of the Push method in JavaScript?</span>
The push method is used to add or append one or more elements to an Array end. Using this method, we can append multiple elements by passing multiple arguments.
### :scroll: <span style="color: aqua">What is the unshift method in JavaScript?</span>
```unshift()``` method is like the push method, but works at the beginning of the array. This method is used to prepend one or more elements to the beginning of the array. Similarly, ```shift()``` acts like pop for the beginning of the array and removes the first element.
### :scroll: <span style="color: aqua">How are object properties assigned?</span>
Properties are assigned to objects in the following way:  
```obj ["class"] = 12;```  
or  
```obj.class = 12;```

### :scroll: <span style="color: aqua">How can a value be appended to an array?</span>
A value can be appended to an array in the given manner:  
```arr[arr.length] = value;```

### :scroll: <span style="color: aqua">What are the important properties of an anonymous function in JavaScript?</span>
A function that is declared without any named identifier is known as an anonymous function. In general, an anonymous function is inaccessible after its declaration.
### :scroll: <span style="color: aqua">What is event bubbling?</span>
JavaScript allows DOM elements to be nested inside each other. In such a case, if the handler of the child is clicked, the handler of the parent will also work as if it were clicked too.
### :scroll: <span style="color: aqua">Is JavaScript case sensitive? Give its example.</span>
Yes, JavaScript is case-sensitive. For example, a function parseInt is not the same as the function Parseint.
### :scroll: <span style="color: aqua">What boolean operators can be used in JavaScript?</span>
The ‘And’ Operator ```&&```, ‘Or’ Operator ```||```, and the ‘Not’ Operator ```!``` can be used in JavaScript.  
### :scroll: <span style="color: aqua">How are DOM utilized in JavaScript?</span>
DOM stands for Document Object Model and is responsible for how various objects in a document interact with each other. DOM is required for developing web pages, which includes objects like paragraphs, links, etc. These objects can be operated to include actions like add or delete. DOM is also required to add extra capabilities to a web page. On top of that, the use of API gives an advantage over other existing models.
### :scroll: <span style="color: aqua">How are event handlers utilized in JavaScript?</span>
Events are the actions that result from activities, such as clicking a link or filling a form by the user. An event handler is required to manage the proper execution of all these events. Event handlers are an extra attribute of the object. This attribute includes the event’s name and the action taken if the event takes place.
### :scroll: <span style="color: aqua">What are the various functional components in JavaScript?</span>
The different functional components in JavaScript are:  
* First-class functions: Functions in JavaScript are utilized as first-class objects. This usually means that these functions can be passed as arguments to other functions, returned as values from other functions, assigned to variables, or can also be stored in data structures.
* Nested functions: The functions, which are defined inside other functions, are called Nested functions. They are called ‘every time the main function is invoked.

### :scroll: <span style="color: aqua">What does the following statement declare?</span>
```var myArray = [[[]]];```  
It declares a three-dimensional array.
### :scroll: <span style="color: aqua">What is TypeScript?</span>
TypeScript is an open-sourced programming language developed & maintained by Microsoft. It is a superset of JavaScript, meaning that any valid TS program, is a valid JS program. It can be thought of as JavaScript with extra features (strongly typed, interfaces, generics). TS cannot run in a browser, and must be _transpiled_ into Javascript before it can be used in the browser. One of the big benefits is to enable IDEs to provide a richer environment for spotting common errors as you type the code and thus flesh out important aspects / details that may go unconsidered in standard JS.
### :scroll: <span style="color: aqua">What is _Transpiling_?</span>
Transpilers, or source-to-source compilers, are tools that read source code written in one programming language and produce the equivalent code in another language. In the context of Typescript, the transpiler converts to functional JavaScript.
