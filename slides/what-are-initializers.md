##  What are initializers

Initializers are tools for performing tasks that are needed to get your App ready to run. Here’s a list of possible use cases:

* Injecting the current user into all Routes and Controllers
* Setting up other Javascript libraries, like Socket.io
* Reading environment configuration data
* Setting a CSRF token to be used on all Ajax requests
* Pre-loading records written to the HTML DOM into the Store for faster initial loading.

NOTE:

As you can see, the Initializer is passed both the container and application instance. 
This allows you to look up things you will most likely want to use, like the Adapter or Store:

You could also look up or set variables on your Application instance. 
For example, assuming you had run the environment config reader from the previous post first, in subsequent Initializers you can look up those environment variables.

Asynchronous Initializers
If your Initializer performs a record lookup, then it’s vital that the Initializer simply doesn’t proceed allowing other Initializers to execute until that record lookup is fulfilled. 
You can tell Ember not to boot up the Application and start routing by utilizing the deferReadiness and advanceReadiness methods on the Application instanced passed to the Initializer.

For example, here’s an Initializer that looks up the Current user from the store, and injects it into the container, making it easily available in Routes and Controllers.