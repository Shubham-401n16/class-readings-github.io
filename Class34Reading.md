class-readings-34-github.io

Reference -

https://reactnative.dev/docs/intro-react

https://reactnative.dev/docs/tutorial


React Native is like React, but it uses native components instead of web components as building blocks.
So to understand the basic structure of a React Native app, you need to understand some of the basic React concepts,
like JSX, components, state, and props. If you already know React, you still need to learn some React-Native-specific stuff, 
like the native components. This tutorial is aimed at all audiences, whether you have React experience or not.

Hello World React native

import React from 'react';
import { Text, View } from 'react-native';

const YourApp = () => {
  return (
    <View style={{ flex: 1, justifyContent: "center", alignItems: "center" }}>
      <Text>
        Try editing me! 🎉
      </Text>
    </View>
  );
}

export default YourApp;

Components
So this code is defining HelloWorldApp, a new Component. When you're building a React Native app, 
you'll be making new components a lot. Anything you see on the screen is some sort of component.

Props
Most components can be customized when they are created, with different parameters. These creation parameters are called props.

Your own components can also use props. This lets you make a single component that is used in 
many different places in your app, with slightly different properties in each place. Refer to props.{NAME} in your functional 
components or this.props.{NAME} in your class components.

State
Unlike props that are read-only and should not be modified, the state allows React components to change their output over time in response to user actions, network responses and anything else.

What's the difference between state and props in React?
In a React component, the props are the variables that we pass from a parent component to a child component. 
Similarly, the state are also variables, with the difference that they are not passed 
as parameters, but rather that the component initializes and manages them internally.
