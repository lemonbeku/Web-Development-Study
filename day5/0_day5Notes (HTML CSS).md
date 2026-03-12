Here are **clean, structured Obsidian-style notes** based on the material. I organized them so they are easier to review when studying web development.

---

# HTML Styles CSS

## What is CSS

**CSS (Cascading Style Sheets)** is used to control the **appearance and layout of webpages**.

It allows developers to style HTML elements such as:

* Text color
* Fonts
* Text size
* Spacing between elements
* Element positioning
* Layout structure
* Background colors or images
* Responsive display for different screen sizes

**Main idea:**
CSS separates **content (HTML)** from **design (CSS)**.

### Why CSS is Important

* Saves a lot of work
* Can control **multiple pages at once**
* Keeps code **clean and organized**

Example uses:

* Manipulating text
* Adding colors
* Styling boxes and layouts

---

# Cascading Concept

The word **cascading** means styles can **inherit from parent elements**.

Example:

If you set the body text color to blue:

```
body {
  color: blue;
}
```

Then all child elements will also become blue unless another style overrides it.

Affected elements may include:

* headings `<h1>–<h6>`
* paragraphs `<p>`
* lists
* other text elements

---

# Ways to Add CSS

CSS can be applied in **three ways**:

1. Inline CSS
2. Internal CSS
3. External CSS

---

# Inline CSS

Inline CSS is used to apply **a style to a single HTML element**.

It uses the **style attribute inside the HTML tag**.

Example:

```html
<h1 style="color:blue;">A Blue Heading</h1>

<p style="color:red;">A red paragraph.</p>
```

Characteristics:

* Applies to **only one element**
* Quick for testing
* Not recommended for large projects

---

# Internal CSS

Internal CSS is used to style **a single HTML page**.

It is placed inside the `<style>` tag within the `<head>` section.

Example:

```html
<!DOCTYPE html>
<html>
<head>
<style>
body {background-color: powderblue;}
h1 {color: blue;}
p {color: red;}
</style>
</head>

<body>
<h1>This is a heading</h1>
<p>This is a paragraph.</p>
</body>
</html>
```

Characteristics:

* Affects **all matching elements on that page**
* Good for **small websites or single pages**

---

# External CSS

External CSS is used to style **multiple HTML pages**.

CSS rules are placed in a **separate .css file**.

Example HTML:

```html
<link rel="stylesheet" href="styles.css">
```

Example CSS file:

```css
body {
  background-color: powderblue;
}

h1 {
  color: blue;
}

p {
  color: red;
}
```

Characteristics:

* Most common method
* Keeps HTML clean
* Allows styling **entire websites from one file**

---

# Linking External CSS

External stylesheets can be linked in three ways.

### Full URL

```html
<link rel="stylesheet" href="https://www.w3schools.com/html/styles.css">
```

### Absolute Path

```html
<link rel="stylesheet" href="/html/styles.css">
```

### Relative Path

```html
<link rel="stylesheet" href="styles.css">
```

---

# Common CSS Properties

## Text Color

Defines the color of text.

```css
color: blue;
```

---

## Font Family

Defines the font used.

```css
font-family: verdana;
```

---

## Font Size

Defines the size of text.

```css
font-size: 300%;
```

Example:

```css
h1 {
  color: blue;
  font-family: verdana;
  font-size: 300%;
}

p {
  color: red;
  font-family: courier;
  font-size: 160%;
}
```

---

# CSS Border

The **border property** adds a border around an element.

Example:

```css
p {
  border: 2px solid powderblue;
}
```

Components:

* border width
* border style
* border color

---

# CSS Padding

Padding defines the **space between text and the border**.

Example:

```css
p {
  border: 2px solid powderblue;
  padding: 30px;
}
```

Visualization:

```
Border
  Padding
    Content
```

---

# CSS Margin

Margin defines the **space outside the border**.

Example:

```css
p {
  border: 2px solid powderblue;
  margin: 50px;
}
```

Visualization:

```
Margin
  Border
    Padding
      Content
```

---

# CSS Layout Structure Concept

A styled element can be visualized as:

```
Margin (outside space)
   Border
      Padding
         Content
```

This is called the **CSS Box Model**.

---
