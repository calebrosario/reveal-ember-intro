##  What are data adapters

```

App.TodoAdapter = DS.RESTAdapter.extend({
	namespace: 'api/v1'
	}); 
//App.TodoAdapter = DS.FixtureAdapter.extend();
```
 The logic for communicating with a backend data store lives in the Adapter.

NOTE:
An adapter is an object that knows about your particular server backend and is responsible for translating requests for and changes to records into the appropriate calls to your server.

DS.Adapter: 
Is the basic adapter with no functionality. It is generally a good starting point if you want to create an adapter that is radically different from the other Ember adapters.

DS.FixtureAdapter: 
Is an adapter that loads records from memory. Its primarily used for development and testing.

DS.RESTAdapter: 
Is the most commonly extended adapter. The RESTAdapter allows your store to communicate with an HTTP server by transmitting JSON via XHR. Most Ember.js apps that consume a JSON API should use the REST adapter.

DS.ActiveModelAdapter: 
Is a specialized version of the RESTAdapter that is set up to work out of the box with Rails-style REST APIs.