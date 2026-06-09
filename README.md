# HTML-PRACTICE
HTML practice files and learning journey.

# HTML Journey 🚀

## What is HTML?

HTML (HyperText Markup Language) is the standard markup language used to create and structure web pages. It provides the basic structure of a website using tags and elements.

### Inventor of HTML

* Invented by Tim Berners-Lee
* Introduced in 1991
* Used to create the structure of web pages

---

# 01. Basic HTML Structure

Every HTML document follows a basic structure.

```html
<!DOCTYPE html>
<html>
<head>
    <title>My First Page</title>
</head>
<body>
    <h1>Hello World</h1>
</body>
</html>
```

### Main Elements

#### `<!DOCTYPE html>`

Declares that the document is HTML5.

#### `<html>`

Root element of an HTML page.

#### `<head>`

Contains metadata and page information.

#### `<title>`

Displays the page title in the browser tab.

#### `<body>`

Contains all visible webpage content.

---

# 02. Headings, Paragraphs and Links

## Headings

HTML provides six heading levels.

```html
<h1>Main Heading</h1>
<h2>Sub Heading</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

### Notes

* `<h1>` is the most important heading.
* `<h6>` is the smallest heading.
* Headings improve readability and SEO.

## Paragraph

```html
<p>This is a paragraph.</p>
```

Used to display text content.

## Links

```html
<a href="https://google.com">Visit Google</a>
```

### href Attribute

Specifies the destination URL.

---

# 03. Images

Images are added using the `<img>` tag.

```html
<img src="image.jpg" alt="Image">
```

### Important Attributes

#### src

Specifies image location.

#### alt

Alternative text shown if image cannot load.

#### width

Sets image width.

#### height

Sets image height.

Example:

```html
<img src="photo.jpg"
     alt="Photo"
     width="300">
```

### Notes

* `<img>` is an empty tag.
* Images can be local or online.

---

# 04. Tables

Tables are used to display data in rows and columns.

## Basic Tags

### `<table>`

Creates a table.

### `<tr>`

Creates a row.

### `<th>`

Creates a heading cell.

### `<td>`

Creates a data cell.

Example:

```html
<table border="1">
    <tr>
        <th>Name</th>
        <th>Branch</th>
    </tr>

    <tr>
        <td>Suraj</td>
        <td>CSE</td>
    </tr>
</table>
```

## Table Sections

### `<caption>`

Table title.

### `<thead>`

Header section.

### `<tbody>`

Main table content.

### `<tfoot>`

Footer section.

## colspan

Merges columns.

```html
<td colspan="2">Sam</td>
```

## rowspan

Merges rows.

```html
<td rowspan="2">Java</td>
```

---

# 05. Lists

Lists are used to organize items.

## Ordered List

```html
<ol>
    <li>HTML</li>
    <li>CSS</li>
</ol>
```

Displays numbered items.

## Unordered List

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
</ul>
```

Displays bullet points.

## Description List

```html
<dl>
    <dt>HTML</dt>
    <dd>Markup Language</dd>
</dl>
```

### List Tags

* `<ol>` Ordered List
* `<ul>` Unordered List
* `<li>` List Item
* `<dl>` Description List
* `<dt>` Description Term
* `<dd>` Description Description

---

# 06. SEO and Core Web Vitals

## SEO

SEO (Search Engine Optimization) is the process of improving a website's visibility in search engine results.

### Important SEO Tags

#### Title Tag

```html
<title>Learn HTML</title>
```

#### Meta Description

```html
<meta name="description"
content="Learn HTML from beginner to advanced">
```

#### Viewport

```html
<meta name="viewport"
content="width=device-width, initial-scale=1.0">
```

### Semantic HTML

```html
<header>
<nav>
<main>
<section>
<article>
<footer>
```

Helps search engines understand page structure.

---

# Core Web Vitals

Google uses Core Web Vitals to measure user experience.

## LCP (Largest Contentful Paint)

Measures loading speed.

Good Score:

```text
Less than 2.5 seconds
```

## INP (Interaction to Next Paint)

Measures responsiveness.

Good Score:

```text
Less than 200 milliseconds
```

## CLS (Cumulative Layout Shift)

Measures visual stability.

Good Score:

```text
Less than 0.1
```

### Improving Core Web Vitals

* Use image width and height.
* Optimize images.
* Use lazy loading.
* Write semantic HTML.

---

🚀 This repository documents my HTML learning journey and practice.
