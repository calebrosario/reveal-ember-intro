##  convention over configuration


```
//Create Application with App Namespace
var App = Ember.Application.create();

//Create Todo Model
App.Todo = Ember.Object.extend(); // or App.Todo = DS.Model.extend();

//Create Todo View
App.TodoView = Ember.View.extend();

//Create Todo Controller
App.TodoController = Ember.Controller.extend();

//Create Todo Route
App.TodoRoute = Ember.Route.extend();

App.Router.map(
	this.route('todos');
);

```
