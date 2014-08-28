##  Create a Model


Ember Object Model

####Original
```
//Create Todo Model
App.Todo = Ember.Object.extend();
```

Ember-Data Model

####Ember-Data Module with Data Store
```
App.Todo = DS.Model.extend(
  title: DS.attr('string'),
  isCompleted: DS.attr('boolean')
);
```

Ember-CLI Generator

####Ember-Data & generates test as well
```
ember generate model todo title:string isCompleted:boolean
```
