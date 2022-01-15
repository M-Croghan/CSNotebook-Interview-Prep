# JAVA OOP CONCEPTS & QUESTIONS
### :coffee: <span style="color: aqua">What are the 4 pillars of Object Oriented Programming? Describe them:</span>
- ***Abstraction***: You don't need to know the inner workings of something to be able use it. 
  - Abstraction is a process of hiding the implementation details and showing only functionality to the user. 
  - Lets you focus on what the object does instead of how it does it.
  - Greatly improves code reusability & maintainability!
  - Data abstraction can be used to provide security for the data from the unauthorized methods.
  - A non-abstract approach is hard coding every possibility in every use case. Abstraction removes this complexity. If you were creating a coffee machine, an abstract example would be a machine with a single button: _Make Coffee_. You don't need to know all of the additional steps.  


- ***Polymorphism***: A method can have multiple implementations (overriding & overloading).
  - Polymorphism in Java occurs when there are one or more classes or objects related to each other by inheritance capable of doing different things.
  - It is the ability of an object to take many forms. Inheritance lets classes inherit attributes and methods, and 
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
  
Data Encapsulation is an Object-Oriented Programming concept of hiding the data attributes and their behaviors in a single unit. It helps developers to follow modularity while developing software by ensuring that each object is independent of other objects by having its own methods, attributes, and functionalities. It is used for the security of the private properties of an object and hence serves the purpose of data hiding.



### :coffee: <span style="color: aqua">What is a class?</span>
A class acts as a blueprint in which objects can be created. A simple example is a pattern to create a dress. The pattern is the class and the dress that is made from it is the object. Classes contain the relevant data and behavior(s) an object has.

### :coffee: <span style="color: aqua">What is an object?</span>
An instance of a class - contains the basic properties / states and behavior. Objects are instantiated using the 'new' keyword

### :coffee: <span style="color: aqua">Discuss some of Java's naming conventions:</span>
- Class names are always the same as the file name, with each class being its own unique & separate file.
- Class names are capitalized and should be a noun
- Methods should be a verb and start with a lowercase letter
- Variables start with a lowercase letter, should be logical & concise, avoiding single character names.
- Packages should be all lowercase. Separate multiple words with dots: ```java.lang```
- Constants should be all uppercase and multiple words separated by underscores: ```MAX_VALUE```
- CamelCasing  


### :coffee: <span style="color: aqua">Explain the difference between an object & a class:</span>
```Class```: The building block that leads to Object-Oriented Programming. It is a user-defined data type, that holds its own data members and member functions, which can be accessed and used by creating an instance of that class. It is the blueprint of any object. 

```Object```: An object is an instance of a class. All data members and member functions of the class can be accessed through objects. Memory is only allocated when an object is instantiated (i.e. an object is created).

Top level classes can only be public or default (not an inner class)  
A file may contain no more than 1 public class. Default classes don't specify an access modifier.  
  
### :coffee: <span style="color: aqua">Explain the difference between method _overloading_ vs method _overriding_:</span>
- Overloading occurs between the methods in the same class.
  - Method Overloading is a Compile time polymorphism. In method overloading, more than one method shares the same method name with a different signature in the class. In method overloading, the return type can or can not be the same, but we have to change the parameter because, in java, we can not achieve the method overloading by changing only the return type of the method. 
- Overriding occurs between superclass and subclass.
  - Method Overriding is a Run time polymorphism. In method overriding, the derived class provides the specific implementation of the method that is already provided by the base class or parent class. In method overriding, the return type must be the same or co-variant (return type may vary in the same direction as the derived class).
  
### :coffee: <span style="color: aqua">What is a ***constructor***?</span>
A constructor is a special method that is used to create an object out of a class definition. Constructors are called first when an object of a class is instantiated. It is essentially responsible for setting up that object including assigning specific data members with values passed to it. If a class lacks a constructor, Java assigns one at run time. This empty constructor which maintains no parameters is known as the default constructor. Constructors cannot be private, they are _always public_. You can have more than 1 constructor which accepts different parameters (overloading).

### :coffee: <span style="color: aqua">Where are objects / variables stored?</span>
- Normal variables are stored in the ***stack***.
- Objects are stored in the ***heap***.
    - The JVM allocates the heap, inside which resides the ***string pool***

