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
 - Provider
We can access the value in the Context using Consumer Component provided by the Context Object.
