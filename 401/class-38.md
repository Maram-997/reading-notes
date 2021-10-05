# Read: Class 38 - Redux - Asynchronous Actions

## How granular should your reducers be?

It depends, since we can separate the reducers for each component if we want to apply an action on that component i don’t think that we need to make general for all components.

## Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched

Well, it is a Pro more than a Con since we have to change multiple states in multiple components, the fact that all the reducers can listen when the action is dispatched can reduce a lot of work, each reducer can provide a different logic to the same dispatcher.

## Name a strategy for preventing the above?

Make a reducer for each component that will be affected by the dispatcher, only effecting a specific amount of the state it self.
