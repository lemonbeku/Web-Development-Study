2026-03-1122:19
Status: #adult 
Tags: [[Web Development]] [[html]]
Full Note

# 0_day4Notes (HTML Colors)
# HTML Colors  
## Overview  
HTML colors can be defined in several ways:  
- Predefined color names  
- RGB values  
- HEX values  
- HSL values  
- RGBA values  
- HSLA values  
These colors are commonly used to style:  
- Text  
- Backgrounds  
- Borders   
HTML supports **140 standard color names**.  
  
---   
# Color Names  
In HTML, colors can be specified using **predefined color names**.  
Examples:  
- Tomato  
- Orange  
- DodgerBlue  
- MediumSeaGreen  
- Gray  
- SlateBlue  
- Violet  
- LightGray  
Example:  
```html
<h1 style="color:Tomato;">Hello World</h1>
```
<h1 style="color:Tomato;">Hello World</h1>

# Background Color
The `background-color` property is used to set the **background color of an element**.
Example:
```html
<h1 style="background-color:DodgerBlue;">Hello World</h1>  
<p style="background-color:Tomato;">Lorem ipsum...</p>
```
<h1 style="background-color:DodgerBlue;">Hello World</h1>  
<p style="background-color:Tomato;">Lorem ipsum...</p>

---
# Text Color
The `color` property is used to set the **text color**.
Example:
```html
<h1 style="color:Tomato;">Hello World</h1>  
<p style="color:DodgerBlue;">Lorem ipsum...</p>  
<p style="color:MediumSeaGreen;">Ut wisi enim...</p>
```
<h1 style="color:Tomato;">Hello World</h1>  
<p style="color:DodgerBlue;">Lorem ipsum...</p>  
<p style="color:MediumSeaGreen;">Ut wisi enim...</p>

---
# Border Color
The `border` property can include a color value.
Syntax:
border: thickness style color
Example:
```html
<h1 style="border:2px solid Tomato;">Hello World</h1>  
<h1 style="border:2px solid DodgerBlue;">Hello World</h1>  
<h1 style="border:2px solid Violet;">Hello World</h1>
```
<h1 style="border:2px solid Tomato;">Hello World</h1>  
<h1 style="border:2px solid DodgerBlue;">Hello World</h1>  
<h1 style="border:2px solid Violet;">Hello World</h1>
Explanation:
- `2px` → border thickness
- `solid` → border style
- `Tomato` → border color
---
# Color Values
Besides color names, HTML also supports **different color value formats**.
## RGB
RGB stands for **Red, Green, Blue**.
Each value ranges from **0 to 255**.

Example:
```html
<h1 style="background-color:rgb(255, 99, 71);"></h1>
```

---
## HEX
HEX colors are written using **hexadecimal numbers**.
Format:
#RRGGBB
Example:
```html
<h1 style="background-color:#ff6347;"></h1>
```
---
## HSL
HSL stands for:
- **Hue**
- **Saturation**
- **Lightness**
Format:
hsl(hue, saturation, lightness)
Example:
```html
<h1 style="background-color:hsl(9, 100%, 64%);"></h1>
```
---
# Transparency Colors
Some color formats allow **transparency using an Alpha channel**.
Alpha value ranges from:
0 → fully transparent  
1 → fully opaque

---
## RGBA
RGBA = RGB + Alpha (transparency).
Example:
```html
<h1 style="background-color:rgba(255, 99, 71, 0.5);"></h1>
```
`0.5` = **50% transparency**

---
## HSLA
HSLA = HSL + Alpha.
Example:
```html
<h1 style="background-color:hsla(9, 100%, 64%, 0.5);"></h1>
```
---
# Summary
Ways to define HTML colors:

|Method|Example|
|---|---|
|Color Name|`Tomato`|
|RGB|`rgb(255, 99, 71)`|
|HEX|`#ff6347`|
|HSL|`hsl(9, 100%, 64%)`|
|RGBA|`rgba(255, 99, 71, 0.5)`|
|HSLA|`hsla(9, 100%, 64%, 0.5)`|

Common uses:
- `color` → text color
- `background-color` → background color
- `border` → border color

# References
[[W3Schools]]