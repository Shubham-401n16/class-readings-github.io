# class-readings-02-github.io

What is a benefit to using express.Router()?

Router is used to create modular, mountable route handlers.

When I say that top-down order matters in Express, what does that mean?

Express executes code from top to bottom. This means that even though Application Middleware is 
typically meant to be run before Handler Middleware, we can change this by moving
an Application Middleware assignment after a Handler Middleware assignment.

Why do we use a model class (with create(), read(), etc.) 
instead of directly calling MongoDB operations (such as save(), find(), etc.) within our Express route handlers?

When running the handler middleware, there is a strong likelyhood that some data operation needs to take place. 
The handler function kicks off this asynchronous data operation by calling a model function such as create(), read(), update() or delete(). This refers to a model class built in a /models folder, utilizing a schema also defined in the /models folder. The handler then awaits this data operation to complete
The model executes CRUD functions themselves by calling MongoDB specific commands such as save(), find(), etc. 
This triggers the Mongoose schema to be called.
