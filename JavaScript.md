# JAVASCRIPT CONCEPTS & QUESTIONS

### :scroll: <span style="color: aqua">What is AJAX?</span>
AJAX stands for Asynchronous JavaScript and XML. It isn't a programming language but rather a method through which we are able to make HTTP requests. AJAX uses a combination of:  
* A browser built-in XMLHttpRequest object (to request data from a web server)  
* JavaScript and HTML DOM (to display or use the data)  

AJAX allows web pages to be updated asynchronously by exchanging data with a web server behind the scenes. Meaning that it is possible to update parts of a web page, without reloading the whole page.

### :scroll: <span style="color: aqua">Tell me about when you may need to use AJAX?</span>
When I want some change to occur within a page in real time without reloading the entire page itself. Chat Bot interaction or Captcha validation / reloading are excellent examples where users would need to interact with something on a page and not have the page reload entirely.

### :scroll: <span style="color: aqua">What does callback mean in JS?</span>
JS functions are executed in the sequence they're called, not in the sequence they're defined. A ***callback*** is a function passed as an argumnt to another function. For instance, a callback function may take an input and display some data on a page. Passing it to a function that performs some calculation and then passing the result to the callback function will then display that calculation. This is a fairly simplified example, callbacks are best seen in asynchronous functions where 1 function has to wait for another function (i.e. waiting for a file to load).

### :scroll: <span style="color: aqua">What is JavaScript?</span>
JavaScript is a client-side and server-side scripting language inserted into HTML pages and is understood by web browsers. JavaScript is also an Object-based Programming language

### :scroll: <span style="color: aqua">Enumerate the differences between Java and JavaScript?</span>
Java is a complete programming language. In contrast, JavaScript is a coded program that can be introduced to HTML pages. These two languages are not at all inter-dependent and are designed for different intent. Java is an object-oriented programming (OOPS) or structured programming languages like C++ or C, whereas JavaScript is a client-side scripting language.
### :scroll: <span style="color: aqua">What are JavaScript Data Types?</span>
Following are the JavaScript Data types:

    Number
    String
    Boolean
    Object
    Undefined

### :scroll: <span style="color: aqua">What is the use of isNaN function?</span>
isNan function returns true if the argument is not a number; otherwise, it is false.
### :scroll: <span style="color: aqua">Which is faster between JavaScript and an ASP script?</span>
JavaScript is faster. JavaScript is a client-side language,, and thus it does not need the assistance of the webserver to execute. On the other hand, ASP is a server-side language and hence is always slower than JavaScript. Javascript now is also a server-side language (nodejs).
### :scroll: <span style="color: aqua">What is negative Infinity?</span>
Negative Infinity is a number in JavaScript which can be derived by dividing negative number by zero.
### :scroll: <span style="color: aqua">What are undeclared and undefined variables?
</span>
Undeclared variables are those that do not exist in a program and are not declared. If the program tries to read the value of an undeclared variable, then a runtime error is encountered.

Undefined variables are those that are declared in the program but have not been given any value. If the program tries to read the value of an undefined variable, an undefined value is returned.
### :scroll: <span style="color: aqua">What are global variables? How are these variable declared? </span>
Global variables are available throughout the length of the code so that it has no scope. The var keyword is used to declare a local variable or object. If the var keyword is omitted, a global variable is declared.

Example:

// Declare a global: globalVariable = “Test”;

The problems faced by using global variables are the clash of variable names of local and global scope. Also, it is difficult to debug and test the code that relies on global variables.
### :scroll: <span style="color: aqua">What is a prompt box?</span>
A prompt box is a box that allows the user to enter input by providing a text box. A label and box will be provided to enter the text or number.
### :scroll: <span style="color: aqua">What is ‘this’ keyword in JavaScript?</span>
‘This’ keyword refers to the object from where it was called.
### :scroll: <span style="color: aqua">What is the working of timers in JavaScript?</span>
Timers are used to execute a piece of code at a set time or repeat the code in a given interval. This is done by using the functions setTimeout, setInterval, and clearInterval.
The setTimeout(function, delay) function is used to start a timer that calls a particular function after the mentioned delay. The setInterval(function, delay) function repeatedly executes the given function in the mentioned delay and only halts when canceled. The clearInterval(id) function instructs the timer to stop.
Timers are operated within a single thread, and thus events might queue up, waiting to be executed.
### :scroll: <span style="color: aqua">Which symbol is used for comments in Javascript?</span>
// for Single line comments and

