# JavaScript

## Introduction

Often abbreviated as **JS**, is a [high-level](https://en.wikipedia.org/wiki/High-level_programming_language), [dynamic](https://en.wikipedia.org/wiki/Dynamic_programming_language), [weakly typed](https://en.wikipedia.org/wiki/Strong_and_weak_typing#Definitions_of_.22strong.22_or_.22weak.22), [object-based](https://en.wikipedia.org/wiki/Object-based_language), [multi-paradigm](https://en.wikipedia.org/wiki/Multi-paradigm_programming_language), and [interpreted](https://en.wikipedia.org/wiki/Interpreted_language) [programming language](https://en.wikipedia.org/wiki/Programming_language). Alongside HTML and CSS, JavaScript is one of the three core technologies of [World Wide Web](https://en.wikipedia.org/wiki/World_Wide_Web) content production.

> Please, do not confuse Java with JavaScript, althought they have similarities, they're way different in design.

Javascript is able to add [interactivity](https://en.wikipedia.org/wiki/Interactivity) to your website, for example, **online games** (you probably know the *Dino Game* from Google Chrome when you are offline), responses when a button is pressed (*let's say, you press a button and it dissapears, unlocking a popup somewhere in the page*) or data is being entered, dynamic styling (such as hiding/showing the navigation menu, turn the page's background colour from white to dark grey...), animation (moving elements in the page with some fancy movements, such as transitions or a character's movement in an online game)...

Let's start with something basic for web browsers!

It's a good practise to have your files organized in different folders: `img`, `scripts`... let's create a `main.js` file inside your new `scripts` folder:

```text
├ Test website
├── img
├─┬ scripts
│ └── main.js
└── index.html
```

```html
<body>
    <h1>
        Testing...
    </h1>
    <script src="scripts/main.js"></script>
</body>
```

> The script's src does the same job as the link element for CSS — it applies the JavaScript to the page, so it can have an effect on the HTML (along with the CSS, and anything else on the page).

And now, in your `scripts/main.js` file:

```javascript
var myHeading = document.querySelector('h1');
myHeading.textContent = 'Hello world!';
```

Make sure all files are saved, and open your `index.html` file from your project's root.

> The reason we've put the script element near the bottom of the HTML file is that HTML is loaded by the browser in the order it appears in the file. If the JavaScript is loaded first and it is supposed to affect the HTML below it, it might not work, as the JavaScript would be loaded before the HTML it is supposed to work on. Therefore, putting JavaScript near the bottom of the HTML page is often the best strategy.

**What happened?**

Your heading text has changed to `Hello World!` using JavaScript, as I mentioned before, the page is loaded when that function got executed, so it has fetched an element which tag is `h1`, and changed the contents from it. In this case, its text.

Want to learn more? Check the following links:

- [Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics) — Most recommended for JS, it has plenty documentation for everything that is implemented in JS, always up-to-date and maintained by the community — it contains the reference of the entire language.
- [Eloquent JavaScript](http://eloquentjavascript.net/) — Free book, check description in the link.
- [CodeCademy Course](https://www.codecademy.com/learn/introduction-to-javascript) — Oriented for browser development, it comes with a lot of content.

And... for Node.js people:

- [NodeSchool](https://nodeschool.io/) — Plenty of information.
- [CodeSchool](https://www.codeschool.com/courses/real-time-web-with-node-js) — Free course for Node.js, teaches you how to write server-side code and build lightweight, scalable network applications.
