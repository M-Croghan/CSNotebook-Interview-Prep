# COMPUTER SCIENCE CONCEPTS & QUESTIONS
### <span style="color: aqua">Discuss the difference between _compiled_ & _interpreted_ languages:</span>
* Compiled Languages (C, C++, Go) - Converts source code to machine code instructions.
* Interpreted Languages (JS, Ruby, Python) - Code executes within an interpreter shell.
* Byte-Code Languages (C#, Scala, Java) - Compiled into bytecode and executed in the JVM. Involves JIT compiler (_just in time_) which inspects code as it executes.

### <span style="color: aqua">Explain "IS-A" & "HAS-A" relationships:</span>
 ```IS-A``` Relationships is ***inheritance***. Classes which inherit are known as sub-classes or child classes.  
 ``` class Apple extends Fruit { ```  
In this case, An apple ***is a*** fruit.  

```HAS-A``` Relationships is composition, meaning that instances have references to other objects. For example, a room has a table. So you will create a class room and then in that class create an instance of type table.  

```class Room {```  
    ```Table table = new Table();```  
    ```}```  

A HAS-A relationship is dynamic (run time) binding while inheritance is a static (compile time) binding. 


### <span style="color: aqua">List the 4 main pillars of OOP</span>
- Abstraction
- Polymorphism
- Encapsulation
- Inheritance

### <span style="color: aqua">What is polymorphism?</span>
The ability for an object to also be present in many forms. Sub classes could inherit attributes and methods from a superclass (i.e. Animal). Polymorphism uses the methods to perform different tasks. For instance, a cat class and a dog class both inherit the animal sound from the Animal superclass. However, the cat 'meows' whereas the dog 'barks'.

### <span style="color: aqua">What is abstraction?</span>
Abstraction is a process of hiding the implementation details and showing only functionality to the user. Abstraction lets you focus on what the object does instead of how it does it.

### <span style="color: aqua">What is inheritance?</span>
Important in the context of DRY (don’t repeat yourself). Inheritance is a mechanism in which one object acquires all the properties and behavior of another object of another class. Gained by implementing interfaces or extending classes. A class cannot inherit more than one class. A class cannot call private methods except indirectly and a superclass can not inherit from a subclass.

### <span style="color: aqua">What is encapsulation?</span>
The bundling of data and the methods that interact with or operate on that data into a single unit in the form of a class. Think of it as like a black box, it doesn’t matter how the internals work, just how you can interact with it. Private fields or methods are an example of protecting the inner workings of a class. 

### <span style="color: aqua">What is Garbage Collection?</span>
Removing unwanted objects to free up memory if they are no longer referenced. Garbage collection is done automatically in Java whenever there is no longer a reference pointed at a specific object. You need not to remove the unwanted objects explicitly. Garbage collector thread does this for you. C/C++ require you to deallocate memory yourself.

### <span style="color: aqua">Explain the Software Developmnt Lifecycle (SDLC)</span>
***Requirements Gathering > Planning > Design > Development > Testing > Deployment > Maintenance***  
* Requirements gathering / pre-planning phase: goal to create a comprehensive list of software requirements specification that reflect all the functional & nonfunction requirements for the end product.
* Architecture Design: involves creating a design document that specifies the architecture based on the data collected. You’re still getting stakeholder input while defining roles and responsibilities.
* Implementation: Main core of the software development process. Involves the actual process of working through the compiled list of necessary work and developing a functional system. It’s the main entry point to production, writing code, testing, and optimizing.
* Testing: generally, a continuous process. Unit testing is an ongoing process throughout development and integration testing is verifying all software components at the final stage of the production.
* Deployment & Delivery
* Maintenance 


### <span style="color: aqua">What is a singleton design pattern?</span>
- A design pattern which ensures a class only has only 1 instance & provides a global point of access to it.
    1. Allows for lazy loading (initialize object creation only when you need it / are going to be using it).
    2. When you need exactly one instance to coordinate actions across a system. (i.e. a database connection)
        - Say if you create an object that is going to be interacting with hardware & two could cause conflict.
- 3 main components
    - Single class
        - Private constructor
        - Private static instance
        - Factory static method responsible for instance creation
        - Can be problematic in multithreading (solution via synchronization block)

### <span style="color: aqua">What is a factory design pattern?</span>
A creational design pattern and one of the most used patterns in Java, it defines an interface or abstract class for creating an object but lets the subclasses decide which class to instantiate. An object is created without exposing the creation logic to the client and refer to newly created object using a common interface.  
Helps keep code clean and concise as all object creation takes place in a centralized location.
Useful:  
- When you want a method to return one of several possible classes that share a common super class
- When you don't know ahead of time what class object you need
- Encapsulate object creation
- Promotes loose-coupling by eliminating the need to bind application specific classes into the code.  

Example:  
A factory method in the interface defers the object creation to one or more concrete subclasses at run time. The subclasses implement the factory method to select the class whose objects need to be created.  

You create an adventure game where a player can battle an array of enemies. A general Enemy interface allows for the creation of several subclasses and a factory design pattern can be used to randomly decide which type of enemy a player will encounter.	
	

### <span style="color: aqua">What are some of the different software development methodologies?</span>
- Waterfall, Agile, Rapid Application Development (RAD), Extreme Programming (XP)
- Waterfall – this approach needs to be well-disciplined as there isn’t planned opportunity to back track. It starts with 
clear and complete requirements and moves through the development process sequentially/linearly in distinct phases. Some 
drawbacks include its relatively rigid and inflexible, there isn’t an avenue for feedback early in the process 
and can be financially devastating if requirements are missing or planning is mismanaged. Its best when projects are 
relatively simple, little change is expected and a project manager is closely involved.
- Agile – Focused on customer / stakeholder feedback & collaboration. There is an emphasis on rapid development to support 
fast delivery and is incredibly adaptable and open to change. The downsides however are that the lack of emphasis makes 
it difficult to truly develop a great design, its easy to get off track if the goals are unclear or the collaborative 
relationship steers the project in a different direction which may result in an unpredictable finished product.


### <span style="color: aqua">Explain MVC</span>
Software design pattern focused on Model, View, Controller components.
- Model aspect comprises the data of the application, Represents an object carrying data. It can also contain logic to update controller if data changes.
- View is the component that operates as a display to the user. Represents the visualization of the data that the model contains.
- Control influences the activity between the model and the view. Acts on both of model & the view. Controls the data flow into model object & updates the view whenever the data changes (Keeps the model & view separate).

### <span style="color: aqua">What is a UML diagram?</span>
UML is a general-purpose modeling language and is used to represent the components related to important OOP concepts. in essence, it’s a general way of defining the whole software architecture or structure.

### <span style="color: aqua">What are design patterns?</span>
Represent best practices / solutions to general problems  frequently faced by software developers.

### <span style="color: aqua">What is an API?</span>
An application-programming interface (API) is a set of programming instructions and standards for accessing a web-based
software application or web tool. A software company releases its API to the public so that other software developers 
can design products that are powered by its service... [it] is a software-to-software interface, not a user interface. 
With APIs, applications talk to each other without any user knowledge or intervention. Notable examples being: Google Maps, 
integrating social media sharing, and a secure payment system through PayPal.

### <span style="color: aqua">What is Unit Testing?</span>
Unit testing is typically done by developers themselves. It focuses on the smallest unit of software design and tests a
piece of code (a unit) for correct behavior. "Does this class / method operate as intended?" A unit test can be targeted 
at an individual unit or group of interrelated units. It is often done using sample input and observing its corresponding outputs.

### <span style="color: aqua">What happens when you type a URL into a browser and hit enter?</span>
- The browser check the cache for a DNS record to find the corresponding IP address of the URL.
- If the requested URL is not in the cache, ISP’s DNS server initiates a DNS query to find the IP address of the server that hosts the URL.
- The browser initiates a TCP connection with the server.
- The browser sends an HTTP request to the webserver.
- The server handles the request and sends back a response.
- The server sends out an HTTP response.
- The browser displays the HTML content (for HTML responses, which is the most common).

### <span style="color: aqua"></span>

### <span style="color: aqua"></span>

### <span style="color: aqua"></span>

### <span style="color: aqua"></span>