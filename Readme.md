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

