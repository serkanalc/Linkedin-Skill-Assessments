# Linkedin-Skill-Assessments

## React.js

#### Q1. To get the first item from the array ("cooking") using array destructuring, how do you adjust this line?

```javascript
const topics = ['cooking', 'art', 'history'];
```

- [ ] `const first = ["cooking", "art", "history"]`
- [ ] `const [] = ["cooking", "art", "history"]`
- [ ] `const [, first]["cooking", "art", "history"]`
- [ ] `const [first] = ["cooking", "art", "history"]`

#### Q2. How do you handle passing through the component tree without having to pass props down manually at every level?

- [ ] React Send
- [ ] React Pinpoint
- [ ] React Router
- [ ] React Context


#### Q3. What is the name of the tool used to take JSX and turn it into createElement calls?

- [ ] JSX Editor
- [ ] ReactDOM
- [ ] Browser Buddy
- [ ] Babel

#### Q4. If you want to import just the Component from the React library, what syntax do you use?

- [ ] `import React.Component from 'react'`
- [ ] `import [ Component ] from 'react'`
- [ ] `import Component from 'react'`
- [ ] `import { Component } from 'react'`

#### Q5. Why might you use useReducer over useState in a React component?

- [ ] when you want to replace Redux
- [ ] when you need to manage more complex state in an app
- [ ] when you want to improve performance
- [ ] when you want to break your production app

#### Q6. Which props from the props object is available to the component with the following syntax?

```javascript
<Message {...props} />
```

- [ ] any that have not changed
- [ ] all of them
- [ ] child props
- [ ] any that have changed

#### Q7. Consider the following code from React Router. What do you call :id in the path prop?

```javascript
<Route path="/:id" />
```

- [ ] This is a route modal
- [ ] This is a route parameter
- [ ] This is a route splitter
- [ ] This is a route link

#### Q8. If you created a component called Dish and rendered it to the DOM, what type of element would be rendered?

```javascript
function Dish() {
  return <h1>Mac and Cheese</h1>;
}
ReactDOM.render(<Dish />, document.getElementById('root'));
```

- [ ] `div`
- [ ] section
- [ ] component
- [ ] `h1`

#### Q9. What does this React element look like given the following function? (Alternative: Given the following code, what does this React element look like?)

```javascript
React.createElement('h1', null, "What's happening?");
```

- [ ] `<h1 props={null}>What's happening?</h1>`
- [ ] `<h1>What's happening?</h1>`
- [ ] `<h1 id="component">What's happening?</h1>`
- [ ] `<h1 id="element">What's happening?</h1>`

#### Q10. What property do you need to add to the Suspense component in order to display a spinner or loading state?

```javascript
function MyComponent() {
  return (
    <Suspense>
      <div>
        <Message />
      </div>
    </Suspense>
  );
}
```

- [ ] lazy
- [ ] loading
- [ ] fallback
- [ ] spinner

#### Q11. What can you use to handle code splitting?

- [ ] `React.memo`
- [ ] `React.split`
- [ ] `React.lazy`
- [ ] `React.fallback`

#### Q12. When do you use `useLayoutEffect`?

- [ ] to optimize for all devices
- [ ] to complete the update
- [ ] to change the layout of the screen
- [ ] when you need the browser to paint before the effect runs

#### Q13. What is the difference between the click behaviors of these two buttons (assuming that this.handleClick is bound correctly)?

```javascript
A. <button onClick={this.handleClick}>Click Me</button>
B. <button onClick={event => this.handleClick(event)}>Click Me</button>
```

- [ ] Button A will not have access to the event object on click of the button.
- [ ] Button B will not fire the handler this.handleClick successfully.
- [ ] Button A will not fire the handler this.handleClick successfully.
- [ ] There is no difference.

#### Q14. How do you destructure the properties that are sent to the Dish component?

```javascript
function Dish(props) {
  return (
    <h1>
      {props.name} {props.cookingTime}
    </h1>
  );
}
```

- [ ] `function Dish([name, cookingTime]) { return <h1>{name} {cookingTime}</h1>; }`
- [ ] `function Dish({name, cookingTime}) { return <h1>{name} {cookingTime}</h1>; }`
- [ ] `function Dish(props) { return <h1>{name} {cookingTime}</h1>; }`
- [ ] `function Dish(...props) { return <h1>{name} {cookingTime}</h1>; }`

