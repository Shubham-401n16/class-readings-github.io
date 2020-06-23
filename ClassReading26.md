# class-readings-26-github.io

What does a component’s lifecycle refer to?

Refers to the phases of each component.

Why are functional components preferred over class components?

Functional components helps to modularize the code better and 
reduce the amount of code needed to biuld it.

What is wrong with the following code?


import React, {useState, useEffect} from 'react'; 
   
function MyComponent(props) {
  const [count, setCount] = useState(0); 
     
  function changeCount(e) {
    setCount(e.target.value); 
  }
     
  let renderedItems = []
     
  for (let i = 0; i < count; i++) {
    useEffect( () => {
      console.log('component mount/update'); 
    }, [count]); 
       
    renderedItems.push(<div key={i}>Item</div>); 
  }
     
  return (<div>
    	<input type='number' value={count} onChange={changeCount}/>
      {renderedItems}
    </div>);
}

 Hooks shouldnot be called inside loops, conditions, or nested functions. 
 They should be used at the top level of React function. 
It ensures that Hooks are called in the same order each time a component renders.
