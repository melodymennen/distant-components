# Redux

## What's the problem with distant components in React?
sharing data or state to distant components is combersome and error-prone.
sometimes parent components must track data that they dont even care about just for the sake of their children. 

## What is Redux? Why/when do we use it?
redux provides a store of data to our application where we can share data among distant components. we use redux only when its less painful than usinf react state. 

## What are the steps to add Redux to a React app?
Redux steps 
Part 1 - read
    A. create store 
    B. hook up <Provider> in index.js (around <App>)
    C. use connect() to connect to store from components that need data (mapStateToProps)
Part 2 - write
    A. create a reducer(s) with actions and action creators 
    B. dispatch actions with dispatch (mapDispatchToProps)

## What is a store?
a collection of data that is used by any component that needs its data. 

## What is a reducer? What does the reducer do for us in Redux?
a reducer is a function. it takes in state and action and returns a modified copy of state. this is the only way to modify state in redux. 

## What is immutability? Why do we use it?
Data is considered immutable when functions that use the data don't mutate it but insteadreturn a modified copy. Because the data is a reference (to an object or array), we'll trivially be able to tell that the data has changed, without needing to dig through the object to see what exactly changed. This is useful in React to know if a component should re-render, or doesn't need to bother.

##Vocab 
*action: a plain object. all actions have a type, but payload is optional. 
*action creator: a function that creates actions for us. keeps code DRY.
*dispatch: we send actions to the store using dispatch

