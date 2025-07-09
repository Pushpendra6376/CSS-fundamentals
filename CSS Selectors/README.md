
# CSS Selectors

CSS selectors are patterns used to select elements in a document. They are used in CSS to apply styles to HTML elements. Here are some common types of CSS selectors:

## Basic Selectors
- **Universal Selector (`*`)**: Selects all elements.
- **Type Selector (`element`)**: Selects all elements of a given type (e.g., `div`, `p`, `span`).
- **Class Selector (`.class`)**: Selects all elements with a specific class.
- **ID Selector (`#id`)**: Selects a single element with a specific ID.
- **Attribute Selector (`[attribute]`)**: Selects elements with a specific attribute.
- **Pseudo-class Selector (`:pseudo-class`)**: Selects elements based on their state (e.g., `:hover`, `:focus`).
## Combinators
- **Descendant Selector (`ancestor descendant`)**: Selects elements that are descendants of a specified ancestor.
- **Child Selector (`parent > child`)**: Selects elements that are direct children of a specified parent.
- **Adjacent Sibling Selector (`previous + next`)**: Selects an element that is immediately preceded by a specified element.
- **General Sibling Selector (`previous ~ siblings`)**: Selects all siblings that follow a specified element.
## Grouping Selectors
- **Grouping Selector (`selector1, selector2`)**: Groups multiple selectors to apply the same styles to different elements.
## Attribute Selectors
- **Attribute Selector with Value (`[attribute="value"]`)**: Selects elements with a specific attribute value.
- **Attribute Selector with Partial Value (`[attribute*="value"]`)**: Selects elements with an attribute that contains a specific value.
- **Attribute Selector with Prefix (`[attribute^="value"]`)**: Selects elements with an attribute that starts with a specific value.
- **Attribute Selector with Suffix (`[attribute$="value"]`)**: Selects elements with an attribute that ends with a specific value.
## Pseudo-classes
- **:first-child**: Selects the first child of a parent element.
- **:last-child**: Selects the last child of a parent element.
- **:nth-child(n)**: Selects the nth child of a parent element.
- **:nth-of-type(n)**: Selects the nth child of a specific type within a parent element.
- **:not(selector)**: Selects elements that do not match a specified selector.
- **:empty**: Selects elements that have no children.
- **:checked**: Selects checked input elements (e.g., checkboxes, radio buttons).
- **:disabled**: Selects disabled form elements.
- **:enabled**: Selects enabled form elements.
- **:active**: Selects elements that are currently being activated by the user (e.g., clicked).
- **:focus**: Selects elements that are currently focused (e.g., input fields).
- **:hover**: Selects elements that are currently being hovered over by the user.
- **:visited**: Selects links that have been visited by the user.
- **:link**: Selects links that have not been visited by the user.
- **:first-of-type**: Selects the first element of its type within a parent.
- **:last-of-type**: Selects the last element of its type within a parent.
- **:nth-last-child(n)**: Selects the nth child from the end of a parent element.
- **:nth-last-of-type(n)**: Selects the nth child of a specific type from the end of a parent element.
- **:root**: Selects the root element of the document (usually the `<html>` element).
- **:lang(language)**: Selects elements based on their language attribute.
- **:target**: Selects the element that is currently targeted by a fragment identifier in the URL (e.g., `#section1`).
- **:before**: Inserts content before an element.
- **:after**: Inserts content after an element.
- **:first-letter**: Selects the first letter of an element.
- **:first-line**: Selects the first line of an element.
- **:placeholder-shown**: Selects input elements that are currently showing placeholder text.
- **:valid**: Selects form elements that are valid according to their validation rules.
- **:invalid**: Selects form elements that are invalid according to their validation rules.
- **:in-range**: Selects input elements with a value within a specified range.
- **:out-of-range**: Selects input elements with a value outside a specified range.
- **:required**: Selects form elements that are required.
- **:optional**: Selects form elements that are optional.
- **:dir(direction)**: Selects elements based on their text direction (e.g., `ltr`, `rtl`).
## Pseudo-elements
- **::before**: Inserts content before an element.
- **::after**: Inserts content after an element.
- **::first-letter**: Selects the first letter of an element.
- **::first-line**: Selects the first line of an element.   
- **::selection**: Selects the portion of an element that has been highlighted by the user.
- **::placeholder**: Selects the placeholder text of an input element.
- **::backdrop**: Selects the backdrop of a modal or dialog element.
- **::marker**: Selects the marker of a list item (e.g., bullet points in unordered lists).
- **::file-selector-button**: Selects the button of a file input element.
- **::spelling-error**: Selects text with a spelling error.
- **::grammar-error**: Selects text with a grammar error.
## Examples
```css
/* Select all paragraphs */
p {
    color: blue;
}
/* Select elements with class "highlight" */
.highlight {
    background-color: yellow;
}
/* Select the element with ID "header" */
#header {
    font-size: 24px;
}
/* Select all links that have been visited */
a:visited {
    color: purple;
}
/* Select the first child of a list */
ul li:first-child {
    font-weight: bold;
}
/* Select all input elements that are checked */
input:checked {
    background-color: lightgreen;
}
/* Select all elements with a data attribute */
[data-custom] {
    border: 1px solid black;
}
/* Select all elements that are not paragraphs */
:not(p) {
    color: red;
}
/* Select all elements with a specific attribute value */
[data-role="admin"] {
    background-color: lightgray;
}
/* Select all elements with a class that starts with "btn-" */
[class^="btn-"] {
    padding: 10px;
    border-radius: 5px;
}
/* Select all elements with a class that ends with "-active" */
[class$="-active"] {
    color: green;
}
/* Select all elements with a class that contains "nav" */
[class*="nav"] {
    font-weight: bold;
}
/* Select all elements that are direct children of a div */
div > p {
    margin: 0;
}
/* Select all paragraphs that are descendants of a section */
section p {
    font-style: italic;
}
/* Select all elements that are adjacent siblings */
h2 + p {
    margin-top: 10px;
}
/* Select all elements that are siblings of a specific element */
h2 ~ p {
    color: gray;
}
/* Select the first letter of all paragraphs */
p::first-letter {
    font-size: 2em;
    color: red;
}
/* Select the first line of all paragraphs */
p::first-line {
    font-weight: bold;
}
/* Select the placeholder text of input elements */
input::placeholder {
    color: lightgray;
}
/* Select the backdrop of a modal */
.modal::backdrop {
    background-color: rgba(0, 0, 0, 0.5);
}
/* Select the marker of list items */
li::marker {
    color: blue;
}
/* Select the button of a file input */
input::file-selector-button {
    background-color: lightblue;
    border: none;
    padding: 5px 10px;
}

/* Select text with a spelling error */
::spelling-error {
    background-color: yellow;
    text-decoration: underline;
}
/* Select text with a grammar error */
::grammar-error {
    background-color: lightcoral;
    text-decoration: underline;
}
/* Select elements based on text direction */
[dir="rtl"] {
    text-align: right;
}
/* Select elements that are currently focused */
input:focus {
    border: 2px solid blue;
}
/* Select elements that are currently hovered over */
a:hover {
    color: red;
}
/* Select elements that are currently active */
button:active {
    background-color: darkgray;
}
/* Select elements that are currently in a valid state */
input:valid {
    border-color: green;
}
/* Select elements that are currently in an invalid state */
input:invalid {
    border-color: red;
}
/* Select elements that are currently in range */
input:in-range {
    background-color: lightgreen;
}
/* Select elements that are currently out of range */
input:out-of-range {
    background-color: lightcoral;
}
/* Select required form elements */
input:required {
    border: 2px solid orange;
}
/* Select optional form elements */
input:optional {
    border: 2px dashed gray;
}
/* Select elements based on their language */
[lang="en"] {
    font-family: Arial, sans-serif;
}
/* Select the root element of the document */
:root {
    --main-color: blue;
}
/* Use a variable defined in the root element */
body {
    color: var(--main-color);
}
