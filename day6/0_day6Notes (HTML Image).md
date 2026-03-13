Here are **structured study notes** for **HTML Images** written in a way that fits your **web development learning notes (Obsidian style)**.

---

# HTML Images

Images improve the **visual appearance and design** of a webpage.

Example:

```html
<img src="pic_trulli.jpg" alt="Italian Trulli">
<img src="img_girl.jpg" alt="Girl in a jacket">
<img src="img_chania.jpg" alt="Flowers in Chania">
```

---

# HTML `<img>` Tag

The `<img>` tag is used to **display images on a webpage**.

Important characteristics:

* Images are **not inserted** into the webpage
* They are **linked to the page**
* The `<img>` tag **does not have a closing tag**
* It only contains **attributes**

Basic syntax:

```html
<img src="url" alt="description">
```

Required attributes:

| Attribute | Function                              |
| --------- | ------------------------------------- |
| `src`     | Path or URL of the image              |
| `alt`     | Alternative text if image cannot load |

---

# The `src` Attribute

`src` specifies the **location of the image file**.

Example:

```html
<img src="img_chania.jpg" alt="Flowers in Chania">
```

Notes:

* The browser **requests the image from a server**
* If the image location changes → **broken image appears**

Broken images show:

* a broken icon
* the **alt text**

---

# The `alt` Attribute

`alt` provides **alternative text** if the image cannot be displayed.

Example:

```html
<img src="img_chania.jpg" alt="Flowers in Chania">
```

When `alt` is shown:

* slow internet
* wrong image path
* screen reader usage

Example with error:

```html
<img src="wrongname.gif" alt="Flowers in Chania">
```

Important for:

* **Accessibility**
* **Visually impaired users**
* **SEO**

Screen readers read the **alt text aloud**.

---

# Image Size

Images can be resized using:

1. `style`
2. `width` and `height` attributes

Example using CSS:

```html
<img src="img_girl.jpg" alt="Girl in a jacket" style="width:500px;height:600px;">
```

Example using attributes:

```html
<img src="img_girl.jpg" alt="Girl in a jacket" width="500" height="600">
```

Important:

* Size is measured in **pixels**
* Always define image size to **avoid page flickering during loading**

---

# Width and Height vs Style

Both methods work, but **CSS style is preferred**.

Example:

```html
<style>
img {
  width: 100%;
}
</style>
```

```html
<img src="html5.gif" alt="HTML5 Icon" width="128" height="128">

<img src="html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">
```

Reason:

* CSS **prevents external stylesheets from overriding image sizes**

---

# Images in Another Folder

If the image is inside a folder, include the folder name.

Example:

```html
<img src="/images/html5.gif" alt="HTML5 Icon">
```

---

# Images from Another Website

You can use images from another server using **absolute URLs**.

Example:

```html
<img src="https://www.w3schools.com/images/w3schools_green.jpg" alt="W3Schools.com">
```

Warnings:

* May violate **copyright**
* The image may **change or be deleted**
* You **do not control the file**

---

# Animated Images

HTML supports **animated GIFs**.

Example:

```html
<img src="programming.gif" alt="Computer Man" style="width:48px;height:48px;">
```

---

# Image as a Link

Images can be used as links by placing them inside an `<a>` tag.

Example:

```html
<a href="default.asp">
  <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
</a>
```

---

# Floating Images

Images can float **left or right** using CSS `float`.

Example (right):

```html
<p>
<img src="smiley.gif" alt="Smiley face" style="float:right;width:42px;height:42px;">
The image floats to the right.
</p>
```

Example (left):

```html
<p>
<img src="smiley.gif" alt="Smiley face" style="float:left;width:42px;height:42px;">
The image floats to the left.
</p>
```

---

# Common Image Formats

| Format | Extension   |
| ------ | ----------- |
| APNG   | .apng       |
| GIF    | .gif        |
| ICO    | .ico        |
| JPEG   | .jpg, .jpeg |
| PNG    | .png        |
| SVG    | .svg        |

