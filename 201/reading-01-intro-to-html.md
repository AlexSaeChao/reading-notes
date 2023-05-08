# Code 201 - Foundations of Software Development
Overview of reading notes
These reading notes will be important as they provide a quick overview of the workings of the web and will provide a quick summary of how HTML, CSS, and JavaScript works.

## Getting Started

1. Compose a short poem describing how HTTP sends data between computers.

HTTP is the messenger swift with this task,
Fetch us the resources we ask,

With TCP as the messenger's trusty shield,
Ensuring our message arrive on the battlefield,

Headers and bodies are what they describe,
Delivering the requests, to the server tribe

With the response it frees
Until the task is done with ease.

2. How HTML, CSS, and JS files are “parsed” in the browser.

* When web browsers request HTML files from servers, looking for link elements refering to CSS and script elements refering to JavaScript.

* Reading the HTML from top to bottom then it generates the DOM which is the structure of the html from the tags.

* These elements will be referencing external CSS and JavaScript files. The order in which HTML, CSS, and JS files are “parsed” is important in how pages are loaded onto a page.

* As the HTML is parsed, the web browser will request to the server for CSS links to be parsed with CSSOM and then finally parsing the Javascript scripts.


3. How can you find images to add to a Website?

Images found on google with the creative commons license are free to use. Unsplash is another great resource to find images.

4. How do you create a String vs a Number in JavaScript?

For strings you can add single quotes '' and backticks `` surrounding characters you want as a string. For numbers you can use a number constructor to make the string or number value after declaring the variable keyware and the variable name.

5. What is a Variable and why are they important in JavaScript?

A variable is important because it bascially is a container hold a set of data. This is important because you can declare the variable and reuse that variable with the assign varible name.

## Introduction to HTML

1. What is an HTML attribute?
An atribute has additional information about how an element should be renderd or behave.

2. Describe the Anatomy of an HTMl element.

  * Opening Tag: names of the type of element you are wanting to use, is usually paired with the closing tag. ie. `<p>`

  * Attributes: if nessasary there may be attributes tha decribe how the content should be rendered or behave.

  * Contents: text that is contained in the opening and closing tags For example,`<p>Hello, world!</p>` has the content "Hello, world!".

  * Closing Tag: denotes the end of the element with a slash before the element ie. `</p>`

3. What is the Difference between < article> and < section> element tags?

Articles tags are used when show a complete or self contained piece of content like blogs and news articles are used for stand alone piece of content. While Sections tags are used to group related content together like chapters.

4. What Elements does a “typical” website include?

* Headers: Titles, a larger heading, or a tagline.
* Nav Bar: main place to have links to other pages of the site.
* Content: the actual content you want to display be it text, images, videos.
* Sidebar: usually has extra information and its usually connected to the content.
* Footer: generally contains fine print copyright notices and contact info.

5. How does metadata influence Search Engine Optimization?

Metadata can influence SEO (Search Engine Optimization) by letting you to input relevant information or descriptions about your page like keywords related to the content to help your pages hit ranking in search engines.

6. How is the HTML tag used when specifying metadata?

The `<meta>` element is placed in the `<head>` element. The meta tag contains characters, descriptions about your page, keywords, the author information, and etc.

## Miscellaneous

### How to start to design a Website.

1. What is the first step to designing a Website?

Defining the purpose and goals of the website.

2. What is the most important question to answer when designing a Website?

Who is the target audience and who is this website for? Does this target their needs and goals?

### Semantics

1. What are the benefits of using semantic tags in our HTML?

Semantic tags benefits accessibility, for the use of SEOs, readbility for screen readers, to provide consistent and standardized way to structure the content of the page.

2. Why should you use an `<h1>` element over a `<span>` element to display a top level heading?
H1 has more impact in the its ranking for SEO and is the top-level heading for accessibility.

### What is JavaScript?

1. Describe 2 things that require JavaScript in the Browser?

Dynamic content for creating interactive elements ofthe page like input and button clicks. Form validation can help make sure that the user has provided the correct information.

2. How can you add JavaScript to an HTML document?

You can add JavaScript to an HTML document by linking an external ccs file in the head.
Internal styling which is within the footer of the HTML document
or inline which is contained in the element tag which has the high priority.

## Things I want to know more about

Nothing at this time.