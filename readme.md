#Interview Prep

(Partially from https://github.com/h5bp/Front-end-Developer-Interview-Questions)

Go through all of the following questions and think about how you would respond to each. You should be able to answer many of the questions from memory, but you may have to research a few of them.

**Copy this md file to your homework folder and add a short answer under each item.** You should try to be as concise as possible, and list any handy resources you used to answer the question. This will be useful for studying for interviews after class.

## General Questions

* What did you learn yesterday/this week?

This week we learned more about Angular, learned MongoDB and Mongoose, and how to tie those together with Node and Express to create MEAN stack applications.

* What excites or interests you about coding?

The ability to make, to build something that adds value to the world, but in a more efficient and scalable way than with physical products.

* What is a recent technical challenge you experienced and how did you solve it?

Learning to code has been a non-stop technical challenge.

* What UI, Security, Performance, SEO, Maintainability or Technology considerations do you make while building a web application or site?

Because my background is in customer service, I constantly think about how the user/customer is _actually_ going to interact with my product, and let that thinking inform my design/development process.

* Talk about your preferred development environment.

I love the synergy of collaborating with others, and so prefer an in-person working environment for developing. I do like to pop earbuds in and rock out to some music while in code-mode, however. 

* Which version control systems are you familiar with?

Git, especially in conjunction with GitHub. 

* Can you describe your workflow when you create a web page?

I start off on paper, making sure that I understand the user requirements, and then begin sketching out some paper prototypes. Once the "final" design is architecture-d out, I'll begin coding.  First I'll get the skeleton laid out, and then work on functionality. Once the product is functioning properly, I will begin styling it and making it look good.

* If you have 5 different stylesheets, how would you best integrate them into the site?

If it's not necessary for them to be kept separate, I would use a minifier to condense them into one stylesheet. If it turns out there is a specific reason for them to be separate, I would strongly encourage that they be kept organized, with separate stylesheets for certain pages/controllers/statuses, but keep them all in a single css folder, to make it easier to use.

* Can you describe the difference between progressive enhancement and graceful degradation?

Progressive enhancement is typically for a project under active development (where further functionality is currently lacking) utilizing thorough testing on features prior to release, to ensure the product remains usable. Graceful degradation is typically for products being shutdown/deprecated, where responsible parties inform their users of plans to cease maintenance of features/products, so their users can either adapt their usage or find useful alternatives. Both ideas relate to being a "good" business or software developer by responsibly balancing customer's needs for functional products with the needs of the business or developer.

* Describe how you would create a simple slideshow page, without any frameworks (HTML/CSS/JS only).

Using JS, I would add an eventListener to caret on the right and left of the image, advancing/reversing to the next/previous photo upon being clicked. Alternatively, I would use JS setTimeOut function along with a recursive function call to make an auto-advancing, never-ending, click-free slideshow.

* If you could master one technology this year, what would it be?

I currently plan to spend the next year mastering JavaScript and the frameworks built on top of it, but also plan to remain flexible and adaptable with market/employer demands.

* Explain the importance of standards and standards bodies.

Standards allow for increased efficiency (and reduction in mistakes-made/time-wasted) by reducing the amount of communication required through utilization of common best-practices, standardizing processes, using uniform jargon, etc. It reduces the amount of time spent getting people on the same page, by having them START from the same page. Or at least use the same book. :-)


## HTML Questions

* What does a `doctype` do?

It tells the client's browser what version of markup language the page is in.

* What's the difference between HTML and XHTML?

While similar, XHTML is more strict than HTML. It's simliar to XML, in that it REQUIRES documents to be "well-formed", whereas HTML on some pages can get a little... sloppy, sometimes.

* What are `data-` attributes good for?

Data- attributes allow you to store extra information on standard HTML elements without using non-standard attributes or unnessary properties on DOM.

* Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.

Cookies are packets of data sent by a server to a browser, and returned by the browser each time it accesses the same server. Cookies are used to identify the user, or to track their access to the server. LocalStorage is more secure than cookies, and larger amounts of data can be stored without affecting website performance. SessionStorage is similar to localStorage, but unlike localStorage which has no expiration date for the data, the data in sessionStorage will be cleared when the page session ends, aka when the browser gets closed.

* Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?

Links should go before the html, so the styling is applied as the page is rendered, rather than rendering once for the bare HTML and then again for the CSS links. It's good practice to put script tags at the end of the body so that the page loads completely before the browser requests the script file, which would stop the parsing of the HTML until the script(s) finished loading. 


## CSS Questions

* What is the difference between classes and IDs in CSS?

IDs are used for only one specific element and hold a higher specificity, so they take precedence in styling. Classes can be applied to multiple elements, but have a lower specificity than IDs, meaning ID styling takes precedence if there are conflicting styles applied.

* What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?



