What is MVC in angular?
https://www.youtube.com/watch?v=O6h4fORtfRs

Controller drives things, what will get bound ot the view
$scope is the glue


View is the presentation filter, it displays certain attributes of the model. It may also update the model by sending appropriate messages. The view may need to know the semantics of the attributes the model represents.

View should not know about the logic found in the controller. 

The controller arranges views on the screen. It provides means for user input, exectutes the logic attached in the controller to that input, and sends back the information back to the appropriate screen.


However, keep in mind that "true" MVC means that the Model contains business Logic, the Controller takes care of communicating user input to the Model, and the View gets its own data from the Model. 