# Event Handlers

Getting data in event handlers - Inside the event handlers, `this` refers to an individual task object. In a collection, every inserted document has a unique `_id` field that can be used to refer to that specific document. We can get the `_id` of the current task with `this._id`.

For example, Once we have the `_id`, we can use `update` and `remove` to modify the relevant task.

###Pre-defined Functions

`update` function on a collection takes two arguments:
+ The first is a selector that identifies a subset of the collection
+ The second is an update parameter that specifies what should be done to the matched objects.

`remove` function takes one argument:
+ a selector that determines which item to remove from the collection.
