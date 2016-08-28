list-of-lists
---
My List of Lists

[TOC]:#

# Table of Contents
- [list-of-lists](#list-of-lists)
- [Application Development](#application-development)
    - [Angular 2](#angular-2)
    - [Ionic 2](#ionic-2)
    - [Javascript](#javascript)
- [Architecture](#architecture)
    - [APIs](#apis)
    - [Database](#database)
    - [Microservices](#microservices)
    - [Reactive Programming](#reactive-programming)
    - [REST (REpresentational State Transfer)](#rest-representational-state-transfer)
    - [Security](#security)
- [Developer Workflows](#developer-workflows)
- [Editors](#editors)
    - [Sublime](#sublime)
    - [[gravzio uml markdown](gravzio.com)](#gravzio-uml-markdowngravziocom)
 


## Application Development 

### Angular 2

### Ionic 2
* [Setup Ionic 2 + TypeScript Debugging with IntelliJ/WebStorm/Jetbrains IDE](http://blog.thecodecampus.de/setup-ionic-2-typescript-debugging-intellijwebstormjetbrains-ide/)

### Javascript

##Architecture

### APIs
* [user-friendly-api - Gleb Bahmutov](http://glebbahmutov.com/blog/user-friendly-api/)

### Database
#### MongoDB
* [Storing Tree Structues w/ MongoDB (slideshare)](http://www.slideshare.net/voronenko/storing-tree-structures-with-mongodb)

#### mySQL & related

### Microservices
* [Micorservices architectural best practices - netflix](https://www.nginx.com/blog/microservices-at-netflix-architectural-best-practices/)
* [Consumer driver contracts - Martin Fowler](http://martinfowler.com/articles/consumerDrivenContracts.html)
* [How to CQRS in Node: Eventually Consistent, Unidirectional Systems with Microservices](http://nycnode.com/videos/matt-walters-how-to-cqrs-in-node-eventually-consistent-unidirectional-systems-with-microservices)

### Reactive Programming
* [The introduction to Reactive Programming you've been missing - @andrestaltz](https://gist.github.com/staltz/868e7e9bc2a7b8c1f754)

### REST (REpresentational State Transfer)
* [Richardson Maturity Model](http://martinfowler.com/articles/richardsonMaturityModel.html)

### Security
* [National Vulnerability Database](https://nvd.nist.gov/home.cfm)

## Developer Workflows
* [Paul Irish - youtube on appdev workflow](https://www.youtube.com/watch?v=vDbbz-BdyYc)
* [Paul Irish - youtube on javascript workflow](https://www.youtube.com/watch?v=f7AU2Ozu8eo)
* [Adventures in JavaScript Development - Rebecca Murphy](http://rmurphey.com/)
* <a href="http://dotfiles.github.io" target="_blank">Your unofficial guide to dotfiles on GitHub. - dotfiles.github.io</a>

##  Editors
### Sublime
* [Sublime Linter User Settings](http://bl.ocks.org/bretdavidson/3189814)

### [gravzio uml markdown](gravzio.com)

#### 

![gravzio diagraph example](http://g.gravizo.com/g?
  digraph G {
    aize ="4,4";
    main [shape=box];
    main -> parse [weight=8];
    parse -> execute;
    main -> init [style=dotted];
    main -> cleanup;
    execute -> { make_string; printf};
    init -> make_string;
    edge [color=red];
    main -> printf [style=bold,label="100 times"];
    make_string [label="make a string"];
    node [shape=box,style=filled,color=".7 .3 1.0"];
    execute -> compare;
  }
)

![Alt text](http://g.gravizo.com/g?
@startuml;
actor User;
participant "First Class" as A;
participant "Second Class" as B;
participant "Last Class" as C;
User -> A: DoWork;
activate A;
A -> B: Create Request;
activate B;
B -> C: DoWork;
activate C;
C --> B: WorkDone;
destroy C;
B --> A: Request Created;
deactivate B;
A --> User: Done;
deactivate A;
@enduml
)