Notes:

* **JPEG** → photographs
* **PNG** → transparent images
* **GIF** → animations
* **SVG** → scalable vector graphics

---

# HTML Image Maps

Image maps allow **different clickable areas within one image**.

Example:

```html
<img src="workplace.jpg" alt="Workplace" usemap="#workmap">
```

Map definition:

```html
<map name="workmap">
  <area shape="rect" coords="34,44,270,350" href="computer.htm">
  <area shape="rect" coords="290,172,333,250" href="phone.htm">
  <area shape="circle" coords="337,300,44" href="coffee.htm">
</map>
```

Important elements:

| Tag      | Function               |
| -------- | ---------------------- |
| `<map>`  | Defines image map      |
| `<area>` | Defines clickable area |
| `usemap` | Connects image to map  |

---

# Image Map Shapes

### Rectangle

```html
<area shape="rect" coords="x1,y1,x2,y2">
```

Example:

```html
<area shape="rect" coords="34,44,270,350">
```

---

### Circle

```html
<area shape="circle" coords="x,y,radius">
```

Example:

```html
<area shape="circle" coords="337,300,44">
```

---

### Polygon

Polygon uses **multiple coordinate points**.

Example:

```html
<area shape="poly" coords="140,121,181,116,204,160,204,222">
```

Used for **custom shapes**.

---

# Image Maps with JavaScript

Clickable areas can trigger JavaScript.

Example:

```html
<area shape="circle" coords="337,300,44" onclick="myFunction()">
```

```html
<script>
function myFunction() {
  alert("You clicked the coffee cup!");
}
</script>
```

---

# HTML Background Images

Background images can be applied to **any HTML element**.

Example:

```html
<p style="background-image: url('img_girl.jpg');">
```

---

# Background Image for Entire Page

Example:

```html
<style>
body {
  background-image: url('img_girl.jpg');
}
</style>
```

---

# Background Repeat

By default, background images **repeat**.

Example:

```css
background-repeat: no-repeat;
```

Example:

```html
<style>
body {
  background-image: url('img_girl.jpg');
  background-repeat: no-repeat;
}
</style>
```

---

# Background Cover

Make the background cover the entire screen.

Example:

```css
background-size: cover;
background-attachment: fixed;
```

Example:

```html
<style>
body {
  background-image: url('img_girl.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
}
</style>
```

---

# Background Stretch

Stretch image to fill the entire element.

Example:

```css
background-size: 100% 100%;
```

---

# HTML `<picture>` Element

The `<picture>` element allows **different images for different devices or screen sizes**.

Example:

```html
<picture>
  <source media="(min-width: 650px)" srcset="img_food.jpg">
  <source media="(min-width: 465px)" srcset="img_car.jpg">
  <img src="img_girl.jpg">
</picture>
```

Important rule:

* Always include an `<img>` tag **as fallback**

---

# When to Use `<picture>`

### 1. Bandwidth Optimization

Small screens load **smaller images**.

### 2. Format Compatibility

Different browsers support **different image formats**.

Example:

```html
<picture>
  <source srcset="img_avatar.png">
  <source srcset="img_girl.jpg">
  <img src="img_beatles.gif" alt="Beatles">
</picture>
```

The browser loads the **first supported format**.

---

# HTML Image Tags Summary

| Tag         | Description                     |
| ----------- | ------------------------------- |
| `<img>`     | Displays images                 |
| `<map>`     | Defines image maps              |
| `<area>`    | Defines clickable regions       |
| `<picture>` | Displays multiple image sources |

---

# Key Points

* `<img>` is used to display images.
* `src` specifies the image path.
* `alt` provides alternative text.
* Image size can be set with `width`, `height`, or CSS.
* Images can be links or floating elements.
* Image maps allow **multiple clickable areas**.
* `<picture>` supports **responsive images**.

---

If you want, I can also make you **Anki flashcards from this chapter (20–30 cards)** so you can memorize **HTML image tags faster while learning web development.**
