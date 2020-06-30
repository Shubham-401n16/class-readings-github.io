# class-readings-28-github.io

[Further Reading](https://github.com/diegohaz/awesome-react-context)

When to Use Context
Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

Before You Use Context
Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.

API
React.createContext
const MyContext = React.createContext(defaultValue);
Creates a Context object. When React renders a component that subscribes to this Context 
object it will read the current context value from the closest matching Provider above it in the tree.

The defaultValue argument is only used when a component does not have a matching Provider above it in the tree. 
This can be helpful for testing components in isolation without wrapping them. Note: passing undefined as a Provider
value does not cause consuming components to use defaultValue.

Context.Provider
<MyContext.Provider value={/* some value */}>

The contextType property on a class can be assigned a Context object created by React.createContext(). 
This lets you consume the nearest current value of that Context type using this.context. 
You can reference this in any of the lifecycle methods including the render function.

Context.Consumer
<MyContext.Consumer>
  {value => /* render something based on the context value */}
</MyContext.Consumer>

Context.displayName
Context object accepts a displayName string property. 
React DevTools uses this string to determine what to display for the context.