#### Q15. When might you use `React.PureComponent`?

- [ ] when you do not want your component to have props
- [ ] when you have sibling components that need to be compared
- [ ] when you want a default implementation of `shouldComponentUpdate()`
- [ ] when you do not want your component to have state

#### Q16. Why is it important to avoid copying the values of props into a component's state where possible?

- [ ] because you should never mutate state
- [ ] because `getDerivedStateFromProps()` is an unsafe method to use
- [ ] because you want to allow a component to update in response to changes in the props
- [ ] because you want to allow data to flow back up to the parent

#### Q17. What is the children prop?

- [ ] a property that adds child components to state
- [ ] a property that lets you pass components as data to other components
- [ ] a property that lets you set an array as a property
- [ ] a property that lets you pass data to child elements

#### Q18. Which attribute do you use to replace innerHTML in the browser DOM?

- [ ] injectHTML
- [ ] dangerouslySetInnerHTML
- [ ] weirdSetInnerHTML
- [ ] strangeHTML

#### Q19. Which of these terms commonly describe React applications?

- [ ] declarative
- [ ] integrated
- [ ] closed
- [ ] imperative

#### Q20. When using webpack, why would you need to use a loader?

- [ ] to put together physical file folders
- [ ] to preprocess files
- [ ] to load external data
- [ ] to load the website into everyone's phone

#### Q21. A representation of a user interface that is kept in memory and is synced with the "real" DOM is called what?

- [ ] virtual DOM
- [ ] DOM
- [ ] virtual elements
- [ ] shadow DOM

#### Q22. You have written the following code but nothing is rendering. How do you fix this problem?

```javascript
const Heading = () => {
  <h1>Hello!</h1>;
};
```

- [ ] Add a render function.
- [ ] Change the curly braces to parentheses or add a return statement before the `h1` tag.
- [ ] Move the `h1` to another component.
- [ ] Surround the `h1` in a `div`.

#### Q23. To create a constant in JavaScript, which keyword do you use?

- [ ] const
- [ ] let
- [ ] constant
- [ ] var

#### Q24. What do you call a React component that catches JavaScript errors anywhere in the child component tree?

- [ ] error bosses
- [ ] error catchers
- [ ] error helpers
- [ ] error boundaries

#### Q25. In which lifecycle method do you make requests for data in a class component?

- [ ] constructor
- [ ] componentDidMount
- [ ] componentWillReceiveProps
- [ ] componentWillMount

#### Q26. React components are composed to create a user interface. How are components composed?

- [ ] by putting them in the same file
- [ ] by nesting components
- [ ] with webpack
- [ ] with code splitting

#### Q27. All React components must act like **\_** with respect to their props.

- [ ] monads
- [ ] pure functions
- [ ] recursive functions
- [ ] higher-order functions

#### Q28. Why might you use a ref?

- [ ] to directly access the DOM node
- [ ] to refer to another JS file
- [ ] to call a function
- [ ] to bind the function

#### Q29. What is `[e.target.id]` called in the following code snippet?

```javascript
handleChange(e) {
  this.setState({ [e.target.id]: e.target.value })
}
```

- [ ] a computed property name
- [ ] a set value
- [ ] a dynamic key
- [ ] a JSX code string

#### Q30. What is the name of this component?

```javascript
class Clock extends React.Component {
  render() {
    return <h1>Look at the time: {time}</h1>;
  }
}
```

- [ ] Clock
- [ ] It does not have a name prop.
- [ ] React.Component
- [ ] Component

#### Q31. What is sent to an `Array.map()` function?

- [ ] a callback function that is called once for each element in the array
- [ ] the name of another array to iterate over
- [ ] the number of times you want to call the function
- [ ] a string describing what the function should do

#### Q32. Why is it a good idea to pass a function to `setState` instead of an object?

- [ ] It provides better encapsulation.
- [ ] It makes sure that the object is not mutated.
- [ ] It automatically updates a component.
- [ ] `setState` is asynchronous and might result in out of sync values.

#### Q33. What package contains the render() function that renders a React element tree to the DOM?

