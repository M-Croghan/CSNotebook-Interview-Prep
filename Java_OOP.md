# JAVA OOP CONCEPTS & QUESTIONS
### <span style="color: aqua">What are the 4 pillars of Object Oriented Programming? Describe them:</span>
- ***Abstraction***: You don't need to know the inner workings of something to be able use it. 
  - Abstraction is a process of hiding the implementation details and showing only functionality to the user. 
  - Lets you focus on what the object does instead of how it does it.
  - Greatly improves code reusability & maintainability!
  - Data abstraction can be used to provide security for the data from the unauthorized methods.
  - A non-abstract approach is hard coding every possiblility in every use case. Abstraction removes this complexity. If you were creating a coffee machine, an abstract example would be a machine with a single button: _Make Coffee_. You don't need to know all of the additional steps.  


- ***Polymorphism***: A method can have multiple implementations (overriding & overloading).
  - Polymorphism in Java occurs when there are one or more classes or objects related to each other by inheritance capable of doing different things.
  - It is the ability of an object to take many forms. Inheritance lets users inherit attributes and methods, and 
  polymorphism uses these methods to perform different tasks. So, the goal is communication, but the approach is different.
    - For instance, a cat class and a dog class both inherit the animal ```sound``` from the Animal superclass. However, the cat 'meows' whereas the dog 'barks'.


- ***Inheritance***: Allows a class to inherit code from another.
  - Improves code reuse and decreased development time. 
  - Java does not support multiple inheritance. 
  - Using the _extends_ keyword, means that a class is inherits from another class.
  - Inheritance is a mechanism in which one class gains the properties & methods of another class. 
  - With inheritance, we can reuse the fields and methods of the existing class.  

  ***Liskov Substitution principle*** states that if you can use a parent class (let's call it ```ParentType```) anywhere you use a child (let's call it ```ChildType```) – and ```ChildType``` inherits from the ```ParentType``` – then you pass the test. The main reason you would fail this test, is if the ```ChildType``` is removing things from the parent. If ```ChildType``` removed methods it inherited from the parent, it'd lead to TypeError's where things are undefined that you are expecting not to be.


- ***Encapsulation***: Related to abstraction, hiding of information which is left free to be manipulated can have harmful / unintended consequences.
  - In object-oriented computer programming languages, the notion of encapsulation (or OOP Encapsulation) refers to 
  the bundling of data, along with the methods that operate on that data, into a single unit. Each unit or object should control its own state.
  - It limits what pieces of your code can access the methods / properties of the object.


### <span style="color: aqua">What is a class?</span>
A class acts as a blueprint in which objects can be created. A simple example is a pattern to create a dress. The pattern is the class and the dress that is made from it is the object. Classes contain the relevant data and behavior(s) an object has.

### <span style="color: aqua">What is an object?</span>
An instance of a class - contains the basic properties / states and behavior. Objects are instantiated using the 'new' keyword

### <span style="color: aqua">Discuss some of Java's naming conventions:</span>
- Class names are always the same as the file name, with each class being its own unique & separate file.
- Class names are capitalized and should be a noun
- Methods should be a verb and start with a lowercase letter
- Variables start with a lowercase letter, should be logical & concise, avoiding single character names.
- Packages should be all lowercase. Separate multiple words with dots: ```java.lang```
- Constants should be all uppercase and multiple words separated by underscores: ```MAX_VALUE```
- CamelCasing  


### <span style="color: aqua">Explain the difference between an object & a class:</span>
```Class```: The building block that leads to Object-Oriented Programming. It is a user-defined data type, that holds its own data members and member functions, which can be accessed and used by creating an instance of that class. It is the blueprint of any object. 

```Object```: An object is an instance of a class. All data members and member functions of the class can be accessed with the help of objects. When a class is defined, no memory is allocated but when it is instantiated (i.e. an object is created), memory is allocated. For example, considering the objects for the Account class is Saving account, Current account, etc.

Top level classes can only be public or default (not an inner class)  
A file may contain no more than 1 public class. Default classes don't specify an access modifier.  
  
### <span style="color: aqua">Explain the difference between method _overloading_ vs method _overriding_:</span>
- Overloading occurs between the methods in the same class.
  - Method Overloading is a Compile time polymorphism. In method overloading, more than one method shares the same method name with a different signature in the class. In method overloading, the return type can or can not be the same, but we have to change the parameter because, in java, we can not achieve the method overloading by changing only the return type of the method. 
- Overriding occurs between superclass and subclass.
  - Method Overriding is a Run time polymorphism. In method overriding, the derived class provides the specific implementation of the method that is already provided by the base class or parent class. In method overriding, the return type must be the same or co-variant (return type may vary in the same direction as the derived class).
  
### <span style="color: aqua">What is a ***constructor***?</span>
A constructor is a special method that is used to create an object out of a class definition. Constructors are called first when an object of a class is instantiated. It is essentially responsible for setting up that object including assigning specific data members with values passed to it. If a class lacks a constructor, Java assigns one at run time. This empty constructor which maintains no parameters is known as the default constructor. Constructors cannot be private, they are _always public_. You can have more than 1 constructor which accepts different parameters (overloading).

