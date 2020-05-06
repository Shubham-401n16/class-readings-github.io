# class-readings-16-github.io

Given the examples of front-end events such as button click, window resize, form submit, etc, what are some examples of back-end events?
Back-end events will be like updating data in a database when an event has been triggered from the front end.
Why are events sometimes better than asynchronous actions with callbacks?
We can work with more than one listener

What does an EventEmitter instance do?
It allows us to both raise new events and to listen to events that have been raised.

When is a program’s call stack, event queue, and event loop active?
The call stack is part of a bigger process which runs for all applications.
Event queue holds the events that has been triggered.
The event loop takes in the event queue and run through until all events have been executed.
