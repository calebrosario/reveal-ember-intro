##  Route Hooks

```
// Taken from "Meet Ember.js; Not just another framework"
// http://miguelcamba.com/talks/meet-ember-js/#/19
App.MessagesRoute = Ember.Router.extend({
  activate: function(){
    /* Hook called when entering the route. */
  },
  redirect: function(){
    /* Hook for redirect to another route right away. */
  },
  beforeModel: function(transition){
    /* Hook usefull to perform any async operation needed before loading the model. */
  },
  model: function(params, transition){
    /* Hook to fetch/build the content of the route's controller. */
  },
  afterModel: function(resolvedModel, transition){
    /* Hook to perform any operation with the model before it is injected in the controller. */
  },
  setupController: function(controller, model){
    /* By default, injected the given model in the given controller. */
  },
  renderTemplate: function(controller, model){
    /* By default renders the route's template with the route's controller as context. */
  },
  deactivate: function(){
    /* Hook for perform any teardown if needed. */
  }
});
```
NOTE:
activate: ()
* Hook called when entering the route.

redirect: ()
* Hook for redirect to another route right away.

beforeModel: (transition)
* Hook usefull to perform any async operation needed before loading the model.

model: (params, transition)
* Hook to fetch/build the content of the route's controller.

afterModel: (resolvedModel, transition)
* Hook to perform any operation with the model before it is injected in the controller.

setupController: (controller, model)
* By default, injected the given model in the given controller.

renderTemplate: (controller, model)
* By default renders the route's template with the route's controller as context.

deactivate: ()
* Hook for perform any teardown if needed.
