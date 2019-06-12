//This is a test - changing a thing

# React Assessments

Try your best to answer each question on your own before looking up the answer online. Once you're done writing your first answer, you can google the question and write the best answer you find.

#### 1. Here is a list of pros and cons to using the React library to build your application -- but some of them are false. Remove the false statements from the list:

<!-- - React was created to be simple, so that even people with minimal code experience could use it and create Single Page Applications (SPAs) -->
- React is a modern, efficient answer to complex UI applications
<!-- - React is a full stack framework for modern web applications -->
- React is a flexible library that plays the role of V in an MVC framework


 #### 2. What are "smart"(logic) and "dumb"(display) components? Explain the difference and also add why we bother to make the distinction between them.


 //Your Answer
 Smart components hold state and contain pieces that perform actions such as functions. Dumb components only display pieces. They can be passed dynamic information as props but are not dynamic themselves. We distinguish between them as a way of keeping our app organized and as a matter of convention.

 //Googled Answer
 A Smart Component is any component which manages its own state. When working with Babel or ES6-style React, we've come to know this as any class-like object that extends Component. A Dumb Component can very easily be defined as a stateless component. A stateless component is much more efficient than a stateful one, because it doesn't require as many computer resources to render (memory, CPU, and GPU in terms of graphic-intensive apps). Contextual Irrelevance is a unique test for determining whether or not your component should be Smart or Dumb. It comes down to the functionality and role your component plays in your application. Does your component contain functionality or handle data that is Contextually Irrelevant? In other words, does your component handle information or functionality that is irrelevant to where you use your component?
 Source: https://coderwall.com/p/znkw-q/smart-vs-dumb-components-when-to-use-which


#### 3. When we use "yarn add ..." in the terminal - what is yarn doing? And what file will always be automatically updated after we add a package with yarn?


 //Your Answer
 Yarn is installing a package or command. I don't know what file is automatically updated but I think it's a JSON file.


 //Googled Answer
 In general, a package is simply a folder with code and a package.json file that describes the contents. When you want to use another package, you first need to add it to your dependencies. This means running yarn add [package-name] to install it into your project.
 This will also update your package.json and your yarn.lock so that other developers working on the project will get the same dependencies as you when they run yarn or yarn install.
 Source: https://yarnpkg.com/lang/en/docs/cli/add/

#### 5. There are three mistakes in this code that would cause it to break our application. Find the mistakes and fix them:

    import React, { Component } from 'react';

    class Recipes extends Component {
      constructor(props){
        super(props)
        this.state = {
          recipes:
            {name: 'Meatballs'},
            {name: 'Mac & Cheese'}

        }
      }

      render() {

        return (

          let recipes = this.state.recipes.map(function(recipe){
            return(
              <li key={recipe.name}>{recipe.name}</li>
            )
          })

          <ul>
            {recipes}
          </ul>
        );
      }
    }

    export default Recipes;


#### 6. Name three html input types. (NOTE: text is the default type - so it doesn't count in this case)

 //Your Answer
number, check, submit

 //Googled Answer
 Button, checkbox, color, date, datetime-local, email, file, hidden, image, month, number, password, radio, range, reset, search, submit, tel, text, time, url, week
Source: https://www.w3schools.com/html/html_form_input_types.asp

 #### 7. How would you explain state to a friend who doesn't know code?

 //Your Answer
Dynamic elements are ones that can change depending on different conditions. State is really just what it sounds like in English: the state of a dynamic element at any given time. For instance, if you're assigning a random number to an element, the state of that element could be 3 when you first load the page, and when you reload the page and a new random number is chosen for that element, its new state could be 347.

 //Googled Answer
State is a plain JavaScript object that holds information that influences the output of render. Unlike props which get passed to the component, state is managed within the component.
Source: https://reactjs.org/docs/faq-state.html

 #### 8. What is the difference between component state and props? Your answer should include a short explanation of both.


 //Your Answer
I didn't read this question before reading number 7, so I accidentally skipped ahead in terms of knowing the googled answer.

 //Googled Answer
 State is a plain JavaScript object that holds information that influences the output of render. Unlike props which get passed to the component, state is managed within the component.
 Source: https://reactjs.org/docs/faq-state.html

#### 9. Write a paragraph or so about your experience with building tic-tac-toe. Some topics to start with might be: things you learned about yourself, concepts from React that stood out to you, something about pair programming (if you paired), or the experience of building something in code from scratch.
