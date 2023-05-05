# HTML Links, JS Functions, and Intro to CSS Layout

These are important to what I am learning so far because links are everywhere, we have to understand the bread and butter of JS (functions), and starting to make our websites pretty.

## Learn HTML

1. To create a basic link, we wrap text or other content inside what element?

* We use an Anchor tag. We wrap the text or content in `<a>` element to open and `</a>` to close it.

2. The href attribute contains what information?

* Href attribute contains the URL for the html files, test files, images, text documents, video or audio files.

3. What are some ways we can ensure links on our pages are accessible to all readers?

* We can use descriptive link text, keeping the decriptions short for screen readers, and not repeating the url links everywhere on the page will help iur page to be accessible to all readers.

## CSS Layout

1. What is meant by “normal flow”?

* Normal flow is talking about the default layout or postioning without any thing applied from CSS yet.They arange themselves in the page the way it was laid out in the HTML file (like bones to a person or the foundation and wood used in homes). They are placed on the page according to their default display propert

2. What are a few differences between block-level and inline elements?

* Block-level elements start on the next new line, the elements are laid out vertically. Inline elements start on the same line as long as they have room to fit on the page.

3. ___ positioning is the default for every html element.

* Static positioning is the default for every html element. Meaning they will be displayed with it's default behavior.

4. Name a few advantages to using absolute positioning on an element.

  You can isolate elements on a page so it does not interfere with the layout of the other elements to make really cool things like UI features. For example popup info boxes, control menus, and other features that can be draged and dropped on the page with UI.

5. What is a key difference between fixed positioning and absolute positioning?

   * Fixed positioning positions an element relative to the browser window, while absolute positioning positions an element relative to its nearest positioned ancestor. This means that an element with fixed positioning will stay in the same position on the page even when the user scrolls like the popup box that scoll with the page, while an element with absolute positioning will move with its parent element if the parent element is scrolled. this would be good for a fixed header with the absolute positioning of a fixed top value so it remains in the same position while scrolling so the user will have quick access to the nav bar or other useful info without having to scroll to the top.

## Learn JS

1. Describe the difference between a function declaration and a function invocation.

* A function declaration is like a container that holds a set of instructions, and it is defined to be used later on when it is invoked. When the function is invoked, the code inside the function is executed. The function can take in arguments, process them, and then return a value or perform a specific action.

2. What is the difference between a parameter and an argument?

* When the function is invoked, the code inside the function is executed. The function can take in arguments, process them, and then return a value or perform a specific action. Meaning it calls back and executes the code inside.

## Miscellaneous

* Pick 2 benefits to pair programming and reflect on how these benefits could help you on your coding journey.
  * for me the 2 most beneficial parts of pair programming areSocial Skills and Job readiness interviews. Learning to communicate the best way to make sure minimal misunderstandings happen and working as part of a team is a must. to be honest it's probably what I need to work on the most.

## Things I want to know more about
* Relative Postioning leaves space behind so that the other elements still intract with the box model .
* Giving an absolute postion to an element, it's space gets elimnated. and content can move behind it.


### References
* [Reading for HTML hyperlinks](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks)
* [CSS Normal Flow](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Normal_Flow)
* [CSS Layout postion](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning)
* [JS Functions - reusable blocks of code](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Functions)
* [6 benefits of pair programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)
