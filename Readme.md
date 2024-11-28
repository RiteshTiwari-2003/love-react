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

