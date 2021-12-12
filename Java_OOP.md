# JAVA OOP
### <span style="color: aqua">What are the 4 pillars of Object Oriented Programming? Describe them:</span>
    - Abstraction: You don't need to know the inner workings of something to use it.  
    - Polymorphism: A method can have multiple implementations (overriding & overloading).  
    - Inheritance: Allows a class to inherit code from another. Improves code reuse and decreased development time. Java does not support multiple inheritence.  
    - Encapsulation: Related to abstraction, hiding of information which if left free to be manipulated can have harmful / unintended consequences.  

### <span style="color: aqua">What is a class?</span>
A class acts as a blueprint in which objects can be created. A simple example is a pattern to create a dress. The pattern is the class and the dress that is made from it is the object. Classes contain the relevant data and behavior(s) an object has.

### <span style="color: aqua">What is an object?</span>
An instance of a class - contains the basic properties and behavior. Objects are instantiated using the 'new' keyword

### <span style="color: aqua">Discuss some of Java's naming conventions:</span>
- Class names are always the same as the file name, with each class being its own unique & seperate file.
- Class names are capitalized.
- Variables should be logical & concise. 
- CamelCasing  


### <span style="color: aqua">Explain the difference between an object & a class:</span>
.  
Top level classes can only be public or default (not an inner class)  
A file may contain no more than 1 public class. Default classes don't specify an access modifier.  
  
