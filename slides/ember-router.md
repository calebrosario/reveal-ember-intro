##  Ember Router


* A state machine/statechart for your whole application.
* The URL is a serialized representation of the application's state.
* When the app is first loaded, the Router uses the information contained in the URL to build the state of the application.
 
```
App.Router.map(
	this.resource('todos', function() {  
		//this.route('index'); // http://localhost/todos/ This is default
		this.route('create');  // http://localhost/todos/create/
		this.route('show');  // http://localhost/todos/show/
		this.route('edit');  // http://localhost/todos/edit/
		this.route('destroy');  // http://localhost/todos/destroy/
	});
);
```
Basic CRUD Todos App Maps all Routes

NOTE:
When your application starts, the router is responsible for displaying templates, loading data, and otherwise setting up application state. 
It does so by matching the current URL to the routes that you've defined.

The map method of your Ember application's router can be invoked to define URL mappings. 
When calling map, you should pass a function that will be invoked with the value this set to an object which you can use to create routes and resources.

You can define groups of routes that work with a resource: