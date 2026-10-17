# HTML

HTML (**HyperText Markup Language**) is used to structure and organize content on web pages.

This section covers HTML elements, attributes, and the basic building blocks required for frontend development.

---

## 📚 Topics Covered

* HTML Tags & Elements
* Links
* Images
* Lists
* Tables
* Forms
* Semantic HTML
* Media
* Embedded Content
* Miscellaneous Elements
* HTML Attributes

---

## 📁 Files

```text
HTML/
│
├── 01-tags.html
├── 02-links.html
├── 03-images.html
├── 04-lists.html
├── 05-tables.html
├── 06-forms.html
├── 07-semantic.html
├── 08-media.html
├── 09-embedded.html
├── 10-misc-elements.html
└── 11-attributes.html
```

---

# 01. Tags & Elements

File: `01-tags.html`

Basic text and content elements.

### Headings

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

### Text Elements

```html
<p>Paragraph</p>
<br>
<hr>

<b>Bold</b>
<strong>Important</strong>

<i>Italic</i>
<em>Emphasized</em>

<u>Underlined</u>
<s>No longer accurate</s>

<mark>Highlighted</mark>
<small>Small text</small>

H<sub>2</sub>O
x<sup>2</sup>

<del>Deleted text</del>
<ins>Inserted text</ins>
```

---

# 02. Links

File: `02-links.html`

The `<a>` element is used to create hyperlinks.

```html
<a href="https://example.com">
    Visit Example
</a>
```

### Important Attributes

```text
href
target
rel
download
title
```

### Common Target Values

```text
_self
_blank
_parent
_top
```

### Other Link Types

```html
<a href="about.html">About</a>

<a href="#section">Go to Section</a>

<a href="mailto:example@email.com">
    Send Email
</a>

<a href="tel:+1234567890">
    Call
</a>
```

---

# 03. Images

File: `03-images.html`

### Image

```html
<img
    src="image.jpg"
    alt="Description of image"
>
```

### Important Attributes

```text
src
alt
width
height
loading
title
```

### Responsive Images

```html
<picture>

    <source
        media="(max-width: 600px)"
        srcset="mobile.jpg"
    >

    <img
        src="desktop.jpg"
        alt="Responsive image"
    >

</picture>
```

### Multiple Image Sources

```html
<img
    src="small.jpg"
    srcset="
        small.jpg 480w,
        medium.jpg 800w,
        large.jpg 1200w
    "
    alt="Responsive image"
>
```

---

# 04. Lists

File: `04-lists.html`

### Unordered List

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

### Ordered List

```html
<ol>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ol>
```

### Ordered List Attributes

```text
type
start
reversed
```

Example:

```html
<ol type="A">
    <li>HTML</li>
    <li>CSS</li>
</ol>
```

### Nested Lists

```html
<ul>

    <li>
        Frontend

        <ul>
            <li>HTML</li>
            <li>CSS</li>
        </ul>

    </li>

</ul>
```

### Description List

```html
<dl>

    <dt>HTML</dt>
    <dd>Markup language</dd>

    <dt>CSS</dt>
    <dd>Styling language</dd>

</dl>
```

---

# 05. Tables

File: `05-tables.html`

Tables are used to represent data in rows and columns.

### Basic Table

```html
<table>

    <tr>
        <th>Name</th>
        <th>Age</th>
    </tr>

    <tr>
        <td>Himanshu</td>
        <td>20</td>
    </tr>

</table>
```

### Table Elements

```text
<table>       → Table
<caption>     → Table title
<tr>          → Table row
<th>          → Table header
<td>          → Table data

<thead>       → Table header section
<tbody>       → Table body
<tfoot>       → Table footer

<colgroup>    → Column group
<col>         → Column
```

### Important Attributes

```text
colspan
rowspan
scope
```

Example:

```html
<th colspan="3">
    Student Information
</th>
```

---

# 06. Forms

File: `06-forms.html`

Forms are used to collect user input.

### Main Form Elements

```text
<form>
<label>
<input>
<textarea>
<select>
<option>
<datalist>
<fieldset>
<legend>
<button>
```

### Common Input Types

```text
text
password
email
number
tel
url
search

date
time
datetime-local
month
week

color
range

checkbox
radio

file

submit
reset
button
hidden
```

### Example

```html
<form>

    <label for="username">
        Username:
    </label>

    <input
        type="text"
        id="username"
        name="username"
        placeholder="Enter username"
        required
    >

    <button type="submit">
        Submit
    </button>

</form>
```

### Important Form Attributes

```text
id
name
value
placeholder

required
disabled
readonly

min
max
step

minlength
maxlength

multiple
accept
selected
autofocus
pattern
list
```

### Form Submission Attributes

```text
action
method
enctype
```

---

# 07. Semantic HTML

File: `07-semantic.html`

Semantic elements describe the meaning and purpose of their content.

### Main Semantic Elements

```text
<header>
<nav>
<main>
<section>
<article>
<aside>
<footer>
<address>
<search>
```

### Common Structure

```html
<body>

    <header>
        <h1>Website</h1>
    </header>

    <nav>
        <a href="/">Home</a>
        <a href="/about">About</a>
    </nav>

    <main>

        <section>

            <h2>Latest Articles</h2>

            <article>
                <h3>HTML Basics</h3>
                <p>...</p>
            </article>

        </section>

        <aside>
            Related content
        </aside>

    </main>

    <footer>
        Copyright
    </footer>

</body>
```

