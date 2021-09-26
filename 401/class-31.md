# Read: Class 31 - Context API

## Describe use cases useState() vs useReducer()?

 1. useState to add state to your functional components.
 2. useReducer React hook function that accepts a reducer function, and an initial state. ... This hook function returns an array with 2 values. The first one is the state value, and the second value is the dispatch function which is further used to trigger an action with the help of array destructuring.

## Why do custom hooks need the use prefix?

*Custom Hooks*
This is mainly to have an extra option for sharing state and logic between components. ... Custom hooks are normal JS functions, named with the prefix 'use', that can use hooks inside of it and contain a common stateful logic to be reused in other components.

## What do custom hooks usually do?

Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.

## Using any list of custom hooks, research and name one that you think will be useful in your applications

1. useClippy
A hook for copying data to the clipboard and retrieving/pasting it using Ctrl-C/Command-C and Ctrl-V/Command-V.
2. useScript
useScript is a hook for loading (and notifying when they’re loaded) external scripts, dynamically.
3. useLocalStorage
This hook simplifies the storage and retrieval of data from the localStorage.
