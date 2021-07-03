# Read: Class 05 - Putting it all together:
## Break The UI Into A Component Hierarchy :
 In the firest you will drow box in all genarelly and inner-components by js or in design .

 In ether you wiil use function or object or to create 
 single responsibility principle , the Single Responsibility Principle
  means that a component is required to have only one reason to change. In short, the Single Responsibility Principle means that code with the same functionality should not exist in multiple places.

## Build A Static Version in React

 A  static build is a compiled version of a program which has been statically linked against libraries .
 Static applications and websites render in the user’s browser without the need for server side processing, this means that all the rendering of HTML, CSS, and JavaScript is done on the client side, rather then relying on server side technologies. Whilst traditionally managing static websites and applications may seem like hard work, the medium has come on leaps and bounds over the past few 
 years to the extent that it’s now perfectly feasible to run heavy content, rich media websites, and applications entirely in the browser .

> If you want to build components that reuse other components and pass data using props. props are a way of passing data from parent to child. If you’re familiar with the concept of state .
     
> State functions are defined by comparing them to path functions. As stated before, a state function is a property whose value does not depend on the path taken to reach that specific function or value.

##  Identify Where Your State Should Live 

React is all about one-way data flow down the component hierarchy. It may not be immediately clear which component should own what state. This is often the most challenging part for newcomers to understand.

### For each piece of state in your application:

Identify every component that renders something based on that state.
Find a common owner component (a single component above all the components that need the state in the hierarchy).
Either the common owner or another component higher up in the hierarchy should own the state.
If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

