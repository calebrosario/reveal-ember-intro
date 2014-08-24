##  What are data serializers

```
App.ApplicationSerializer = DS.RESTSerializer.extend({
  keyForAttribute: function(attr) {
    return Ember.String.underscore(attr).toUpperCase();
  }
});
```

A serializer is responsible for turning a raw JSON payload returned from your server into a record object.
