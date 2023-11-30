
# Exploration Activity 2: Library/Package Overview


## 1. Which package/library did you select?

The library selected for the second exploration activity is the JavaScript **React** library.


## 2. What is the package/library?

React is a free and open-source front-end JavaScript library for building user interfaces based on components. React can be used to develop single-page, mobile, or server-rendered applications.[ref](https://en.wikipedia.org/wiki/React_(software))

### What purpose does it serve?

React's primary prupose is to manage the view layer of an application by providing optimal rendering and execution. The main features of React which pose an advantage are:[ref](https://legacy.reactjs.org/)
1. *Declarative*: Declarative views make code predictable and easier to debug. Simple views can be designed for every state of an appplication and React will update and render the correct components once data changes, thus, making it painless to create interactive UIs.
2. *Component-Based*: Create self-contained components that handle their own state, and then combine them to create intricate user interfaces.
3. *JavaScript-Based*: Rich data can be easily passed through an application and keep state out of DOM since component logic is written in JavaScript instead of templates.
4. *Learn Once, Code Anywher*: Develop new features in React without rewriting existing code.
5. *Versatile Rendering*: React seamlessly renders on servers using Node and powers mobile apps through React Native.

### How do you use it?

In order to use React, one should use a fast and modern development server tool called Vite.

**Create a project using Vite:**
1. Open a terminal and ```cd``` to your project folder's directory(must be an empty folder).
2. Run ```npm create vite@latest```
3. Type a name for the project or simply type '.' to use the current directory.
4. Select the ```React``` framework.
5. Select ```JavaScript``` or ```JavaScript + SWC``` for the variant.
6. Run the specified commands one after the other.
7. You shoulld see a link after ```Local:``` which will take you to the application that will change according to your code.

**Begin modifying the React application:**[ref](https://www.w3schools.com/react/react_getstarted.asp)
1. Look for a ```src``` folder in your project directory. You should find a ```App.jsx``` file. Open that file.
2. Replace all the content inside the ```<div className="App">``` with a ```<h1>``` element as below:
```
function App() {
  return (
    <div className="App">
      <h1>Test!</h1>
    </div>
  );
}
```
3. Save the file and go to your application in the browser. You should see ```Test!``` displayed on the webpage.
4. You can now begin customizing and adding more components to your webpage in a similar manner! Refer to the functionalities mentioned in the next section to see the various components you can incorporate.

## 3. What are the functionalities of the package/library?
React has a wide range of functionalities and applications such as:[ref](https://www.freecodecamp.org/news/react-components-jsx-props-for-beginners/)[ref](https://www.geeksforgeeks.org/what-are-the-features-of-reactjs/)
1. *JSX*: JSX is a combination of JavaScript and HTML where JavaScript can be embedded inside HTML components.
2. *Functional Components*: A functional component is a JavaScript/ES6 function that returns a React element (JSX). A valid functional component can be represented by the following two versions:

```
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```

```
const Welcome = (props) => { 
  return <h1>Hello, {props.name}</h1>; 
}
```
3. *Class Components*: Class components are ES6 classes that return JSX.
```
class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```
4. *Export/Import*: It is required that a componenent be first exported so that it can be imported it somewhere else for later use.
```
export default Welcome;
```

```
import Welcome from './Welcome';
```
5. *Props*: A prop is a special object (stands for property) which can be used to transport data from one component to another (one-way flow from parent to child components).
Define a prop on the Welcome component:
```
import Welcome from './Welcome';

function App() { 
  return (
    <div className="App">
      <Welcome name="John"/>
      <Welcome name="Mary"/>
      <Welcome name="Alex"/>
    </div>
  );
}
```
Since the Welcome component is the child, the props is defined on its parent (App), values can be passed and the result appears by accessing the prop "name".
```
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```
Output: 
![Sample output after using props for the Welcome component.](image-2.png)
6. *Virtual DOM*(Document Object Model): JavaScript Frameworks update the whole DOM at once, which makes the web application slow. But react uses virtual DOM which is an exact copy of real DOM. Whenever there is a modification in the web application, the whole virtual DOM is updated first and finds the difference between real DOM and Virtual DOM. Once it finds the difference, then DOM updates only the part that has changed recently and everything remains the same. 
7. *Performance*: DOM executes in memory so separate components can be created which makes the DOM run faster.
8. *Conditional Statements*: JSX allows to write conditional statements. The data in the browser is displayed according to the conditions provided inside the JSX.
```
const age = 12;
if (age >= 10)
{ 
    <p> Greater than { age } </p>;
} 
else 
{ 
    <p> { age } </p>;
}
```

## 4. When was it created?
The first signs of React were seen in 2010 through Xhp. An early prototype, FaxJS, was created in 2011. Finally, React was released on May 29, 2013.[ref](https://blog.risingstack.com/the-history-of-react-js-on-a-timeline/)


## 5. Why did you select this package/library?
I am interested in visual design and graphics. My previous exploration activity comprised of working with the python Bokeh library dedicated to create dynamic visuals. I decided to continue down a similar path by gaining some insight into creating user interfaces through JavaScript's React library. I would like to take courses regarding human-computer interaction and interface design in the future, therefore, I wanted to use this opportunity to get some basic familiarity to the concepts.


## 6. How did learning the package/library influence your learning of the language?
At first, JavaScript was a language that I simply saw as a derivation of Java and easier to code since I had already learned Java. Working with the React library opened me to a wider spectrum of using JavaScript for something of my interest making me see JavaScript as a more useful language for me.


## 7. How was your overall experience with the package/library?
Learning React is extremely complicated. Since there is an integration of HTML and JavaScript, it is difficult to remember the syntax and various tags along with the functionalities. Personally, following online video tutorials and using sample programs has been helpful in understanding the code, however, it will take a lot practice to get familiarized with React.

### When would you recommend this package/library to someone?
I would recomment this library to someone who is looking to create extensive and intricate interfaces. However, I would not recommend this library to someone who is looking for one-time easy and simple design.

### Would you continue using this package/library? Why or why not?
I would continue using this library as I would like to know how websites and other intricate interfaces can be created and how far the customizations can go. I would also like to know how easy it will become to use React once familiarized.
