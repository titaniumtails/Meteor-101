# Routing
Not included with Meteor. Its used because of convention, and people want to structure.


```unix
meteor add iron:router
```

Iron Router helps with:
1) Setting up paths
2) Assigning actions
3) Control access rights to database

Route templates - each route needs to point to a template. Routes will look for templates with the same name if we don’t specify.

```javascript
Router.configure({
  layoutTemplate: 'layout',
  loadingTemplate: 'loading',
  notFoundTemplate: 'notFound',
  waitOn: function() { return Meteor.subscribe('posts'); }
});

Router.route('/', {name: 'postsList'});
Router.route('/posts/:_id', {
  name: 'postPage',
  data: function() { return Posts.findOne(this.params._id); }
});

Router.onBeforeAction('dataNotFound', {only: 'postPage'});
```

Javascript notes:
Parenthesis cal a function. Whatever is inside them is an argument.

Braces - means its an object. With key value pairs inside. Separated by commas. Order doesn't matter within thekey value pairs, because you are accessing it by its keys. Commas are a must to separate pairs, but not for the last one.

