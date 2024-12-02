# cretae react app

run this terminal first
npx create-react-app myreactapp
cd myreactapp
npm start

we create a one more folder alongwith myreactapp in main folder MyReact which name is react-tailwind-css-starter-pack
and in this folder for installation of all packages in package.json we run
npm i aand enter
and when we start running this command
cd react-tailwind-css-starter-pack
and then run npm start
then error come but when in package.json of this folder we go in script and start key and add this thing in string
set NODE_OPTIONS=--openssl-legacy-provider && react-scripts start

# package.json work like a entry point for project beacuase from which command we start the program and from which command we terminated from execution all the thing describe in the package.json

# what is script in package.json

in react project , the script section in the package.json file contains predefined command that you can run using npm or yarn ,
this script simplify running common task for development , testing, and building your application
here is the example of key script:

1. build:
   command : npm run build
   purpose: to create an optimized production ready build of your react application
   what it does:
   bundle all your code (javascript, css) into static file.
   minifies and optimize the code for better performance
   output the build in the build/ directory by default
   use case: when you are ready to deploy your app to production , you run the build command

2: start:

command: npm start
purpose: start the development server
what is does :
run the app in development mode
opens the app in your default web browser at http://localhost:3000

3: eject:
command : npm run eject
purose: exposes the hidden configuration files (webpack, babel, eslint) used by create react app.

what it does:
copies all the configuration files into your project , allowing you to customize them

breaks the create react app abstraction by making you fully responsible for managing the configuration
we install also a dev dependencies which is tailwindcss we need to add -D at the last when we run the command of install any dev dependencies
like npm i tailwindcss -D

if you want to uninstall any package then you can also do like
npm uninstall tailwindcss

but when you install tailwindcss like this
npm i tailwindcss without dev dependencies them it go in dependencies in package.json

# what is the node module?

the node_module folder in a node.js project is a directory that contains all the libraries (dependencies) and their sub dependencies required for your project of function,these libraries are installed when you run the npm install or yarn install command.
purpose of node module:

1. dependencies storage: the folder store all the package and module you specify in the dependencies or devdependencies section of your package.json file.
2. it also include subdependencies required by those package

# how the node module work?

when you run npm install;
node package manager reads the package.json file to determine which packages are needed
npm install those packages and their dependencies from the npm registry
the download packages are placed in the node module

node module basically the storage of dependencies and packages and subdependencies
like third party packages like random-number in this many code have written down that code written down into node module of all the packages and dependencies

# what is react basically ?

react is javascript library which soul purpose is to create user interface.
library is what , library is basically a segment of code where vast amount of functionality provided to user
user's code invoked the all of that functionality whenever they needed that functionality

a magical line about react is react is all about components, react is the component based architecture , then here one question is arises that what is component?
then we simply say that components are the reusable peace of code .
in js when we want to use same code again and again then we make function of that code but in react we make components for that code
component is nothing more while a function in react.
you can assume in your mind that component create a custom html element for you, you can assume but dont tell this in interview.

like when we create a website inside the website there can be many components inside the website one is header two side bar one main component and one is footer. then we simply say that we have five component inside my website.

# why we need the reactjs when react is a javascript library and all thing written in the javascript then why we need react js why not we use js for everything?

because normal js is based on imperetive approach whatmeans of this that suppose you want to create x thing x functinality x ui for your app. then you need to tell everything that from here fetch the body tag, and upon that create the children component in that chil create this component and attach that componet to the tag.

but in react you only need to tell about end point , imperetive approach means everything done by step by step line by line
but in react only tell about end point and give up all the thing on react for completion
but how?

and this is declarative approach that only tell about end point to react and all thing give up on the react.

# what is the spa (single page application)?

like we have single page of html and in that you changes all the time .
once the that page is loaded then after that you change all time dynamically
in single page application basically we create a html file and after that when changes occur we changes dynamically into that single html file.
when you simply write thin in paragraph tagthis is called static value but when you fetch paragraph from api call with the help of js in paragraph tag this is called dynamically change .

# react alternatives

