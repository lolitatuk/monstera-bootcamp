# Monstera Bootcamp

For exercices create a new repo, and create the files inside folders with the index number on the topics before. And send Pull requests for each of this topics. All the folders and all PRs are must be

Exercices:
1. Create a basic .html file with a header displaying "Hello World".

    1.1. Change the header to "My todo list".
    1.2. Add a list of "todo items" for your daily chores.
    1.3. Create another .html file. Create a table for your expenses.
    1.4. Create another .html file. Add an image, a video, and a sound.
      ## Notes: 
        You may find this book useful: http://diveintohtml5.info/
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
