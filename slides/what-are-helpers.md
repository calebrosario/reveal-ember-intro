##  What are Helpers

Custom Handlebars helpers are one of the ways that you can use the same HTML multiple times in your web application. Registering your custom helper allows it to be invoked from any of your Handlebars templates. Custom helpers are located under app/helpers.


NOTE:
input helpers:
The {{input}} and {{textarea}} helpers in Ember.js are the easiest way to create common form controls. 
The {{input}} helper wraps the built-in Ember.TextField and Ember.Checkbox views, while {{textarea}} wraps Ember.TextArea. 
Using these helpers, you can create these views with declarations almost identical to how you'd create a traditional <\input>\ or <\textarea>\ element.


dev helpers:
The {{log}} helper makes it easy to output variables or expressions in the current rendering context into your browser's console.

The {{debugger}} helper provides a handlebars equivalent to JavaScript's debugger keyword. 
It will halt execution inside the debugger helper and give you the ability to inspect the current rendering context.


Just before the helper is invoked two useful variables are defined:

templateContext: The current context that variables are fetched from. This is likely a controller.
typeOfTemplateContext: A string describing what the templateContext is.
For example, if you are wondering why a specific variable isn't displaying in your template, you could use the {{debugger}} helper. When the breakpoint is hit, you can use the templateContext in your console to lookup properties:


```templateContext.get('name')```