### :coffee: <span style="color: aqua">What are some of the benefits / features of Java?</span>
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

### :coffee: <span style="color: aqua">Discuss Exception Handling (Errors vs. Exceptions)</span>
* ***Errors*** refers to an illegal operation performed by the user which results in the abnormal working of the program.  Programming errors often remain undetected until the program is compiled or executed. Some of the errors inhibit the program from getting compiled or executed. Thus errors should be removed before compiling and executing. It is of three types: Compile-time, Run-time, Logical.  

* ***Exceptions*** refer to an unwanted or unexpected event, which occurs during the execution of a program i.e at run time, that disrupts the normal flow of the program’s instructions. They indicates conditions that a reasonable application might want to catch. Exceptions are the conditions that occur at runtime and may cause the termination of the program. But they are recoverable using try, catch and throw keywords. (Checked & Unchecked Exceptions)


### :coffee: <span style="color: aqua">Discuss Abstract Classes:</span>
Abstract classes aim to implement the same or different behavior among multiple related objects. They provide just a method signature which allows you to implement a framework / template method design pattern. They can contain both abstract and concrete methods but the abstract methods must be implemented elsewhere. Concrete methods are distinguished by having a full name & method body. They cannot be instantiated. Can have final methods which will force the subclass to not change the method body.

***Abstract Class***: a class which is declared with the “abstract” keyword. Cannot be instantiated thus you cannot create an object with it. It’s a collection of subclass methods and can have multiple concrete methods but includes at least 1 abstract method. When you require a base class or when several implementations of the same type share a common behavior.  

### :coffee: <span style="color: aqua">Discuss Interfaces:</span>
Interfaces are totally incomplete, they do not have any properties, only method signatures. They merely act as a contract with the compiler which states that these specific methods must be implemented by whatever class implements the interface. They must show that the inheriting children are capable of doing something. You cannot instantiate abstract classes or interfaces. In Java 8, functional interfaces allowed for static methods.

***Interface***: Is like a blueprint to implement a class. Maintains a collection of abstract methods but contains no concrete methods. But it offers full abstraction (something an abstract class can’t do). A declaration of the methods of a class but not the implementation. The operations an object can perform is defined and are used by the classes which implement that interface. Best used when various implementations share only method signature. When your classes need additional behavior or dependency injection.
### :coffee: <span style="color: aqua">Can you achieve multiple inheritance in Java:</span>
No, You can only extend from a single class. BUT - you can achieve multiple inheritance through the use of interfaces. (I.e. extending an abstract class, and implementing multiple interfaces). 

### :coffee: <span style="color: aqua">Using an abstract class vs. an interface</span>
- Use abstract classes when:  
  - You need both static / non-static methods  
  - You need both abstract & non-abstract methods  
  - You don't want all of your fields to be final

- Use interfaces when:  
  - All methods are abstract  
  - You need future devs to follow a pattern in development  
  - You need to use more than one interface (A class can implement multiple interfaces <- an advantage over an abstract class)

- ```Availability of methods```: Only abstract methods are available in interfaces, whereas non-abstract methods can be present along with abstract methods in abstract classes.
- ```Variable types```: Static and final variables can only be declared in the case of interfaces, whereas abstract classes can also have non-static and non-final variables.
- ```Inheritance:``` Multiple inheritances are facilitated by interfaces, whereas abstract classes do not promote multiple inheritances.
- ```Data member accessibility```: By default, the class data members of interfaces are of the public- type. Conversely, the class members for an abstract class can be protected or private also.
- ```Implementation```: With the help of an abstract class, the implementation of an interface is easily possible. However, the converse is not true;


### :coffee: <span style="color: aqua">Prove: Everything in Java is an object.</span> :question:
It could be argued that everything in java is an object as a great deal inherits from the object class. ```java.lang.Object```. But, Java makes use of primitives: byte, short, int, long, boolean, char, float, and double which themselves are not objects. Not 100%. Java does not satisfy all the OOP conditions (predefined types must be objects) because it uses eight primitive data types(Boolean, byte, char, int, float, double, long, short) which are not objects.

