---
layout: post
title:  "What is Model-View-Controller (MVC)?"
date:   2015-08-07 14:45:00
categories: Model-View-Controller MVC
author: Carlos R. Mendoza
<!-- permalink: -->
---

# Separation of Concerns
Developing software applications is a complex matter. To cope with this complexity, it is important to implement *separation of concerns* when developing software. In computer science, *separation of concerns* is a key design and architecture principle for dividing a computer program into defined sections - each addressing a specific aspect of your program's functionality. The goal is to break down a program's code base into distinct sections that overlap in responsibility as little as possible as this will help make your code easier to reuse, maintain, debug, and test.

# Model-View-Controller (MVC)
The Model-View-Controller (MVC) software architectural pattern is an excellent example of *separation of concerns*. MVC calls for an application to be divided into three distinct but interconnected sections - you might have guessed it - the _**M**odel_, the _**V**iew_, and the _**C**ontroller_. 

MVC was introduced in 1979 by Trygve Reenskaug, who maintains a webpage that explains MVC from his perspective ([here](http://heim.ifi.uio.no/~trygver/themes/mvc/mvc-index.html)). MVC became widely implemented starting in the 1980s and is today one of the most utilized models of *separation of concerns*. If you are a software developer, it is likely that you have used a framework that follows MVC conventions.

# The **M**odel

Think data and the logic responsible for managing the data. The Model is responsible for responding to requests for and modifying information. The Model is independent of the user interface and often provides an API so that other parts of the programs can access it. In MVC, the Model responds to instructions received from the Controller. The goals is to make the Model reusable, regardless of any changes to the user interface. 

# The **V**iew

The View is a visual representation of the Model. It is the presentation layer, the user interface. The View renders the information received from the Controller, which communicates with the Model. When there is user input, the View sends commands to the Controller to request or modify information on the Model. 

# The **C**ontroller

The Controller contains the necessary logic to connect the Model and the View. Think of it as the messenger between the Model and the View. It contains the logic necessary to make information received from the Model presentable in the View. On the other hand, when there is user input on the View, the Controller sends commands to the Model to retrieve or modify information. 

# So, How Does MVC Work?

<br>
![Model-View-Controller Diagram](../img/what-is-mvc/what-is-mvc.png)   
<br>

The simple diagram above displays of how I like to think of MVC. The Model and the View never directly talk to one another and communication between these two is handled by the Controller.

In this case, the Model and View run in isolated environments, completely independent of one another. The Controller is tightly aligned with the View, containing the logic to interpret user input on the View and to retrieve and handle information from the Model so that the View can be appropriately rendered. 

Keep in mind that MVC is only a paradigm for architecting the structure of a program to cope with the complexity of creating and maintaining software. It is up to the developer or team of developers to decide how the concept of MVC will be implemented.