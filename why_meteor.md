#Why Meteor?
These principles will help outline whats so amazeballs about Meteor.

####The 7 Principles of Meteor:

1. Data on the Wire
2. One Language
3. Database Everywhere
4. Latency Compensation
5. Full Stack Reactivity
6. Embrace the Ecosystem
7. Simplicity Equals Productivity

#####I. Data on the Wire
Rather than send full payloads of html, everything is JSON back and forth between client and server.

#####II. One Language
Just Javascript

#####III. Database Everywhere
MongoDB is fully integrated with Meteor. There are more choices and intergrations to come.

There is a miniMongo database that runs on the
client side, so you have some local storage that keeps collections of data locally. So we're not making trips to the server every time.

There are controls in Meteor for when you want to go to the server, and when you just want to work locally with client data that you already have. This means you don't have to waste any time and effort.

#####IV. Latency Compensation
This is super slick stuff! Data is first saved locally (to the browser) and dislayed to user. So it seems to the user rapidly fast.

In other traditional web technologies, it goes to the server, it churns and churns and thats how we've got big server farms.

In Meteor, data saves in the browser first, then it does async back to the server and saves it there when it, when it can. This makes your app usually pretty quick and slick, as this all happens in the background.

#####V. Full Stack Reactivity

Components throughout Meteor, actually are reactive automatically, because of the relationship that Meteor has, Meteor-core has with the database and with all the other socket connections that are being made across the internet.

_For example_, if I'm looking at a list of blog posts and somebody somewhere else in the world makes a change or edits the title, and I'm on a page where that title is that title immediately updates. Immediate means by the time it makes the trip across clients. I don't have to refresh the page; it just happens right there in the browser, which is awesome!

#####VI. Embrace the Ecosystem
Instead of trying to say "Hey, my kung-fu is so good and I can write all of this stuff myself. I don't need Underscore. I don't need JQuery. You know, I don't need all of these other tools."

Meteor is saying "Hey, if there's tools out there that exist, we're gonna pull them in. We're gonna use them as needed and we're not gonna rewrite 'em.

It already includes: node.js, mongoDB, jQuery, underscore.js.

The "ecosystem" also refers to the to the package system.
There are already 2,000 packages out there!


#####VII. Simplicity Equals Productivity
Some folks remember what it is was like at the beginning of the Rails framework revolution, where the reason people fell in love with Rails was because it was so easy to build the web application at that time you know.

Rails has matured and things are, things can get a little more complicated and Rails apps can get more complicated.

With Meteor, they're trying to recapture that simplicity,  but also keep that simplicity throughout the project as it matures. This also makes Meteor accessible to people learning to develop web applications.

