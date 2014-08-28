##  Dependency Injection

####Original
```
App = Ember.Application.extend();
App.Logger = Ember.Object.extend({
  log: function(m){ console.log(m); }
});
App.IndexRoute = Ember.Route.extend({
  activate: function(){
    // The logger property is injected into all routes
    this.logger.log('Entered the index route!');
  }
});

Ember.Application.initializer({
  name: 'logger',
  initialize: function(container, application){
    application.register('logger:main', App.Logger);
    application.inject('route', 'logger', 'logger:main');
  }
});

App.create();
```

####Ember-CLI Generator

```
import Logger from '/path/to/my/logger';

export default {
  name: 'logger',
  initialize: function(container, application){
    application.register('logger:main', Logger);
    application.inject('route', 'logger', 'logger:main');
  }
};
```
