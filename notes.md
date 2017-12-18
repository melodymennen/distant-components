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

## What is immutability? Why do we use it?


