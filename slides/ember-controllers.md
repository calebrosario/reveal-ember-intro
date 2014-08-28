##  Ember Controllers

![picture of controller sketch](images/assets/controller.png)

In Ember.js, controllers allow you to decorate your models with display logic. In general, your models will have properties that are saved to the server, while controllers will have properties that your app does not need to save to the server.

NOTE:
Contains non-persistent application state. (state that is derived from persistent state and user interaction) 
Singleton objects whose creation and destruction is managed by Ember. 

Can act as a proxy to a model object (ObjectController, ArrayController). 
Serves as a communication channel between different areas of the application (controller's can gain references to each other through dependency injection).

*They can end up doing A LOT. In my first Ember app, the majority of the code and application complexity resided in controllers.