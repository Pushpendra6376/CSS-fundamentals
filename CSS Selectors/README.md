# CSS Selectors Guide

This repository contains a comprehensive guide to **CSS Selectors** – the fundamental building blocks used to target and style HTML elements.

## 📌 What are CSS Selectors?

CSS selectors are patterns used in stylesheets to select HTML elements and apply styles to them. This guide includes explanations, examples, and syntax for:

- Basic selectors
- Combinators
- Attribute selectors
- Pseudo-classes
- Pseudo-elements
- Real-world examples

---

## 🔹 Basic Selectors
- `*` – Universal selector  
- `element` – Type selector  
- `.class` – Class selector  
- `#id` – ID selector  
- `[attribute]` – Attribute selector  
- `:pseudo-class` – Pseudo-class selector  

## 🔹 Combinators
- `ancestor descendant` – Descendant selector  
- `parent > child` – Child selector  
- `prev + next` – Adjacent sibling  
- `prev ~ siblings` – General sibling  

## 🔹 Grouping Selectors
- `selector1, selector2` – Apply same styles to multiple selectors

## 🔹 Attribute Selectors
- `[attribute="value"]`  
- `[attribute*="value"]`  
- `[attribute^="value"]`  
- `[attribute$="value"]`

## 🔹 Pseudo-classes
Examples:  
`:first-child`, `:last-child`, `:nth-child(n)`, `:hover`, `:checked`, `:disabled`, `:not(selector)`, `:focus`, `:required`, etc.

## 🔹 Pseudo-elements
Examples:  
`::before`, `::after`, `::first-letter`, `::selection`, `::placeholder`, `::backdrop`, `::marker`

---

## 🧪 Examples
```css
/* Select all paragraphs */
p {
  color: blue;
}

/* Select elements with class 'highlight' */
.highlight {
  background-color: yellow;
}

/* Select first letter of paragraph */
p::first-letter {
  font-size: 2em;
  color: red;
}

/* Input elements in valid state */
input:valid {
  border-color: green;
}
