# Event Listeners
Event listeners are added to templates in much the same way as helpers are: by calling `Template.templateName.events(...)`.

The keys - describe the event to listen for
The values - are event handlers that are called when the event happens.

```javascript
Template.body.events({
  "submit .new-task": function (event) {
    // This function is called when the new task form is submitted

    var text = event.target.text.value;

    // Clear form
    event.target.text.value = "";

    // Prevent default form submit
    return false;
  }
});
```

Here we are listening to the `submit` event on any element that matches the CSS selector `.new-task`. When this event is triggered by the user pressing enter inside the input field, our event handler function is called.

The event handler gets an argument called `event` that has some information about the event that was triggered. In this case `event.target` is our form element, and we can get the value of our input with `event.target.text.value`. You can see all of the other properties of the `event` object by adding a `console.log(event)` and inspecting the object in your browser console.

The last two lines of our event handler perform some cleanup — first we make sure to make the input blank, and then we return `false` to tell the web browser to not do the default form submit action since we have already handled it.
