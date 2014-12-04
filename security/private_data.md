# Private Data

First, we can add another property to tasks called "private" and a button for users to mark a task as private. This button should only show up for the owner of a task. It will display the current state of the item.

[See Meteor Try](https://www.meteor.com/try/11)

To test that this functionality works, you can use your browser's private browsing mode to log in as a different user. Put the two windows side by side and mark a task private to confirm that the other user can't see it. Now make it public again and it will reappear!

In order to finish up our private task feature, we need to add checks to our deleteTask and setChecked methods to make sure only the task owner can delete or check off a private task:

We're done with our private task feature! Now our app is secure from attackers trying to view or modify someone's private tasks.
