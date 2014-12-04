# Collections

Collections are Meteor's way of storing persistent data. The special thing about collections in Meteor is that they can be accessed from both the server and the client, making it easy to write view logic without having to write a lot of server code. They also update themselves automatically, so a template backed by a collection will automatically display the most up-to-date data.

Collections are like _tables_ in Ruby on Rails/SQL.

Creating a new collection is as easy as calling `MyCollection = new Mongo.Collection("my-collection")`. On the server, this sets up a MongoDB collection called `my-collection`; on the client, this creates a cache connected to the server collection.
