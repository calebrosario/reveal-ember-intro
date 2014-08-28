##  Create an Initializer


####Original
```
Ember.Application.initializer({
  name: "configMyApp",
  before: "websocketInit",
 
  initialize: function(container, application) {
    ... your code ...
  }
});
 
Ember.Application.initializer({
  name: "websocketInit",
  after: "configMyApp",
 
  initialize: function(container, application) {
    ... your code ...
  }
});
```

####Ember-CLI Generator
```
ember generate initalizer configMyApp

ember generate initalizer websocketInit 
```