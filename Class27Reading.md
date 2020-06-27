# class-readings-27-github.io

Why do custom hooks need the use prefix?

By adding the word use to the beginning, it lets us know that this function follows the rules of Hooks.
As React will treat this function differently, allowing the function to return a stateful variable. 
We don’t need to ever set the value of the stateful variable in our App component, so we only receive the getter and not the setter. 
This drasitically simplifies our component code!

What do custom hooks usually do?

Custom hooks can be very useful because we can create module files that export various hook functions for you to use anywhere in our application.

Using the links above, list one custom hook that you would be interested in trying/using.

I will probably use react-use-form-state hook.
react-use-form-state is a small React Hook that attempts to simplify managing form state, using the native form input elements you are familiar with.
