##  What is a Service Lookup

When a dependency is created or fetched on demand. A common use-case for service lookup is that of a singleton service. Often, these services will live near application state, and thus Ember provides an API that makes controller services easy to write. The ```needs``` property within a controller allows access to the state of other controllers. This can also be used with the render helper within templates, allowing service lookups within the DOM.
 