# Latency Compensation

When you call a method on the client using `Meteor.call`, two things happen in parallel:

1. The client sends a request to the server to run the method in a secure environment, just like an AJAX request would work

2. A simulation of the method runs directly on the client to attempt to predict the outcome of the server call using the available information

What this means is that a newly created task actually appears on the screen before the result comes back from the server.

If the result from the server comes back and is consistent with the simulation on the client, everything remains as is. If the result on the server is different from the result of the simulation on the client, the UI is patched to reflect the actual state of the server.

With Meteor methods and latency compensation, you get the best of both worlds — the security of server code and no round-trip delay.
