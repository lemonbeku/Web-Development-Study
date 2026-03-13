# HTML Favicon

A **favicon** is a small icon shown **next to the page title in the browser tab**.

Example location:

```
[icon] My Website Title
```

Favicons help users **identify a website quickly** when multiple tabs are open.

---

# How to Add a Favicon

Steps:

1. Create or download a favicon image.
2. Place the image in your website folder.
3. Add a `<link>` tag inside the `<head>` section.

Example:

```html
<!DOCTYPE html>
<html>
<head>
  <title>My Page Title</title>
  <link rel="icon" type="image/x-icon" href="/images/favicon.ico">
</head>

<body>
<h1>This is a Heading</h1>
<p>This is a paragraph.</p>
</body>
</html>
```

---

# `<link>` Element

The `<link>` element defines the **relationship between the document and an external resource**.

For favicons:

| Attribute    | Function                                    |
| ------------ | ------------------------------------------- |
| `rel="icon"` | Specifies that the file is the website icon |
| `type`       | Defines the image type                      |
| `href`       | Specifies the file location                 |

Example:

```html
<link rel="icon" type="image/x-icon" href="/images/favicon.ico">
```

---

# Where to Store the Favicon

Two common locations:

### Root folder

```
/favicon.ico
/index.html
```

Example:

```html
<link rel="icon" href="favicon.ico">
```

### Images folder

```
/images/favicon.ico
/index.html
```

Example:

```html
<link rel="icon" href="/images/favicon.ico">
```

---

# Recommended Favicon Characteristics

Favicons should be:

* **Small**
* **Simple**
* **High contrast**

Reason:

* They appear in **very small sizes** (usually 16×16 or 32×32 pixels).

---

# Common Favicon File Names

Most websites use:

```
favicon.ico
```

But other names also work.

---

# Supported Favicon Formats

Most modern browsers support several image formats.

| Format | Extension |
| ------ | --------- |
| ICO    | `.ico`    |
| PNG    | `.png`    |
| GIF    | `.gif`    |
| JPEG   | `.jpg`    |
| SVG    | `.svg`    |

Browsers that support these formats:

* Chrome
* Firefox
* Edge
* Safari
* Opera

---

# Example With PNG Favicon

```html
<link rel="icon" type="image/png" href="favicon.png">
```

---

# Chapter Summary

* A **favicon** is the small icon in the browser tab.
* Favicons are added using the `<link>` element.
* The `<link>` tag must be inside the `<head>` section.
* The `href` attribute specifies the favicon file path.
* Common favicon formats include **ICO, PNG, GIF, JPEG, and SVG**.

---