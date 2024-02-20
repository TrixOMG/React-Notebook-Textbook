# React Theory

## What is React?

React is a JavaScript library for building a reusable user interface(UI).

It was initially released on May 29, 2013.

React was created by Facebook. React makes creating UI components very easy.

When we work with React we do not interact directly with the DOM.

React has its own way to handle the DOM(Document Object Model) manipulation.

React uses its virtual DOM to make new changes and it updates only the element, that needs changing.

Do not directly interact with DOM when you build a React Application and leave the DOM manipulation job for the React virtual DOM.

A web application, or a website, is made of buttons, links, forms with different input fields, header, footer, sections, articles, texts, images, audios, videos and boxes with different shapes.

We use react to make a reusable UI components of a website.

- React was released in May 2013
- React was created by Facebook
- React is a JavaScript library for building user interfaces
- React is used to build single page applications - An application which has only one HTML page.
- React allows us to create reusable UI components

## Why React?

React is one of the most popular JavaScript libraries.

Why we choose to use React ? We use it because of the following reasons:

- fast
- modular
- scalable
- flexible
- big community and popular
- open source
- High job opportunity

## JSX

JSX stands for JavaScript XML.

JSX allows us to write HTML elements with JavaScript code.

An HTML element has an opening and closing tags, content, and attribute in the opening tag.

However, some HTML elements may not have content and a closing tag - they are self closing elements.

To create HTML elements in React we do not use the createElement() instead we just use JSX elements.

Therefore, JSX makes it easier to write and add HTML elements in React.

JSX will be converted to JavaScript on browser using a transpiler - babel.js.

Babel is a library which transpiles JSX to pure JavaScript and latest JavaScript to older version.

```js
const jsxElement = <h1>I am a JSX element</h1>;
```

### JSX Element

JSX element could be a single HTML element or many HTML elements wrapped in a parent HTML element.

Every HTML element should be wrapped by an outer HTML element to create a valid JSX element.

```js
const header = (
  <header>
    <h1>My Personal React Notebook-Textbook</h1>
    <h2>Getting Started React</h2>
    <h3>JavaScript Library</h3>
  </header>
);
```

### Commenting a JSX Element

```js
{
  /*
  <header>
    <h1>My Personal React Notebook-Textbook</h1>
    <h2>Getting Started React</h2>
    <h3>JavaScript Library</h3>
  </header>
*/
}
```

### Rendering a JSX Element

To render a JSX element to HTML document, we should first create an index HTML.

The index.html is the only HTML file you will have in any React Application.

That is why we say that every React Application is a single page application.

We can get started with React in two ways - either by using CDN or create-react-app.

The create-react-app creates a React project boilerplate "out the box".

...

### Style and className in JSX

To add style to a JSX element we use inline style or className.

We inject the style object using {}.

Every CSS property becomes a key and every CSS property value becomes a value for the the object.

All two word CSS properties will change to camelCase when we use them as key in the CSS object in React or JavaScript.

```js
const header = (
  <header>
    <h1 style={{ color: "blue", fontSize: "18px" }}>
      My Personal React Notebook-Textbook
    </h1>
    <h2 style={{ color: "red" }} className='heading-2'>
      Getting Started React
    </h2>
    <h3 style={{ color: "green" }}>JavaScript Library</h3>
  </header>
);
```

It is a good practice to open the browser console while you are developing your application to know, if everything goes well.

### Injecting data ot a JSX Element

To inject data to a JSX we use the {} bracket.

```js
const headerOneText = "My Personal React Notebook-Textbook";

const header = (
  <header>
    <h1 style={{ color: "blue", fontSize: "18px" }}>
      {headerOneText}
    </h1>
    <h2 style={{ color: "red" }} className='heading-2'>
      Getting Started React
    </h2>
    <h3 style={{ color: "green" }}>JavaScript Library</h3>
  </header>
);
```
