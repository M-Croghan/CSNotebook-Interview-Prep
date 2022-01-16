# SPRING FRAMEWORK CONCEPTS & QUESTIONS

### :leaves: <span style="color: aqua">What is a framework?</span>
Frameworks make building applications faster and more efficient. It provides the basis on which developers can build programs for a specific platform. For example, a framework may include predetermined classes as well as functions. It can be used to process inputs, manage hardware, and interact with system software. (ex. Spring is one of the more popular frameworks for Java.)

### :leaves: <span style="color: aqua">What is the default web server built-in to Spring?</span>
Apache Tomcat

### :leaves: <span style="color: aqua">What is Maven?</span>
Build tools are programs that automate the creation of executable applications from source code (e.g., .apk for an Android app). Building incorporates compiling, linking, and packaging the code into a usable or executable form.
Maven is a build tool / project management & comprehension tool. One perk is that it will download all the libraries that you use and the libraries that they use for you automatically
- Makes the build process easier
- Provides a uniform build system
- Provides high quality project info
- Provides guidelines for best practices development
- Allows transparent migration to new features

### :leaves: <span style="color: aqua">What purpose does the pom.xml file serve?</span>
- POM: Project Object Model
  - The fundamental unit of work in Maven
  - Contains info about the project and configuration details used by maven to build the project
    - The dependencies.
### :leaves: <span style="color: aqua">What is Inversion of Control (IoC)?</span>
Instead of the programmer controlling the flow of the program, external sources (framework, services, etc.) take over. The framework makes most of the decisions until it comes time for the application specific logic written by the developer to be called upon, after which the developers code returns control back to the framework.

### :leaves: <span style="color: aqua">What is Dependency Injection?</span>
A dependency is a requirement necessary for something to function. Dependency injection generally means passing a dependent object as a parameter to a method, rather than having the method create the dependent object. This means that a method doesn't need to be dependent on any particular implementation, but one that meets the requirements can be passed to it as parameter. A subset of IoC, an already instantiated instance can be injected into a class, so it can use its methods.  

An example would be that of programming a house-building robot. As it builds the walls of a house, every time it gets to a doorway, it has to make a decision on what door should be installed. It depends on having the exact type and specifications of the door and needs to figure those things out at each doorway. Dependency injection would be purchasing the doors we want from a supplier and passing them to the robot to install.

The process of injecting dependent bean objects into target bean objects is called dependency injection.  

- Setter Injection: The IOC container will inject the dependent bean object into the target bean object by calling the setter method.
- Constructor Injection: The IOC container will inject the dependent bean object into the target bean object by calling the target bean constructor.
- Field Injection: The IOC container will inject the dependent bean object into the target bean object by Reflection API

### :leaves: <span style="color: aqua">What is Aspect-Oriented Programming</span>
***Cross-cutting concerns*** are parts of a program that rely on or must affect many other parts of the system. They form the basis for the development of ***aspects***. A concern means logic or functionality (some examples: logging / security). The idea is to encapsule the logic of the concern into a module / aspect, and apply it to the relevant portions of your code. The aspect is created in one location and it can be applied anywhere in the application based on the application.
- Example:
  - Say you want to incorporate logging into your application: there could be hundreds of areas where it may need to be applied, bundling logging into an aspect can allow for it to exist in one location but be used anywhere else in the application.
### :leaves: <span style="color: aqua">Discuss POJOs & Beans</span>
- POJO: Plain Old Java Object.
  - Any java object is a POJO.
  - Not bound by any special restriction (no convention followed).
- A Bean is also a POJO
  - They have restrictions (private fields, include getters/setters, no-arg constructor)
  - But, with a bean, only ***one*** exists of a particular instance.
    - Singleton Pattern is default on beans.
      - Singleton Beans = Stateless Beans

In Spring Singleton refers to One bean per Spring container where as in Java Singleton refers to one object per class loader. So Spring singleton is not same as java singleton. Don't get confused between these two.


### :leaves: <span style="color: aqua">What is a profile?</span>
Profiles serve as the configuration that govern a given environment (i.e. development, production, etc.). Within a Spring application, the resources' folder holds the profiles. These profiles are .properties files and follow a naming convention to denote which environment they pertain to (i.e. ***application-dev.properties***).
Spring Boot provides various properties which can be specified inside our project's application.properties file. These properties have default values and you can set that inside the properties file. Properties are used to set values like: server-port number, database connection configuration etc.
### :leaves: <span style="color: aqua">What is Spring Boot?</span>
Spring Boot is a Spring module which provides RAD (Rapid Application Development) feature to Spring framework. It is used to create stand alone spring based application that you can just run because it needs very little spring configuration.
### :leaves: <span style="color: aqua">How to create Spring Boot application using Maven?</span>
There are multiple approaches to create Spring Boot project. We can use any of the following approach to create application.
- Spring Maven Project
- Spring Starter Project Wizard
- Spring Initializr
- Spring Boot CLI

