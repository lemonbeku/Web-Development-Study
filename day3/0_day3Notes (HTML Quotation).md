2026-03-1014:32
Status: #adult 
Tags: [[html]] [[Interactions Between Front-end and Back-End]] [[Web Development]]
Full Note

# 0_day3Notes

# HTML Quotation and Citation Elements  
  
HTML provides several elements used to represent **quotes, citations, abbreviations, and contact information**.    
These elements help give **semantic meaning** to text, making it easier for **browsers, search engines, and accessibility tools** to understand the content.  
The main elements in this topic are:  
- `<blockquote>`  
- `<q>`  
- `<abbr>`  
- `<address>`  
- `<cite>`  
- `<bdo>`  
---  
# `<blockquote>` Block Quotations  
The `<blockquote>` element defines a **section of text quoted from another source**.  
### Characteristics  
- Used for **long quotations**  
- Usually displayed with **indentation** by browsers  
- Can include the `cite` attribute to reference the source URL.  
### Syntax  
<blockquote cite="source-url"> Quoted text </blockquote> 

```html
<blockquote cite="source-url"> Quoted text </blockquote> 
```
### Example
<p>Here is a quote from WWF's website:</p>  
<blockquote cite="http://www.worldwildlife.org/who/index.html">  
For 60 years, WWF has worked to help people and nature thrive.  
</blockquote>
```html
<p>Here is a quote from WWF's website:</p>  
  
<blockquote cite="http://www.worldwildlife.org/who/index.html">  
For 60 years, WWF has worked to help people and nature thrive.  
</blockquote>
```
### Notes
- The `cite` attribute provides the **source of the quotation**, but it is **not usually visible on the page**.
---
# `<q>` Short Quotations
The `<q>` element defines a **short inline quotation**.
### Characteristics
- Used for **short quotes within a sentence**
- Browsers automatically **add quotation marks**
### Example
<p>WWF's goal is to:  
<q>Build a future where people live in harmony with nature.</q>  
</p>
```html
<p>WWF's goal is to:  
<q>Build a future where people live in harmony with nature.</q>  
</p>
```
### When to Use
Use `<q>` when quoting **a small phrase or sentence inside a paragraph**.

---
# `<abbr>` Abbreviations and Acronyms
The `<abbr>` element defines an **abbreviation or acronym**.
Examples:
- HTML
- CSS
- Dr.
- ASAP
### Benefits
Marking abbreviations helps:
- Browser
- Search engines
- Translation systems
- Screen readers
### Important Attribute
`title` attribute → shows the **full meaning when hovering the mouse**
### Example
<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
When a user hovers over **WHO**, the full phrase appears.
```html
<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
When a user hovers over WHO, the full phrase appears.
```
---
# `<address>` Contact Information
The `<address>` element defines **contact information for the author or owner of a document or article**.
### Can Include
- Email address
- Website URL
- Physical address
- Phone number
- Social media
### Default Browser Behavior
- Usually displayed in **italic**
- Browsers add a **line break before and after the element**
### Example
<address>  
Written by John Doe.<br>  
Visit us at:<br>  
Example.com<br>  
Box 564, Disneyland<br>  
USA  
</address>

```html
<address>  
Written by John Doe.<br>  
Visit us at:<br>  
Example.com<br>  
Box 564, Disneyland<br>  
USA  
</address>
```
### Important
Use `<address>` only for **contact information related to the document or article author**.

---
# `<cite>` Title of a Work
The `<cite>` element defines the **title of a creative work**.
### Examples of Creative Works
- Books
- Movies
- Poems
- Songs
- Paintings
- Sculptures
### Important Rule
A **person's name is NOT a title**, so it should not be inside `<cite>`.
### Default Browser Behavior
Text usually appears **italicized**.
### Example
<p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>
```html
<p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>
```
Here:
- `<cite>` = title of the painting
- "Edvard Munch" = artist (not inside `<cite>`)
---
# `<bdo>` Bi-Directional Override
`BDO` stands for **Bi-Directional Override**.
The `<bdo>` element is used to **override the default text direction**.
### Common Directions
`ltr` → Left to Right  
`rtl` → Right to Left
### Syntax
```html
<bdo dir="direction">  
text  
</bdo>
```
### Example
<bdo dir="rtl">This text will be written from right to left</bdo>
```html
<bdo dir="rtl">This text will be written from right to left</bdo>
```
### Use Cases
Useful for languages that use **different writing directions**, such as:
- Arabic
- Hebrew
# References
[[W3Schools]]
