# HTML Tables

HTML tables are used to **organize data into rows and columns**.

Example structure:

| Company                    | Contact         | Country |
| -------------------------- | --------------- | ------- |
| Alfreds Futterkiste        | Maria Anders    | Germany |
| Centro comercial Moctezuma | Francisco Chang | Mexico  |

---

# Basic Table Structure

A table consists of:

* rows
* columns
* cells

Example:

```html
<table>
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
</table>
```

---

# Table Elements

| Tag       | Meaning           |
| --------- | ----------------- |
| `<table>` | Defines a table   |
| `<tr>`    | Table row         |
| `<td>`    | Table data cell   |
| `<th>`    | Table header cell |

---

# Table Cells (`<td>`)

`<td>` stands for **table data**.

Example:

```html
<td>Emil</td>
```

Cells can contain:

* text
* images
* links
* lists
* other HTML elements

---

# Table Rows (`<tr>`)

`<tr>` defines a **table row**.

Example:

```html
<tr>
  <td>Emil</td>
  <td>Tobias</td>
  <td>Linus</td>
</tr>
```

Each row usually contains the **same number of cells**.

---

# Table Headers (`<th>`)

`<th>` defines **header cells**.

Example:

```html
<tr>
  <th>Name</th>
  <th>Age</th>
</tr>
```

Default styling:

* **bold**
* **centered**

Can be styled with CSS.

---

# HTML Table Tags

| Tag          | Description          |
| ------------ | -------------------- |
| `<table>`    | Defines a table      |
| `<tr>`       | Table row            |
| `<td>`       | Table data cell      |
| `<th>`       | Header cell          |
| `<caption>`  | Table title          |
| `<thead>`    | Table header section |
| `<tbody>`    | Table body section   |
| `<tfoot>`    | Table footer section |
| `<colgroup>` | Group of columns     |
| `<col>`      | Column properties    |

---

# Table Borders

Borders are added using **CSS**.

Example:

```css
table, th, td {
  border: 1px solid black;
}
```

---

# Border Collapse

Removes double borders.

```css
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
```

---

# Border Styles

Possible styles:

* `solid`
* `dotted`
* `dashed`
* `double`
* `groove`
* `ridge`
* `inset`
* `outset`
* `none`

Example:

```css
th, td {
  border-style: dotted;
}
```

---

# Border Color

Change border color:

```css
th, td {
  border-color: #96D4D4;
}
```

---

# Table Size

Tables can have **custom width and height**.

### Table Width

```html
<table style="width:100%">
```

### Column Width

```html
<th style="width:70%">Firstname</th>
```

### Row Height

```html
<tr style="height:200px">
```

---

# Table Headers (Vertical)

Headers can also be **first column**.

Example:

```html
<tr>
  <th>Firstname</th>
  <td>Jill</td>
  <td>Eve</td>
</tr>
```

---

# Align Table Headers

Default alignment:

* centered

Change alignment:

```css
th {
  text-align: left;
}
```

---

# Colspan

`colspan` allows a cell to **span multiple columns**.

Example:

```html
<th colspan="2">Name</th>
```

Meaning: the cell covers **2 columns**.

---

# Rowspan

`rowspan` allows a cell to **span multiple rows**.

Example:

```html
<th rowspan="2">Phone</th>
```

Meaning: the cell covers **2 rows**.

---

# Table Padding

Padding = **space inside a cell**.

Example:

```css
th, td {
  padding: 15px;
}
```

Specific sides:

```css
padding-top
padding-bottom
padding-left
padding-right
```

---

# Table Spacing

Spacing = **space between cells**.

Example:

```css
table {
  border-spacing: 30px;
}
```

---

# Zebra Stripe Tables

Zebra stripes improve readability.

Example:

```css
tr:nth-child(even) {
  background-color: #D6EEEE;
}
```

Result: every **second row is colored**.

---

# Vertical Zebra Stripes

Style columns instead of rows.

Example:

```css
td:nth-child(even),
th:nth-child(even) {
  background-color: #D6EEEE;
}
```

---

# Hoverable Table

Highlight row on hover.

```css
tr:hover {
  background-color: #D6EEEE;
}
```

---

# Horizontal Dividers

Add lines between rows.

```css
tr {
  border-bottom: 1px solid #ddd;
}
```

---

# `<colgroup>` Element

`<colgroup>` is used to **style entire columns**.

Example:

```html
<table>
  <colgroup>
    <col span="2" style="background-color:#D6EEEE">
  </colgroup>
</table>
```

Meaning:

* first **2 columns get styling**

---

# `<col>` Element

Defines styling for specific columns.

Example:

```html
<col span="3" style="background-color:pink">
```

---

# Hide Columns

Columns can be hidden.

Example:

```css
visibility: collapse;
```

Example:

```html
<col span="3" style="visibility: collapse">
```

---

# Key Concepts Summary

HTML tables are built with:

* `<table>` – container
* `<tr>` – rows
* `<td>` – data cells
* `<th>` – header cells

Important features:

* borders
* padding
* spacing
* colspan / rowspan
* zebra stripes
* hover effects
* column styling with `<colgroup>`