### Important Difference

```text
<section>  → Meaningful section of content
<article>  → Independent/self-contained content
<div>      → Generic container
```

---

# 08. Media

File: `08-media.html`

### Audio

```html
<audio controls>

    <source
        src="music.mp3"
        type="audio/mpeg"
    >

</audio>
```

### Video

```html
<video controls>

    <source
        src="movie.mp4"
        type="video/mp4"
    >

</video>
```

### Media Elements

```text
<audio>
<video>
<source>
<track>
```

### Common Media Attributes

```text
controls
autoplay
loop
muted
preload
```

### Video-Specific

```text
width
height
poster
```

### Track Attributes

```text
kind
src
srclang
label
default
```

---

# 09. Embedded Content

File: `09-embedded.html`

### iframe

Used to embed another webpage or external content.

```html
<iframe
    src="https://example.com"
    width="600"
    height="400"
    title="Example Website"
>
</iframe>
```

### iframe Attributes

```text
src
width
height
title
loading
allowfullscreen
sandbox
```

### Other Embedded Elements

```text
<embed>
<object>
<canvas>
<svg>
```

### Object

```html
<object
    data="document.pdf"
    type="application/pdf"
>
</object>
```

### Canvas

```html
<canvas
    id="gameCanvas"
    width="800"
    height="600"
>
</canvas>
```

Canvas is commonly controlled using JavaScript.

### SVG

```html
<svg width="300" height="200">

    <circle
        cx="100"
        cy="100"
        r="50"
    >

    </circle>

</svg>
```

Basic SVG elements covered:

```text
<svg>
<circle>
<rect>
<line>
<polygon>
```

---

# 10. Miscellaneous Elements

File: `10-misc-elements.html`

### Figure

```html
<figure>

    <img
        src="image.jpg"
        alt="Example"
    >

    <figcaption>
        Image caption
    </figcaption>

</figure>
```

```text
<figure>        → Self-contained content
<figcaption>    → Figure caption
```

### Quotations

```html
<blockquote>
    Long quotation
</blockquote>

<p>
    He said <q>Hello</q>.
</p>
```

```text
<blockquote>    → Long quotation
<q>             → Short quotation
<cite>          → Creative work title
```

### Text Semantics

```text
<abbr>          → Abbreviation
<dfn>            → Defined term
<code>           → Code
<pre>            → Preformatted text
<kbd>            → Keyboard input
<samp>           → Program output
<var>            → Variable
<data>           → Machine-readable value
<time>           → Date/time
```

### Bidirectional Text

```text
<bdi>            → Bidirectional isolation
<bdo>            → Bidirectional override
```

### Ruby Annotations

```text
<ruby>
<rt>
<rp>
```

### Other Elements

```text
<wbr>            → Word break opportunity

<details>        → Expandable content
<summary>        → Details heading

<dialog>         → Dialog/modal

<progress>       → Task progress
<meter>          → Measurement

<output>         → Calculation/result

<template>       → Hidden reusable HTML template
<slot>           → Web Component placeholder
```

---

# 11. HTML Attributes

File: `11-attributes.html`

Attributes provide additional information or configuration for HTML elements.

## Global Attributes

These can generally be used on many HTML elements.

```text
id
class
title
style
lang
dir
hidden

tabindex
contenteditable
spellcheck
draggable
translate
accesskey

data-*
```

### Example

```html
<div
    id="user-card"
    class="card active"
    title="User information"
    data-user-id="101"
>
    User
</div>
```

---

## Boolean Attributes

A boolean attribute is generally true when it is present and false when it is absent.

```text
disabled
required
readonly
checked
selected
multiple
autofocus

controls
autoplay
loop
muted
hidden
```

Example:

```html
<input
    type="text"
    required
>
```

---

## Link Attributes

```text
href
target
rel
download
```

Example:

```html
<a
    href="https://example.com"
    target="_blank"
    rel="noopener"
>
    Open Example
</a>
```

---

## Image Attributes

```text
src
alt
width
height
loading
```

---

## Form Attributes

```text
name
value
placeholder

min
max
step

minlength
maxlength

pattern
accept
list
```

---

## Form Submission

```text
action
method
enctype
```

Example:

```html
<form
    action="/login"
    method="post"
>
    ...
</form>
```

---

# 🧩 Void Elements

Void elements do not have closing tags.

```text
<area>
<base>
<br>
<col>
<embed>
<hr>
<img>
<input>
<link>
<meta>
<source>
<track>
<wbr>
```

Example:

```html
<img src="cat.jpg" alt="Cat">
<br>
<hr>
<input type="text">
```

---

# 📝 Important Notes

### Tag vs Element

A tag:

```html
<p>
```

An element:

```html
<p>Hello World</p>
```

### HTML Declaration

```html
<!DOCTYPE html>
```

`<!DOCTYPE html>` is a **document type declaration**, not an HTML element.

---

# 🎯 Learning Order

The HTML topics were practiced in the following order:

```text
01. Tags & Elements
        ↓
02. Links
        ↓
03. Images
        ↓
04. Lists
        ↓
05. Tables
        ↓
06. Forms
        ↓
07. Semantic HTML
        ↓
08. Media
        ↓
09. Embedded Content
        ↓
10. Miscellaneous Elements
        ↓
11. Attributes
```

HTML fundamentals are now covered. The next phase is **CSS**.
