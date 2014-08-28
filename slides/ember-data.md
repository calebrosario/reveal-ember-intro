##  Ember Data

![picture of Ember-Data sketch](images/assets/ember-data-sketch.png)

###Moving Parts

| Data Store | Records | Adapters | Serializers |


NOTE:
Ember Data is also designed to work with streaming APIs like socket.io, Firebase, or WebSockets. 
You can open a socket to your server and push changes to records into the store whenever they occur.

Without any configuration, Ember Data can load and save records and their relationships served via a RESTful JSON API, provided it follows certain conventions.