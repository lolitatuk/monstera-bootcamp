# Monstera Bootcamp

For exercices fork this repo, and create the files inside folders with the index number on the topics below. And send Pull requests for each of this topics. All the folders and all PRs are must be there.

Exercices:
1. Create a basic .html file with a header displaying "Hello World".

    1.1. Change the header to "My todo list".
    
    1.2. Add a list of "todo items" for your daily chores.
    
    1.3. Create another .html file. Create a table for your expenses.
    
    1.4. Create another .html file. Add an image, a video, and a sound.
    
    > Notes: 
    > You may find this book useful: [http://diveintohtml5.info/](http://diveintohtml5.info/)
    
    1.5. Create a "sign up" form with fields for: first name, last name, email, birthday, a dropdown to choose your favourite sport, and a text-area to include a small bio for the user. Add a button at the end to submit the form, and another one to clear the form. Add relevant validation rules for all fields (like required fields, valid email).
    
    1.6. Test your HTML files in at least Firefox, Chrome, IE, and Chrome for Android or iOS Safari.
    
2. Create a basic index.html file
    
    2.1. Create an empty style.css file and link it to the index.html using the link tag.
    
    2.2. Learn why is a best-practice to use a reset stylesheet [here](http://meyerweb.com/eric/tools/css/reset/). Then include [normalize.css](http://necolas.github.io/normalize.css/) before linking your style.css.
Add a basic page structure using HTML as depicted by the following picture:

![alt text](https://github.com/globant-ui/css-lab/blob/master/images/html5-structure.png "Logo Title Text 1")

3. Create a basic html with the structure of the image above.
    3.1. Add background to the header, footer, aside and nav. 
    
    3.2. Add a global font definition (at html element) with a value of 14px, using a font-family you like. 
    
    3.3. Center the header and footer text.
    
    3.4. Experiment with specificity right now using CSS3 selectors http://specificity.keegan.st/
    
    3.5 Now add the following classes to the document created above:
    
      - To <header> add class .header
      - To <footer> add class .footer
      - To <section> add class .content
      - To <nav> add class .navigation
      - To <aside> add class .sidebar

    3.6. Using the new added classes figure out how to override:
      - .header must have a font size of 46px
      - .footer must have a font size of 10px
      - .content must have a font size of 14px
      - .navigation must have a font size of 12px
      - .sidebar must have a font size of 10px
      - If the class attribute finishes with `r` (example header, footer), the background must be magenta.
      - If the class attribute contains an `a` (example nav) but do NOT finish with `r`, the background must be blue.
      - How could you add weight to the global font definition to win over the classes added by point 3.5?
      - Imagine there is a declaration like class=”oh-no-inline-styles” style=”background:red” and you need to change the background to green without changing the inline style. How could you accomplish this?
      
4. Use latest IE, Chrome, or Firefox browser to develop. Try to use as much ECMAScript 6 syntax as you can. Favor let and const over var

    4.1. Open your IDE, create a new file text, save it as index.html. Add the correct doctype, and a few tags with random content.
    
    4.2. Add a stylesheet to the index.html. Use the stylesheet to center the text of all section elements of the page.
    
    4.3. Add a hidden section with the following text inside: "Hello world".
    
    4.4. When the page has finished loading the section must fade in. Hint: Use JavaScript, Browser Events, and CSS3
    
    4.5. Add a button below the section to your index.html.
    
    4.6. Attach a click event to the created button which calls a function that gets a response from http://api.icndb.com/jokes/random. Write the response to the section element. Hint: use the XMLHttpRequest to fetch data from the service
    
    4.7. From the previous exercise create a reusable function to perform AJAX calls. The function must accept a config object and return an ES6 Promise.
    
    4.8. Show section content in red when a server error occurs.
    
    4.9. Use the function created in exercise 6 to get the response from https://api.github.com/search/repositories with parameters data "q = 'JavaScript'". First log the service response in Chrome's console to analyze data (see provided link on Chrome console), then display repository's full_name as a list in the right side of the screen. The ul element must be used to list the repositories data.
    
    4.10. Add an input type="text", and reuse the code for exercise 9, so the user can perform search for any repository.

    4.11. Validate your page using W3C validator: https://addons.mozilla.org/en-US/firefox/addon/web-developer/

    4.12. Write a function that takes as input a matrix of data and outputs a DOM structure representing a table. Attach it to the body of a given page. Hint: use document.createElement, document.createTextNode, and Node.appendChild methods
    
 ## Test your code in a mobile device or in Android emulator.

Hint: A good option to test your code in a mobile device is to use Genimotion Android Emulator [http://www.genymotion.com/], which is one of the most fast and easy mobile emulators to install.

5. Reading:
 - Understand how prototypes works in ECMAScript 5.1 http://yehudakatz.com/2011/08/12/understanding-prototypes-in-javascript/
 - ECMAScript 6 New Features: http://es6-features.org/. You can compare ECMAScript 5 and 6 code.
 - Read the Chapter on JavaScript classes from Understanding ECMAScript6
 - Read about ES6 Modules
 - Extra: Read about AMD, CommonJS, and ES6 Modules Writing Modular JavaScript
 - An overview on all the features ECMAScript provides https://github.com/lukehoban/es6features

    5.1 Create a Movie object:
<table>
    <tr>
        <td>Movie</td>
    </tr>
    <tr>
        <td>- title <br />- year <br />- duration</td>
    </tr>
    <tr>
        <td>+ play() <br />+ pause()<br />+ resume()<br /></td>
    </tr>
</table>
   
   5.2. Instantiate some of your favorite movies and play with them in the console.

   5.3. Create an EventEmitter class with the following methods: `on`, `emit`, `off`. The on method will allow to pass a callback or listener that will be executed each time a given event is triggered. The emit method will allow a class to trigger events to be consumed by other functions/objects. The off method will delete the listener.

   5.4. Make Movie a subclass of EventEmitter. Publish "play" event on Movie.play(), "pause" event on Movie.pause(), and "resume" event on Movie.resume()

   5.5. Create a Logger class with a log(info) method that will output info to the console. Make log listen to a Movie's 'play' event. You should be able to do something like this in the console:

```javascript
let terminator = new Movie('Terminator', 1984, 90);
let logger = new Logger();
terminator.on('play', logger.log);
// ...
terminator.play(); // output: The 'play' event has been emitted
```

   5.6. Create an object called Social with methods share(friendName) and like(friendName) that will generate the following output "{friendName} likes/share {Movie Name}". Hint: declare Social as an object literal, use Object.assign to mix Social methods into a Movie instance. Use Template Literals to generate the like/share method output. You should be able to do something like this in the console:

`ironman.share('Mike Blossom'); // output: Share Iron Man with Mike Blossom`

   5.7. Create an Actor class and create some actors from one of your favorite movies.

   5.8. Add a method to Movie that will allow to add one or more actors at the same time.

```javascript
let terminator = new Movie('Terminator I', 1985, 60);
let arnold = new Actor('Arnold Schwarzenegger', 50);
let otherCast = [
  new Actor('Paul Winfield', 50),
  new Actor('Michael Biehn', 50),
  new Actor('Linda Hamilton', 50)
];

terminator.addCast(arnold);
terminator.addCast(otherCast); //Movie must contain an array of 4 actors
```

Using ES6 Modules split all your classes declarations into diferent files. Use Babel to create a single bundle. Hint: check this [tutorial](https://babeljs.io/docs/usage/cli/)

6. Reading:
What is [ReactJS](http://facebook.github.io/react/)?. [Here](http://www.instrument.com/latest/an-introduction-to-react-js) is an introduction to it.

First [get started with ReactJS](https://facebook.github.io/react/docs/getting-started.html) then [Think in React](https://facebook.github.io/react/docs/thinking-in-react.html).

Understand [Props & States](https://github.com/uberVU/react-guide/blob/master/props-vs-state.md).

Read about some ReactJS's [Best Practices, Patterns & Anti-patters](https://github.com/planningcenter/react-patterns).

Check some ReactJS's [Test utils](https://facebook.github.io/react/docs/test-utils.html).

Try on using [Reactify](https://github.com/andreypopp/reactify) [ReactJS + Browserify workflow](https://www.codementor.io/reactjs/tutorial/react-js-browserify-workflow-part-1).

#####Extra reading:#####

[Full guide on ReactJS](https://scotch.io/tutorials/learning-react-getting-started-and-concepts).

[Read some ReactJS tips](https://facebook.github.io/react/tips/introduction.html).

   6.1. Create the needed components to allow the user create a new Movie.

   6.2. Create the needed components to show a list of your favorite Movies.

   6.3. Create the needed components to allow the user edit a Movie.

   6.4. Update the movie listing to allow the user delete movies.

   6.5. Update the application to use ReactRouter and Flux.
   
 - First, try to think which should be your app structure (in terms of components).
 - Second, figure out which component should handle the movies.
 - You should create a component when trying to create a view (a view is also a component).
 - To update the application with ReactRouter and Flux you may split out the add logic and the display logic into two views. Also you may provide the data storage (object) responsibility to Flux's storages.
 
# Final Project
You will work on a project to achieve a fully working multi platform mobile app developed in JavaScript and using the latest tags and APIs available in HTML5. You will need to create an application in React that will handle todos in a list, that will allow to create edit and remove them, and save them to the session of the user on the localstorage so if I reload the page, the todos still there.
Also, on the header of the app, must be a Joke using the service above, and the current date and time, showed in format for instance: Friday, March 21, 2012. 12:03:05
Make sure you create unit tests for all your code, and your coverage is 100%.
