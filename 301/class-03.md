# Read: Class 03 - Passing Functions as Props:

A **`key`** is a special string attribute you need to include when creating lists of elements in React. Keys are used to React to identify which items in the list are changed, updated, or deleted. In other words, we can say that keys are used to give an identity to the elements in the 
 ## Rendering Multiple Components :
 
 render you still can't render multiple items because react needs a root. So you can render a single component inside the ReactDOM. render and render an array of items in the internal component

 ## Basic List Component :
 
 Usually you would render lists inside a component.you can refactor the previous example into a component that accepts an array of numbers and outputs a list of elements.

## Keys :
Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity.The best way to pick a key is to use a string that uniquely identifies a list item among its siblings. Most often you would use IDs from your data as keys.When you don’t have stable IDs for rendered items, you may use the item index as a key as a last resort. 




## Keys must be unique, but only amongst siblings
Keys help ensure that only the components that have changed get re-rendered. The only way it's possible to keep track on which components have actually been changed is to tag them with a unique key