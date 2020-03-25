# class-readings-02-github.io

What makes an interface useful?
An interface makes it easier to enact more complex operations.

Why is middleware called middleware?

Middleware typically means “software between two other softwares”.More of  a 
middleman between two operations that helps the process go more smoothly.


Fundamentally, what does it mean to have a mock of something? Why is this useful?

Testing can be a challenge with databases, since we don’t ever want to modify our actual 
database when we run our tests. Due to this reason when testing databases, we usually create a 
fake or “mock” database to run our tests upon.
This is useful in testing our operations and not modify any real data.


What does it mean to have a mock database?

This mock database has the same structure as our application database. 
It has the same data models and commands. 
The only difference is that this mock database only exists during the lifetime of the test: 
it is created and initialized when we start our tests and deleted when tests are complete. 
We give this mock database some dummy data to initialize with as well, and thus we can be
confident that any secure and application related data is not messed with when testing.

