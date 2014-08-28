##  What are Records

```
var records = this.store.find('todos');
```
A record is an instance of a model that contains data loaded from a server. Your application can also create new records and save them back to the server.

NOTE:
A record is an instance of a model that contains data loaded from a server. Your application can also create new records and save them back to the server.

A record is uniquely identified by its model type and id.

IDs are usually assigned by the server when you save them for the first time, but you can also generate IDs client-side.

Suggest against assigning IDs clientside.