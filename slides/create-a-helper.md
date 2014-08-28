##  Create a Helper

####Original
```
Ember.Handlebars.helper('highlight', function(value, options) {
  var escaped = Handlebars.Utils.escapeExpression(value);
  return new Ember.Handlebars.SafeString('<span class="highlight">' + escaped + '</span>');
});
```

####Ember-CLI Generator

```
ember generate helper highlight
```
