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


# 07. HTML Forms and Input Tags

## Introduction

HTML Forms are used to collect data from users. Forms are commonly used for login pages, registration forms, contact forms, surveys, feedback forms, and online applications.

The `<form>` element acts as a container that holds different form controls such as text fields, radio buttons, checkboxes, dropdown lists, and buttons.

---

# Form Tag

The `<form>` tag is used to create a form.

```html
<form action="" method="post">
</form>
```

## Form Attributes

### action

Specifies the location where form data will be sent after submission.

```html
<form action="submit.php">
```

### method

Specifies how form data will be transmitted.

```html
method="get"
```

or

```html
method="post"
```

---

# Input Element

The `<input>` element is used to accept user input.

```html
<input type="text">
```

Input is an empty element and does not require a closing tag.

---

# Common Input Types

## Text Input

Used to enter text such as names and usernames.

```html
<input type="text">
```

---

## Password Input

Used to enter passwords. Characters are hidden for security.

```html
<input type="password">
```

---

## Email Input

Used to enter email addresses.

```html
<input type="email">
```

The browser validates the email format automatically.

---

## Number Input

Used to enter numeric values.

```html
<input type="number">
```

---

## Date Input

Used to select dates from a calendar.

```html
<input type="date">
```

---

## Radio Button

Used when only one option can be selected from a group.

```html
<input type="radio" name="gender" value="male">
<input type="radio" name="gender" value="female">
```

### Important Note

Radio buttons must have the same `name` attribute to work as a group.

---

## Checkbox

Used when multiple options can be selected.

```html
<input type="checkbox" name="hobby" value="cricket">
```

---

## File Input

Used to upload files.

```html
<input type="file">
```

---

## Submit Button

Used to submit form data.

```html
<input type="submit" value="Submit">
```

---

## Reset Button

Used to clear all form fields.

```html
<input type="reset" value="Reset">
```

---

# Label Element

The `<label>` element provides a description for an input field.

```html
<label for="username">Username</label>
<input type="text" id="username">
```

## Benefits

* Improves accessibility.
* Clicking the label focuses the related input field.
* Makes forms more user-friendly.

---

# Important Input Attributes

## id

Provides a unique identifier for an element.

```html
<input type="text" id="username">
```

---

## name

Defines the name of the data sent to the server.

```html
<input type="text" name="username">
```

Example:

```
username = Suraj
```

---

## value

Specifies the value submitted with the form.

```html
<input type="radio" value="male">
```

---

## placeholder

Displays a hint inside the input field.

```html
<input type="text" placeholder="Enter your name">
```

---

## autofocus

Automatically places the cursor inside the field when the page loads.

```html
<input type="text" autofocus>
```

---

## required

Makes a field mandatory.

```html
<input type="email" required>
```

The form cannot be submitted if the field is empty.

---

# Textarea Element

The `<textarea>` element is used for multi-line text input.

```html
<textarea rows="4" cols="50"></textarea>
```

## Attributes

### rows

Defines the height of the textarea.

```html
rows="4"
```

### cols

Defines the width of the textarea.

```html
cols="50"
```

---

# Select and Option Elements

Used to create a dropdown list.

```html
<select name="fruits">
    <option value="apple">Apple</option>
    <option value="banana">Banana</option>
</select>
```

## select

Creates a dropdown menu.

## option

Defines items inside the dropdown.

---

# Data Submission Example

If a user enters:

```
Username : Suraj
Gender : Male
Comment : Learning HTML
Fruit : Banana
```

The server may receive:

```
username = Suraj
gender = male
comment = Learning HTML
fruits = banana
```

---

# Difference Between id and name

| id                          | name                            |
| --------------------------- | ------------------------------- |
| Must be unique              | Can be reused                   |
| Used by CSS and JavaScript  | Used to send data to the server |
| Connects labels with inputs | Identifies form data            |

---

# Advantages of HTML Forms

* Collect user information.
* Enable user interaction.
* Used in login and registration systems.
* Support data validation.
* Essential for web applications.

---

# Conclusion

HTML Forms are used to collect and submit user data. Important form elements include:

* form
* input
* label
* textarea
* select
* option
* button

Forms are one of the most important features of modern web development.



🚀 This repository documents my HTML learning journey and practice.
