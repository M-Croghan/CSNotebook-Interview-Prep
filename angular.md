# ANGULAR QUESTIONS & CONCEPTS
### :a: <span style="color: aqua">What is Angular?</span>
Angular is an open-source, web application framework wholly written in TypeScript that was developed and is maintained by Google. It uses HTML's syntax to express your application's components clearly. This framework brings structure and consistency to web applications and provides excellent scalability and maintainability. It integrates a range of features like declarative templates, dependency injection, end-to-end tooling, etc. that facilitates web application development. It excels in creating Single Page Applications (SPAs).

### :a: <span style="color: aqua">What is a SPA?</span>
 A Single Page Application in which only a single page (index.HTML), is maintained although the URL keeps on changing. Unlike traditional web technology, SPA technology is faster and easy to develop as well.  This is made possible through JavaScript's ability to manipulate the DOM elements on the existing page itself. A SPA approach is faster, thus providing a seamless user experience.

In conventional web technology, as soon as a client requests a webpage, the server sends the resource. However, when again the client requests for another page, the server responds again with sending the requested resource. The problem with this technology is that it requires a lot of time.

### :a: <span style="color: aqua">What are decorators in Angular?</span>
Decorators are a design pattern or functions that define how Angular features work. They are used to make prior modifications to a class, service, or filter. Angular supports four types of decorators, they are:
1. Class Decorators
2. Property Decorators
3. Method Decorators
4. Parameter Decorators

### :a: <span style="color: aqua">What are Templates in Angular?</span>
Angular Templates are written with HTML that contains Angular-specific elements and attributes. In combination with the model and controller's information, these templates are further rendered to provide a dynamic view to the user.

### :a: <span style="color: aqua">What are Annotations in Angular?</span>
Annotations in Angular are used for creating an annotation array. They are the metadata set on the class that is used to reflect the Metadata library.

### :a: <span style="color: aqua">What are Directives in Angular?</span>
Directives are attributes that allow the user to write new HTML syntax specific to their applications. They execute whenever the Angular compiler finds them in the DOM. Angular supports three types of directives.  
1. Component Directives
2. Structural Directives
3. Attribute Directives 

### :a: <span style="color: aqua">What are Components in Angular?</span>
Components are the basic building blocks of the user interface in an Angular application. Every component is associated with a template and is a subset of directives. An Angular application typically consists of a root component, which is the AppComponent, that then branches out into other components creating a hierarchy.

### :a: <span style="color: aqua">What are pipes?</span>
Pipes are simple functions designed to accept an input value, process, and return as an output, a transformed value in a more technical understanding. Angular supports several built-in pipes. However, you can also create custom pipes that cater to your needs. 

Some key features include: 
* Pipes are defined using the pipe “|” symbol. 
* Pipes can be chained with other pipes.
* Pipes can be provided with arguments by using the colon (:) sign.

### :a: <span style="color: aqua">What is an ngModule?</span>
NgModules are containers that reserve a block of code to an application domain or a workflow. @NgModule takes a metadata object that generally describes the way to compile the template of a component and to generate an injector at runtime. In addition, it identifies the module's components, directives, and pipes, making some of them public, through the export property so that external components can use them.

### :a: <span style="color: aqua">What are Services in Angular?</span>
Angular Services perform tasks that are used by multiple components. These tasks could be data and image fetching, network connections, and database management among others. They perform all the operational tasks for the components and avoid rewriting of code. A service can be written once and injected into all the components that use that service. 

### :a: <span style="color: aqua">What are Promises?</span>
Promises emit a single value at a time. They execute immediately after creation and are not cancellable. They are Push errors to the child promises. 
### :a: <span style="color: aqua">What are Observables?</span>
Observables are only executed when subscribed to them using the subscribe() method. They emit multiple values over a period of time. They help perform operations like forEach, filter, and retry, among others. They deliver errors to the subscribers. When the unsubscribe() method is called, the listener stops receiving further values.

### :a: <span style="color: aqua">What is ngOnInit? How is it defined?</span>
ngOnInit is a lifecycle hook and a callback method that is run by Angular to indicate that a component has been created. It takes no parameters and returns a void type.

### :a: <span style="color: aqua">How is ngFor used in a tag?</span>
The ngFor directive is used to build lists and tables in the HTML templates. In simple terms, this directive is used to iterate over an array or an object and create a template for each element. 

### :a: <span style="color: aqua">What is Bootstrap? How is it embedded into Angular?</span>
Bootstrap is a powerful toolkit. It is a collection of HTML, CSS, and JavaScript tools for creating and building responsive web pages and web applications.  

There are two ways to embed the bootstrap library into your application. 
1. Angular Bootstrap via CDN - Bootstrap CDN is a public Content Delivery Network. It enables you to load the CSS and JavaScript files remotely from its servers. 
2. Angular Bootstrap via NPM - Another way to add Bootstrap to your Angular project is to install it into your project folder by using NPM (Node Package Manager). 

- npm install bootstrap 
- npm install jquery

### :a: <span style="color: aqua">What are the biggest advantages of using Angular?  </span>
1. Angular supports two-way data-binding.
2. It follows MVC pattern architecture.
3. It supports static templates and Angular template.
4. It facilitates you to add a custom directive.
5. It also supports RESTfull services.
6. Validations are supported in Angular.
7. Angular provides client and server communication.
8. It provides support for dependency injection.
9. It provides powerful features like Event Handlers, Animation, etc.

### :a: <span style="color: aqua">What is the package.json file?</span>
Package.json is an important file for the project where you import all of the relevant metadata / dependencies to be used in your project. There are three basic types of dependencies:
1. Dependency
2. DevDependency
3. peerDependency

### :a: <span style="color: aqua">What is a Module in Angular?</span>
A module is a mechanism to group components, directives, pipes and services that are related, in such a way that can be combined with other modules to create an application. An Angular application can be thought of as a puzzle where each piece (or each module) is needed to be able to see the full picture.

### :a: <span style="color: aqua">What is the observable pattern?</span>
The observer design pattern enables a subscriber to register with and receive notifications from a provider. It is suitable for any scenario that requires push-based notification. The pattern defines a provider (also known as a subject or an observable) and zero, one, or more observers. Observers register with the provider, and whenever a predefined condition, event, or state change occurs, the provider automatically notifies all observers by calling one of their methods. In this method call, the provider can also provide current state information to observers. 

### :a: <span style="color: aqua"></span>

### :a: <span style="color: aqua"></span>

### :a: <span style="color: aqua"></span>

### :a: <span style="color: aqua"></span>

### :a: <span style="color: aqua"></span>

### :a: <span style="color: aqua"></span>

### :a: <span style="color: aqua"></span>

### :a: <span style="color: aqua"></span>