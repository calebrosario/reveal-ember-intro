##  What is a Mixin

objects whose properties and functions can be shared amongst other classes and instances. This allows for an easy way to share behavior between objects as well as design objects that may need multiple inheritance.

NOTE:
Mixin class can create objects whose properties and functions can be shared amongst other classes and instances. This allows for an easy way to share behavior between objects as well as design objects that may need multiple inheritance.

Mixins are great for abstracting pieces of reusable code into smaller single responsibility objects. For larger applications this makes code easier to reason about and easier to test.

Mixins can also be applied to instances of objects at runtime. This allows for only certain objects to gain behavior.

An object can quickly be checked for the presence of a mixin using the detect function. Building off the example above.

Ember comes with many mixins available to use in any class or instance. There are mixins to deal with a very wide range of abstractions such as immutability, sorting, enumeration, and events. A full list of mixins can be found in ember-runtime.