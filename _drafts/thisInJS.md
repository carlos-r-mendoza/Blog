In JavaScript, context is everything.

JavaScript has a special keyword to grant access to a specific context.

The "this" keyword can be uses to access values, methods, and objects on a context specific basis. 

"This" changes where it is used. 


Different application context. 

4 Ways that "this" takes a value
1. In normal function calls
2. Within methods on objects
3. Within an object that has been constructed
4. A function invoked with .call, .apply, or bind

1. In a normal function call
function helloWorld() {
	console.log("Hello world");
	console.log(this); // the Global context // In a browser, it is the Window object
}

helloWorld();

2. Within methods on object (one of the most powerful ways to use this)

var Portland = {
	bridges: 12,
	airport: 1,
	soccerTeams: 1,
	logNumberOfBridges: function() {
		console.log("There are " + this.bridges + " bridges in Portland")
	}
}

function logTeams() {
	console.log(this.soccerTeams)
}

Portland.foo = logTeams;
Portland.foo();


3. Within an object that has been constructed
// when we use a constructor function to create a new object, the keyword 'this' will refer to the object that is created not the constructor function.
// It is the most powerful because it allows code to be very reusable/ highly replicable code

var City = function(name, state) {
	// the instance will be either value
	// corresponds to the object instance itself
	this.name = name || 'Portland';
	this.state = state || 'Oregon';
	this.printMyCityAndState = function() {
		console.log('My city is ' + this.name + ' and my state is ' + this.state)
	}
}

portland = new City();
seattle = new City('Seattler', 'Washington');
seattle.printMyCityAndState();

console.log(portland);
console.log(seattle);


4. Apply, Bind,

Apply - the apply method lets us construct an array of arguments to use to invoke a function. It also lets us choose the value of this. The apply method takes two parameters. The first is the value that should be bound to this. The second is an array of parameters.

var array = [3, 4];
var sum = add.apply(null, array); // sum is 7

//make object with status member

Quo.prototype.get_status = function() {
	return this.status;
}

var statusObject = {
	status: 'A-OK'
}

// statusObject does not inherit from Quo.prototype
//but we can invoke the get_status method on
// statusObject even though statusObject does not have
// a get_status method


var status. Quo.prototype.get_statys.apply(statusObject);
//status is A-OK