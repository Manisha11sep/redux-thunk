### [Redux Thunk](https://github.com/gaearon/redux-thunk)

- Allows you to write an action creator that returns a function instead of an action
  - This allows you to have async functionality inside of your action creator or a conditional dispatch

###### What is a thunk?
- A `thunk` is a function that wraps an expression to delay its evaluation
```js
// Calculation of 1 + 2 is immediate
let x = 1 + 2 
// x === 3 // true

// Calculation of 1 + 2 is delayed
// foo can be called later to perform the calculation
// foo is a thunk!
let foo = () => 1 + 2
```
> Example from [react-redux](https://github.com/gaearon/redux-thunk) documentation

Another example of a `thunk` in React would be:
```js
<button onClick={ () => this.doSomething() }>Click Me!</button>
// onClick is a thunk!
```

