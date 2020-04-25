# class-readings-13-github.io

When is Basic Authorization used vs. Bearer Authorization?
Basic Authorization can be used but not very secure.If we want to make the authentication extra secure we can 
use Bearer Authentication.The Bearer authentication scheme is dedicated to the authentication using a token where
as  Basic Authentication schemes are dedicated to the authentication using a username and a secret.

What does the JSON Web Token package do?
While there are many encryption methods out there, a common way to generate tokens is to use the JSON Web Token (JWT) standard. 
This standard defines a compact and self-contained way to securely transmit information between two systems (servers, clients, etc.)
as a JSON object. This information can be verified and trusted because it is “digitally signed”. 
This signing process uses a secret key that only the server knows.

What considerations should we make when creating and storing a SECRET?
We should not store any password or secret in jwt as it might get cracked