- [ ] `React`
- [ ] `ReactDOM`
- [ ] `Render`
- [ ] `DOM`

#### Q34. How do you set a default value for an uncontrolled form field?

- [ ] Use the `value` property.
- [ ] Use the `defaultValue` property.
- [ ] Use the `default` property.
- [ ] It assigns one automatically.

#### Q35. What do you need to change about this code to get it to run?

```js
class clock extends React.Component {
  render() {
    return <h1>Look at the time: {this.props.time}</h1>;
  }
}
```

- [ ] Add quotes around the return value
- [ ] Remove `this`
- [ ] Remove the render method
- [ ] Capitalize `clock`

#### Q36. Which Hook could be used to update the document's title?

- [ ] `useEffect(function updateTitle() { document.title = name + ' ' + lastname; });`
- [ ] `useEffect(() => { title = name + ' ' + lastname; });`
- [ ] `useEffect(function updateTitle() { name + ' ' + lastname; });`
- [ ] `useEffect(function updateTitle() { title = name + ' ' + lastname; });`

#### Q37. What can you use to wrap Component imports in order to load them lazily?

- [ ] `React.fallback`
- [ ] `React.split`
- [ ] `React.lazy`
- [ ] `React.memo`

#### Q38. How do you invoke setDone only when component mounts, using hooks?

```javascript
function MyComponent(props) {
  const [done, setDone] = useState(false);
  return <h1>Done: {done}</h1>;
}
```

- [ ] `useEffect(() => { setDone(true); });`
- [ ] `useEffect(() => { setDone(true); }, []);`
- [ ] `useEffect(() => { setDone(true); }, [setDone]);`
- [ ] `useEffect(() => { setDone(true); }, [done, setDone]);`

#### Q39. Which of the following click event handlers will allow you to pass the name of the person to be hugged?

```javascript
class Huggable extends React.Component {
  hug(id) {
    console.log("hugging " + id);
  }
  render() {
    let name = "kitteh";
    let button = // Missing Code
    return button;
  }
}
```

- [ ] `<button onClick={(name) => this.hug(name)}>Hug Button</button>`
- [ ] `<button onClick={this.hug(e, name)}>Hug Button</button>`
- [ ] `<button onClick={(e) => hug(e, name)}>Hug Button</button>`
- [ ] `<button onClick={(e) => this.hug(name,e)}>Hug Button</button>`

#### Q40. Currently, `handleClick` is being called instead of passed as a reference. How do you fix this?

```javascript
<button onClick={this.handleClick()}>Click this</button>
```

- [ ] `<button onClick={this.handleClick.bind(handleClick)}>Click this</button>`
- [ ] `<button onClick={handleClick()}>Click this</button>`
- [ ] `<button onClick={this.handleClick}>Click this</button>`
- [ ] `<button onclick={this.handleClick}>Click this</button>`

#### Q41. Which answer best describes a function component?

- [ ] A function component is the same as a class component.
- [ ] A function component accepts a single props object and returns a React element.
- [ ] A function component is the only way to create a component.
- [ ] A function component is required to create a React component.

#### Q42. What will happen when this useEffect Hook is executed, assuming name is not already equal to John?

```javascript
useEffect(() => {
  setName('John');
}, [name]);
```

- [ ] It will cause an error immediately.
- [ ] It will execute the code inside the function, but only after waiting to ensure that no other component is accessing the name variable.
- [ ] It will update the value of name once and not run again until name is changed from the outside.
- [ ] It will cause an infinite loop.

#### Q43. Which choice will not cause a React component to rerender?

- [ ] if the component calls `this.setState(...)`
- [ ] the value of one of the component's props changes
- [ ] if the component calls `this.forceUpdate()`
- [ ] one of the component's siblings rerenders

#### Q44. You have created a new method in a class component called handleClick, but it is not working. Which code is missing?

```javascript
class Button extends React.Component{
  constructor(props) {
    super(props);
    // Missing line
  }
  handleClick() {...}
}
```

- [ ] `this.handleClick.bind(this);`
- [ ] `props.bind(handleClick);`
- [ ] `this.handleClick.bind();`
- [ ] `this.handleClick = this.handleClick.bind(this);`

