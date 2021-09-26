# Read: Class 32 - Context API - Behaviors

## When you have multiple contexts, what component type should you use (class/function) and why?

The static contextType property won't work if you need more than one, so instead you need to use a context consumer.

## What are some good use cases for using the Context API for global state?

Context is primarily used when some data needs to be accessible by many components at different nesting levels.

## How can you best test context?

The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing).
