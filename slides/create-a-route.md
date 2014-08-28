##  Create a Route

All transitions and redirects should happen here

####Original
```
App.TodoRoute = Ember.Route.extend(
	beforeModel: function() {
		this._super(transition);
		if (this.get('session.isAuthenticated')) {
			this.transitionTo('campaigns.all');
		}
	},
	model: function(params) {
		return this.store('todos', params.todo_id);  //returns a promise that resolves to the TODOs Records from the Data Store
	},
	afterModel: function() {

	},
	setupController: function(controller, model) {
    	controller.set('model', model);
    }
);
```


####Ember-CLI Generator
```
ember generate route todo 
```




