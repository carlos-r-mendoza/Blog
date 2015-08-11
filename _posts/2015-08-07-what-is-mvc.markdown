---
layout: post
title:  "What is Model-View-Controller (MVC)?"
date:   2015-08-07 14:45:00
categories: Model-View-Controller MVC
author: Carlos R. Mendoza
<!-- permalink: -->
---

*Last Update on Aug 11, 2015.*

# Separation of Concerns
Developing software applications is a complex matter. To cope with this complexity, it is important to implement *separation of concerns* when developing software. In computer science, *separation of concerns* is a key design and architecture principle for dividing a computer program into defined sections - each addressing a specific aspect of your program's functionality. The goal is to break down a program's code base into distinct sections that overlap in responsibility as little as possible as this will help make your code easier to reuse, maintain, debug, and test.

# Model-View-Controller (MVC)
The Model-View-Controller (MVC) software architectural pattern is an excellent example of *separation of concerns*. MVC calls for an application to be divided into three distinct but interconnected sections - you might have guessed it - the _**M**odel_, the _**V**iew_, and the _**C**ontroller_. 

MVC was introduced in 1979 by Trygve Reenskaug, who maintains a webpage that explains MVC from his perspective ([here](http://heim.ifi.uio.no/~trygver/themes/mvc/mvc-index.html)). MVC became widely implemented starting in the 1980s and is today one of the most utilized models of *separation of concerns*. If you are a software developer, it is likely that you have used a framework that follows MVC conventions.

# The **M**odel

Think data and the logic responsible for managing the data. The Model is responsible for responding to requests for and modifying information. The Model is independent of the user interface and often provides an API so that other parts of the programs can access it. In MVC, the Model responds to instructions received from either the View or Controller. The goals is to make the Model reusable, regardless of any changes to the user interface. 

# The **V**iew

The View is a visual representation of the Model. It is the presentation layer, the user interface. The View renders certain attributes of the Model. The information rendered on the View can come from either the Model or Controller.

# The **C**ontroller

The Controller contains logic to arrange the views on the screen. It is triggered into action when there is user input on the View. At this point the logic in the Controller attached to the input is executed, resulting in the Controller sending commands to the Model to retrieve or modify information and subsequently sending back the information received from the Model to the appropriate View. The Controller often serves as the messenger between the Model and the View.

# So, How Does MVC Work?

#### *MVC Scenario 1*
![Model-View-Controller Diagram 1](../img/what-is-mvc/mvc-diagram-1)   
<br>

The diagram above represents the traditional way of MVC implementation. The View renders certain information from the Model. This is achieved in an application in two ways: 

1. The View can *filter information* coming from the Model to display certain information. It can also *update* the Model by sending it certain commands.

2. When there is *user input* on the View, commands are executed in the Controller that then communicate with the Model to obtain information. Once the information from the Model is received, the Controller renders the correct View. In this scenario, the Controller is tightly aligned with the View, containing the logic to interpret when there is User input on the View and to retrieve and handle information from the Model so that the View can be appropriately rendered. 

#### *MVC Scenario 2*
![Model-View-Controller Diagram 2](../img/what-is-mvc/mvc-diagram-2)   
<br>

There is also another popular way to implement MVC, displayed by the diagram above. The Model and the View never directly talk to one another and the Controller handles communication between these two.

In this case, the Model and View run in isolated environments, completely independent of one another. 

# Takeaway

Keep in mind that MVC is only a paradigm for architecting the structure of a program to cope with the complexity of creating and maintaining software. It is up to the developer or team of developers to decide how the concept of MVC will be implemented.