### :coffee: <span style="color: aqua">Difference between constructor vs. method?</span>
A method is a block of code which only runs when it is called. You can pass data, known as parameters, into a method. Methods are used to perform certain actions and are an ordinary member of a class used to describe a behavior of some object / class. 

A constructor is a special member of the class with the same name as the class with no return type. It is called in order to create / instantiate an object from that class.

### :coffee: <span style="color: aqua">Give an example of ***checked*** vs. ***unchecked*** exceptions</span>
- ***Checked Exceptions*** - fall under Exceptions; must be thrown or surrounded in a try/catch block otherwise the JVM won't compile the code. Outside resource failing.
    - Exception, IOException, FileNotFoundException, SQLException    
- ***Unchecked Exceptions*** - fall under RuntimeExceptions, which is a subclass of Exception. Unchecked Exceptions can be compiled and will throw an exception at runtime. Unchecked exceptions can be caught or handled with logic.
    - RuntimeException, ArrayIndexOutOfBoundsException, ArithmeticException


### :coffee: <span style="color: aqua">Final vs. Finally vs. Finalize</span>
* ***FINAL*** is used to denote a variable whose value is constant, meaning that it cannot change in the future. Can also be used in method declaration to assert that the method cannot be overridden by sub-classes. Final classes cannot be inherited, variables value cannot be changed, and methods cannot be overridden.

* The keyword ***FINALLY*** used in the exception handler to clear some post-task after the execution of try or catch block. It defines code that's always run after the try and any catch block, before the method is completed.

* The ***FINALIZE*** finalize is the method in Java which is used to perform clean up processing just before object is garbage collected.


### :coffee: <span style="color: aqua">Discuss these access modifiers: Public / Private / Protected / Default</span>
These are access modifiers which control the accessibility / scope of a field, method, constructor, or class.
* ***Public*** – can be accessed anywhere, within the package, outside it, in or outside the class.
* ***Private*** – Access is restricted to only within the class. (i.e. need methods to interact with a private field (i.e. getters / setters))
    * Cannot be overridden
* ***Protected*** – access level is protected within the package and outside it through a child class. If you don’t create a child class, you cannot access it from outside the package.
* ***Default*** – set by default, access level only within the package

### :coffee: <span style="color: aqua">How are Java & Javascript different?</span>
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


### :coffee: <span style="color: aqua">Discuss the difference between _class_ & _instance_ variables / methods</span>
- Class variables (or _static_ variables) are bound / belong to the class itself, they're not available to the object. 
This means that regardless of how many instances of that class are created, that single class variable is shared among them.
Static methods belong to the entire class and aren't visible to an individual instance. They can be accessed without instantiating an instance of the class. 
- Instance variables (or member variables) are declared within a class and are essential to holding values to each specific instance created.
Similarly, instance methods represent behavior that each instance / object possesses.
- The static class variables that are shared among a class can be accessed without creating an instance of the class.
- Local variables which are declared in methods, constructors, or blocks exist only within the local scope and are discarded after the method exists or are unavailable outside their scope.

### :coffee: <span style="color: aqua">Discuss Multithreading</span>
Multithreading is a technique in which a process is divided into threads and thus multiple activities can proceed concurrently in the same program. Multi-threading extends the idea of multitasking into applications where you can subdivide specific operations within a single application into individual threads. Each of the threads can run in parallel. The OS divides processing time not only among different applications, but also among each thread within an application. If your class is intended to be executed as a thread then you can achieve this by implementing a Runnable interface.

### :coffee: <span style="color: aqua">What is Synchronization?</span>
Synchronization in Java is the capability to control the access of multiple threads to any shared resource at the same time. Acts as a safety for a thread. If we declare a method synchronized, then only one thread can use this method at a time. Synchronization is built around an internal entity known as the lock or monitor. Every object has a lock associated with it. By convention, a thread that needs consistent access to an object's fields has to acquire the object's lock before accessing them, and then release the lock when it's done with them.

### :coffee: <span style="color: aqua">Discuss Mutable Objects</span>
- ```Mutable``` objects support both setter & getter methods. They allow for the states and fields of an object to be changed after the object has been created. (StringBuilder, StringBuffer, Date).
- ```Immutable``` objects cannot be changed after creation. (Primitives, String, Wrapper classes).

