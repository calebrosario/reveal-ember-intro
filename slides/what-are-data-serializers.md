##  What are data serializers

```
App.ApplicationSerializer = DS.RESTSerializer.extend({
  keyForAttribute: function(attr) {
    return Ember.String.underscore(attr).toUpperCase();
  }
});
```

A serializer is responsible for turning a raw JSON payload returned from your server into a record object.

NOTE:
A serializer is responsible for turning a raw JSON payload returned from your server into a record object.

JSON APIs may represent attributes and relationships in many different ways. For example, some attribute names may be camelCased and others may be under_scored. Representing relationships is even more diverse: they may be encoded as an array of IDs, an array of embedded objects, or as foreign keys.

When the adapter gets a payload back for a particular record, it will give that payload to the serializer to normalize into the form that Ember Data is expecting.

While most people will use a serializer for normalizing JSON, because Ember Data treats these payloads as opaque objects, there's no reason they couldn't be binary data stored in a Blob or ArrayBuffer.