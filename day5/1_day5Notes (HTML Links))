# HTML Links

Links are found in nearly all web pages. They allow users to move from one page to another.

In HTML, links are called **hyperlinks**.

When a user clicks a hyperlink, the browser opens another document or resource.

When the mouse pointer moves over a link, it changes into a **hand pointer**.

Important:
Links do not have to be text. Links can also be:
- Images
- Buttons
- Other HTML elements

---

# HTML Hyperlink Syntax

The HTML `<a>` tag defines a hyperlink.

Syntax:

<a href="url">link text</a>

Explanation:

`<a>`  
Anchor tag used to create hyperlinks.

`href`  
Specifies the destination URL.

`link text`  
The visible and clickable text.

Example:

<a href="https://www.w3schools.com/">Visit W3Schools.com!</a>

Clicking the link text sends the user to the specified URL.

---

# Default Link Appearance

By default, browsers display links as:

Unvisited link  
Blue and underlined

Visited link  
Purple and underlined

Active link  
Red and underlined

These styles can be customized using **CSS**.

---

# The target Attribute

The `target` attribute specifies **where the linked document will open**.

Syntax:

<a href="url" target="value">link text</a>

Common values:

_self  
Default behavior. Opens the link in the **same tab or window**.

_blank  
Opens the link in a **new tab or window**.

_parent  
Opens the link in the **parent frame**.

_top  
Opens the link in the **full window**, removing frames.

Example:

<a href="https://www.w3schools.com/" target="_blank">Visit W3Schools</a>

This opens the link in a **new tab**.

---

# Absolute URLs vs Relative URLs

## Absolute URL

An **absolute URL** is a complete web address.

Example:

<a href="https://www.google.com/">Google</a>

Characteristics:
- Includes protocol (`https://`)
- Includes domain name
- Can link to external websites

Example:

<a href="https://www.w3.org/">W3C</a>

---

## Relative URL

A **relative URL** links to another page within the same website.

It does not include the domain name.

Example:

<a href="html_images.asp">HTML Images</a>

Example linking to a folder:

<a href="/css/default.asp">CSS Tutorial</a>

Relative URLs are used for **internal navigation**.

---

# Using an Image as a Link

An image can be used as a link by placing the `<img>` tag inside the `<a>` tag.

Example:

<a href="default.asp">
<img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
</a>

When the user clicks the image, the browser opens the linked page.

---

# Link to an Email Address

You can create a link that opens the user's **email program**.

This uses the `mailto:` scheme.

Example:

<a href="mailto:someone@example.com">Send email</a>

When clicked:
- The user's email program opens
- A new email message is created

---

# Button as a Link

Buttons do not act as links by default.

To make a button navigate to another page, **JavaScript** is used.

Example:

<button onclick="document.location='default.asp'">
HTML Tutorial
</button>

When clicked, the browser goes to `default.asp`.

---

# Link Titles

The `title` attribute provides **extra information about an element**.

This information appears as a **tooltip** when the mouse hovers over the link.

Example:

<a href="https://www.w3schools.com/html/" title="Go to W3Schools HTML section">
Visit our HTML Tutorial
</a>

---

# File Path Examples

Full URL (external site):

<a href="https://www.w3schools.com/html/default.asp">
HTML tutorial
</a>

File inside a folder:

<a href="/html/default.asp">
HTML tutorial
</a>

File in the same folder:

<a href="default.asp">
HTML tutorial
</a>

Understanding file paths is important when organizing website pages.

---

# HTML Links Different Colors

HTML links can appear in different colors depending on their **state**.

Link states include:

- Unvisited
- Visited
- Hover
- Active

---

# Default Link Colors

By default:

Unvisited link  
Blue and underlined

Visited link  
Purple and underlined

Active link  
Red and underlined

These styles can be customized using **CSS**.

---

# Changing Link Colors with CSS

CSS pseudo-classes allow styling links depending on their state.

Example:

<style>

a:link {
  color: green;
  background-color: transparent;
  text-decoration: none;
}

a:visited {
  color: pink;
  background-color: transparent;
  text-decoration: none;
}

a:hover {
  color: red;
  background-color: transparent;
  text-decoration: underline;
}

a:active {
  color: yellow;
  background-color: transparent;
  text-decoration: underline;
}

</style>

Explanation:

a:link  
Styles **unvisited links**.

a:visited  
Styles links that have already been clicked.

a:hover  
Styles links when the mouse pointer is over them.

a:active  
Styles links while they are being clicked.

---

# Link Buttons

Links can be styled to look like **buttons** using CSS.

Example:

<style>

a:link, a:visited {
  background-color: #f44336;
  color: white;
  padding: 15px 25px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
}

a:hover, a:active {
  background-color: red;
}

</style>

Explanation:

background-color  
Sets the button background color.

color  
Sets the text color.

padding  
Adds space inside the button.

text-align  
Centers the text.

text-decoration  
Removes underline.

display: inline-block  
Allows the link to behave like a block element.

---

# HTML Links Create Bookmarks

HTML links can be used to create **bookmarks**, allowing users to jump to specific sections of a webpage.

Bookmarks are useful for:
- Long pages
- Documentation
- Tutorials
- Table of contents navigation

---

# Creating a Bookmark

Step 1: Create the bookmark using the `id` attribute.

Example:

<h2 id="C4">Chapter 4</h2>

This creates a bookmark called **C4**.

---

# Linking to a Bookmark on the Same Page

Example:

<a href="#C4">Jump to Chapter 4</a>

When clicked, the page scrolls to the element with `id="C4"`.

---

# Linking to a Bookmark on Another Page

Example:

<a href="html_demo.html#C4">Jump to Chapter 4</a>

This will:
1. Open `html_demo.html`
2. Scroll to the section with `id="C4"`

---

# HTML Link Tag

<a>  
Defines a hyperlink used to navigate between web pages or sections.