### :coffee: <span style="color: aqua">StringBuffer vs. StringBuilder</span>
* StringBuffer is mutable and  is also thread-safe / synchronized: does not let two threads to simultaneously access the same method.
* StringBuilder is mutable and allows for dynamic modification of a string. It has its own methods. The difference between StringBuilder and StringBuffer is that StringBuilder is more efficient but non-thread safe (not synchronized) synchronized where StringBuffer is synchronized.

Concatenating a string involves creating a new string with each character that is copied over. Thus StringBuilder is a more optimal solution.

### :coffee: <span style="color: aqua">Explain Overriding</span>
- Method overriding is used to provide the specific implementation of the method that is already provided by its super class.
  - It replaces the superclass method with a different version.
- In case of method overriding, parameter must be same.
- Method overriding is the example of run time polymorphism.
- Return type must be same or covariant in method overriding.
- Cannot override private, static, or final methods. (Only non-static)… (Hiding for static methods)

### :coffee: <span style="color: aqua">What is a Stream? What qualifies as one?</span>
A stream is a sequence of objects that supports various methods which can be pipelined to produce the desired result. 
The keyword ***collection*** is a prerequisite to be considered a stream.
- A stream is not a data structure instead it takes input from the Collections, Arrays or I/O channels.

- Streams don’t change the original data structure, they only provide the result as per the pipelined methods.

- Each intermediate operation is lazily executed and returns a stream as a result, hence various intermediate operations can be pipelined. Terminal operations mark the end of the stream and return the result.

### :coffee: <span style="color: aqua">How would you order the filtering & sorting of a stream?</span>
The most appropriate approach is to filter the collection first, then sort it. Filter will reduce the total number of elements to sort and thus result in fewer calls when sorting.

### :coffee: <span style="color: aqua">What is the Optional Class?</span>
Optional is a special class used to deal with NullPointerExceptions. It can be used if you suspect a value to be null rather than having to handle numerous null checks. Optional is a container object which may or may not contain a non-null value. You can specify alternate values to return or alternate code to run. This makes the code more readable because the facts which were hidden are now visible.

### :coffee: <span style="color: aqua">What is the JIT Compiler?</span>
JIT stands for Just-In-Time and it is used for improving the performance during run time. It does the task of compiling parts of byte code having similar functionality at the same time thereby reducing the amount of compilation time for the code to run.
The compiler is nothing but a translator of source code to machine-executable code. But what is special about the JIT compiler? Let us see how it works:
First, the Java source code (.java) conversion to byte code (.class) occurs with the help of the Java compiler.
Then, the .class files are loaded at run time by JVM and with the help of an interpreter, these are converted to machine understandable code.
JIT compiler is a part of JVM. When the JIT compiler is enabled, the JVM analyzes the method calls in the .class files and compiles them to get more efficient and native code. It also ensures that the prioritized method calls are optimized.
Once the above step is done, the JVM executes the optimized code directly instead of interpreting the code again. This increases the performance and speed of the execution.


### :coffee: <span style="color: aqua">What is the difference in checking equality with .equals() vs. '=='?</span>
* == operator compares reference or memory location of objects in the heap, whether they point to the same location or not.

* equals() method should be used for content comparison. equals() main purpose is to compare the state of two objects or the contents of the objects.

### :coffee: <span style="color: aqua">Can Static Methods be Overridden or Overloaded?</span>
Yes! There can be two or more static methods in a class with the same name but differing input parameters
No! Declaration of static methods having the same signature can be done in the subclass but run time polymorphism can not take place in such cases.
Overriding or dynamic polymorphism occurs during the runtime, but the static methods are loaded and looked up at the compile time statically. Hence, these methods cant be overridden

### :coffee: <span style="color: aqua">What is the point of garbage collection & what area of memory does it address?</span>
The main objective of this process is to free up the memory space occupied by the unnecessary and unreachable objects during the Java program execution by deleting those unreachable objects. This ensures that the memory resource is used efficiently, but it provides no guarantee that there would be sufficient memory for the program execution. Focuses on the heap and is facilitated by the JVM.


