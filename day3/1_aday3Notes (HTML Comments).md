# 0_day3Notes (HTML Comments)
## HTML Comments
**Definition**
- HTML comments are notes in the code that **are not displayed in the browser**.
- Used to **document, explain, or temporarily disable code**.
**Syntax**
<!-- Write your comment here -->
- The **start tag includes `!`** (`<!--`)
- The **end tag does not** (`-->`)
**Example**
```html
<!-- This is a comment -->  
<p>This is a paragraph.</p>
```

**Common Uses**
1. **Adding notes or reminders**
<!-- Remember to add more information here -->
2. **Hiding content temporarily**
<!-- <p>This paragraph is hidden</p> -->
3. **Hiding multiple lines**
<!--  
<p>Look at this cool image:</p>  
<img src="pic_trulli.jpg" alt="Trulli">  
-->
4. **Debugging code**
- Developers comment out parts of code to **find errors**.
1. **Hiding inline content**
```html
<p>This <!-- hidden text --> is a paragraph.</p>
```
<p>This <!-- hidden text --> is a paragraph.</p>
- Everything between `<!--` and `-->` **will not appear on the webpage**.

# References
[[W3Schools]]
