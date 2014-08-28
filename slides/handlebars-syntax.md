##  Handlebars Syntax


```
{{#with person as user}}
  {{#each book in books}}
    {{user.firstName}} has read {{book.name}}!
  {{/each}}
{{/with}}

```
NOTE:

 {{#with}} changes the context of the block you pass to it. The context, by default, is the template's controller. By using the {{#with}} helper, you can change the context of all of the Handlebars expressions contained inside the block.

it's possible to store the context within a variable for nested usage using the "as" keyword: