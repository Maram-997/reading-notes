# Read: Class 37 - Redux - Combined Reducers

## Why choose Redux instead of the Context API for global state?

Context API: Resourceful and ideal for small applications where state changes are minimal
Redux: Perfect for larger applications where there are high-frequency state updates

## What is the purpose of a reducer?

A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently.

## What does an action contain?

`let {type, payload} = action`

## Why do we need to copy the state in a reducer?

If the new state is different, the reducer must create new object, and making a copy is a way to describe the unchanged part.
> this will be used the first time we run the app, since the state will be undefined.

`export default (state = initialState, action) => {}`
