# Filtering Subscribed Data

Now that we have moved all of our app's sensitive code into methods, we need to learn about the other half of Meteor's security story. Until now, we have worked assuming the entire database is present on the client, meaning if we call `Tasks.find()` we will get every task in the collection. That's not good if users of our application want to store privacy-sensitive data. We need a way of controlling which data Meteor sends to the client-side database.

Just like with insecure in the last step, all new Meteor apps start with the autopublish package. Let's remove it:

```unix
meteor remove autopublish
```

When the app refreshes, the task list will be empty. Without the autopublish package, we will have to specify explicitly what the server sends to the client. The functions in Meteor that do this are `Meteor.publish` and `Meteor.subscribe`.
