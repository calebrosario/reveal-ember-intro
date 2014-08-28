##  What is a resolver

The Ember resolver plays a huge role when unit testing your application. It provides the lookup functionality based on name, such as ```route:index``` or ```model:post```.

```
import Ember from 'ember';
import Resolver from 'ember/resolver';
import loadInitializers from 'ember/load-initializers';

Ember.MODEL_FACTORY_INJECTIONS = true;

var App = Ember.Application.extend({
  Resolver: Resolver
});

loadInitializers(App, 'todos');

export default App;
```

Using the custom resolver, Ember CLI applications have similar abilities, but using ES6 modules instead of a global namespace.