/* Multi
Line
Comment
*/
### :scroll: <span style="color: aqua">What is the difference between ViewState and SessionState?</span>
    ‘ViewState’ is specific to a page in a session.
    ‘SessionState’ is specific to user-specific data that can be accessed across all web application pages.

### :scroll: <span style="color: aqua">What is === operator?</span>
=== is called a strict equality operator, which returns true when the two operands have the same value without conversion.
### :scroll: <span style="color: aqua">How you can submit a form using JavaScript?</span>
To submit a form using JavaScript use  

document.form[0].submit();  
document.form[0].submit();  

### :scroll: <span style="color: aqua">Does JavaScript support automatic type conversion?</span>
Yes, JavaScript does support automatic type conversion. It is the common way of type conversion used by JavaScript developers
### :scroll: <span style="color: aqua">How can the style/class of an element be changed?</span>
It can be done in the following way:  
    document.getElementById("myText"). style. fontSize = "20";  
or  
    document. getElementById ("myText"). className = "anyclass";  

### :scroll: <span style="color: aqua">How to read and write a file using JavaScript?</span>
There are two ways to read and write a file using JavaScript
    Using JavaScript extensions
    Using a web page and Active X objects

### :scroll: <span style="color: aqua">What are all the looping structures in JavaScript?</span>
Following are looping structures in Javascript:
    For
    While
    Do-while loops

### :scroll: <span style="color: aqua">What is called Variable typing in Javascript?</span>
Variable typing is used to assign a number to a variable. The same variable can be assigned to a string.  
- Example:  
    - i = 10;  
    - i = "string;"  

### :scroll: <span style="color: aqua">How can you convert the string of any base to an integer in JavaScript?</span>
The parseInt() function is used to convert numbers between different bases. parseInt() takes the string to be converted as its first parameter. The second parameter is the base of the given string.
To convert 4F (or base 16) to integer, the code used will be – parseInt ("4F", 16);

### :scroll: <span style="color: aqua">Difference between “==” and “===”?</span>
“==” checks only for equality in value, whereas “===” is a stricter equality test and returns false if either the value or the type of the two variables are different.
### :scroll: <span style="color: aqua">What would be the result of 3+2+”7″?</span>
Since 3 and 2 are integers, they will be added numerically. And since 7 is a string, its concatenation will be done. So the result would be 57.
### :scroll: <span style="color: aqua">How to detect the operating system on the client machine?</span>
In order to detect the operating system on the client machine, the navigator. Platform string (property) should be used.
### :scroll: <span style="color: aqua">What do you mean by NULL in Javascript?</span>
The NULL value is used to represent no value or no object. It implies no object or null string, no valid boolean value, no number, and no array object.
### :scroll: <span style="color: aqua">What is the function of the delete operator?</span>
The delete keyword is used to delete the property as well as its value.
- Example
    - var student= {age:20, batch:"ABC"};
    - Delete student. age;

### :scroll: <span style="color: aqua">What is an undefined value in JavaScript?</span>
Undefined value means the
    Variable used in the code doesn’t exist
    Variable is not assigned to any value
    Property does not exist.

### :scroll: <span style="color: aqua">What are all the types of Pop up boxes available in JavaScript?</span>
    Alert
    Confirm and
    Prompt

### :scroll: <span style="color: aqua">What is the use of Void (0)?</span>
Void(0) is used to prevent the page from refreshing, and parameter “zero” is passed while calling.  
Void(0) is used to call another method without refreshing the page.
### :scroll: <span style="color: aqua">How can a page be forced to load another page in JavaScript?</span>
The following code has to be inserted to achieve the desired effect:  
```<script language="JavaScript" type="text/javascript" >```
```<!-- location. href="http://newhost/newpath/newfile.html"; //--></script>```

