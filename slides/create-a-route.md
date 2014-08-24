##  Create a Route

All transitions and redirects should happen here

```
App.TodoRoute = Ember.Route.extend(
	beforeModel: function() {
			this.transitionTo('todos/create');  // transitions to http://localhost/todos/create/
		}
);
```