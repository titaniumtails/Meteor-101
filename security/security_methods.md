# Defining Security Methods

First, we need define some methods. We need one method for each database operation we want to perform on the client.

Methods should be defined in code that is executed on the client and the server, We do this to enable a feature called **[Latency compensation]()**.

Our client code is now more separated from our database logic. Instead of a lot of stuff happening inside our event handlers, we now have methods that can be called from anywhere.
