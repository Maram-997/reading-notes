# Read: Class 33 - `<Login />` and `<Auth />`

## Why is the Context API useful?

The Context API is a React structure that enables you to exchange unique details and assists in solving prop-drilling from all levels of your application.

## Can a component outside of a provider get its context?

Yes we can call useContext in each component to pull out the values we need. It doesn’t matter how far apart the components are as long as they’re wrapped in a provider.

## What are some common use cases for using the Context API?

Some sample use cases where the Context API proves helpful are: Theming — Pass down app theme. i18n — Pass down translation messages. Authentication — Pass down current authenticated user.

## Describe “Context Hell”

What is the React Context hell? Like the callback hell, usual when jQuery was used for everything, the React Context hell is the nasty code you get taking advantage of the React Context API.
