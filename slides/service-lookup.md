##  Service Lookup

```
var App = Ember.Application.create();

App.SessionController = Ember.Controller.extend({
  isAuthenticated: false
});

// The index controller may need access to that state:
App.IndexController = Ember.Controller.extend({
  needs: ['session'],
  // Using needs, the controller instance will be available on `controllers`
  isLoggedIn: Ember.computed.alias('controllers.session.isAuthenticated')
});
```