#### Q45. React does not render two sibling elements unless they are wrapped in a fragment. Below is one way to render a fragment. What is the shorthand for this?

```javascript
<React.Fragment>
  <h1>Our Staff</h1>
  <p>Our staff is available 9-5 to answer your questions</p>
</React.Fragment>
```

- [ ] A

```javascript
<...>
  <h1>Our Staff</h1>
  <p>Our staff is available 9-5 to answer your questions</p>
</...>
```

- [ ] B

```javascript
<//>
  <h1>Our Staff</h1>
  <p>Our staff is available 9-5 to answer your questions</p>
<///>
```

- [ ] C

```javascript
<>
  <h1>Our Staff</h1>
  <p>Our staff is available 9-5 to answer your questions</p>
</>
```

- [ ] D

```javascript
<Frag>
  <h1>Our Staff</h1>
  <p>Our staff is available 9-5 to answer your questions</p>
</Frag>
```

#### Q46. If you wanted to display the count state value in the component, what do you need to add to the curly braces in the `h1`?

```javascript
class Ticker extends React.component {
  constructor(props) {
    super(props);
    this.state = { count: 0 };
  }
  render() {
    return <h1>{}</h1>;
  }
}
```

- [ ] this.state.count
- [ ] count
- [ ] state
- [ ] state.count

#### Q47. How do you fix the syntax error that results from running this code?

```javascript
const person =(firstName, lastName) =>
{
  first: firstName,
  last: lastName
}
console.log(person("Jill", "Wilson"))
```

- [ ] Wrap the object in parentheses.
- [ ] Call the function from another file.
- [ ] Add a return statement before the first curly brace.
- [ ] Replace the object with an array.

#### Q48. If you see the following import in a file, what is being used for state management in the component?

`import React, {useState} from 'react';`

- [ ] React Hooks
- [ ] stateful components
- [ ] math
- [ ] class components

#### Q49. Per the following code, when is the Hello component displayed?

```javascript
const greeting = isLoggedIn ? <Hello /> : null;
```

- [ ] never
- [ ] when `isLoggedIn` is true
- [ ] when a user logs in
- [ ] when the Hello function is called

#### Q50. In the following code block, what type is orderNumber?

```javascript
ReactDOM.render(<Message orderNumber="16" />, document.getElementById('root'));
```

- [ ] string
- [ ] boolean
- [ ] object
- [ ] number

#### Q51. You have added a style property to the `h1` but there is an unexpected token error when it runs. How do you fix this?

```javascript
const element = <h1 style={ backgroundColor: "blue" }>Hi</h1>;
```

- [ ] `const element = <h1 style="backgroundColor: "blue""}>Hi</h1>;`
- [ ] `const element = <h1 style={{backgroundColor: "blue"}}>Hi</h1>;`
- [ ] `const element = <h1 style={blue}>Hi</h1>;`
- [ ] `const element = <h1 style="blue">Hi</h1>;`

#### Q52. Which function is used to update state variables in a React class component?

- [ ] `replaceState`
- [ ] `refreshState`
- [ ] `updateState`
- [ ] `setState`

#### Q53. Consider the following component. What is the default color for the star?

```javascript
const Star = ({ selected = false }) => <Icon color={selected ? 'red' : 'grey'} />;
```

- [ ] black
- [ ] red
- [ ] grey
- [ ] white

#### Q54. Which answer best describes a function component?(Not sure answer)

- [ ] `A function component is the same as a class component.`
- [ ] `A function component accepts a single props object and returns a React element.`
- [ ] `A function component is the only way to create a component.`
- [ ] `A function component is required to create a React component.`

#### Q55.Which library does the fetch() function come from?

- [ ] `FetchJS`
- [ ] `ReactDOM`
- [ ] `No library. fetch() is supported by most browsers.`
- [ ] `React`

#### Q56.What is the difference between the click behaviors of these two buttons(assuming that this.handleClick is bound correctly)

```javascript
  A. <button onClick=this.handleClick>Click Me</button>
  B. <button onClick={event => this.handleClick(event)}>Click Me</button>
```

- [ ] `Button A will not have access to the event object on click of the button`
- [ ] `Button A will not fire the handler this.handleClick successfully`
- [ ] `There is no difference`
- [ ] `Button B will not fire the handler this.handleClick successfully`

