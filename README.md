# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Context 

*Create a context file that contains states or functions that need to be passed down to sub-components.

*Create the context in that file:
```
const MyContext = createContext();
```

*Export a provider that contains these states/functions (children) using:
```
return <ContextComponent.Provider value={{
    state1,
    function1,
    function2,
    etc...
  }}>
    {children}
  </ContextComponent.Provider>
```

*Then in any component that needs to access the context set a const:
```
const {state1, function1, function2 etc.} = useContext(MyContext);
```