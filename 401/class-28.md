# Read: Class 28 - Component Lifecycle / useEffect()

## Why do we not need more .html pages in a multi-page React app?

Because react is a single page app, A React app consists of a single HTML file index.html. The views are coded in JSX format as components.

## If we wanted a component to show up on every page, where would we put it and why ? Outside the`<BrowserRouter/>`Inside the `<BrowserRouter />`, outside a `<Route />`Inside a `<Route />`

will be inside the Route that will be as an instance of BrowserRouter, to allow the React App render needed component that is exisiting inside the Route, and each time the active route “by path” will be rendered.

## What does routing do with the components that were rendered when a new route is requested

switching component from React-router, first route will match the clicked path will be rendered, and will go out the switch and will not see or render the other components.

## What does props.children contain?

props. children does is that it is used to display whatever you include between the opening and closing tags when invoking a component.

## How do useState() and this.setState() differ?

setState() The setState function is used to handle the state object in a React class component.(applied in class component)
useState()  This simplifies the creation of a state component and the function that updates it.(applid in functional component)