#### Q57.What will happen when this useEffect Hook is executed, assuming name is not already equal to John?

```javascript
useEffect(() => {
  setName('John');
}, [name]);
```

- [ ] `It will cause an error immediately.`
- [ ] `It will execute the code inside the function, but only after waiting to ensure that no other component is accessing the name variable.`
- [ ] `It will update the value of name once and not run again until name is changed from the outside.`
- [ ] `It will cause an infinite loop.`

#### Q58. How would you add to this code, from React Router, to display a component called About?

```javascript
<Route path="/:id" />
```

- [ ] A

```javascript
<Route path="/:id">
  {' '}
  <About />
</Route>
```

- [ ] B

```javascript
<Route path="/tid" about={Component} />
```

- [ ] C

```javascript
<Route path="/:id" route={About} />
```

- [ ] D

```javascript
<Route>
  <About path="/:id" />
</Route>
```

#### Q59. Which class-based component is equivalent to this function component?

```javascript
const Greeting ({ name }) > <h1>Hello {name}!</h1>;
```

- [ ] A

```javascript
class Greeting extends React.Component {
  constructor() {
    return <h1>Hello {this.props.name}!</h1>;
  }
}
```

- [ ] B

```javascript
class Greeting extends React.Component {
  <h1>Hello {this.props.name}!</h1>;
}
```

- [ ] C

```javascript
class Greeting extends React.Component {
  render() {
    return <h1>Hello {this.props.name}!</h1>;
  }
}
```

- [ ] D

```javascript
class Greeting extends React.Component {
  render({ name }) {
    return <h1>Hello {name}!</h1>;
  }
}
```

#### Q60. Give the code below, what does the second argument that is sent to the render function describe?

```javascript
ReactDOM.render(
  <h1>Hi<h1>,
    document.getElementById('root')
)
```

- [ ] where the React element should be added to the DOM
- [ ] where to call the function
- [ ] where the root component is
- [ ] where to create a new JavaScript file

#### Q61. Why should you use React Router's Link component instead of a basic `<a>` tag in React?

- [ ] The link component allows the user to use the browser's `Back` button.
- [ ] There is no difference--the `Link` component is just another name for the `<a>` tag.
- [ ] The `<a>` tag will cause an error when used in React.
- [ ] The `<a>` tag triggers a full page reload, while the `Link` component does not.

#### Q62. What is the first argument, `x`, that is sent to the `createElement` function?

```javascript
React.createElement(x, y, z);
```

- [ ] the element that should be created
- [ ] the order in which this element should be placed on the page
- [ ] the properties of the element
- [ ] data that should be displayed in the element

#### Q63. Which class-based lifecycle method would be called at the same time as this effect Hook?

```javascript
useEffect(() => {
  // do things
}, []);
```

- [ ] componentWillUnmount
- [ ] componentDidMount
- [ ] render
- [ ] componentDidUpdate

#### Q64. Given the code below, what does the second argument that is sent to the render function describe?

```javascript
ReactDOM.render(<h1>Hi</h1>, document.getElementById('root'));
```

- [ ] where the React element should be added to the DOM
- [ ] where to call the function
- [ ] where the root component is
- [ ] where to create a new JavaScript file


#### Q65. What is the name of this component?

```javascript
class Comp extends React.Component {
  render() {
    return <h1>Look at the time: {time}</h1>;
  }
}
```

- [ ] Comp
- [ ] h1
- [ ] React.Component
- [ ] Component

This question might be an updated version of Q37.

#### Q66. When using a portal, what is the first argument?

```javascript
ReactDOM.createPortal(x, y);
```

- [ ] the current state
- [ ] the element to render
- [ ] the App component
- [ ] the page

#### Q67. What is `setCount`?

```javascript
const [count, setCount] = useState(0);
```

- [ ] the initial state value
- [ ] a variable
- [ ] a state object
- [ ] a function to update the state

#### Q68. What is the use of map function below?

```javascript
const database = [user1:{},user2:{},user3:{}];
database.map((user)=><h1>user.data</h1>);
```

