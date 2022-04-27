 ## React js
 
 React is a library for building user interfaces. React is not a framework – it's not even exclusive to the web. It's used with other libraries to render
 to certain environments. For instance, React Native can be used to build mobile applications.
 
To build for the web, developers use React in tandem with ReactDOM. React and ReactDOM are often discussed in the same spaces as — and utilized to solve 
the same problems as — other true web development frameworks. When we refer to React as a "framework", we're working with that colloquial understanding.

**React**'s primary goal is to minimize the bugs that occur when developers are building UIs. It does this through the use of components — self-contained, logical 
pieces of code that describe a portion of the user interface. 

These components can be composed together to create a full UI, and React abstracts away much of the 
rendering work, leaving you to concentrate on the UI design.

React utilizes features of modern JavaScript for many of its patterns. Its biggest departure from JavaScript comes with the use of JSX syntax. JSX extends JavaScript's
syntax so that HTML-like code can live alongside it.

## JSX
What JSX ?
it is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like. JSX may remind you of a template language, but it comes with the full power of JavaScript.

Why JSX?
React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.

Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both. We will come back to components in a further section, but if you’re not yet comfortable putting markup in JS, this talk might convince you otherwise.

React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.
## DOM

DOM: DOM stands for ‘Document Object Model’. In simple terms, it is a structured representation of the HTML elements that are present in a webpage or web-app. DOM represents the entire UI of your application. The DOM is represented as a tree data structure. It contains a node for each UI element present in the web document. It is very useful as it allows web developers to modify content through JavaScript, also it being in structured format helps a lot as we can choose specific targets and all the code becomes much easier to work with
