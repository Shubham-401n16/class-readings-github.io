class-readings-31-github.io

Reference -

https://redux.js.org/api/combinereducers/
https://redux.js.org/recipes/structuring-reducers/using-combinereducers/

Core Concepts
The most common state shape for a Redux app is a plain Javascript object containing "slices" of 
domain-specific data at each top-level key. Similarly, the most common approach to writing reducer
logic for that state shape is to have "slice reducer" functions, each with the same (state, action) 
signature, and each responsible for managing all updates to that specific slice of state. 
Multiple slice reducers can respond to the same action, independently update their own slice as needed, 
and the updated slices are combined into the new state object.

combineReducers is simply a utility function to simplify the most common use case when writing Redux reducers.

There are two ways to define the initial shape and contents of your store's state. 
1. First, the createStore function can take preloadedState as its second argument. 
This is primarily intended for initializing the store with state that was previously persisted elsewhere, such as the browser's localStorage. 

2. The other way is for the root reducer to return the initial state value when the state argument is undefined. 
These two approaches are described in more detail in Initializing State, but there are some additional concerns to be aware of when using combineReducers.

Example

rootReducer = combineReducers({potato: potatoReducer, tomato: tomatoReducer})
// This would produce the following state object
{
  potato: {
    // ... potatoes, and other state managed by the potatoReducer ...
  },
  tomato: {
    // ... tomatoes, and other state managed by the tomatoReducer, maybe some nice sauce? ...
  }
}