Anguler , vue
but when you talk about framework not about library then on thing also come which is next js anguler js also framework

# component

when we use any code for many time then we make its component and component create custom html element of that we make custome html tag which name in example we give <Custome></Custom>
why react?
reusability
dry(dont repeat yourself)
readiability
soc (seperation of concern)
maintainability

# create new react project

step1 : install node js
step2: vs code
step 3: create a new folder: ReactFolio
step 4: change directory to reactFolio
step 5: npx create-react-app demoshopapp
step6: change directory to demoshopapp
step 7: npm start

# way no. 2:

Replit
go in replit and click on create reple templete is react javascript we give title demoshopapp click on create

# way 3:

tailwind wala starter pack

# in react in src folder what is done by index.js why we write index.js file

this is the entry point of the react project, first of all we execute index.js file in react
this is first js file which is execute in react project
in react we import first component as app component in index.js file in reder function which is property of root which is accessed by react from
public folder index.html file.

basically first in src first index,js file run and take the root element from index.html file of public folder and make the root of react and with the help of root react rander the App component or function so after this app.js is called, then react take its root element and for showing anything on ui if we want to show anything in that root element , when we want to display something on the display we can say that thing to do rendering

so in react one function present which name is basically render , but what we render in root.render function then answer is App
in app.js component we add that code which i want to show on display

# why we use className at the place of class?

because in app component basically we use js (a custom html) not a html and in js class is basically a reserved keyword , so we can not use class so because of this we use className .
so basically app component replace the index.html file div tag because react take root from div element in index.html and make its root
and after this pass the root with render function then it call app component and app component show whichever thing you want to see on the server or on the display

like in app.js and other thing in react we use language that is not proper javascript then how it is run properly because it is not js it is jsx javascriptxml(html inside javascript)

and when you run the npm start it convert the user friendly code in browser understanding code like normal html and js.

# other components

if we want to make some other components then we can make component in src folder in components folder and we can export and import it into App.js
and in App function we call this component but if we add <Item></Item> then it shows error because in react in any component like App we only pass the components in one global tag ont seperatly which is also called as fregments which is describe like this <></>
we can also replace this with div tag.

# one importent question about props property

like i have one global tag in which two tag present then if in inner tags one tag have own style that color:red but also we give style to global tag that its color is green then in in inner tag whatever you write follow whcih tag property?
and why? this is related to {props.className}
in react how to we handle event handling then we can say props using props you can also done eventhandling and every props from which you can do event handling is start with on as like onClick

if you want to change anything on ui using event or anything then we want to use state
like we change my variable but that variable in doesnot change because of absencs of state, using state we change also ui when we update the variable, like a variable title has a value "Nirma" but i changed the cariable as "surfaxel" then react put the surfaxel inside the tilte variable and rerender all the ui,state basically when you put new value inn variable then state basically render the whole ui.
if we want state inside my code then we must import that state like this
import React,{useState} from "react";

# what is useState ?

useState is basically is the rreact hook,that allow you to add state management to functional component with useState, you can create a stATEFUL variable (a value that react keeps track of) and update it dynamically as your app interact with user or other events.
why use useState?
state is used to store information that change over time,such as :
user input form
a counter value
data fetched from an api
ui toggles
before react hook,state management was only possible in class component, but with useState
functionasl component can now manage state

syntex of useState
const [state,setState]=useState(initialvalue);
state: the current value of the state
setState: a function to update the state value
initial value: the starting value of the state

useState basically return two variable as a output like one is state and one is function which is use to update the state whenever any change occur
like in initial point in variable title has a value "nirma" but you want to change this like this
title = "surfaxel" then by only initializing this nothing have done but is you change value like this setState("surfaxel")

meaning of thus line const[title,setTitle]=useState(props.title);
basically in title block basically in initial time props.title stored but whenever you want to change the title value you call this function setState()
now in ui basically a button shown which is click and whenevr we click on click button, click event basically fired.click event basically mapped with onClick props,onClick props is mapped with clickHandler function and in this function basically one syntex is written that setTitle performed
settitle function basically what done:
basically go first and change the title variable value from props.title to surfexel and after this render the ui.

