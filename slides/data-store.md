##  Data Store

```
App.Store = DS.Store.extend();
```
```DS.Store ``` is created for you automatically and is shared among all controllers and routes in your application.

Note:
All data is retrieved from this centralized source.
This also maintains the cache of the data, along with any updates. 
Routes and Controllers are only allowed to request data from the store. 
Store returns a promise. 
Using an Identity Map, this can keep all records in sync for you. no need to do it manually. 
Using an identity map is important because it ensures that changes you make in one part of your UI are propagated to other parts of the UI.
 It also means that you don't have to manually keep records in sync—you can ask for a record by ID and not have to worry about whether other parts of your application have already asked for and loaded it.

The store is the central repository of records in your application. 
You can think of the store as a cache of all of the records available in your app. 
Both your application's controllers and routes have access to this shared store; when they need to display or modify a record, they will first ask the store for it.