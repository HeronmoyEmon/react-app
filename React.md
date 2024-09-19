# React Setup and Overview

**Date:** 19-09-2024

## 1. Set Up Environment

```bash
node -v
npm create vite@4.1.0
```

- Provide project name
- Select framework: React
- Select variant: TypeScript

```bash
cd to project folder
npm install / npm i
```

- Open in VSCode
- Run development server

```bash
npm run dev
```

## React Overview

### React

React is a JavaScript library used for building dynamic and interactive user interfaces (UI).

### Library vs Framework

- **Library:** A tool that provides specific functionality.
- **Framework:** A set of tools and guidelines for building apps.

Since React is just a library and not a framework like Angular or Vue, we often need other tools for concerns such as routing, state management, internationalization, form validation, etc.

### DOM: Document Object Model

In React applications, we don't query and update the DOM directly. Instead, we describe our application using small, reusable components. React efficiently creates and updates DOM elements.

### React Components

React components can be created using a function or a class. Function-based components are the preferred approach as they're more concise and easier to work with.

### JSX

JSX stands for JavaScript XML. It is a syntax used for writing components that combine HTML and JavaScript in a readable and expressive way, making it easier to create complex user interfaces.

### What Happens Under the Hood

When our application starts, React takes a tree of components and builds a JavaScript data structure called the virtual DOM. This virtual DOM is different from the actual DOM in the browser. It's a lightweight, in-memory representation of our component tree.

When the state or the data of a component changes, React updates the corresponding node in the virtual DOM to reflect the new state. Then, it compares the current version of the virtual DOM with the previous version to identify the nodes that should be updated. It will then update those nodes in the actual DOM.

In browser-based apps, updating the DOM is done by a companion library called ReactDOM. In mobile apps, React Native uses native components to render the user interface.
