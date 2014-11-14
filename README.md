why-react
=========

Why React?

Ronn's daughter story - rethinking your approach to the internet

Give us 5 minutes

React - A library for creating user interfaces

- The V in MVC?

Combine DOM generation and display logic
Re-render the whole app on every update
Virtual DOM and synthetic events

1. Build components, not templates
 - Templates encourage a poor separation of concerns
  - higher coupling, less cohesion

  View model tightly couples template to display logic
  Display logic and markup are tightly coupled and cohesive

  Templates have primitive abstractions (show josh's ember each example)

  React component
  - highly cohesive building block
  - loosely coupled with other components
  - reusable
  - composable
  - unit testable

  JSX
  - optional preprocessor for HTML like syntax
  - easy for designers to contribute code

2. Re-render the whole app on every update
  - UIs have a lot of state
  - "Data changing over time is the root of all evil."
  - React re-renders the entire component when data changes.
  - React components are idempotent functions
    - describe UI at any point in time like a server rendered app
    - no magical data binding
    - everything guaranteed to be up to date

3. Virtual DOM
  - Rebuilding entire DOM on each update
    - slow
    - lose form state and scroll position
  - React has a virtual DOM and events system optimized for performance
  - On every update
    - React builds a new virtual DOM subtree
    - Diffs it with old one
    - computes minimal set of DOM mutations and puts them in a queue
    - batch executes all updates
  - Virtual DOM can run in Node.js

Key Takeaways

Components, not templates
Re-render, don't mutate
Virtual DOM is simple and fast

