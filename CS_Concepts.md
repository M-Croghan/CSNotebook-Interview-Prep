# COMPUTER SCIENCE CONCEPTS
### <span style="color: aqua">Disucss the difference between _compiled_ & _interpreted_ languages:</span>
* Compiled Languages (C, C++, Go) - Converts source code to machine code instructions.
* Interpreted Languages (JS, Ruby, Python) - Code executes within an interpreter shell.
* Byte-Code Languages (C#, Scala, Java) - Compiled into bytecode and executed in the JVM. Involves JIT compiler (_just in time_) which inspects code as it executes.

### <span style="color: aqua">Explain "IS-A" & "HAS-A" relationships:</span>
.

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


### <span style="color: aqua">What is a singleton design pattern</span>
- A design pattern which ensures a class only has 1 instance & provides a global point of access to it.
    1. Allows for lazy loading (initialize object creation only when you need it / are going to be using it).
    2. Only when you need 1 instance (i.e. a database connection)
        - Say if you create an object that is going to interacting with hardware & two could cause conflict.
- 3 main components
    - Single class
        - Private constructor
        - Private static instance
        - Factory static method responsible for instance creation
        - Can be problematic in multithreading (solution via synchronization block)

### <span style="color: aqua">What are some of the different software development methodologies?</span>
    - Waterfall, Agile, Rapid Application Development (RAD), Extreme Programming (XP)
    - Waterfall – this approach needs to be well disciplined as there isn’t planned opportunity to back track. It starts with clear and complete requirements and moves through the development process sequentially/linearly in distinct phases. Some of the drawbacks include its relatively rigid and inflexible, there isn’t an avenue for feedback early in the process and can be financially devastating if requirements are missing or planning is mismanaged. Its best when projects are relatively simple, little change is expected and a project manager is closely involved.
    - Agile – Focused on customer / stakeholder feedback & collaboration. There is an emphasis on rapid development to support fast delivery and is incredibly adaptable and open to change. The downsides however are that the lack of emphasis makes it difficult to truly develop a great design, its easy to get off track if the goals are unclear or the collaborative relationship steers the project in a different direction which may result in an unpredictable finished product.


### <span style="color: aqua">Explain MVC</span>
Software design pattern focused on Model, View, Controller components.
- Model aspect comprises the data of the application, Represents an object carrying data. It can also contain logic to update controller if data changes.
- View is the component that operates as a display to the user. Represents the visualization of the data that the model contains.
- Control influences the activity between the model and the view. Acts on both of model & the view. Controls the data flow into model object & updates the view whenever the data changes (Keeps the model & view separate).

### <span style="color: aqua">What is a UML diagram?</span>
UML is a general-purpose modeling language and is used to represent the components related to important OOP concepts. in essence it’s a general way of defining the whole software architecture or structure.

### <span style="color: aqua">What are design patterns?</span>
Represent best practices / solutions to general problems  frequently faced by software developers.

### <span style="color: aqua"></span>

### <span style="color: aqua"></span>

### <span style="color: aqua"></span>

### <span style="color: aqua"></span>

### <span style="color: aqua"></span>

### <span style="color: aqua"></span>

### <span style="color: aqua"></span>