##  Ember Routes

```
App.TodoRoute = Ember.Route.extend(
	model: function() {
			return this.store.find('todos');  // GET - all todos HTTP Req.
		}
);
```
###Hooks
| beforeModel | model | afterModel |