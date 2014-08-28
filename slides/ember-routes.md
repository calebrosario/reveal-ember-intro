##  Ember Routes

* Responsible for deserializing the url into an application model.
* Connects the controller to the model and handles template rendering.
* Communication with application backend typically happens in Routes.

NOTE:
In Ember.js, each of the possible states in your application is represented by a URL. Because all of the questions we asked above— Are we logged in? What post are we looking at? —are encapsulated by route handlers for the URLs, answering them is both simple and accurate.

At any given time, your application has one or more active route handlers. The active handlers can change for one of two reasons:

The user interacted with a view, which generated an event that caused the URL to change.
The user changed the URL manually (e.g., via the back button), or the page was loaded for the first time.
When the current URL changes, the newly active route handlers may do one or more of the following:

Conditionally redirect to a new URL.
Update a controller so that it represents a particular model.
Change the template on screen, or place a new template into an existing outlet.