### <span style="color: aqua">Explain the difference between method _overloading_ vs method _overriding_:</span>
(Discuss method signature as well: the # of paramters specific to the constructor / method)
  
### <span style="color: aqua">What is a ***constructor***?</span>
A constructor is a special method that is used to create an object out of a class definition. Constructors are called first when an object of a class is instantiated. It is essentially responsible for setting up that object including assigning specific data members with values passed to it. If a class lacks a constructor, Java assigns one at run time. This empty constructor which maintains no parameters is known as the default constrcutor. Constructors cannot be private, they are _always public_. You can have more than 1 constructor which accepts different parameters (overloading).

### <span style="color: aqua">Where are objects / varibles stored?</span>
- Normals variables are stored in the ***stack***.
- Objects are stored in the ***heap***.
    - The JVM allocates the heap, inside of which resides the ***string pool***

### <span style="color: aqua">What are some of the benefits / features of Java?</span>
*	Object oriented - every is an object / easily extended.
*	Platform independent - Compiled and run on the JVM ("Write once, run anywhere" / Bytecode)
*	Simple - relatively simple to learn if understand OOP
*	Secure - enables virus / tamper-free systems.
*	Architecture-Neutral - file format which compiled code can run on many processors.
*	Portable - due to its arch. neutrality / no implementation independent aspects.
*	Supports Multithreading
*	Robust - emphasizes compile time & runtime error checks
*	Interpreted - byte code translated on the fly to native machine languages.
*   Memory Management (JVM handles garbage collection)
*   Backward Compatible (Older versions supported despite new changes)
*   Maturity & Support (Libaries & extensive documentation)

### <span style="color: aqua">Discuss Exception Handling (Errors vs. Exceptions)</span>
* ***Errors*** occur only at runtime (unknown to the compiler) whereas ***Exceptions*** occur at compile time or runtime.
* Errors involve program termination; exceptions can be recovered from provided they're handled appropriately through try/catch or throws keyword.


### <span style="color: aqua">Discuss Abstract Classes:</span>
Abstract classes provide just a method signature which allows you to implement a framework / template method design pattern. They can contain both abstract and concrete methods but the abstract methods must be implemented elsewhere. Concrete methods are distinguished by having a full name & method body.

### <span style="color: aqua">Discuss Interfaces:</span>
You cannot instantiate abstract classes or interfaces. By default, all methods are abstract. Methods themselves are the only things composing an interface, it merely acts as a contract with the compiler which states that these specific methods must be implemented by whatever class implements the interface. They cannot be static or involve any implementation.

### <span style="color: aqua">Can you achieve multiple inheritance in Java:</span>
No, BUT - you can achieve multiple inheritance through the use of interfaces. (I.e. extending an abstract class, and implementing multiple interfaces).

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
Everything in java inherits from the object class.

### <span style="color: aqua">Difference between constructor vs. method?</span>
A method is an ordinary member of a class used to describe a behavior of some object / class. A constructor is a special member of the class with the same name as the class with no return type.

### <span style="color: aqua">Give an example of ***checked*** vs. ***unchecked*** exceptions</span>
- ***Checked Exceptions*** - fall under Exceptions; must be thrown or surrounded in a try/catch block otherwise the JVM won't compile the code. Outside resource failing.
    - Exception, IOException, FileNotFoundException, SQLException    
- ***Unchecked Exceptions*** - fall under RuntimeExceptions, which is a subclass of Exception. Unchecked Exceptions can be compiled and will throw an exception at runtime. Unchecked exceptions can be caught or handled with logic.
    - RuntimeException, ArrayIndexOutOfBoundsException, ArithmeticException


### <span style="color: aqua">Final vs. Finally vs. Finalize</span>
* With ***FINAL*** We are not able to inherit a final class and cannot override a final method. Used to denote a variable whose value is constant - can also be used in method declaration to assert that the method cannot be overridden by subclasses. The keyword final is used to make a class, variable, or methods final. Final classes cannot be inherited, variables value cannot be changed, and methods cannot be overridden. 
* The keyword ***FINALLY*** used in the exception handler to clear some post-task after the execution of try or catch block. 
* The ***FINALIZE*** keyword used to clean up some tasks before the object is removed from memory. The finalize method mainly used in garbage collection.


### <span style="color: aqua">Discuss these access modifiers: Public / Private / Protected / Default</span>
These are access modifiers which control the accessibility / scope of a field, method, constructor, or class.
* ***Public*** – can be accessed anywhere, within the package, outside it, in or outside of the class.
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


### <span style="color: aqua">Discuss the difference between _class_ & _instance_ variables</span>
- Class variables (denoted with the _static_ keyword) are bound to the class itself. This means that regardless of how many instances of that class are created, that single class variable is shared among them.  
- Instance variables (or member variables) are delcared within a class and are essential to holding values to each specific instance created.
- The static class variables that are shared among a class can be be accessed without creating an instance of the class.
- Local variables which are delcared in methods, constructors, or blocks exist only within the local scope and are discarded after the method exists or are unavailable outside of their scope.

### <span style="color: aqua">Discuss Multithreading</span>
Multithreading is a technique in which a process is divided into threads that can run concurrently. There are two ways to create threads in java: Implement Runnable interface or By extending Thread class

### <span style="color: aqua">What is Synchronization?</span>
Acts as a safety for a thread. A technique to control access of a method with multiple threads at the same time. If we declare a method synchronized, then only one thread can use this method at a time.

### <span style="color: aqua">Discuss Mutable Objects</span>
Mutable objects support both setter & getter methods. They allow for the states and fields of an object to be changed after the object has been created. Conversely, immutable objects cannot be changed after creation.

### <span style="color: aqua">StringBuffer vs. StringBuilder</span>
* StringBuffer is mutable and the object created through it is stored in the heap. It is also thread-safe. It is synchronized and does not let two threads to simultaneously access the same method.
* StringBuilder allows for dynamic modification of a string. It has it's own methods. The difference between StringBuilder and StringBuffer is that StringBuilder is unsynchronized where StringBuffer is synchronized.

### <span style="color: aqua">Explain Overriding</span>
    - Method overriding is used to provide the specific implementation of the method that is already provided by its super class.
        - It replaces the superclass method with a different version.
    - In case of method overriding, parameter must be same.
    - Method overriding is the example of run time polymorphism.
    - Return type must be same or covariant in method overriding.
    - Cannot override private, static, or final methods. (Only non-static)… (Hiding for static methods)


### <span style="color: aqua"></span>

### <span style="color: aqua"></span>

### <span style="color: aqua"></span>