- [ ] gives a map of all the entries in database
- [ ] returns a heading tag for every entry in the database containing it's data
- [ ] returns one heading tag for all the entries in database
- [ ] checks which entry in the database is suitable for heading tag

#### Q69. Describe what is happening in this code?

```javascript
const { name: firstName } = person;
```

- [ ] It is creating a new object that contains the same name property as the person object.
- [ ] It is assigning the value of the person object's firstName property to a constant called name.
- [ ] It is retrieving the value of person.name.firstName.
- [ ] It is assigning the value of the person object's name property to a constant called firstName.

#### Q70. What is wrong with this code?

```javascript
const MyComponent = ({ names }) => (
  <h1>Hello</h1>
  <p>Hello again</p>
);
```

- [ ] React components cannot be defined using functions.
- [ ] React does not allow components to return more than one element.
- [ ] The component needs to use the return keyword.
- [ ] String literals must be surrounded by quotes.

#### Q71. Given this code, what will be printed in the `<h1>` tag?

```javascript
const MyComponent = ({ children }) => (
  <h1>{children.length}</h1>
);
...
<MyComponent>
<p>Hello</p>
<p>Goodbye</p>
</MyComponent>
```

- [ ] It will produce an error saying "cannot read property "length" of undefined."
- [ ] 1
- [ ] undefined
- [ ] 2

#### Q72. What is this pattern called?

```javascript
const [count, setCount] = useState(0);
```

- [ ] object destructuring
- [ ] array destructuring
- [ ] spread operating
- [ ] code pushing

#### Q73. What is the first file loaded by the browser in a basic React project?

- [ ] src/App.js
- [ ] src/index.js
- [ ] public/manifest.json
- [ ] public/index.html

#### Q74. The code below is rendering nothing, and there is an error that says "ReactDOM is not defined." How do you fix this issue?

```javascript
import React from 'react';
import { render } from 'react-dom';
const element = <h1>Hi</h1>;
ReactDOM.render(element, document.getElementById('root'));
```

- [ ] `render(element, document.getElementById("root"));`
- [ ] `ReactDOM(element, document.getElementById("root"));`
- [ ] `renderDOM(element, document.getElementById("root"));`
- [ ] `DOM(element, document.getElementById("root"));`

#### Q75. In this component, how do you display whether the user was logged in or not?

```javascript
render() {
  const isLoggedIn = this.state.isLoggedIn;
  return (
    <div>
      The user is:
    </div>
  );
}
```

- [ ] `The user is loggedIn ? logged in : not logged in.`
- [ ] `Write a function to check the login status.`
- [ ] `The user is {isLoggedIn = "no"}.`
- [ ] `The user is {isLoggedIn ? "logged in." : "not logged in"}.`

#### Q76. You are rendering a list with React when this warning appears in the console: "Warning: Each child in a list should have a unique 'key' prop." How do you fix this issue?

- [ ] Pass the name of each item as its key.
- [ ] Add a key prop with the same value to each item the list.
- [ ] Clear the console warnings.
- [ ] When iterating over the list items, add a unique property to each list item.

#### Q77. How would you generate the boilerplate code for a new app that you are building to collect underpants?

- [ ] npm create-react-app collect-underpants
- [ ] npx start-app collect-underpants
- [ ] react new collect-underpants
- [ ] npx create-react-app collect-underpants

#### Q78. Add the code that will fire the photon torpedoes when the button is clicked.

```javascript
class StarTrekkin extends React.Component {
  firePhotonTorpedoes(e) {
    console.log('pew pew');
  }
  render() {
    return; // Missing code
  }
}
```

- [ ] `<button onClick={firePhotonTorpedoes()}>Pew Pew</button>`
- [ ] `<button onClick={firePhotonTorpedoes}>Pew Pew</button>`
- [ ] `<button onClick={this.firePhotonTorpedoes()}>Pew Pew</button>`
- [ ] `<button onClick={this.firePhotonTorpedoes}>Pew Pew</button>`

#### Q79. What is the process of deciding whether an update is necessary?

- [ ] shadow DOM
- [ ] fiber
- [ ] reconciliation
- [ ] setting state

#### Q80. React is an open-source project but is maintained by which company?

- [ ] Intuit
- [ ] Twitter
- [ ] Facebook
- [ ] Snapchat

