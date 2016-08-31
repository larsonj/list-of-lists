**My list-of-lists**

<a href="#toc"></a>
[TOC levels=1-3]:# "#### Contents"

#### Contents
- [Data Visualization](#data-visualization)
- [Dev](#dev)
    - [Languages & Frameworks](#languages--frameworks)
        - [HTML & CSS](#html--css)
        - [JS Engines](#js-engines)
        - [JS Frameworks](#js-frameworks)
        - [Javascript Style Guides](#javascript-style-guides)
        - [NodeJS](#nodejs)
    - [Architecture](#architecture)
        - [APIs](#apis)
        - [Backend Server Platforms](#backend-server-platforms)
        - [Database](#database)
        - [Microservices](#microservices)
        - [Reactive Programming](#reactive-programming)
        - [REST (REpresentational State Transfer)](#rest-representational-state-transfer)
    - [Security](#security)
    - [Developer tools & workflows](#developer-tools--workflows)
        - [Editors and IDEs](#editors-and-ides)
        - [Scource Code Management](#scource-code-management)
- [DevOps](#devops)
    - [Docker](#docker)
- [Philosophy](#philosophy)

# Data Visualization
* [Flame Graphs](http://www.brendangregg.com/flamegraphs.html) 

# Dev

## Languages & Frameworks

### HTML & CSS
* [multiple.js -An experiment in sharing background across multiple elements using CSS](http://multiple.js.org/) 
 
### JS Engines 
* [Demystifying js engines - a list of resources](https://github.com/a0viedo/demystifying-js-engines?utm_campaign=explore-email&utm_medium=email&utm_source=newsletter&utm_term=weekly) 

### JS Frameworks

#### Angular 2

#### Ionic 2
* [Setup Ionic 2 + TypeScript Debugging with IntelliJ/WebStorm/Jetbrains IDE](http://blog.thecodecampus.de/setup-ionic-2-typescript-debugging-intellijwebstormjetbrains-ide/)
* [Ionic 2 resources](https://github.com/candelibas/awesome-ionic2)
* [Ionic 2 reference application](https://github.com/driftyco/ionic-conference-app) 

#### Ionic Framework
* [A collection of Ionic Framework Resources](http://emersonthompson.com.br/ionic-collection/)

### Javascript Style Guides
* [Google javascript styleguide](https://google.github.io/styleguide/javascriptguide.xml)
* [Airbnb javascript styleguide](https://github.com/airbnb/javascript)

### NodeJS
[Node.js Playbook](https://github.com/HiFaraz/node-playbook?utm_campaign=explore-email&utm_medium=email&utm_source=newsletter&utm_term=weekly#workflow) 

## Architecture

### APIs
* [user-friendly-api - Gleb Bahmutov](http://glebbahmutov.com/blog/user-friendly-api/)

### Backend Server Platforms
#### Deepstream.io
* [deepstream.io](http://www.deepstream.io)

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

## Security
* [National Vulnerability Database](https://nvd.nist.gov/home.cfm)

## Developer tools & workflows
* [Paul Irish - youtube on appdev workflow](https://www.youtube.com/watch?v=vDbbz-BdyYc)
* [Paul Irish - youtube on javascript workflow](https://www.youtube.com/watch?v=f7AU2Ozu8eo)
* [Adventures in JavaScript Development - Rebecca Murphy](http://rmurphey.com/)
* <a href="http://dotfiles.github.io" target="_blank">Your unofficial guide to dotfiles on GitHub. - dotfiles.github.io</a>
###  Editors and IDEs
#### Sublime
* [Sublime Linter User Settings](http://bl.ocks.org/bretdavidson/3189814)
#### UML markdown 
* [Graphviz is open source graph visualization software](http://www.graphviz.org/)
* [gravzio uml markdown](http://gravizo.com)
#### Markdown
[webstorm idea-markdown wiki](https://github.com/vsch/idea-multimarkdown/wiki/Adding-a-Table-of-Contents) 
#### Webstorm
[Jet Brains Webstorm Javascript IDE](https://www.jetbrains.com/webstorm/) 
##### gravzio - directed graph example 
![Alt text](http://g.gravizo.com/g?
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

#### sequence diagram example

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

### Scource Code Management
#### Git
#### Github
[A better git log](https://coderwall.com/p/euwpig/a-better-git-log) 

# DevOps
## Docker
* [Docker Storage Introduction](https://deis.com/blog/2016/docker-storage-introduction/?mkt_tok=eyJpIjoiTXpNNU1tUXhZVGRrTXpnNSIsInQiOiJreDk2b0h3TDJmcjBEcjVsOXZVMUl4dXd2RGFcL0pKWUFnWkcwUFZDbEFYYU56QWhnaTlsUXpDMDVEQ1R2TCt4R2N3Z0tnaFFUMERlQWVXNGo2elQwWUpRVnVTS1NcLzkrS1A0Q3FvTGZNeVNVPSJ9)
* [Auto Scaling with Docker](https://botleg.com/stories/auto-scaling-with-docker/?mkt_tok=eyJpIjoiTXpNNU1tUXhZVGRrTXpnNSIsInQiOiJreDk2b0h3TDJmcjBEcjVsOXZVMUl4dXd2RGFcL0pKWUFnWkcwUFZDbEFYYU56QWhnaTlsUXpDMDVEQ1R2TCt4R2N3Z0tnaFFUMERlQWVXNGo2elQwWUpRVnVTS1NcLzkrS1A0Q3FvTGZNeVNVPSJ9) 

# Philosophy
* [Nick Bostrom on the Simulation Argument](http://philosophybites.com/2011/08/nick-bostrom-on-the-simulation-argument.html) 

* <a href="#toc">back to Table of Contents</a> 