### :scroll: <span style="color: aqua">What is the data type of variables in JavaScript?</span>
All variables in JavaScript are object data types.
### :scroll: <span style="color: aqua">What is the difference between an alert box and a confirmation box?</span>
An alert box displays only one button, which is the OK button.
But a Confirmation box displays two buttons, namely OK and cancel.
### :scroll: <span style="color: aqua">What are escape characters?</span>
Escape characters (Backslash) is used when working with special characters like single quotes, double quotes, apostrophes, and ampersands. Place backslash before the characters to make it display.
### :scroll: <span style="color: aqua">What are JavaScript Cookies?</span>
Cookies are the small test files stored in a computer, and they get created when the user visits the websites to store information that they need. Examples could be User Name details and shopping cart information from previous visits.
### :scroll: <span style="color: aqua">What a pop() method in JavaScript is?</span>
The pop() method is similar to the shift() method, but the difference is that the Shift method works at the array’s start. The pop() method takes the last element off of the given array and returns it. The array on which it is called is then altered.
### :scroll: <span style="color: aqua">Does JavaScript has concept level scope?</span>
No. JavaScript does not have concept-level scope. The variable declared inside the function has scope inside the function.
### :scroll: <span style="color: aqua">What are the disadvantages of using innerHTML in JavaScript?</span>
If you use innerHTML in JavaScript, the disadvantage is:
    Content is replaced everywhere
    We cannot use it like “appending to innerHTML
    Even if you use +=like “innerHTML = innerHTML + ‘html'” still the old content is replaced by html
    The entire innerHTML content is re-parsed and builds into elements. Therefore, it’s much slower
    The innerHTML does not provide validation, and therefore we can potentially insert valid and broken HTML in the document and break it

### :scroll: <span style="color: aqua">What is break and continue statements?</span>
Break statement exits from the current loop.  
Continue statement continues with next statement of the loop.
### :scroll: <span style="color: aqua">What are the two basic groups of data types in JavaScript?</span>
    They are as—Primitive
    Reference types
Primitive types are number and Boolean data types. Reference types are more complex types like strings and dates.
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
Catch(exp){  
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
Variable typing assigns a number to a variable and then assigns a string to the same variable. An example is as follows:  
- i= 8;
- i="john";

### :scroll: <span style="color: aqua">How to find an operating system in the client machine using JavaScript?</span>
The ‘Navigator. the app version is used to find the operating system’s name in the client machine.
### :scroll: <span style="color: aqua">What are the different types of errors in JavaScript?</span>
There are three types of errors:  
    Load time errors: Errors that come up when loading a web page, like improper syntax errors, are known as Load time errors and generate the errors dynamically.
    Runtime errors: Errors that come due to misuse of the command inside the HTML language.
    Logical Errors: These are the errors that occur due to the bad logic performed on a function with a different operation.

### :scroll: <span style="color: aqua">What is DOM in JavaScript?</span>
JavaScript can access all the elements in a web page using the Document Object Model (DOM). The web browser creates a DOM of the webpage when the page is loaded.
### :scroll: <span style="color: aqua">What is the use of the Push method in JavaScript?</span>
The push method is used to add or append one or more elements to an Array end. Using this method, we can append multiple elements by passing multiple arguments.
### :scroll: <span style="color: aqua">What is the unshift method in JavaScript?</span>
Unshift method is like the push method, which works at the beginning of the array. This method is used to prepend one or more elements to the beginning of the array.
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
The ‘And’ Operator (&&), ‘Or’ Operator (||), and the ‘Not’ Operator (!) can be used in JavaScript.  
*Operators are without the parenthesis.
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
### :scroll: <span style="color: aqua"></span>

### :scroll: <span style="color: aqua"></span>

### :scroll: <span style="color: aqua"></span>

### :scroll: <span style="color: aqua"></span>

### :scroll: <span style="color: aqua"></span>