# class-readings-29-github.io

Why would you wrap your entire application within a context?

It makes it easier to share methods between parent and child components

What is the purpose of a reducer?

Reducer functions are used to update state of redux store

What does an action contain?

Type and payload

Why do we need to copy the state in a reducer?

A reducer’s purpose is to take in the current state and an action, 
and then determine how to modify the state based on the action. 
This is why it is common to begin each reducer function with copying the current 
state and then running a switch statement based on the type of action. 
