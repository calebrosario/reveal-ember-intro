##  Ember Router

 
```
App.Router.map(
	this.resource('todos', function() {  // http://localhost/todos/ 
		this.route('create');  // http://localhost/todos/create/
		this.route('show');  // http://localhost/todos/show/
		this.route('edit');  // http://localhost/todos/edit/
		this.route('destroy');  // http://localhost/todos/destroy/
	});
);
```
Basic CRUD Todos App Maps all Routes
