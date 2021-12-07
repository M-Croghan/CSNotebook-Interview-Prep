# JAVA OOP
### <span style="color: aqua">What are the 4 pillars of Object Oriented Programming? Describe them:</span>
    - Abstraction: You don't need to know the inner workings of something to use it.  
    - Polymorphism: A method can have multiple implementations (overriding & overloading).  
    - Inheritance: Allows a class to inherit code from another. Improves code reuse and decreased development time. Java does not support multiple inheritence.  
    - Encapsulation: Related to abstraction, hiding of information which if left free to be manipulated can have harmful / unintended consequences.  

### <span style="color: aqua">What is a class?</span>
A class acts as a blueprint in which objects can be created. A simple example is a pattern to create a dress. The pattern is the class and the dress that is made from it is the object. Classes contain the relevant data and behavior(s) an object has.

### <span style="color: aqua">Discuss some of Java's naming conventions:</span>
- Class names are always the same as the file name, with each class being its own unique & seperate file.
- Class names are capitalized.
- Variables should be logical & concise. 
- CamelCasing  

### <span style="color: aqua">Does Java Support Multiple Inheritance?</span>
No

### <span style="color: aqua">Explain the difference between an object & a class:</span>
.  
Top level classes can only be public or default (not an inner class)  
A file may contain no more than 1 public class. Default classes don't specify an access modifier.  
  
### <span style="color: aqua">Explain the difference between method _overloading_ vs method _overriding_:</span>
(Discuss method signature as well: the # of paramters specific to the constructor / method)
  
### <span style="color: aqua">What is a ***constructor***?</span>
Constructors are called first when an object of a class is instantiated. It is essentially responsible for setting up that object  
including assigning specific data members with values passed to it. If a class lacks a constructor, Java assigns one at run time.  
This empty constructor which maintains no parameters is known as the default constrcutor. Constructors cannot be private, they  
are _always public_.

### <span style="color: aqua">Where are objects / varibles stored?</span>
Normals variables are stored in the ***stack***.  
Objects are stored in the ***heap***.  


### <span style="color: aqua">Disucss the difference between _compiled_ & _interpreted_ languages:</span>
.

### <span style="color: aqua">What are some of the benefits / features of Java?</span>
* Platform Independent ("Write once, run anywhere" / Bytecode)
* Memory Management (JVM handles garbage collection)
* Backward Compatible (Older versions supported despite new changes)
* Maturity & Support (Libaries & extensive documentation)

### <span style="color: aqua">Discuss Exception Handling:</span>