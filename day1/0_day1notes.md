# Day 1 HT

Tags: #html #webdev #w3schools

---

## `html` Introduction

### What is HTML
- HTML stands for **HyperText Markup Language**
- It is the standard language for creating web pages
- HTML describes the **structure** of a webpage
- HTML consists of **elements** represented by **tags**
- A browser reads HTML and renders it visually

### What HTML Can Do
HTML can define:
- Headings
- Paragraphs
- Links
- Images
- Lists
- Tables
- Forms
- And more

HTML is **not a programming language**.  
It is a **markup language** used to structure content.

---

## `html` Editors

### How to Write HTML
You only need:
- A text editor
- A web browser

### Common Editors
- Notepad / Notepad++
- VS Code
- Sublime Text
- Online editors like W3Schools Tryit

### Basic Steps
1. Open a text editor
2. Write HTML code
3. Save file as `filename.html`
4. Open it in a browser

---

## `html` Basic Structure

### Minimal HTML Template
```html
<!DOCTYPE html>
<html>
<head>
    <title>Page Title</title>
</head>
<body>

    <h1>My First Heading</h1>
    <p>My first paragraph.</p>

</body>
</html>
```

### Explanation
- `<!DOCTYPE html>` → Declares the document type (HTML5)
- `<html>` → Root element of the page
- `<head>` → Contains metadata (title, styles, etc.)
- `<title>` → Title shown in browser tab
- `<body>` → Visible page content

---

## `html` Elements

### What is an HTML Element?
An element usually consists of:
- Opening tag
- Content
- Closing tag

Example:
```html
<p>This is a paragraph.</p>
```

Structure:
```html
<tagname>Content</tagname>
```

### Nested Elements
HTML elements can be inside other elements:
```html
<p>This is <b>bold</b> text.</p>
```

### Empty Elements
Some elements have no closing tag:
```html
<br>
<hr>
<img>
```

---

## `html` Basic Elements

### Headings
```html
<h1>Main Heading</h1>
<h2>Sub Heading</h2>
<h3>Smaller Heading</h3>
```
- `<h1>` is the most important
- `<h6>` is the least important

### Paragraph
```html
<p>This is a paragraph.</p>
```

### Links
```html
<a href="https://www.example.com">Visit Example</a>
```

### Images
```html
<img src="image.jpg" alt="Description of image">
```

### Line Break
```html
<br>
```

---

## `html` Attributes

### What Are Attributes?
- Provide extra information about elements
- Written inside the opening tag
- Usually written as `name="value"`

Example:
```html
<a href="https://www.google.com">Google</a>
```

Here:
- `href` is the attribute
- The URL is the value

### Common Attributes
- `href` → link destination (a)
- `src` → image source (img)
- `alt` → alternative text for images (img)
- `style` → inline styling (any element)
- `title` → extra information (tooltip) (p or any element)
- `lang` → language of document (used in `<html>`)

Example:
```html
<html lang="en">
```

---

## Important Rules I Learned

- HTML is case-insensitive (but lowercase is recommended)
- Attributes should always be quoted
- Proper nesting matters
- Indentation improves readability
- Always include `<!DOCTYPE html>`

---

## Personal Reflection Day 1

Today I learned:
- What HTML is and why it is important
- How browsers interpret HTML
- The basic structure of a webpage
- The difference between elements and attributes
- How to create headings, paragraphs, links, and images
- Attrivutes
