##  Ember Models

```
App.Todo = DS.Model.extend();
```
A model is a class that defines the properties and behavior of the data that you present to the user. Anything that the user expects to see if they leave your app and come back later (or if they refresh the page) should be represented by a model.

NOTE:
Object's representing persistent application state. 
Land of Ember Data. Ember Data isn't necessary to build an Ember App. 
Rolling your own persistence layer is fairly simple. Big topic; different talk.

After you have defined a model class, you can start finding and creating records of that type. When interacting with the store, you will need to specify a record's type using the model name. For example, the store's find() method expects a string as the first argument to tell it what type of record to find.

DS.attr takes an optional hash as a second parameter:

defaultValue: Pass a string or a function to be called to set the attribute to a default value if none is supplied.