# [ES6 Syntax and Feature Overview](https://www.taniarascia.com/es6-syntax-and-feature-overview/)


***A commonly accepted practice is to use `const` except in cases of loops and reassignment. However, in this resource I'll be using `let` in place of `var` for all ES6 examples.***

<hr>

***Knowledge Level Assumptions***

*React is a JavaScript library, and so we’ll assume you have a basic understanding of the JavaScript language. If you don’t feel very confident, we recommend going through a JavaScript tutorial to check your knowledge level and enable you to follow along this guide without getting lost. It might take you between 30 minutes and an hour, but as a result you won’t have to feel like you’re learning both React and JavaScript at the same time.*

<hr>

***Why JSX?***

*React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.*

*Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both. We will come back to components in a further section, but if you’re not yet comfortable putting markup in JS, this talk might convince you otherwise.*

*React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.*

<hr>

***Components and Props***

*Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. This page provides an introduction to the idea of components. You can find a detailed component API reference here.*

<hr>

***Converting a Function to a Class***

> ***You can convert a function component like Clock to a class in five steps:***

- Create an ES6 class, with the same name, that extends React.Component.
- Add a single empty method to it called render().
- Move the body of the function into the render() method.
- Replace props with this.props in the render() body.
- Delete the remaining empty function declaration.

<hr>

***Handling Events***

> *Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:*

* React events are named using camelCase, rather than lowercase.
* With JSX you pass a function as the event handler, rather than a string.
