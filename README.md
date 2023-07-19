# [React Context](https://sspwindowsapp.ccbp.tech/)

## 1. Prop Drilling
Props are passed from one Component to another Component that does not need the data but only helps in passing it through the tree is called Prop Drilling.

## 2. React Context
Context is a mechanism that provides different Components and allows us to pass data without doing prop drilling.

### Creating Context
React.createContext(INITIAL_VALUE)
It returns an object with different properties to update and access values from the context.

### Context Properties
The Context object provides two properties.

 - Consumer
 - Provider </br>
##### We can access the value in the Context using Consumer Component provided by the Context Object.

## 3. Consumer Component

<ContextObject.Consumer>
  {/*callback function*/}
</ContextObject.Consumer>

- We access the Consumer component using dot notation from the context object.
- We will give a callback function as children for Consumer Component.
##### The callback function receives the current context value as an argument and returns a component or a JSX element.
Look at the code to understand the syntax of callback function.

## 4. Provider
- Provider Component updates the value of Context.
- When the provider updates context, all the nested consumers of that provider will be re-rendered.
- Updated context value can only be accessed by the consumers nested within the provider. <br/>

ContextObject.Provider value={/* some value */}>
   .......
<ContextObject.Provider/><br/>

To update context value, we have to pass it as a prop to the Provider component.
- The context value should have the data which the consumers need.
- It should also contain the required methods to update that data.
