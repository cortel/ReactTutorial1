# ReactTutorial1
Purpose to learn React

#Documentation

#REACT:
-React is a javascript library
-Purpose of React: show content (html) to users and handle User Interaction
-‘React’ library knows what a component is and how to make components work together
-‘ReactDOM’ knows how to take a component and make it show up in the dom
-React Native- for mobile devices

#React Components:
-React Components are made using either javascript functions or classes
-Used to present content on the screen
-Used to create an Event Handler

#JSX:
-Html lookalike and can be placed in JS Code
-Determines the content of our React App just like normal HTML

#Event Handles
-Event handlers are used to detect user interaction and respond to it (onClick, onMouseHover, etc etc,)

#Create React Project in VS

https://docs.microsoft.com/en-us/visualstudio/javascript/tutorial-nodejs-with-react-and-jsx?view=vs-2019

-Transpile the jsx
-In Solution Explorer, right-click the project node and choose Open Command Prompt Here.

In the command prompt, type the following command:

-node_modules\.bin\webpack app.tsx --config webpack-config.js

 package.json - scrips :
 "build": "webpack-cli app.tsx --config webpack-config.js"
- Each time you make changes to app.tsx, you must rerun the webpack command. To automate this step, add a build script to transpile the JSX.
 nstead of transpiling JSX at the command line (as shown in the preceding section), you can transpile JSX when building from Visual Studio.

#React project directory Components

-src : source code
-public - folder that stores static files like images, html file that doesnt change etc..
-node_modules - folder that contains all of our project dependencies
-package.json - records out project dependecies and configures our project
-package-lock.json- records the exact version of packages that we install
-Readme.md -> instructions on how to use this project

#Good To know Tips
-stopping a react app in node.js Ctrl + c
-Starting the app up run npm start in project directory

#Javascript Module Systems

-Bundleler system called webpack
-every file created inside the project is "esentially its own tiny universe (protected /not public if you think in access moddifer)"
-for access to any library or any other code in the project, you need to write the import statements
-Import syntax  example : Import React from 'react' (get dependency/code - assign to variable React - from - 'react' dependency )
-Import syntax basically it assigns a variable(convention : Nameofthelibrary = name of variable) with the value of the imported dependency
-How does it work :
-Javascript sees you search for 'react' -> looks into node_modules and goes into the 'react' folder and gets all the code there
-other syntaxes const React = require('react');
-Import Statement -> refers to ES2015 Modules (set of rulles that governs how to share code between different files)
-Require - > refers to CommonJS Modules (different set of rules)

#Displaying Content with Functional Components

-A component is a (Function or a Class) -> That produces HTML to show the user (Using JSX) -> And handles feedback from the user (using Event Handlers)