# class-readings-18-github.io

What does it mean that web sockets are bidirectional? Why is this useful?

Bidirectional means data can flow both ways. 

It allows web sockets remain connected during their lifetime, and they are really well suited for real-time data transfer over the web.
Does socket.io use HTTP? Why?

It uses  HTTP as it keeps that the connection active.

What happens when a client emits an event? What happens when a server emits an event?

When client emits it goes to the server and when a server emits an event it reaches to all clients connected to the server.