### <span style="color: aqua">Where are objects / variables stored?</span>
- Normal variables are stored in the ***stack***.
- Objects are stored in the ***heap***.
    - The JVM allocates the heap, inside which resides the ***string pool***

### <span style="color: aqua">What are some of the benefits / features of Java?</span>
*	Object-oriented - every is an object / easily extended.
*	Platform independent - Compiled and run on the JVM ("Write once, run anywhere" / Bytecode)
*	Simple - relatively simple to learn if understand OOP
*	Secure - enables virus / tamper-free systems.
*	Architecture-Neutral - file format which compiled code can run on many processors.
*	Portable - due to its arch. neutrality / no implementation independent aspects.
*	Supports Multithreading
*	Robust - emphasizes compile time & runtime error checks
*	Interpreted - byte code translated on the fly to native machine languages.
* Memory Management (JVM handles garbage collection)
* Backward Compatible (Older versions supported despite new changes)
* Maturity & Support (Libraries & extensive documentation)

### <span style="color: aqua">Discuss Exception Handling (Errors vs. Exceptions)</span>
* ***Errors*** refers to an illegal operation performed by the user which results in the abnormal working of the program.  Programming errors often remain undetected until the program is compiled or executed. Some of the errors inhibit the program from getting compiled or executed. Thus errors should be removed before compiling and executing. It is of three types: Compile-time, Run-time, Logical.  

* ***Exceptions*** refer to an unwanted or unexpected event, which occurs during the execution of a program i.e at run time, that disrupts the normal flow of the program’s instructions. They indicates conditions that a reasonable application might want to catch. Exceptions are the conditions that occur at runtime and may cause the termination of the program. But they are recoverable using try, catch and throw keywords. (Checked & Unchecked Exceptions)


### <span style="color: aqua">Discuss Abstract Classes:</span>
Abstract classes aim to implement the same or different behavior among multiple related objects. They provide just a method signature which allows you to implement a framework / template method design pattern. They can contain both abstract and concrete methods but the abstract methods must be implemented elsewhere. Concrete methods are distinguished by having a full name & method body. They cannot be instantiated. Can have final methods which will force the subclass to not change the method body.

### <span style="color: aqua">Discuss Interfaces:</span>
Interfaces are totally incomplete. They do not have any properties. They must show that the inheriting children are capable of doing something. You cannot instantiate abstract classes or interfaces. By default, all methods are abstract. Methods themselves are the only things composing an interface, it merely acts as a contract with the compiler which states that these specific methods must be implemented by whatever class implements the interface. They cannot be static or involve any implementation.

### <span style="color: aqua">Can you achieve multiple inheritance in Java:</span>
No, You can only extend from a single class. BUT - you can achieve multiple inheritance through the use of interfaces. (I.e. extending an abstract class, and implementing multiple interfaces). 

### <span style="color: aqua">Using an abstract class vs. an interface</span>
Use abstract classes when:  
    - You need both static / non-static methods  
    - You need both abstract & non-abstract methods  
    - You don't want all of your fields to be final

Use interfaces when:  
    - All methods are abstract  
    - You need future devs to follow a pattern in development  
    - You need to use more than one interface (A class can implement multiple interfaces <- an advantage over an abstract class)

***Abstract Class***: a class which is declared with the “abstract” keyword. Cannot be instantiated thus you cannot create an object with it. It’s a collection of subclass methods and can have multiple concrete methods but includes at least 1 abstract method. When you require a base class or when several implementations of the same type share a common behavior.  

***Interface***: Is like a blueprint to implement a class. Maintains a collection of abstract methods but contains no concrete methods. But it offers full abstraction (something an abstract class can’t do). A declaration of the methods of a class but not the implementation. The operations an object can perform is defined and are used by the classes which implement that interface. Best used when various implementations share only method signature. When your classes need additional behavior or dependency injection.

### <span style="color: aqua">Prove: Everything in Java is an object.</span>
With the exception of primatives, references, variables everything in java inherits from the object class. ```java.lang.Object```

### <span style="color: aqua">Difference between constructor vs. method?</span>
A method is a block of code which only runs when it is called. You can pass data, known as parameters, into a method. Methods are used to perform certain actions and are an ordinary member of a class used to describe a behavior of some object / class. 

A constructor is a special member of the class with the same name as the class with no return type. It is called in order to create / instantiate an object from that class.

### <span style="color: aqua">Give an example of ***checked*** vs. ***unchecked*** exceptions</span>
- ***Checked Exceptions*** - fall under Exceptions; must be thrown or surrounded in a try/catch block otherwise the JVM won't compile the code. Outside resource failing.
    - Exception, IOException, FileNotFoundException, SQLException    
- ***Unchecked Exceptions*** - fall under RuntimeExceptions, which is a subclass of Exception. Unchecked Exceptions can be compiled and will throw an exception at runtime. Unchecked exceptions can be caught or handled with logic.
    - RuntimeException, ArrayIndexOutOfBoundsException, ArithmeticException