* Describe Floats and how they work.
* Describe z-index and how stacking context is formed.
* Have you ever used a grid system, and if so, what do you prefer?
* Have you used or implemented media queries or mobile specific layouts/CSS?
* How do you optimize your webpages for print?
* What are the advantages/disadvantages of using CSS preprocessors?
  * Describe what you like and dislike about the CSS preprocessors you have used.
* How would you implement a web design comp that uses non-standard fonts?
* Explain how a browser determines what elements match a CSS selector.
* Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.
* What does ```* { box-sizing: border-box; }``` do? What are its advantages?
* List as many values for the display property that you can remember.
* What's the difference between inline and inline-block?
* What's the difference between a relative, fixed, absolute and statically positioned element?
* The 'C' in CSS stands for Cascading.  How is priority determined in assigning styles (a few examples)?  How can you use this system to your advantage?
* What existing CSS frameworks have you used locally, or in production? How would you change/improve them?
* Have you played around with the new CSS Flexbox or Grid specs?
* Have you ever worked with retina graphics? If so, when and what techniques did you use?
* Explain some of the pros and cons for CSS animations versus JavaScript animations.

## JS Questions

* Explain event delegation

Event delegation lets you attach an event listener to a parent element, that will only trigger on descendants matching a selector, affecting existing elements as well as any elements that may be created before the next page reload.

* Explain how `this` works in JavaScript

The simplest explanation is that 'this' refers to the object of which the function is a method of. It gets more complex after that, but basically 'this' generally refers to the owner of the function.

* Explain how prototypal inheritance works



* Why is it called a Ternary expression, what does the word "Ternary" indicate?
* What's the difference between a variable that is: `null`, `undefined` or `undeclared`?
  * How would you go about checking for any of these states?
* What is a closure, and how/why would you use one?
* What's a typical use case for anonymous functions?
* Difference between: `function Person(){}`, `var person = Person()`, and `var person = new Person()`?
* What's the difference between `.call` and `.apply`?
* Explain `Function.prototype.bind`.
* What's the difference between feature detection, feature inference, and using the User Agent string?
* Explain AJAX in as much detail as possible.
* Have you ever used JavaScript templating?
  * If so, what libraries have you used?
* Explain "hoisting".
* Describe event bubbling.
* What's the difference between an "attribute" and a "property"?
* Why is extending built-in JavaScript objects not a good idea?
* What is the difference between `==` and `===`?
* Explain the same-origin policy with regards to JavaScript.
* What is the extent of your experience with Promises and/or their polyfills?
* What are the pros and cons of using Promises instead of callbacks?
* What tools and techniques do you use debugging Javascript code?
* What language constructions do you use for iterating over object properties and array items?

## Database Questions

* Design a database schema for Facebook, with at least 4 models, a complete set of attributes for each model, a 1:M association, and a M:M association.

## Ruby/Rails
* What are ruby gems?
* What is the difference between a symbol and a string?
* What is the difference between a class method and an instance method?
* What is the difference between local variables, instance variables, and class variables?
* What is a range?
* In ruby, what does attr_accessor do?  
* What is the purpose of environment files under the config folder in Rails? (development, test, production)
* What is the purpose of the application.rb file in Rails?
* How can you define a constant?
* What is the purpose of `yield`?
* How do you store API keys when creating an app?
* How do I send parameters through a url?
* Explain MVC
* What is a `before_action`? When would you use it?
* What do controllers do in rails?
* What is RESTful routing?
* What is a polymorphic association?
* What are params?
* How do I make a migration to add a column in Rails?
* What is CSRF? How does Rails protect an app against this?
* What's the difference between `User.find_by_id(1)` and `User.find(1)`?
* What's are classes in Ruby? What are modules? And what's the difference?

## Testing Questions

* What are some advantages/disadvantages to testing your code?
* What tools would you use to test your code's functionality?
* What is the difference between a unit test and a functional/integration test?
* What is the purpose of a code style linting tool?
* What is End-to-end (E2E) testing? How can it be implemented in frameworks like Angular and Rails?

## Coding Questions:

*Question: What is the value of `foo`?*
```javascript
var foo = 10 + '20';
```

*Question: How would you make this work?*
```javascript
add(2, 5); // 7
add(2)(5); // 7
```

*Question: What value is returned from the following statement?*
```javascript
"i'm a lasagna hog".split("").reverse().join("");
```

*Question: What is the outcome of the two alerts below?*
```javascript
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```

*Question: What is the value of `foo.length`?*
```javascript
var foo = [];
foo.push(1);
foo.push(2);
```

*Question: What is the value of `foo.x`?*
```javascript
var foo = {n: 1};
var bar = foo;
foo.x = foo = {n: 2};
```

*Question: What does the following code print?*
```javascript
console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
```

## Fun Questions:

* What's a cool project that you've recently worked on?
* What are some things you like about the developer tools you use?
* Do you have any pet projects? What kind?
* How do you like your coffee?
