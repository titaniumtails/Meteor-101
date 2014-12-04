# Helpers

Helpers allow you to add logic and data to templates.
You can pass data into templates from your JavaScript code by defining **helpers**.

For example, `Template.body.helpers`

A longer example:
```javascript
Template.body.helpers({
  tasks: function () {
    // Show newest tasks first
    return Tasks.find({}, {sort: {createdAt: -1}});
  }
});
```
