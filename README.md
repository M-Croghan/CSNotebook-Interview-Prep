# INTERVIEW TOPICS, QUESTIONS & DISCUSSIONS
# INTRODUCTION

This repository serves as a knowledge base exploring technical interview questions related to topics and concepts
within computer science, as well as Java specific discussions. There exist many great resources on technical interview questions (linked below), but I wanted to be able to compile a list of questions specific to my own experiences that would be relevant to a junior role.

# TABLE OF CONTENTS
1. [Java & OOP]()
2. [Computer Science Concepts]()
3. [SQL & Databases / Data Management]()
4. [HTML / CSS]()
5. [JavaScript]()
6. [Spring Framework]()
7. [Python]()
8. [Git / GitHub]()
9. [Angular]()
10. [AWS]()
11. [Linux]()
12. [Reading List]()
13. [Resources]()

## <img src="img/java_red.png" alt="Java logo in red" width="40"/> JAVA / OOP <img src="img/java.png" alt="java logo" width="50"/>
:ballot_box_with_check: [What are the 4 pillars of Object-Oriented Programming? Describe them:](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#what-are-the-4-pillars-of-object-oriented-programming-describe-them)  
:ballot_box_with_check: [What is a class?](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#what-is-a-class)  
:ballot_box_with_check: [What is an object?](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#what-is-an-object)  
:ballot_box_with_check: [Discuss some of Java's naming conventions](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#discuss-some-of-javas-naming-conventions)  
:ballot_box_with_check: [Explain the difference between an object & a class](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#explain-the-difference-between-an-object--a-class)  
:ballot_box_with_check: [Explain the difference between method _overloading_ vs method _overriding_](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#explain-the-difference-between-method-overloading-vs-method-overriding)  
:ballot_box_with_check: [What is a ***constructor***?](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#what-is-a-constructor)  
:ballot_box_with_check: [Where are objects / variables stored?](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#where-are-objects--variables-stored)  
:ballot_box_with_check: [What are some benefits / features of Java?](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#what-are-some-of-the-benefits--features-of-java)  
:ballot_box_with_check: [Discuss Exception Handling](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#discuss-exception-handling-errors-vs-exceptions)  
:ballot_box_with_check: [Discuss Abstract Classes](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#discuss-abstract-classes)  
:ballot_box_with_check: [Discuss Interfaces](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#discuss-interfaces)  
:ballot_box_with_check: [Can you achieve multiple inheritance in Java](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#can-you-achieve-multiple-inheritance-in-java)  
:ballot_box_with_check: [Using an abstract class vs. an interface](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#using-an-abstract-class-vs-an-interface)  
:ballot_box_with_check: [Prove: Everything in Java is an object](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#prove-everything-in-java-is-an-object)  
:ballot_box_with_check: [Difference between constructor vs. method?](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#difference-between-constructor-vs-method)  
:ballot_box_with_check: [Give an example of ***checked*** vs. ***unchecked*** exceptions](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#give-an-example-of-checked-vs-unchecked-exceptions)  
:ballot_box_with_check: [Final vs. Finally vs. Finalize](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#final-vs-finally-vs-finalize)  
:ballot_box_with_check: [Discuss these access modifiers: Public / Private / Protected / Default](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#discuss-these-access-modifiers-public--private--protected--default)  
:ballot_box_with_check: [How are Java & JavaScript Different](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#how-are-java--javascript-different)  
:ballot_box_with_check: [Discuss the difference between _class_, _instance_, & _local_ variables](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#discuss-the-difference-between-class--instance-variables--methods)  
:ballot_box_with_check: [Discuss Multithreading](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#discuss-multithreading)  
:ballot_box_with_check: [What is Synchronization?](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#what-is-synchronization)  
:ballot_box_with_check: [Discuss Mutable Objects](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#discuss-mutable-objects)  
:ballot_box_with_check: [StringBuffer vs. StringBuilder](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#stringbuffer-vs-stringbuilder)  
:ballot_box_with_check: [Explain Overriding](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#explain-overriding)  
:ballot_box_with_check: [What is a Stream? What qualifies one?](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#what-is-a-stream-what-qualifies-as-one)  
:ballot_box_with_check: [How would you order the filtering & sorting of a stream?](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#how-would-you-order-the-filtering--sorting-of-a-stream)  
:ballot_box_with_check: [What is the Optional Class?](https://github.com/M-Croghan/Interview-Prep/blob/main/Java_OOP.md#what-is-the-optional-class)  
  


## <img src="img/binary.png" alt="binary folder" width="50"/> COMPUTER SCIENCE CONCEPTS <img src="img/tree.png" alt="tree ds" width="50"/>
:ballot_box_with_check: [Discuss the difference between _compiled_ & _interpreted_ languages:](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#discuss-the-difference-between-compiled--interpreted-languages)  
:ballot_box_with_check: [Explain "IS-A" & "HAS-A" relationships](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#explain-is-a--has-a-relationships)  
:ballot_box_with_check: [List the 4 main pillars of OOP](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#list-the-4-main-pillars-of-oop)  
:ballot_box_with_check: [What is polymorphism?](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#what-is-polymorphism)  
:ballot_box_with_check: [What is abstraction?](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#what-is-abstraction)  
:ballot_box_with_check: [What is inheritance?](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#what-is-inheritance)  
:ballot_box_with_check: [What is encapsulation?](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#what-is-encapsulation)  
:ballot_box_with_check: [What is Garbage Collection?](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#what-is-garbage-collection)  
:ballot_box_with_check: [Explain the Software Development Lifecycle (SDLC)](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#explain-the-software-developmnt-lifecycle-sdlc)  
:ballot_box_with_check: [What is a singleton design pattern?](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#what-is-a-singleton-design-pattern)  
:ballot_box_with_check: [What is a factory design pattern?](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#what-is-a-factory-design-pattern)  
:ballot_box_with_check: [What are some different software development methodologies?](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#what-are-some-of-the-different-software-development-methodologies)  
:ballot_box_with_check: [Explain MVC](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#explain-mvc)  
:ballot_box_with_check: [What is a UML Diagram?](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#what-is-a-uml-diagram)  
:ballot_box_with_check: [What are design patterns?](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#what-are-design-patterns)  
:ballot_box_with_check: [What is an API?](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#what-is-an-api)  
:ballot_box_with_check: [What is Unit Testing?](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#what-is-unit-testing)  
:ballot_box_with_check: [What happens when you type a URL into a browser and hit enter?](https://github.com/M-Croghan/Interview-Prep/blob/main/CS_Concepts.md#what-happens-when-you-type-a-url-into-a-browser-and-hit-enter)  


## <img src="img/pg.png" alt="postgresql logo" width="45"/> SQL / DATABASES <img src="img/mysql.png" alt="mysql logo" width="50"/>
:ballot_box_with_check:[What is a database?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-is-a-database)  
:ballot_box_with_check: [What is a relational database?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-is-a-relational-database)  
:ballot_box_with_check: [What is a database management system?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-is-a-database-management-system)
:ballot_box_with_check: [What is SQL?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-is-sql)  
:ballot_box_with_check: [What are aggregate functions in SQL?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-are-aggregate-functions-in-sql)  
:ballot_box_with_check: [What are scalar functions in SQL?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-are-scalar-functions-in-sql)  
:ballot_box_with_check: [Discuss Normalization](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#discuss-normalization)  
:ballot_box_with_check: [What do we need to do to decrease the retrieval time?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-do-we-need-to-do-to-decrease-the-retrieval-time)  
:ballot_box_with_check: [What are the different types of joins in SQL?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-are-the-different-types-of-joins-in-sql)  
:ballot_box_with_check: [Tables vs. Views in SQL](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#tables-vs-views-in-sql)  
:ballot_box_with_check: [What is group by, order by in SQL?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-is-group-by-order-by-in-sql)  
:ballot_box_with_check: [What is the having clause?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-is-the-having-clause)  
:ballot_box_with_check: [Types of keys in SQL](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#types-of-keys-in-sql)  
:ballot_box_with_check: [What is a primary key?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-is-a-primary-key)  
:ballot_box_with_check: [What is a foreign key?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-is-a-foreign-key)  
:ballot_box_with_check: [What are two different types of indexes for a table?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-are-two-different-types-of-indexes-for-a-table-)  
:ballot_box_with_check: [What is an index?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-is-an-index)  
:ballot_box_with_check: [What are clustered / non-clustered indexes?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-are-clustered--non-clustered-indexes)  
:ballot_box_with_check: [Discuss how to build relationships?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#discuss-how-to-build-relationships)  
:ballot_box_with_check: [ACID Test](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#acid-test)  
:ballot_box_with_check: [What is Referential Integrity?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-is-referential-integrity)  
:ballot_box_with_check: [What is an ERD?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-is-an-erd)  
:ballot_box_with_check: [How can you get a list of all your databases?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#how-can-you-get-a-list-of-all-your-databases)  
:ballot_box_with_check: [How can you get the list of all the tables in a database?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#how-can-you-get-the-list-of-all-the-tables-in-a-database)  
:ballot_box_with_check: [How do you delete a table? ](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#how-do-you-delete-a-table)  
:ballot_box_with_check: [What is NoSQL?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-is-nosql)  
:ballot_box_with_check: [What is a candidate key?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-is-a-candidate-key)  
:ballot_box_with_check: [What is a composite key?](https://github.com/M-Croghan/Interview-Prep/blob/main/SQL_Databases.md#what-is-a-composite-key)  


## <img src="img/html-css.png" alt="html css logos" width="50"/> HTML & CSS <img src="img/html-css.png" alt="html css logos" width="50"/>
:ballot_box_with_check: [What does it mean for a website to be responsive?](https://github.com/M-Croghan/Interview-Prep/blob/main/HTML_CSS.md#what-does-it-mean-for-a-website-to-be-responsive)  
:ballot_box_with_check: [What is CSS specificity?](https://github.com/M-Croghan/Interview-Prep/blob/main/HTML_CSS.md#what-is-css-specificity)  
:ballot_box_with_check: [Where would you link a JS file in your HTML?](https://github.com/M-Croghan/Interview-Prep/blob/main/HTML_CSS.md#where-would-you-link-a-js-file-in-your-html)  
:ballot_box_with_check: [What are the benefits of maintaining an external Javascript file?](https://github.com/M-Croghan/Interview-Prep/blob/main/HTML_CSS.md#what-are-the-benefits-of-maintaining-an-external-javascript-file)  



## <img src="img/js.png" alt="yellow js logo" width="50"/> JAVASCRIPT <img src="img/javascript.png" alt="green js logo" width="37"/>
:ballot_box_with_check: [What is AJAX?](https://github.com/M-Croghan/Interview-Prep/blob/main/JavaScript.md#what-is-ajax)  
:ballot_box_with_check: [Tell me about when you may need to use AJAX?](https://github.com/M-Croghan/Interview-Prep/blob/main/JavaScript.md#tell-me-about-when-you-may-need-to-use-ajax)  
:ballot_box_with_check: [What does callback mean in JS?](https://github.com/M-Croghan/Interview-Prep/blob/main/JavaScript.md#what-does-callback-mean-in-js)  



## <img src="img/spring.png" alt="spring logo" width="40"/> SPRING FRAMEWORK <img src="img/sboot.png" alt="spring boot logo" width="50"/>
:ballot_box_with_check: [What is a framework?](https://github.com/M-Croghan/Interview-Prep/blob/main/Spring.md#what-is-a-framework)  
:ballot_box_with_check: [What is the default web server built-in to Spring?](https://github.com/M-Croghan/Interview-Prep/blob/main/Spring.md#what-is-the-default-web-server-built-in-to-spring)  
:ballot_box_with_check: [What is Maven?](https://github.com/M-Croghan/Interview-Prep/blob/main/Spring.md#what-is-maven)  
:ballot_box_with_check: [What purpose does the pom.xml file serve?](https://github.com/M-Croghan/Interview-Prep/blob/main/Spring.md#what-purpose-does-the-pomxml-file-serve)  
:ballot_box_with_check: [What is Inversion of Control (IoC)?](https://github.com/M-Croghan/Interview-Prep/blob/main/Spring.md#what-is-inversion-of-control-ioc)  
:ballot_box_with_check: [What is Dependency Injection?](https://github.com/M-Croghan/Interview-Prep/blob/main/Spring.md#what-is-dependency-injection)  
:ballot_box_with_check: [What is Aspect-Oriented Programming?](https://github.com/M-Croghan/Interview-Prep/blob/main/Spring.md#what-is-aspect-oriented-programming)  
:ballot_box_with_check: [Discuss POJOs & Beans](https://github.com/M-Croghan/Interview-Prep/blob/main/Spring.md#discuss-pojos--beans)  
:ballot_box_with_check: [What is a profile?](https://github.com/M-Croghan/Interview-Prep/blob/main/Spring.md#what-is-a-profile)  

## <img src="img/py.png" alt="python logo" width="40"/> PYTHON <img src="img/py.png" alt="python logo" width="40"/>
:ballot_box_with_check: []()  
:ballot_box_with_check: []()  
:ballot_box_with_check: []()  
## <img src="img/git.png" alt="git logo" width="40"/> GIT / GITHUB <img src="img/github_white.png" alt="github logo" width="40"/>
:ballot_box_with_check: []()  
:ballot_box_with_check: []()  
:ballot_box_with_check: []()  
## <img src="img/angular.png" alt="angular logo" width="50"/> ANGULAR <img src="img/angular.png" alt="angular logo" width="50"/>
:ballot_box_with_check: []()  
:ballot_box_with_check: []()  
:ballot_box_with_check: []()  
## <img src="img/aws1.png" alt="aws logo" width="80"/> AWS <img src="img/aws2.png" alt="aws logo" width="60"/>
:ballot_box_with_check: []()  
:ballot_box_with_check: []()  
:ballot_box_with_check: []()  
## <img src="img/linux.png" alt="linux logo" width="50"/> LINUX <img src="img/linux.png" alt="linux logo" width="50"/>
:ballot_box_with_check: []()  
:ballot_box_with_check: []()  
:ballot_box_with_check: []()  


## LINKS / RESOURCES
----------------------------------------------------------------------------------------------
# [READING / BOOK LIST]()
----------------------------------------------------------------------------------------------
* Preparation
    * [Tech Interview Handbook](https://github.com/yangshun/tech-interview-handbook)
        * [Direct Link](https://techinterviewhandbook.org/landscape/)
    * [Coding Interview University](https://github.com/jwasham/coding-interview-university)
    * [Awesome Interview Questions](https://github.com/DopplerHQ/awesome-interview-questions) <-- Where many of the below resources are sourced from!
    * [Interview Guide](https://github.com/Olshansk/interview)
    * [System Design Primer](https://github.com/donnemartin/system-design-primer)  
----------------------------------------------------------------------------------------------
* General Data Structures & Algorithms
    * [40 Data Structure Interview Questions](https://www.interviewbit.com/data-structure-interview-questions/)
    * [Top 50 Data Structures Interview Questions & Answers](https://career.guru99.com/top-50-data-structure-interview-questions/)
----------------------------------------------------------------------------------------------
* Java
    * [15 DS&A Interview Questions & Answers in Java](https://javarevisited.blogspot.com/2013/03/top-15-data-structures-algorithm-interview-questions-answers-java-programming.html)
    * [Java Coding Interview Problems](https://java2novice.com/java-interview-programs/)
    * [150 Java Interview Questions and Answers – The ULTIMATE List](https://www.javacodegeeks.com/java-interview-questions.html)
    * [Basic Java Interview Questions](https://www.interviewbit.com/java-interview-questions/)
    * [Top 40 Core Java Interview Questions Answers](https://www.java67.com/2015/03/top-40-core-java-interview-questions-answers-telephonic-round.html)
----------------------------------------------------------------------------------------------
* Spring
    * [Spring Interview Questions and Answers](https://www.journaldev.com/2696/spring-interview-questions-and-answers)
    * [Top 50 Spring Interview Questions You Must Know!](https://www.edureka.co/blog/interview-questions/spring-interview-questions/)
----------------------------------------------------------------------------------------------
* SQL
    * [SQL Interview Questions](https://www.interviewbit.com/sql-interview-questions/)
    * [20 General SQL Interview Questions and Answers](https://www.indiabix.com/technical/sql-server-general-questions/4)
    * [10 MySQL Database Interview Questions for Beginners and Intermediates](https://www.tecmint.com/10-mysql-database-interview-questions-for-beginners-and-intermediates/)
-----------------------------------------------------------------------------------------------
* Design Patterns
    * [Design Patterns for Humans!](https://github.com/kamranahmedse/design-patterns-for-humans)
    * [Design Patterns with Java](https://github.com/iluwatar/java-design-patterns)
----------------------------------------------------------------------------------------------
* HTML
    * [10 Typical HTML Interview Exercises](https://www.sitepoint.com/10-typical-html-interview-exercises/)
    * [16 Essential HTML5 Interview Questions](https://www.toptal.com/html5/interview-questions)
    * [40 important HTML 5 Interview questions with answers](https://www.codeproject.com/Articles/702051/important-HTML-Interview-questions-with-answe)
    * [HTML Interview Questions](https://www.interviewbit.com/html-interview-questions/)
----------------------------------------------------------------------------------------------
* CSS
    * [61 CSS Interview Questions and Answers](https://www.careerride.com/Interview-Questions-CSS.aspx)
    * [CSS interview questions and answers](https://www.techrepublic.com/blog/software-engineer/css-interview-questions-and-answers/)
    * [Interview Questions and Exercises About CSS](https://css-tricks.com/interview-questions-css/)
----------------------------------------------------------------------------------------------
* JavaScript
    * [10 Interview Questions Every JavaScript Developer Should Know](https://medium.com/javascript-scene/10-interview-questions-every-javascript-developer-should-know-6fa6bdf5ad95)
    * [21 Essential JavaScript Interview Questions](https://www.codementor.io/@nihantanu/21-essential-javascript-tech-interview-practice-questions-answers-du107p62z)
    * [20 Essential javascript-developers Interview Questions](https://adevait.com/javascript-developers/interview-questions)
    * [37 Essential JavaScript Interview Questions](https://www.toptal.com/javascript/interview-questions)
    * [5 Typical JavaScript Interview Exercises](https://www.sitepoint.com/5-typical-javascript-interview-exercises/)
----------------------------------------------------------------------------------------------
* Angular
    * [51 Angular Interview Questions](https://www.onlineinterviewquestions.com/angular2-interview-questions/)
    * [Angular Questions to Test Yourself](https://github.com/Yonet/Angular-Interview-Questions)
----------------------------------------------------------------------------------------------
* Python
    * [11 Essential Python Interview Questions](https://www.toptal.com/python/interview-questions)
    * [Python interview questions. Part I. Junior](https://luminousmen.com/post/python-interview-questions-junior)
    * [Python Coding Problems](https://www.bogotobogo.com/python/python_interview_questions.php)
    * [26 Essential python](https://adevait.com/python/interview-questions)
----------------------------------------------------------------------------------------------
* Linux
    * [11 Basic Linux Interview Questions and Answers](https://www.tecmint.com/basic-linux-interview-questions-and-answers/)
    * [11 Essential Linux Interview Questions](https://www.toptal.com/linux/interview-questions)
----------------------------------------------------------------------------------------------
* AWS
    * [Top 90 AWS Interview Questions and Answers for 2022](https://www.simplilearn.com/tutorials/aws-tutorial/aws-interview-questions)


