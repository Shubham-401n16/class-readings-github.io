# class-readings-19-github.io

What is the main benefit of a message queue server?

queue server makes sure that all connected clients are up to date with the data they need. 
Subscribed clients can now “catch up” and pull down any events (or messages). they may have missed while disconnected.
If a client is offline when data is available for them, the server will wait for the appropriate client to connect before sending the data.

Why might we want to initiate messages from an HTTP request?

It is because messages are a type of events.

Is the Message Queue Server a socket.io client, a socket.io server, or an api server?
It is a socket.io server or an api server