### :coffee: <span style="color: aqua">Does Java Operate: "Pass by Reference" or "Pass by Value"?</span>
Java uses only call by value. It creates a copy of a reference and passes them as value to a method. If reference contains objects, then the value of an object can be modified in the method but not the entire object. When an object is passed by value, this means that a copy of the object is passed. Thus, even if changes are made to that object, it does not affect the original value. When an object is passed by reference, this means that the actual object is not passed, rather a reference of the object is passed. Thus, any changes made by the external method, are also reflected in all places.

### :coffee: <span style="color: aqua">What happens if there is no static modifier in the main method signature in Java?</span>
There wouldn't be any compilation error. But then the program is run, since the JVM cant map the main method signature, the code throws “NoSuchMethodError” error at the runtime.

### :coffee: <span style="color: aqua">What happens if there are multiple main methods inside one class in Java?</span>
The program can't compile as the compiler says that the method has been already defined inside the class.

### :coffee: <span style="color: aqua">How does an exception propagate in the code?</span>
When an exception occurs, first it searches to locate the matching catch block. If the matching catch block is located, then that block would be executed. Else, the exception propagates through the method call stack and goes into the caller method where the process of matching the catch block is performed. This propagation happens until the matching catch block is found. If the match is not found, then the program gets terminated in the main method.

### :coffee: <span style="color: aqua">Is it mandatory for a catch block to be followed after a try block?</span>
No, it is not necessary for a catch block to be present after a try block. But to compile, it must be followed either by a catch block or by a finally block. If the exceptions likelihood is high, then they should be declared using the throws clause of the method. 
### :coffee: <span style="color: aqua">Can you call a constructor of a class inside the another constructor?</span>
Yes, the concept can be termed as constructor chaining and can be achieved using this()
### :coffee: <span style="color: aqua">Difference between ArrayList and LinkedList in Java?</span>
In short, ArrayList is backed by an array in Java, while LinkedList is just a collection of nodes, similar to a linked list data structure. ArrayList also provides a random search if you know the index, while LinkedList only allows a sequential search. On the other hand, adding and removing an element from the middle is efficient in LinkedList as compared to ArrayList because it only requires modifying links, and no other element is rearranged.
### :coffee: <span style="color: aqua">Difference between HashMap and Hashtable in Java?</span>
...
### :coffee: <span style="color: aqua">Difference between TreeSet and TreeMap in Java?</span>
...
### :coffee: <span style="color: aqua">Can we have a return statement in the finally clause? What will happen?</span>
Yes, you can use the return statement in finally block, but it will not prevent finally block from being executed. BTW, if you also used the return statement in the try block then return the value from the finally block with override whatever is returned from the try block.
### :coffee: <span style="color: aqua">What is: Composition, Association, Aggregation?</span>

### :coffee: <span style="color: aqua">What is the JVM?</span>
A Java virtual machine (JVM) is a process virtual machine that can execute Java bytecode. Each Java source file is compiled into a bytecode file, which is executed by the JVM.
### :coffee: <span style="color: aqua">Why is Java called the Platform Independent Programming Language?</span>
Java was designed to allow application programs to be built that could be run on any platform, without having to be rewritten or recompiled by the programmer for each separate platform. A Java virtual machine makes this possible because it is aware of the specific instruction lengths and other particularities of the underlying hardware platform.
### :coffee: <span style="color: aqua">What is the Difference between JDK and JRE?</span>
The Java Runtime Environment (JRE) is basically the Java Virtual Machine (JVM) where your Java programs are being executed. It also includes browser plugins for applet execution. The Java Development Kit (JDK) is the full-featured Software Development Kit for Java, including the JRE, the compilers and tools (like JavaDoc, and Java Debugger), in order for a user to develop, compile and execute Java applications.
JDK	JRE
JDK stands for the term : Java Development Kit.	JRE stands for the term: Java Runtime Environment.
JDK is the tool for compiling, documenting and packaging Java software.	JRE is a runtime environment. JavaByte code gets executed in the environment.
JDK has JRE and development tools.	JRE is a JVM implementation
### :coffee: <span style="color: aqua">What are wrapper classes?</span>
A wrapper class converts java primitives into objects. So a primitive wrapper class is a wrapper class that encapsulates, hides or wraps data types from the eight primitive data types so that these can be used to create instantiated objects with methods in another class or in other classes. The primitive wrapper classes are found in the Java API.
