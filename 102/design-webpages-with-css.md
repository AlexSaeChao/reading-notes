# Design Webpages with CSS

CSS syntax has the html tag with curly brakets. Inside the brakets have declaration(s) that will effect the properties and values of the color, size, or where it lives on the HTML page. The last question for the reading you can see that the ``<p>`` element has red as its declared color. You can place it in it's own CSS file or directly into the HTML document.  

## Questions for reading 05

* What is the purpose of CSS? **The purpose of CSS (Cascading Style Sheets) is to control the layout, design, and presentation of the HTML page. Think of CSS as the instructions to paint a house while HTML is the foundation and frames of a home.**
* What are the three ways to insert CSS into your project? **External CSS: using a ``<link>`` tag to connect a CSS file to an HTML Document, this has the lowest priority of the 3. Internal CSS: adding CSS rules directly into the head section of an HTML document, using the ``<style>`` tag this has a higher priority than External CSS. Inline CSS: This involves adding CSS rules directly into the HTML elements themselves, using the style attribute. This one has the highest priority**
* Write an example of a CSS rule that would give all <p> elements red text.
``p {
  color: red;
}``