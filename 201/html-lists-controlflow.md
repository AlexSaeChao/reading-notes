# HTML Lists, Control Flow with JS, and the CSS Box Model

## Learn HTML

1. When should you use an unordered list in your HTML document?

* You should should use an unordered list when the order of the list does not matter. no indcation of any sequence or order.

2. How do you change the bullet style of unordered list items?

* Using CSS you can change the bullet styles. using a list-style-type property can be used to specify the type of marker or bullet that can be used for the list of items 

3. When should you use an ordered list vs an unorder list in your HTML document?

* If ranking or order is involved, you should use an ordered list. Unordered lists should be used if there is not hierarchy or rank to the list.

4. Describe two ways you can change the numbers on list items provided by an ordered list?
Learn CSS

* With CSS you can change normal numbers to lower-roman numerals.(i, ii, iii, iv, v, etc) there is also decimals to display regular numbers (1, 2, 3, 4, 5, etc.) 

## Learn CSS 
### The Box Model.

1. Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?

* The box model, picture a house (the border) with an adjustable fence that is always planted in the ground, you can move it around and the content outside the fence can and should move away or closer unless it is another house that has a rigid fence already. Padding, you can think of them as adjustable containers in the house itself. You can have multiple containers (other content) move them in and around the house. Though things may over lap and the contents of the containers may spill out.

2. List and describe the four parts of an HTML elements box as referred to by the box model.

* Content: The actual content of the element, like text, images
* Padding: The space between the content and the border of the element.
* Border: The line or area that surrounds the padding and content.
* Margin: The space outside the border that separates the element from other elements in the page layout.

## Learn JS

### Arrays. Operators and Expressions. Conditionals. Loops.


1. What data types can you store inside of an Array?

* In js you can store any data type in the array. Numbers, Strings, objects, even functions.

2. Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?

* Think of it like a narrow excel sheet, a military map, or the game battleship. You can access the stored values with coordinates. Lets say you have a list of names and indexing (starting) at 0 for the first value

example below:
```
const people = ['Kevin', 'Patty', 'Zeke'];
console.log(people[2]);

//  would be Zeke at the index of 2 and would be logged in the console.

```

* This people array would be a valid JavaScript. For example you can access the value of 'accountant' with `people[1][2]`

```
 const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];
 ```

3. List five shorthand operators for assignment in javascript and describe what they do.

* `++`: Increments the value of a variable by one. Example: `a++;` is equivalent to `a = a + 1;`
* `--`: Decrements the value of a variable by one. Example: `a--;` is equivalent to `a = a - 1;`
* `+=`: Adds the right operand to the left operand and assigns the result to the left operand. Example: `a += 7;` is equivalent to `a = a + 7;`
* `-=`: Subtracts the right operand from the left operand and assigns the result to the left operand. Example: `a -= 4;` is equivalent to `a = a - 4;`
* `*=`: Multiplies the left operand by the right operand and assigns the result to the left operand. Example: `a *= 5;` is equivalent to `a = a * 5;`

4. Read the code below and evaluate the last expression and explain what the result would be and why.

* It would evaluate to `'10dog'` It would take the value 10 with the boolean false which is considered to be the value 0 (`10 + 0`) after converting thesum of those values into a string then tack on dog within the string.

```
 let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;
```

1. Describe a real world example of when a conditional statement should be used in a JavaScript program.

* if a site for voting for 18+ asks you how old you are (prompt) and you input that you are younger (the comparison happens here)then it says that you are not able to vote yet. Else if you are 18 then you are able to vote and will take you to the site to see the polls.

2. Give an example of when a Loop is useful in JavaScript.

* A loop is useful when you have to perform a task that is repetitive until it meets a certain condition.
