# CSS Pseudo-Classes & Pseudo-Elements Cheat Sheet 🧠🎨

## 🎯 Pseudo-Classes

### 1. `:first-child`
Selects the first child of its parent.
```css
div:first-child {
  color: red;
}

:first-of-type
Selects the first element of its type among siblings.

css
Copy
Edit
p:first-of-type {
  font-weight: bold;
}

:last-child
Selects the last child of its parent.

css
Copy
Edit
li:last-child {
  background-color: lightgray;
}
4. :last-of-type
Selects the last element of its type among siblings.

css
Copy
Edit
div:last-of-type {
  border: 2px solid blue;
}
5. :nth-child(n)
Selects the nth child of its parent.

css
Copy
Edit
li:nth-child(2) {
  color: green;
}
6. :nth-of-type(n)
Selects the nth element of its type among siblings.

css
Copy
Edit
p:nth-of-type(3) {
  font-size: 1.5rem;
}
7. :root
Selects the root element of the document (usually <html>).

css
Copy
Edit
:root {
  --primary-color: #ff6600;
}
8. :not(selector)
Selects every element that does not match the selector.

css
Copy
Edit
div:not(.skip) {
  padding: 10px;
}
9. :empty
Selects elements with no children (including no text).

css
Copy
Edit
div:empty {
  display: none;
}
✨ Pseudo-Elements
10. ::first-letter
Selects the first letter of the element’s text.

css
Copy
Edit
p::first-letter {
  font-size: 2rem;
  color: purple;
}
11. ::first-line
Selects the first visible line of text.

css
Copy
Edit
p::first-line {
  text-transform: uppercase;
}
12. ::selection
Styles text selected by the user.

css
Copy
Edit
::selection {
  background: yellow;
  color: black;
}
✅ Use : for pseudo-classes and :: for pseudo-elements (double colon preferred for modern browsers).
Happy Styling! ✨

yaml
Copy
Edit

---

Agar tu chaahe toh main isko `.md` file bana ke bhi de sakta hoon download ke liye. Bata dena.







You said:
markdown file me sabko ek sath likh ke do mere bhai 


ChatGPT said:
Bhai, neeche poora markdown file ka content ek hi block me diya gaya hai — saare pseudo-classes aur pseudo-elements ek saath likhe gaye hain, ready to copy-paste in your .md file:

markdown
Copy
Edit
# 🎨 CSS Pseudo-Classes & Pseudo-Elements Cheat Sheet

This markdown file includes examples and explanations for important CSS pseudo-classes and pseudo-elements.

---

## 🟢 Pseudo-Classes

### 1. `:first-child`
Selects the first child of its parent.

```css
div:first-child {
  color: red;
}
2. :first-of-type
Selects the first element of its type among siblings.

css
Copy
Edit
p:first-of-type {
  font-weight: bold;
}
3. :last-child
Selects the last child of its parent.

css
Copy
Edit
li:last-child {
  background-color: lightgray;
}
4. :last-of-type
Selects the last element of its type among siblings.

css
Copy
Edit
div:last-of-type {
  border: 2px solid blue;
}
5. :nth-child(n)
Selects the nth child of its parent (regardless of type).

css
Copy
Edit
li:nth-child(2) {
  color: green;
}
6. :nth-of-type(n)
Selects the nth element of its type among siblings.

css
Copy
Edit
p:nth-of-type(3) {
  font-size: 1.5rem;
}
7. :root
Selects the root element of the document (usually <html>).

css
Copy
Edit
:root {
  --main-color: #ff6600;
}
8. :not(selector)
Selects elements that do not match the given selector.

css
Copy
Edit
div:not(.exclude) {
  padding: 10px;
}
9. :empty
Selects elements with no children (including no text or comments).

css
Copy
Edit
div:empty {
  display: none;
}
🟣 Pseudo-Elements
10. ::first-letter
Selects the first letter of the text in an element.

css
Copy
Edit
p::first-letter {
  font-size: 2rem;
  color: purple;
}
11. ::first-line
Selects the first line of text in an element (depends on width).

css
p::first-line {
  text-transform: uppercase;
}
12. ::selection
Applies styles to the text selected by the user.

css
::selection {
  background: yellow;
  color: black;
}