# COMPUTER SCIENCE CONCEPTS & QUESTIONS
### :computer: <span style="color: aqua">Discuss the difference between _compiled_ & _interpreted_ languages:</span>
* Compiled Languages (C, C++, Go) - Converts source code to machine code instructions.
* Interpreted Languages (JS, Ruby, Python) - Code isn't compiled into machine code, but rather it is read & executes within an interpreter shell.
* Byte-Code Languages (C#, Scala, Java) - Compiled into bytecode and executes in a virtual machine. Byte-Code is a form of instruction set designed for efficient execution by a software interpreter.
    * Java & the JVM is a popular example. Involves JIT compiler (_just in time_) which inspects code as it executes.

### :computer: <span style="color: aqua">Explain "IS-A" & "HAS-A" relationships:</span>
 ```IS-A``` Relationships involve ***inheritance***. Classes which inherit are known as sub-classes or child classes.  
 ``` class Apple extends Fruit { ```  
In this case, An apple ***is a*** fruit.  

```HAS-A``` Relationships is composition, meaning that instances have references to other objects. For example, a room has a table. So you will create a class room and then in that class create an instance of type table.  

```class Room {```  
    ```Table table = new Table();```  
    ```}```  

A HAS-A relationship is dynamic (run time) binding while inheritance is a static (compile time) binding. 


### :computer: <span style="color: aqua">List the 4 main pillars of OOP</span>
- Abstraction
- Polymorphism
- Encapsulation
- Inheritance

### :computer: <span style="color: aqua">What is polymorphism?</span>
The ability for an object to also be present in many forms. Sub classes could inherit attributes and methods from a superclass (i.e. Animal). Polymorphism uses the methods to perform different tasks. For instance, a cat class and a dog class both inherit the animal sound from the Animal superclass. However, the cat 'meows' whereas the dog 'barks'. Polymorphism is the ability of programming languages to present a single interface to entities of different types.A polymorphic type is a type whose operations can also be applied to values of some other type. Some types include:  
- Runtime (Sub-type) - Most common (The above animal example).
- Parametric (Overloading) - Provide 1 function to interact with multiple types.
- Compile-Time (Ad-Hoc) - Functions with the same name act differently for different types (Addition in Python).
- Casting (Coercion) - The direct transformation of one type into another.

### :computer: <span style="color: aqua">What is abstraction?</span>
Abstraction is a process of hiding the implementation details and showing only functionality to the user. It lets you focus on what the object does instead of how it does it. By separating ideas from specific instances you can develop classes in terms of their own functionality, instead of their implementation details. Java supports the creation and existence of abstract classes that expose interfaces, without including the actual implementation of all methods. The abstraction technique aims to separate the implementation details of a class from its behavior.

### :computer: <span style="color: aqua">What is inheritance?</span>
Inheritance is a mechanism in which an object acquires all the properties and behavior of another object or another class. It provides reusability of code and can be used to add additional features to an existing class, without modifying it. This is important in the context of the DRY principle (don’t repeat yourself). The superclass or base class allows child or sub-classes to acquire it's fields and methods. A superclass however, cannot inherit from one of it's subclasses. Inheritance is gained by implementing interfaces or extending classes, but in Java: a class cannot inherit more than one class.

### :computer: <span style="color: aqua">What is encapsulation?</span>
Encapsulation provides objects with the ability to hide their internal characteristics and behavior. It is the bundling of data / methods that interact with or operate on that data into a single unit in the form of a class. A good rule of thumb is to encapsulate as much as possible. The last thing you want is data being changed or manipulated in a way not intended. Private fields or methods are an example of protecting the inner workings of a class. Some of the advantages of using encapsulation are:
- The internal state of every object is protected by hiding its attributes.
- It increases usability and maintenance of code, because the behavior of an object can be independently changed or extended.
- It improves modularity by preventing objects to interact with each other, in an undesired way.

### :computer: <span style="color: aqua">What is Garbage Collection?</span>
Garbage collection involves freeing up of memory if there no longer exists a reference to a specific object. In Java, the JVM handles garbage collection automatically whenever this condition exists so you need not to remove the unwanted objects explicitly, unlike C/C++ which require you to de-allocate memory yourself.

### :computer: <span style="color: aqua">Explain the Software Developmnt Lifecycle (SDLC)</span>
***Requirements Gathering > Planning > Design > Development > Testing > Deployment > Maintenance***  
* _Requirements gathering_ / pre-planning phase: What problems need to be solved?
    * The goal is to create a comprehensive list of software requirements / specifications that reflect all the functional & non-functional requirements for the end product.
* _Planning:_ What do we want to do?
* _Architectural / Software Design:_ How do we reach our goal?
    * Involves creating a design document that specifies the architecture based on the data collected. You’re still getting stakeholder input while defining roles and responsibilities.
* _Software Development / Implementation:_ Start Building!
    * Main core of the software development process. Involves the actual process of working through the compiled list of necessary work and developing a functional system. It’s the main entry point to production, writing code, testing, and optimizing.
* _Testing:_ Let's ensure what was built works!
    * Generally, a continuous process. Unit testing is an ongoing process throughout development and integration testing is verifying all software components at the final stage of the production.
* _Deployment & Delivery:_ Lets take our solution & use it!
* _Maintenance:_ Continual support.  

### :computer: <span style="color: aqua">What is a singleton design pattern?</span>
- A a creational design pattern which involves a single class that can only create a single object & provides a global point of access to it. (Can be problematic in multithreading (solution via synchronization block))
    1. Allows for lazy loading (initialize object creation only when you need it / are going to be using it).
    2. When you need exactly one instance to coordinate actions across a system. (i.e. a database connection)
        - Say if you create an object that is going to be interacting with hardware & two could cause conflict.
- ```public SingleObject {```
    - Private static instance of the object instantiated in the class:
    - ```private static SingleObject instance = new SingleObject();```
    - Private constructor:
    - ```private SingleObject(){}```
    - Public static method responsible for getting the object / instance:
    - ```public static SingleObject getObject(){return instance}```
        

### :computer: <span style="color: aqua">What is a factory design pattern?</span>
A creational design pattern and one of the most used patterns in Java, it defines an interface or abstract class for creating an object but lets the subclasses decide which class to instantiate. An object is created without exposing the creation logic to the client and refer to newly created object using a common interface.  
Helps keep code clean and concise as all object creation takes place in a centralized location.
Useful:  
- When you want a method to return one of several possible classes that share a common super class
- When you don't know ahead of time what class object you need
- Encapsulate object creation
- Promotes loose-coupling by eliminating the need to bind application specific classes into the code.  

Example:  
A factory method in the interface defers the object creation to one or more concrete subclasses at run time. The subclasses implement the factory method to select the class whose objects need to be created. Say you create an adventure game where a player can battle an array of enemies. A general Enemy interface allows for the creation of several subclasses and a factory design pattern can be used to randomly decide which type of enemy a player will encounter.	
	

### :computer: <span style="color: aqua">What are some of the different software development methodologies?</span>
Two main areas:
- Waterfall – this approach needs to be well-disciplined as there isn’t planned opportunity to back track. It starts with 
clear and complete requirements and moves through the development process sequentially/linearly in distinct phases. Some 
drawbacks include its relatively rigid and inflexible, there isn’t an avenue for feedback early in the process 
and can be financially devastating if requirements are missing or planning is mismanaged. Its best when projects are 
relatively simple, little change is expected and a project manager is closely involved.
- Agile – Focused on customer / stakeholder feedback & collaboration. There is an emphasis on rapid development to support 
fast delivery and is incredibly adaptable and open to change. The downsides however are that the lack of emphasis makes 
it difficult to truly develop a great design, its easy to get off track if the goals are unclear or the collaborative 
relationship steers the project in a different direction which may result in an unpredictable finished product.
    - Variations: Rapid Application Development, Extreme Programming, DevOps... etc.  

### :computer: <span style="color: aqua">Explain MVC</span>
MVC is a software design pattern focusing on 3 main components:
- The Model comprises all of the data of the application. All info to be displayed and its requirements with respect to access and other validations are all specified here.
- View is the component that operates as a display to the user. Specifically it represents the visualization of the data that the model contains.
- Control influences the activity between the model and the view. Acts on both the model & the view. Controls the data flow into model object & updates the view whenever the data changes (Keeps the model & view separate).

### :computer: <span style="color: aqua">What is a UML diagram?</span>
UML is a general-purpose modeling language and is used to represent the components related to important OOP concepts. In essence, it’s a general way of defining the whole software architecture or structure. I.e. using UML to flesh out details of classes and their properties, methods, and relationships (inheritance).

### :computer: <span style="color: aqua">What are design patterns?</span>
Represent best practices / solutions to general problems  frequently faced by software developers.

### :computer: <span style="color: aqua">What is an API?</span>
Basically, an API is a service that provides raw data for public use. As third-party software developers, we can access an organization's API and use their data within our own applications.
An application-programming interface (API) is a set of programming instructions and standards for accessing a web-based software application or web tool. It is a software-to-software interface, not a user interface. With APIs, applications talk to each other without any user knowledge or intervention. In practice, a software company releases its API to the public so other developers 
can design products that are powered by its service. Notable examples being: Google Maps, integrating social media sharing, and a secure payment system through PayPal.

### :computer: <span style="color: aqua">What is Unit Testing?</span>
Unit testing is typically done by developers themselves. It focuses on the smallest unit of software design and tests a
piece of code (a unit) for correct behavior. It asks: "Does this class / method operate as intended?". A unit test can be targeted 
at an individual unit or group of interrelated units. It is often done using sample input and observing its corresponding outputs.

### :computer: <span style="color: aqua">What happens when you type a URL into a browser and hit enter?</span>
- The browser checks the cache for a DNS record to find the corresponding IP address of the URL.
- If the requested URL is not in the cache, ISP’s DNS server initiates a DNS query to find the IP address of the server that hosts the URL.
- The browser initiates a TCP connection with the server.
- The browser sends an HTTP request to the webserver.
- The server handles the request and sends back a response.
- The server sends out an HTTP response.
- The browser displays the HTML content (for HTML responses, which is the most common).

### :computer: <span style="color: aqua">What are the differences between Abstraction and Encapsulation?</span>
Abstraction and encapsulation are complementary concepts. On the one hand, abstraction focuses on the behavior of an object. On the other hand, encapsulation focuses on the implementation of an object’s behavior. Encapsulation is usually achieved by hiding information about the internal state of an object and thus, can be seen as a strategy used in order to provide abstraction.
### :computer: <span style="color: aqua">What are the types of Polymorphism?</span>
Compile-time polymorphism (Static binding) – Method overloading
Runtime polymorphism (Dynamic binding) – Method overriding
### :computer: <span style="color: aqua">What is: Composition, Association, Aggregation?</span>
Composition is a way to design or implement a "has-a" relationship. We use an instance variable that refers to another object.
- Association represents the ability of one instance to send a message to another instance. (1-1, 1-Many, Many-1, Many-Many).
    - This is typically implemented with a pointer or reference instance variable, although it might also be implemented as a method argument or the creation of a local variable.
Aggregation represents HAS-A relationship. It is the typical whole/part relationship. This is exactly the same as an association with the exception that instances cannot have cyclic aggregation relationships.
### :computer: <span style="color: aqua">What is the computer system?
</span>
A computer system is a combination of memory, CPU, peripheral devices that are connected to it, and OS (Operating System).

### :computer: <span style="color: aqua">List out components of a computer system</span>
The components of a computer system are:
- CPU (Central Processing Unit) including control unit and arithmetic logic unit
- Memory like primary and secondary
- Input and output devices like keyboard mouse, printer scanner, etc.

### :computer: <span style="color: aqua">What is a microprocessor?</span>
A microprocessor is an integrated circuit having all the functionality of a central processing unit of a PC.

### :computer: <span style="color: aqua">Explain the meaning of file.</span>
A file is a named location that stores information or data permanently. It is always stored in the storage device using a file name with primary and secondary name, which is separated by a “.”(DOT).
### :computer: <span style="color: aqua">What is Integrated Development Environment?</span>
An IDE is a GUI-based software program. It is designed to help programmers build applications with all the needed programs and libraries.
### :computer: <span style="color: aqua">List the types of constructors</span>
There are two types of the constructor:  
1. Parameterized constructor - Has no parameters. If you don't create one the class will automatically call default constructor when an object is created.
2. Default constructor - Has at least one parameter is called a parametrized constructor.
3. Copy Constructor - Creates an object by copying variables from another object.
4. Static Constructor - Used to initialize any static data, or to perform a particular action that needs to be performed once only. It is called automatically before the first instance is created or any static members are referenced.
5. Private constructor - generally used in classes that contain static members only. If a class has one or more private constructors and no public constructors, other classes (except nested classes) cannot create instances of this class. The use of private constructor is to serve singleton classes.
### :computer: <span style="color: aqua">What is artificial intelligence?</span>
Artificial Intelligence or machine intelligence is a common term that is used to build smart machines capable of performing tasks. The main aim of AI is to solve problems in a way that are better and faster. Simply put: AI refers to systems / machines that mimic human intelligence to perform tasks and can iteratively improve themselves based on the information they collect.
### :computer: <span style="color: aqua">What is machine learning?</span>
Machine Learning is a subset of AI: It is focused on teaching computers to learn from data and to improve with experience – instead of being explicitly programmed to do so.
### :computer: <span style="color: aqua">What is deep learning?</span>
Deep learning is a machine learning technique that teaches computers to do what comes naturally to humans: learn by example. Deep learning is computer software that mimics the network of neurons in a brain. It is a subset of machine learning and is called deep learning because it makes use of deep neural networks. Models are trained by using a large set of labeled data and neural network architectures that contain many layers.
### :computer: <span style="color: aqua">List out Layers of OSI Model</span>
Layers of OSI models are:  
1. Physical
2. Application
3. Presentation
4. Session
5. Transport
6. Network
7. Data Link Layer
### :computer: <span style="color: aqua">What is s the primary difference between process and thread?</span>
Process is called as a program which is in execution. Thread is a segment of a process, so; a process can have more than one thread.
### :computer: <span style="color: aqua">Explain primary memory</span>
Primary memory, RAM is the main memory of a computer which can be directly accessed by the Central Processing Unit (CPU). It stores temporary information until the process finishes its execution. It is said to be volatile as it persists only as long as the computer is powered on.
### :computer: <span style="color: aqua">What is the operating system?</span>
An Operating system (OS) is is a fully integrated set of specialized instructions (software) that handle all the operations of the computer and acts as an interface between the end-user and computer hardware. A computer doesn't need to have an OS to run other programs but if this is the case an application must handle / perform its functions, including managing resources (processes, memory, etc.). 
### :computer: <span style="color: aqua">What is an Algorithm?</span>
An algorithm is a rule or step-by-step process that must be followed in order to solve a particular problem.
### :computer: <span style="color: aqua">What is cryptography?</span>
Cryptography is the study of techniques that hide the real meaning of information. It transforms this information into a format that cannot be read by humans and vice versa. It involves secure communications techniques that allow only the sender and intended recipient of a message to view its contents.
### :computer: <span style="color: aqua">What is a Virtual Machine?</span>
A virtual machine, commonly shortened to just VM, is no different than any other physical computer like a laptop, smart phone, or server. It has a CPU, memory, disks to store your files, and can connect to the internet if needed. While the parts that make up your computer (called hardware) are physical and tangible, VMs are often thought of as virtual computers or software-defined computers within physical servers, existing only as code. Virtualization is the process of creating a software-based, or "virtual" version of a computer, with dedicated amounts of CPU, memory, and storage that are "borrowed" from a physical host computer—such as your personal computer— and/or a remote server—such as a server in a cloud provider's datacenter. A virtual machine is a computer file, typically called an image, that behaves like an actual computer. It can run in a window as a separate computing environment, often to run a different operating system—or even to function as the user's entire computer experience—as is common on many people's work computers. The virtual machine is partitioned from the rest of the system, meaning that the software inside a VM can't interfere with the host computer's primary operating system.
### :computer: <span style="color: aqua">What is a Framework?</span>
Frameworks make building applications faster and more efficient. It provides the basis on which developers can build programs for a specific platform. For example, a framework may include predetermined classes as well as functions. It can be used to process inputs, manage hardware, and interact with system software. (ex. Spring is one of the more popular frameworks for Java.)

Pros:  
- Enables devs to build applications faster and more efficiently.
- Reduces the code length...allowing you to add conventional functionality without long lines of code.
- More practical for junior devs... (gives them "guardrails" as they build new applications).
- Most "popular" frameworks are free.
- Allow you to write and integrate unit tests and integrations tests with ease.
- Help establish an "appropriate" use of design patterns.
- Typically, large popular frameworks are well-maintained (including documentation).

Cons:  
- They can have a lot of extra code... which can lead to longer load times and decreased performance.
- Stops many devs from taking the time to learn CSS. (Specifically for UI Frameworks).
- Over-complicates simple projects - using a lot more data, space, unnecessary files, etc... for something that could simply be done with a few files.
- Frameworks are inflexible... cannot modify core tenants of their structure.
- Once a framework is chosen... switching to another is difficult.
- Updates can introduce bugs into your implementation of the framework.


### :computer: <span style="color: aqua">What is a Library?</span>
A code library is used to solve a specific problem or add a specific feature to your program.

Pros:
- The programmer is in charge of the flow of the program.
- Designed to perform often-time highly specific tasks.
- Tend ot have less structure than a Framework...which can speed up development time when you know what you're doing.
- You can easily replace one library for another.
- Libraries require significantly less code than a framework to implement... typically.
- Flexibility of being able to pick and choose what libraries you do and don't want to use... unlike frameworks.

Cons:  
- Updates can introduce bugs into your implementation of the library.
- You have to re-compile your program each time you wish to run.
- The need to utilize the entire library codebase to use one piece.
- Tend ot have less structure than a Framework... which can create unnecessary headaches.
- You can often end up using multiple libraries to achieve your end goal.
- Often the documentation for a specific library can be sparse.