### <span style="color: aqua">Final vs. Finally vs. Finalize</span>
* ***FINAL*** is used to denote a variable whose value is constant, meaning that it cannot change in the future. Can also be used in method declaration to assert that the method cannot be overridden by sub-classes. Final classes cannot be inherited, variables value cannot be changed, and methods cannot be overridden.

* The keyword ***FINALLY*** used in the exception handler to clear some post-task after the execution of try or catch block. 

* The ***FINALIZE*** keyword used to clean up some tasks before the object is removed from memory. The finalize method is mainly used in garbage collection.


### <span style="color: aqua">Discuss these access modifiers: Public / Private / Protected / Default</span>
These are access modifiers which control the accessibility / scope of a field, method, constructor, or class.
* ***Public*** – can be accessed anywhere, within the package, outside it, in or outside the class.
* ***Private*** – Access is restricted to only within the class. (i.e. need methods to interact with a private field)
    * Cannot be overridden
* ***Protected*** – access level is protected within the package and outside it through a child class. If you don’t create a child class, you cannot access it from outside the package.
* ***Default*** – set by default, access level only within the package

### <span style="color: aqua">How are Java & Javascript different?</span>
* JAVA:
    * OOP – Programming Language
    * Compiled & runs on JVM
    * Creates full scale applications
    * Supports multi-threading (thread-based concurrency)

* JAVASCRIPT:
    * OOP – Scripting Language
    * Runs on the browser / client side
    * Provides a level of interactivity unable to be produced through normal web development (HTML)
    * No multi-threading (event-based concurrency)


### <span style="color: aqua">Discuss the difference between _class_ & _instance_ variables / methods</span>
- Class variables (or _static_ variables) are bound / belong to the class itself, they're not available to the object. 
This means that regardless of how many instances of that class are created, that single class variable is shared among them.
Static methods belong to the entire class and aren't visible to an individual instance. They can be accessed with instantiating an instance of the class. 
- Instance variables (or member variables) are declared within a class and are essential to holding values to each specific instance created.
Similarly, instance methods represent behavior that each instance / object possesses.
- The static class variables that are shared among a class can be accessed without creating an instance of the class.
- Local variables which are declared in methods, constructors, or blocks exist only within the local scope and are discarded after the method exists or are unavailable outside their scope.

### <span style="color: aqua">Discuss Multithreading</span>
Multithreading is a technique in which a process is divided into threads that can run concurrently. There are two ways to create threads in java: Implement Runnable interface or By extending Thread class

### <span style="color: aqua">What is Synchronization?</span>
Acts as a safety for a thread. A technique to control access of a method with multiple threads at the same time. If we declare a method synchronized, then only one thread can use this method at a time.

### <span style="color: aqua">Discuss Mutable Objects</span>
Mutable objects support both setter & getter methods. They allow for the states and fields of an object to be changed after the object has been created. Conversely, immutable objects cannot be changed after creation.

### <span style="color: aqua">StringBuffer vs. StringBuilder</span>
* StringBuffer is mutable and the object created through it is stored in the heap. It is also thread-safe. It is synchronized and does not let two threads to simultaneously access the same method.
* StringBuilder allows for dynamic modification of a string. It has its own methods. The difference between StringBuilder and StringBuffer is that StringBuilder is non-thread safe (not synchronized) synchronized where StringBuffer is synchronized.

Concatenating a string involves creating a new string with each character that is copied over.

### <span style="color: aqua">Explain Overriding</span>
- Method overriding is used to provide the specific implementation of the method that is already provided by its super class.
  - It replaces the superclass method with a different version.
- In case of method overriding, parameter must be same.
- Method overriding is the example of run time polymorphism.
- Return type must be same or covariant in method overriding.
- Cannot override private, static, or final methods. (Only non-static)… (Hiding for static methods)


### <span style="color: aqua">What is a Stream? What qualifies as one?</span>
A stream is a sequence of objects that supports various methods which can be pipelined to produce the desired result. 
The keyword ***collection*** is a prerequisite to be considered a stream.
- A stream is not a data structure instead it takes input from the Collections, Arrays or I/O channels.


- Streams don’t change the original data structure, they only provide the result as per the pipelined methods.


- Each intermediate operation is lazily executed and returns a stream as a result, hence various intermediate operations 
can be pipelined. Terminal operations mark the end of the stream and return the result.

### <span style="color: aqua">How would you order the filtering & sorting of a stream?</span>
The most appropriate approach is to filter the collection first, then sort it. Filter will reduce the total number of elements to
sort and thus result in fewer calls when sorting.

### <span style="color: aqua">What is the Optional Class?</span>
Optional is a special class used to deal with NullPointerExceptions. It can be used if you suspect a value to be null rather than having to handle numerous null checks. Optional is a container object which may or may not contain a non-null value. You can specify alternate values to return or alternate code to run. This makes the code more readable because the facts which were hidden are now visible.

### <span style="color: aqua"></span>

### <span style="color: aqua"></span>

### <span style="color: aqua"></span>

### <span style="color: aqua"></span>

### <span style="color: aqua"></span>

### <span style="color: aqua"></span>

### <span style="color: aqua"></span>