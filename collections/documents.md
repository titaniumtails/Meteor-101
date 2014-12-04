# Documents
Items inside collections are called **documents**. This is like a _row_ in Ruby on Rails/SQL

You can access the database:
```unix
meteor mongo
```

This opens a console into your app's local development database. You can type:
```unix
db.tasks.insert({ text: "Hello world!", createdAt: new Date() });
```

In your web browser, you will see the UI of your app immediately update to show the new task. You can see that we didn't have to write any code to connect the server-side database to our front-end code — it just happened automatically.
