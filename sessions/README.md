# Sessions
Session is a temporary reactive state. We can use the `Session` function to store temporary reactive state on the client.

In Metero, Session is a reactive data store for the client.

Until now, we have stored all of our state in collections, and the view updated automatically when we modified the data inside these collections. This is because `Meteor.Collection` is recognized by Meteor as a reactive data source, meaning Meteor knows when the data inside has changed.

`Session` is the same way, but is not synced with the server like collections are. This makes `Session` a convenient place to store temporary UI state like the checkbox above. Just like with collections, we don't have to write any extra code for the template to update when the Session variable changes — just calling `Session.get(...)` inside the helper is enough.