### :leaves: <span style="color: aqua">What are the Spring Boot Starters?</span>
Starters are a set of convenient dependency descriptors which we can include in our application.
Spring Boot provides built-in starters which makes development easier and rapid. For example, if we want to get started using Spring and JPA for database access, just include the spring-boot-starter-data-jpa dependency in your project.
### :leaves: <span style="color: aqua">What is Spring Boot Actuator?</span>
Actuator is mainly used to expose operational information about the running application — health, metrics, info, dump, env, etc. It uses HTTP endpoints or JMX beans to enable us to interact with it. Once this dependency is on the classpath, several endpoints are available for us out of the box. Spring Boot provides actuator to monitor and manage our application. Actuator is a tool which has HTTP endpoints. When application is pushed to production, you can choose to manage and monitor your application using HTTP endpoints. Spring Actuator is a cool feature of Spring Boot with the help of which you can see what is happening inside a running application. So, whenever you want to debug your application, and need to analyze the logs you need to understand what is happening in the application right? In such a scenario, the Spring Actuator provides easy access to features such as identifying beans, CPU usage, etc. The Spring Actuator provides a very easy way to access the production-ready REST points and fetch all kinds of information from the web. These points are secured using Spring Security’s content negotiation strategy.
### :leaves: <span style="color: aqua">How to connect Spring Boot to the database using JPA?</span>
Spring Boot provides spring-boot-starter-data-jpa starter to connect Spring application with relational database efficiently. You can use it by adding it into the project's POM.xml (Project Object Model) file.
### :leaves: <span style="color: aqua">What is @RequestMapping annotation in Spring Boot?</span>
The @RequestMapping annotation is used to provide routing information. It tells to the Spring that any HTTP request should map to the corresponding method. We need to import org.springframework.web.annotation package in our file.
### :leaves: <span style="color: aqua">Spring Vs Spring Boot?</span>
Spring is a web application framework based on Java. It provides tools and libraries to create a complete customized web application. Whereas Spring Boot is a spring module which is used to create spring application project that can just run.
### :leaves: <span style="color: aqua">What is the need for Spring Boot DevTools?</span>
Spring Boot Dev Tools are an elaborated set of tools that aims to make the process of developing an application easier. If the application runs in the production, then this module is automatically disabled, repackaging of archives are also excluded by default. So, the Spring Boot Developer Tools applies properties to the respective development environments.

### :leaves: <span style="color: aqua">Mention the differences between JPA and Hibernate.</span>
- JPA is a Data Access Abstraction used to reduce the amount of boilerplate code.
  - Java Persistence API is a collection of classes and methods to persistently store the vast amounts of data into a database.
-	Hibernate is an implementation of Java Persistence API and offers the benefits of loose coupling.
  - Hibernate is a high-performance Object/Relational persistence and query service. It not only takes care of the mapping from Java classes to database tables (and from Java data types to SQL data types), but also provides data query and retrieval facilities.
### :leaves: <span style="color: aqua">Explain Spring Data:</span>
Spring Data aims to make it easy for the developers to use relational and non-relational databases, cloud-based data services, and other data access technologies. So, basically, it makes it easy for data access and still retains the underlying data.
### :leaves: <span style="color: aqua">Features of Spring Boot that make it different?</span>
- Creates stand-alone spring application with minimal configuration needed.
- It has embedded tomcat, jetty which makes it just code and run the application.
- Provide production-ready features such as metrics, health checks, and externalized configuration.
- Absolutely no requirement for XML configuration.

### :leaves: <span style="color: aqua">What are the Spring Boot key components?</span>
Below are the four key components of spring-boot:
- Spring Boot auto-configuration.
- Spring Boot CLI.
- Spring Boot starter POMs.
- Spring Boot Actuators
### :leaves: <span style="color: aqua">How does a spring boot application get started?</span>
Just like any other Java program, a Spring Boot application must have a main method. This method serves as an entry point, which invokes the SpringApplication#run method to bootstrap the application.
### :leaves: <span style="color: aqua">What is Spring Initializer?</span>
Spring Initializer is a web application that helps you to create an initial spring boot project structure and provides a maven or gradle file to build your code. It solves the problem of setting up a framework when you are starting a project from scratch
### :leaves: <span style="color: aqua">Is it possible to change the port of the embedded Tomcat server in Spring Boot?</span>
Yes, it is possible. By setting ```server.port``` to the desired port in the application.properties file.
### :leaves: <span style="color: aqua">What is the default port of tomcat in spring boot?</span>
The default port of the tomcat server-id 8080. It can be changed by adding sever.port properties in the application.property file.
### :leaves: <span style="color: aqua">Can we override or replace the Embedded tomcat server in Spring Boot?</span>
Yes, we can replace the Embedded Tomcat server with any server by using the Starter dependency in the pom.xml file. Like you can use spring-boot-starter-jetty as a dependency for using a jetty server in your project.
### :leaves: <span style="color: aqua">Can we disable the default web server in the Spring boot application?</span>
Yes, we can use application.properties to configure the web application type i.e spring.main.web-application-type=none
### :leaves: <span style="color: aqua">Explain @RestController annotation in Spring boot?</span>
It is a combination of @Controller and @ResponseBody, used for creating a restful controller. It converts the response to JSON or XML. It ensures that data returned by each method will be written straight into the response body instead of returning a template.

### :leaves: <span style="color: aqua">What is the difference between @RestController and @Controller in Spring Boot?</span>
@Controller Maps the model object to view or template and makes it human readable but @RestController simply returns the object and object data is directly written in HTTP response as JSON or XML.
### :leaves: <span style="color: aqua">What is the difference between RequestMapping and GetMapping?</span>
RequestMapping can be used with GET, POST, PUT, and many other request methods using the method attribute on the annotation. Whereas getMapping is only an extension of RequestMapping which helps you to improve on clarity on request.
### :leaves: <span style="color: aqua">What is an IOC container?</span>
The IoC container is responsible to instantiate, configure and assemble the objects. The IoC container gets information from the XML file and works accordingly. The main tasks performed by IoC container are:
- Instantiate the application class
- Configure the object
- Assemble the dependencies between the objects

There are two types of IoC containers. They are:
- BeanFactory
- ApplicationContext

### :leaves: <span style="color: aqua">Default HTML template engine in Spring Boot?</span>
Thymeleaf