#### Q81. What command can you use to generate a React project?

- [ ] react-starter
- [ ] create-react-app
- [ ] react-gen
- [ ] react-start

#### Q82. What is the browser extension called that React developers use to debug applications?

- [ ] React Developer Tools
- [ ] React Tooling Add-on
- [ ] React Codewatch
- [ ] React Debug

#### Q83. Which tool is not part of Create React App?

- [ ] React
- [ ] jQuery
- [ ] webpack
- [ ] ReactDOM

#### Q84. What is the JavaScript syntax extension that is commonly used to create React elements?

- [ ] HTML
- [ ] JavaScriptX
- [ ] JSX
- [ ] React JavaScript

#### Q85. How might you check property types without using Flow or TypeScript?

- [ ] Check Manually.
- [ ] Use `prop-helper`.
- [ ] use `prop-types`.
- [ ] user `checker-types`.

#### Q86. How do you add an id of heading to the following h1 element?

`let dish = <h1>Mac and Cheese</h1>; `

- [ ] `let dish = <h1 id={heading}>Mac and Cheese</h1>;`
- [ ] `let dish = <h1 id="heading">Mac and Cheese</h1>;`
- [ ] `let dish = <h1 id:"heading">Mac and Cheese</h1>;`
- [ ] `let dish = <h1 class="heading">Mac and Cheese</h1>;`

#### Q87. When using a portal, what is the second argument?

```javascript
ReactDOM.createPortal(x, y);
```

- [ ] the App component
- [ ] the page
- [ ] the current state
- [ ] the DOM element that exists outside of the parent component

#### Q88. What is the first argument, x, that is sent to the `createElement` function?

`React.createElement(x,y,z);`

- [ ] the element that should be created
- [ ] the order in which this element should be placed on the page
- [ ] the properties of the element
- [ ] data that should be displayed in the element.

#### Q89. Which library does the `fetch()` function come from?

- [ ] FetchJS
- [ ] ReactDOM
- [ ] No library. `fetch()` is supported by most browsers.
- [ ] React

#### 90. What do you call the message wrapped in curly braces below?

```javascript
const message = 'Hi there';
const element = <p>{message}</p>;
```

- [ ] a JS function
- [ ] a JS element
- [ ] a JS expression
- [ ] a JSX wrapper

#### Q91. What should the console read when the following code is run?

```javascript
const [, , animal] = ['Horse', 'Mouse', 'Cat'];
console.log(animal);
```

- [ ] Horse
- [ ] Cat
- [ ] Mouse
- [ ] undefined

#### Q92. If a function component should always render the same way given the same props, what is a simple performance optimization available for it?

- [ ] Wrap it in the `React.memo` higher-order component.
- [ ] Implement the `useReducer` Hook.
- [ ] Implement the `useMemo` Hook.
- [ ] Implement the `shouldComponentUpdate` lifecycle method.


#### Q93. Using object literal enhancement, you can put values back into an object. When you log person to the console, what is the output?

```javascript
const name = 'Rachel';
const age = 31;
const person = { name, age };
console.log(person);
```

- [ ] `{{name: "Rachel", age: 31}}`
- [ ] `{name: "Rachel", age: 31}`
- [ ] `{person: "Rachel", person: 31}}`
- [ ] `{person: {name: "Rachel", age: 31}}`

#### Q94. What is the testing library most often associated with React?

- [ ] Mocha
- [ ] Chai
- [ ] Sinon
- [ ] Jest

#### Q95. When using a portal, what is the first argument?

```javascript
ReactDOM.createPortal(x, y);
```

- [ ] the current state
- [ ] the element to render
- [ ] the App component
- [ ] the page

#### Q96. What is `setCount`?

```javascript
const [count, setCount] = useState(0);
```

- [ ] the initial state value
- [ ] a variable
- [ ] a state object
- [ ] a function to update the state

#### Q97. What is the use of map function below?

```javascript
const database = [user1:{},user2:{},user3:{}];
database.map((user)=><h1>user.data</h1>);
```

- [ ] gives a map of all the entries in database
- [ ] returns a heading tag for every entry in the database containing it's data
- [ ] returns one heading tag for all the entries in database
- [ ] checks which entry in the database is suitable for heading tag
