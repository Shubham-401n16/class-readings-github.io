
What does protocol mean?

A protocol is a set of rules that must be followed. 
HTTP was developed as a way for clients and servers to interact over the web in a consistent way.

How does any web browser understand how to open any webpage?
The url (often called endpoint) specifies which server (and what part of that server) to direct the request to.

Name one thing a request object must have, and one thing a response object must have
 A request must have request headers and a response must have a status code.

What is the difference between HTTP and REST?

HTTP puts rules upon this transfer process, dictating how a request and response should look like. 
HTTP is a set of schema for request and response objects, ensuring that anyone using HTTP follows that schema. 
These schema specify required and optional fields, and utilize some standard enumerated values that HTTP defines.
Whereas the REST guidelines dictate how to format a server’s APIs so that a client can access all the methods / functionality they need.


Why is REST important?
REST is just a collection of guidelines and there is no enforced limitation on how API should be structured.
It is encouraged to use REST guidelines when building APIs, so that various servers can have some sense of consistency. 
If every API adopts the same standards, it makes it easier for clients to understand how to use our API.