# here some question come when you write this line that

# const[title,setTitle]=usestate(initialvalue);

# setTitle("surfaxel");

# then when in 210 line there is const present then how you change the value from setTitle function how it is possible.

if in your code any data which you want to change and also reflect it on ui then you must use state(useState)

# in react this is very importent question that we can easily access give object from parents component to chid component ut how parents take or access object from child component?

we all know that children access object from component using props but in reverse if parent component want or access component from child component
then how can access it?
so we can say that in parent basically a function define for accessing object from child component and pass that function as a props to the child component
and child component call parents function with that object as a parameter and when child component call the function
it goes in parents and parent easily access object from child component using this.

like a super parent component A and its child component is B and b's child component is component c , and component c 's child is component component D
like in A handler function and pass that handler function to component B and component b's handler function and inthat function call function A using props
and also pass the handler function to c from b and in component c define the handler function call the function b inside the handler function and also pass the handler function into component d from component call
inn component d define handler function and in this handler function call the component c dunction using props.

in handle multiple state using the useState hooks in react, you can call the useState function multiple times , once for each state you want to manage
here's is the example:
import {useState} from 'react';
function MyComponent(props){
const[count,setCount]=useState(0);
const[text,setText]=useState("");
function handleIncrement(){
setCount(count+1);
}
function handleText(event){
setText(event.target.value);
}
return(
<div>
<p>Count:{count}</p>
<button onClick={handleIncrement}>Increment</button>
<br/>
<input type="text" value={text} onChange={handletextChange}/>
<p>Text: {text}</p>
</div>
);
}
in this example we are managing the two state using useState: count and text.we are also defining two function : handleincrement, which update the count when a
a button is clicked and handletextChange, which update the text state when the text input changes.
by calling useState twice , we are creating two independent piece of state that can be managed seperatly , we are also using destructing to 
assign the current value of each stae and its corresponding setter function to seperate variable 

other alternative:
we can also manage the multiple state using a single useState hook by passing an object as the initial state and using destructuring to access individual state variable and their corresponding update function,

import {useState} from "react";
function MyComponent(props){
   const[state,setState]=useState({
      count:0,
      text:''
   });
   function handleIncrement(){
      setState(prevState=>{...prevState,count:prevState.count+1})
   }
   function handleTextChange(event){
      setState(prevState=>({...prevState,text:event.target.value}))
   }
   return (
      <div>
      <p>Count :{state.count}</p>
      <button onClick={handleIncrement}>increment</button>
      <br/>
      <input type="text" value={state.text} onChange={handleTextChange}/>
      <p>Text:{state.text}</p>
      </div>

   );
}

# main difference between onClick={()=>setCategory(data.title)} and onClick={setCategory(data.title)} is when the setcategory function is failed
in the first case, onClick={()=>setcategory(data.title)}, an arrow function is used as a callback function for the onclick event handler 
this is means that when the element is called , the arrow function will be executed and then call the setcategory function with the data.title
, this is useful when you need to perform some additional logic or calculation before the calling setcategory function

in the second case , onClick={setcategory(data.title)}, the setcategory function is called immediately when the component is rendered ,
and the return the value of the setcategory function is assigned to the onClick event handler.
this is not desirable because it will call the setcategory function on every render, which can lead to unneccessary re render and performance issue.

therfore the correct way to pass the function with argument to an onclick event handler is to use the first approach 
with an arrow function , this way the setcategory function is called when the element is clicked , and not on every render.

# basic hooks which is very importent
# basic hooks
> useState hook
> useEffect hook
> useContext hook

# additional hooks;
useReducer
>useCallback
>useMemo
>useRef
> useImperativeHandle
> useLayoutEffect
> useId

# about the useState:
const[state,setState]=useState(initialState);
return a statefull value and a function to update it 
during the initial render , the returned state(state) is same as the value passed as the first argument (initialState).
the setState function is used to update the state, it accept the new state value and enqueue  a rerender of component.


